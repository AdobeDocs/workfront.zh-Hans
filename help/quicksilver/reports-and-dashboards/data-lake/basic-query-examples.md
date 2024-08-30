---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect查询示例
description: 您可以使用示例查询来熟悉特定类型查询的语法和结构。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: ffa599ff0e25ba960ce01f3f492482ee2e747122
workflow-type: tm+mt
source-wordcount: '245'
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

您需要将此信息包含在针对Data Connect的查询的响应中。 数据湖中记录的自定义数据值包含在标题为`parameterValues`的列中。 此列将存储为JSON对象。

### 查询：

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit" :: int as BusinessUnit,
    parametervalues:"DE:Project ID" :: int as ProjectID,
    parametervalues:"DE:Expanded Project Name" :: text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### 响应

上述查询返回以下数据：

* `projectid` — 本机Workfront项目ID
* `parametervalues` — 存储JSON对象的列
* `name` — 本机Workfront项目名称
* `Business Unit` - `parametervalues`对象中包含的自定义数据值
* `Project ID` - `parametervalues`对象中包含的自定义数据值
* `Expanded Project Name` - `parametervalues`对象中包含的自定义数据值

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
