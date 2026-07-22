---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect查询示例
description: 您可以使用示例查询来熟悉特定类型查询的语法和结构。
author: Courtney
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/flDonZVaLR3bTF2aZcY9iy2ZnWbfrdhctL7J8esvxng
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: edee967a5c19d86fd471c4571a0b458f72bf370e
workflow-type: tm+mt
source-wordcount: 2201
ht-degree: 0%

---

# Workfront Data Connect查询示例

为了帮助您更好地利用Workfront Data Connect数据，本页包含一些基本的示例查询，您可以使用这些查询来熟悉特定类型查询的语法和结构。

## 自定义数据查询

此示例演示如何在Workfront中构建查询以返回自定义数据，如自定义表单和自定义字段。

### 场景

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

### 场景

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

查询使用Data Connect的更改事件跟踪功能。它确定触发事件的日期，该事件的新状态值与上一个事件不同。 

从内到外检查查询： 

1. 计算先前状态不同的记录： 
   * 对于每个更改事件，使用lag()函数来标识状态的上一个值。 

2. 仅筛选已更改的记录： 

   * 从步骤1中的计算中选择记录，其中前一个状态!=当前状态。 

3. 以天为单位计算开始/结束有效时间戳和持续时间： 

   * `<status_begin_effective_timestamp>`：在步骤2中计算。 

   * `<status_end_effective_timestamp>`：根据下一个(lead())进行计算。 `<status_begin_effective_timestamp>`：仅在`<status_begin_effective_timestamp>`不为NULL时显示状态。 
   * `<status_duration_days>`： `<status_begin_effective_timestamp>`和`<status_end_effective_timestamp>`之间的数据差异。 

>[!NOTE]
>
>建议在PowerBI或Tableau中将此查询用作自己的“视图”。如果要从`<object>_event view`引入其他字段，请将此查询的输出连接回`<object>_event view`。连接字段应为： <br>
>对于projects_event： 
>`From projects_event p`>`Join <above query> c on c.projectid = p.projectid  `>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`

## Planning：单个记录类型查询

此示例演示如何查询Workfront Planning数据，以查找存储在Data Connect数据湖中的单个记录类型。

### 场景

您的组织使用Workfront Planning跟踪活动。 每个Campaign记录包括名称、状态、开始日期、结束日期和所有者。 您需要提取所有活动营销活动及其关键详细信息的列表，以供在功能板中使用。

* 规划记录类型数据存储在PLANNINGRECORD_CURRENT视图中。
* 每一行表示一个记录，并且所有字段值都存储在名为FIELD_VALUES的JSON列中。
* 记录类型由RECORDTYPEID列标识。
* 记录的工作区由WORKSPACEID列（或人类可读筛选器的WORKSPACENAME列）标识。

### 查询

```sql
SELECT
  recordid,
  FIELD_VALUES:"Name"::text AS campaign_name,
  FIELD_VALUES:"Status"::text AS campaign_status,
  FIELD_VALUES:"Start Date"::date AS start_date,
  FIELD_VALUES:"End Date"::date AS end_date,
  FIELD_VALUES:"Owner"::text AS owner
FROM PLANNINGRECORD_CURRENT
WHERE WORKSPACEID = '<your_campaign_workspace_id>'
AND RECORDTYPEID = '<your_campaign_record_type_id>'
AND FIELD_VALUES:"Status"::text = 'Active'
ORDER BY start_date ASC
```

### 响应

上述查询返回以下数据：

* **recordid**：营销活动的唯一规划记录ID。
* **campaign_name**：从FIELD_VALUES JSON对象提取的营销活动名称。
* **campaign_status**：营销活动的当前状态。
* **start_date**：营销活动的开始日期，转换为日期数据类型。
* **end_date**：营销活动的结束日期，强制转换为日期数据类型。
* **所有者**：分配为营销活动所有者的用户或团队的名称。

### 解释

Data Connect中的Planning记录共享单个表结构，而不管记录类型如何。 RECORDTYPEID列用于将查询范围限定为特定的记录类型，在本例中为“促销活动”。 将`<your_campaign_record_type_id>`替换为您要查询的记录类型的ID，可在Workfront Planning记录类型设置中或通过查询RECORDTYPE_CURRENT找到该ID。

字段值作为JSON对象存储在FIELD_VALUES列中，可使用与自定义表单数据相同的冒号表示法访问：

```
<field_column>:"<field_name>"::<data_type> AS <alias>
```

字段名称引用必须与在Planning记录类型字段配置中定义的字段名称完全匹配，包括大小写、间距和表情符号。

>[!NOTE]
>
>在Workfront Planning中查看记录类型时，可以在URL中找到Planning记录类型ID。 它是以“Rt...”开头的URL的路径。 也可以在Data Connect中使用以下SQL调用找到记录类型：
>
>
>```sql
>SELECT
>ID AS recordtypeid,
>DISPLAYNAME AS record_type_name,
>WORKSPACEID
>FROM RECORDTYPE_CURRENT
>ORDER BY record_type_name ASC
>```

## Planning：连接的记录类型查询

此示例演示如何跨两个连接的Planning记录类型（父记录类型及其连接的记录类型）查询数据。

### 场景

贵组织在Workfront Planning中将Campaign记录关联到策略记录。 您希望生成一份报告，其中显示每个营销活动及其相关战术的关键详细信息。 他们特别希望显示策略名称、策略优先级和预算分配，以便领导可以审查按策略组织的营销活动。

在数据连接中，本地Planning记录类型之间的连接直接存储在PLANNINGRECORD_CURRENT的FIELD_VALUES_RAW列中。 对于名为“战术”的参考字段，该值是连接的记录对象的JSON数组，每个记录对象都包含具有连接记录的RECORDID的id属性。 使用Snowflake的LATERAL FLATTEN将此数组展开为行，并连接到连接的记录类型。

### 查询

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  t.FIELD_VALUES:"Name"::text AS tactic_name,
  t.FIELD_VALUES:"Strategic Priority"::text AS strategic_priority,
  t.FIELD_VALUES:"Budget Allocation"::float AS budget_allocation
FROM PLANNINGRECORD_CURRENT c,
INNER JOIN REFERENCE_CURRENT R 
ON r.FROM_REFERENCEID = c.REFERENCE_IDS:"Tactics"::text
INNER JOIN PLANNINGRECORD_CURRENT t
-- Join to the Tactic record using the connected record ID from the array
ON t.RECORDID = r.TO_RECORDID
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
ORDER BY tactic_name, campaign_name
```

### 响应

上述查询返回以下数据：

* **campaign_id**：营销活动的唯一规划记录ID。
* **campaign_name**：营销活动记录的名称。
* **campaign_status**：营销活动的当前状态。
* **tactics_name**：连接的策略记录的名称。
* **strategic_priority**：所连接“策略”记录的“策略优先级”字段值。
* **budget_allocation**：已连接策略记录中的“预算分配”字段值，强制转换为浮点数。

### 解释 — 修改的KP

本机Planning记录类型之间的连接存储在REFERENCE_CURRENT联接表中。  REFERENCE_CURRENT联接表用于RecordType之间的联接。   在RecordType之间连接时，应使用TO_RECORDID字段。

PLANNINGRECORD视图中的REFERENCE_ID列包含适用于该计划记录的所有REFERENCEID字段的列表。 您可以使用与field_value相同的JSON表示法来访问ID。

```
<reference_ids>:"<reference_name>"::text
```

REFERENCE_CURRENT视图包含一个或多个记录，其中TO_RECORDID指向PLANNINGRECORD_*视图中的其他计划`recordId`字段。

要将另一个REFERENCE字段联接到其他Planning记录，则上述查询中将添加与REFERENCE_CURRENT和PLANNINGRECORD_*相同的联接到模式。


## 规划：记录类型已联接到工作流数据查询Workfront

此示例演示如何使用Planning的本机连接功能（该功能将外部对象引用存储在REFERENCE_CURRENT视图中）将Workfront Planning记录类型连接到本机Workfront工作流对象（在本例中为“项目”）。

### 场景

贵组织使用Planning的本机连接功能将Workfront Planning中的Campaign记录连接到Workfront项目。 您要生成一个组合报告，其中显示活动详细信息以及链接项目的实时执行数据（特别是项目的当前完成百分比、计划完成日期和已分配项目所有者），以便活动经理可以跟踪投放进度，而无需离开其Planning工作区上下文。

### 查询

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  conn.TO_EXTERNALID AS linked_project_id,
  p.name AS project_name,
  p.percentcomplete AS project_percent_complete,
  p.plannedcompletiondate AS project_planned_completion,
  p.ownerid AS project_owner_id,
  u.name AS project_owner_name
FROM WORKFRONT.PLANNING.PLANNINGRECORD_CURRENT c
-- Join to the references table to find Workfront Project connections
INNER JOIN WORKFRONT.PLANNING.REFERENCE_CURRENT conn
ON conn.REFERENCE_ID = c.REFERENCE_IDS:"ProjectId"::text
-- Join to the Workfront Projects table on the external ID
INNER JOIN WORKFRONT.WF.PROJECTS_CURRENT p
ON p.projectid = conn.TO_EXTERNALID
-- Join to Users to resolve the project owner name
LEFT JOIN WORKFRONT.WF.USERS_CURRENT u
ON u.userid = p.ownerid
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
AND p.completiontype != 'CPL' -- Exclude completed projects
ORDER BY campaign_name
```

### 响应

上述查询返回以下数据：

* **campaign_id**：营销活动的唯一规划记录ID。
* **campaign_name**：营销活动记录的名称。
* **campaign_status**：营销活动的当前状态，从“计划”开始。
* **linked_project_id**：来自REFERENCE_CURRENT.TO_EXTERNALID的Workfront项目ID，用于标识连接的Workfront项目。
* **project_name**：来自PROJECTS_CURRENT的本机Workfront项目名称。
* **project_percent_complete**：项目的当前完成百分比值。
* **project_planned_completion**：链接的Workfront项目的计划完成日期。
* **project_owner_id**：项目所有者的Workfront用户标识。
* **project_owner_name**：通过加入USERS_CURRENT解析的项目所有者的显示名称。

### 解释

从Planning记录类型到本机Workfront工作流对象的连接存储在REFERENCE_CURRENT中。 此视图中的每一行表示一个方向链接：TO_EXTERNALID保存连接的Workfront对象的ID。 表示Workfront连接的行由`TO_EXTERNALCONNECTIONNAME = 'workfront'`和与该Workfront对象类型的API代码（例如，项目的PROJ）相对应的TO_EXTERNALOBJECTNAME值标识。

PLANNINGRECORD表中的REFERENCE_ID列包含适用于该记录的所有REFERENCEID字段的列表。  您可以使用与field_value相同的JSON表示法来访问ID。\
PLANNINGRECORD_CURRENT中的单个REFERENCE_ID可以包含REFERENCE_CURRENT表中链接到Workfront表中特定对象类型对象的一个或多个引用链接。

```
<reference_ids>:"<reference_name>"::text
```

请注意，Planning视图(PLANNINGRECORD_CURRENT、REFERENCE_CURRENT)位于WORKFRONT.PLANNING架构中，而本机Workfront工作流视图（PROJECTS_CURRENT、USERS_CURRENT等）位于 驻留在WORKFRONT.WF架构中。 跨模式连接需要完全限定的表名。

查询执行三个联接：

1. **引用表** REFERENCE_CURRENT的Planning记录在`TO_RECORDID = c.RECORDID`上联接，以查找源自每个Campaign记录的所有连接。 `TO_EXTERNALCONNECTIONNAME = 'workfront'`和`TO_EXTERNALOBJECTNAME = 'PROJ'`上的筛选器将结果范围缩小到专门表示与Workfront项目的连接的行。
1. **对Workfront项目的引用表：** TO_EXTERNALID包含所连接项目的本机Workfront projectid。 此项目直接加入`PROJECTS_CURRENT.projectid`以检索实时项目数据。
1. **用户项目：** USERS_CURRENT的LEFT JOIN将项目上的ownerid外键解析为人类可读的名称。 此处使用LEFT JOIN，以便仍可在结果中包含未分配所有者的项目。

>[!NOTE]
>
>当联接到Planning外部的表时，请勿使用查询中的TO_RECORDID字段。  在连接到外部表时不需要它。
>
>此模式可应用于Planning支持连接的任何Workfront Workflow对象，如项目、项目组合或程序，方法是将TO_EXTERNALOBJECTNAME过滤器更改为相应的对象API代码（例如，项目组合的PORT或程序的PRGM），然后加入相应的WORKFRONT.WF表。 有关每种对象类型的正确表和ID列名称，请参阅Workfront Data Connect数据字典。

要将另一个REFERENCE字段连接到其他外部记录，与上述加入REFERENCE_CURRENT和Workfront Workflow视图的模式相同的模式将被添加到上述查询中。

通过使用适当的联接模式多次联接到REFERENCE_CURRENT表，可以在同一查询中联接外部和Planningrecord值。


<!--
## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.
-->
