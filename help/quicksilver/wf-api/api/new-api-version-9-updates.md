---
content-type: api
navigation-topic: api-navigation-topic
title: API版本9的更新
description: 更新的资源
author: John
feature: Workfront API
exl-id: 51892846-d93f-4363-8416-4118fb2ef84d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 47%

---

# API版本9的更新

## 更新的资源

以下现有资源已使用此版本的Adobe Workfront API进行更新。 要查看版本9中的新资源，您可以访问 [API版本9的新增功能](../../wf-api/api/new-api-version-9.md) 和 [API版本9的新增功能（续）](../../wf-api/api/new-api-version-9-continue.md). 以下方式表示对资源所做的更改：

* 添加内容仅列出
* 删除使用删除线文本进行指示
* 表后面的注释中会记录更改

### AgileWork

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `opTaskID`<sup>2</sup> |  |  |  |  |  |  |
| `taskID`<sup>2</sup> |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹标记已删除：可报告\
²标记已删除：NOT_GROUPABLE

### 审批

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

分配

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|  |  |  |  | `assignUserToRoleOnProjects`<sup>1</sup> |  |  |
|  |  |  |  | `assignUserToRoleOnTasks`<sup>1</sup> |  |  |
|  |  |  |  | `swapUsersOnProjects`<sup>1</sup> |  |  |
|  |  |  |  | `swapUsersOnTasks`<sup>1</sup> |  |  |

{style=&quot;table-layout:auto&quot;}

¹添加了以下字段：lockToRole

### 客户首选项

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup> |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对possibleValues的更改

### 小时

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `days` |  |  |  |  |  |  |
| `workHoursPerDay` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 迭代

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|  |  |  |  | `moveIssues` |  |  |

{style=&quot;table-layout:auto&quot;}

### 布局模板

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `groupID` | `group` |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 注释

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `html` |  |  |  |  |  |  |
| `json` |  |  |  |  |  |  |
| `richTextNoteID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Op 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `color` | `agileWork` |  |  | `convertToProject` |  |  |
| `isReady` |  |  |  | `convertToTask` |  |  |
| `storyBoardOrder` |  |  |  | `linkExternalObject` |  |  |
|  |  |  |  | `unlinkExternalObject` |  |  |

{style=&quot;table-layout:auto&quot;}

### 资源预算

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `ID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹标记已删除：可报告

### 计划

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `homeGroupID` | `homeGroup` |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|  | `agileWork` |  |  | `convertToProject` |  |  |
|  |  |  |  | `linkExternalObject` |  |  |
|  |  |  |  | `unlinkExternalObject` |  |  |

{style=&quot;table-layout:auto&quot;}

### 团队

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `includeIssues` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 时间表配置文件

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `groupID` | `group` |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### UIFilter

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|  |  |  |  |  | `filtersForObjCode` |  |

{style=&quot;table-layout:auto&quot;}

### UIView

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|  |  |  |  |  | `viewsForObjCode` |  |

{style=&quot;table-layout:auto&quot;}

### 用户

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `logTimeInDays` |  |  |  |  |  |  |
| `workHoursPerDay` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 工作

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |  |  | `getWFHomeObjects` |  |  |
