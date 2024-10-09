---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect查询示例
description: 您可以使用示例查询来熟悉特定类型查询的语法和结构。
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Workfront Data Connect查询示例

为了帮助您更好地利用Workfront Data Connect数据，本页包含一些基本的示例查询，您可以使用这些查询来熟悉特定类型查询的语法和结构。

## 自定义数据查询

此示例演示如何在Workfront中构建查询以返回自定义数据，如自定义表单和自定义字段。

### 方案：

您的组织使用名为Finance Integration的自定义表单。 该表单附加到每个项目，并包含以下字段：

* **业务单元** — 包含字符串的自定义字段。
* **ProjectID** — 包含数字字符串的自定义字段。
* **扩展的项目名称** — 计算出的自定义数据字段，它将业务单元、项目ID和本机Workfront项目名称的值连接到单个字符串中。

您需要将此信息包含在针对Data Connect的查询的响应中。 数据湖中记录的自定义数据值包含在标题为`parametervalues`的列中。 此列将存储为JSON对象。

### 查询：

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

### 响应：

上述查询返回以下数据：

* `projectid` — 本机Workfront项目ID
* `parametervalues` — 存储JSON对象的列
* `name` — 本机Workfront项目名称
* `Business Unit` - `parametervalues`对象中包含的自定义数据值
* `Project ID` - `parametervalues`对象中包含的自定义数据值
* `Expanded Project Name` - `parametervalues`对象中包含的自定义数据值

### 说明：

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

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
