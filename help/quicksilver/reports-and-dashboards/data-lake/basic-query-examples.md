---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect查询示例
description: 您可以使用示例查询来熟悉特定类型查询的语法和结构。
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: c8a25bcc8c9b56a649ca7764918c86f9cdd5b3e2
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Workfront Data Connect查询示例

为了帮助您更好地利用Workfront Data Connect数据，本页包含一些基本的示例查询，您可以使用这些查询来熟悉特定类型查询的语法和结构。

## 自定义数据查询

此示例演示如何在Workfront中构建查询以返回自定义数据，如自定义表单和自定义字段。

### 方案

您的组织使用名为Finance Integration的自定义表单。 该表单附加到每个项目，并包含以下字段：

* **业务单元**：包含字符串的自定义字段。
* **ProjectID**：包含数字字符串的自定义字段。
* **扩展的项目名称**：将业务单元、项目ID和本机Workfront项目名称的值连接到单个字符串的计算自定义数据字段。

您需要将此信息包含在针对Data Connect的查询的响应中。 数据湖中记录的自定义数据值包含在标题为`parametervalues`的列中。 此列将存储为JSON对象。

### 查询

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### 响应

上述查询返回以下数据：

* `projectid`：本机Workfront项目ID。
* `parametervalues`：存储JSON对象的列。
* `name`：本机Workfront项目名称。
* `Business Unit`： `parametervalues`对象中包含的自定义数据值。
* `Project ID`： `parametervalues`对象中包含的自定义数据值。
* `Expanded Project Name`： `parametervalues`对象中包含的自定义数据值。

### 解释

查询`parametervalues` JSON对象时，可以使用以下内容将每个自定义数据字段作为列进行访问：

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>`是正在查询的表中的JSON对象的名称。 在自定义数据的情况下，此值始终为`parametervalues`。
* `<parameter_name>`是在表单配置工具中找到的`parametername`字符串，尽管它可能并不总是与此值匹配。

>[!NOTE]
>
>如果在Workfront表单配置工具中更改了参数的名称，则该名称将在JSON对象中表示为新列。 因此，我们建议在表单配置工具中创建列后不要更改其名称。 但是，标签可以更改，而不会影响JSON对象。
>
>如果参数名称的文本字符串不正确，则该列将返回NULL值，而不是错误。

* `<data_type>`将从JSON对象返回的值转换为适用于该字段的数据类型。 为返回的值选择不兼容的数据类型将导致数据类型不匹配错误。 可能的数据类型包括：

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` （例如，`Number(32,4)`将返回1234.0987）
   * `date`
   * `timestamp`

* `<column_name>`是您为每个自定义数据列创建的标签。

>[!NOTE]
>
>只有表单中指定了值的参数才会包含在JSON对象中。 如果表单上的自定义数据字段为空，它将不会显示。

## 状态查询中的时间

此示例演示了如何测量项目在以前分配的状态下所花费的时间。 它可以很容易地适于测量处于状态的任务或发放时间，或者它可以适于测量对象应用了任何其他属性（包括自定义数据值）的时间长度。

### 方案

您的组织领导层认为您在工作生命周期的每个阶段都花费了太多的时间。 在提出改进过程的建议之前，您需要创建一个基线测量，用于测量项目状态随时间变化的频率以及项目处于任何给定状态的天数。

您将使用PROJECTS_EVENT数据视图来拉入针对项目对象的每个状态更改的列表。 您将新状态与以前状态进行比较，获取以前分配的状态的有效时间范围，然后计算在该状态中花费的天数。

利用每个项目在每个状态中所花费时间的原始输出，您可以开始构建可视化图表或进一步聚合数据以构建按状态、项目类型或时间划分的状态持续时间平均值。 然后，此基线用于设置一个基准，您可以根据此基准进行衡量，以满足领导层的期望。

以下查询使用Data Connect PROJECTS_EVENTS数据视图来比较每个项目状态更改事件并显示状态中的时间。

### 查询

```
-- Calculate the begin/end effective timestamp and duration in days 

SELECT 

    projectid, 
    name as project_name, 
    prev_status as previous_status, 
    status, 
    status_change_date as status_begin_effective_timestamp, 
    case 
        when status_change_date is null then NULL
        else
            nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp) 
    end as status_end_effective_timestamp, 
    datediff('DAYS',status_change_date, nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp)) as status_duration_days 

FROM 
    ( -- Filter to just the records that have changed 
     SELECT projectid, 
        name, 
        prev_status, 
        status, 
        begin_effective_timestamp as status_change_date    
     FROM 
        (  -- Calculate records where previous status is different 
          SELECT DISTINCT  
           pe.projectid, 
           pe.name AS name, 
           pe.STATUS, 
           nvl(lag(pe.STATUS) over (partition by pe.projectid order by pe.BEGIN_EFFECTIVE_TIMESTAMP), status) prev_status, 
           begin_effective_timestamp 

          FROM projects_event pe 
         -- Set any WHERE conditions to limit the results as needed 
         --WHERE 
            -- pe.PROJECTID = '5ebe…c1e1' 
        ) 
        WHERE prev_status != status 
    ) 
    order by status_change_date; 
```

### 响应

上述查询返回以下数据：

* `PROJECTID`：与状态更改事件关联的Workfront项目ID。
* `PROJECT_NAME`： Workfront项目名称。
* `PREVIOUS_STATUS`：项目状态紧跟更改前。
* `STATUS`：更改后的项目状态。
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP`：更改事件时间戳，在此时间戳之前已设置状态。
* `STATUS_END_EFFECTIVE_TIMESTAMP`：设置更新状态值时的更改事件时间戳。
* `STATUS_DURATION_DAYS`：结束有效时间戳和开始有效时间戳之间的差异（以天为单位）。

### 解释

查询使用Data Connect的变更事件跟踪功能。  它确定触发事件的日期，该事件的新状态值与上一个事件不同。 

从内到外检查查询： 

1. 计算先前状态不同的记录： 
   * 对于每个更改事件，使用lag()函数来标识状态的上一个值。 

2. 仅筛选已更改的记录： 

   * 从步骤1中的计算中选择记录，其中前一个状态！=当前状态。 

3. 以天为单位计算开始/结束有效时间戳和持续时间： 

   * `<status_begin_effective_timestamp>`：在步骤2中计算。 

   * `<status_end_effective_timestamp>`：根据下一个(lead())进行计算。 `<status_begin_effective_timestamp>`：仅在`<status_begin_effective_timestamp>`不为NULL时显示状态。 
   * `<status_duration_days>`： `<status_begin_effective_timestamp>`和`<status_end_effective_timestamp>`之间的数据差异。 

>[!NOTE]
>
>建议您将此查询用作其自身在PowerBI或Tableau中的“视图”。  如果要从`<object>_event view`引入其他字段，请将此查询的输出连接回`<object>_event view`。  连接字段应为： <br>
>>对于projects_event： 
>>`From projects_event p`
>>`Join <above query> c on c.projectid = p.projectid  `
>>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`



<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
