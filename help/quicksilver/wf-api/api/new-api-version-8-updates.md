---
content-type: api
navigation-topic: api-navigation-topic
title: API版本8的更新
description: 以下现有资源已使用此版本的Adobe Workfront API进行更新。 要查看版本8的新资源，请参阅API版本8的新增功能。 对资源所做的更改以以下方式表示 — 编辑我。
author: John
feature: Workfront API
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 37%

---

# API版本8的更新

## 更新的资源

以下现有资源已使用此版本的Adobe Workfront API进行更新。 要查看版本8的新资源，请参阅 [API版本8的新增功能](../../wf-api/api/new-api-version-8.md). 以下方式表示对资源所做的更改：

* 添加内容仅列出
* 删除使用删除线文本进行指示
* 表后面的注释中会记录更改

### AccessRequest

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 操作¹  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

### AccessRule¹ 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| coreAction²  |   |   |   |   |   |   |
| forbiddenActions² |   |   |   |   |   |   |
| secondaryActions² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹标记已删除：可报告\
²对可能值的更改

### 审批

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  | resourcePools |   |   |   |   |
| backlogOrder² | 看板板  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改\
²添加了标记：动态、延迟读取和不分组

### 分配

|   |   |   |   | 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnTasks | getAssignmentForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignmentsForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 客户

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| bizRuleExclusions¹ |   |   |   | getPackagingOptionValue |   |   |
| proofPlan¹ |   |   |   | isPackagingOptionEnabled |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

### 客户首选项

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| name¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

### DocumentApproval

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹标记已添加：NOT_FILTERABLE

### DocumentVersion

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| activeProofStages |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 组

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   | 所有者 |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### HourType

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| appGlobalID¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹标记已添加：NOT_FILTERABLE

### 迭代

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | moveStories |   |   |

{style=&quot;table-layout:auto&quot;}

### 喜欢

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 注释

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| auditType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

### Op 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   | defaultShownedTimesleIssues  |   |
| 积压订单 | 迭代 |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| 估计 |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

### 项目组合

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

### 项目群

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

### 项目

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| auditTypes¹ |   | resourcePools |   |   | defaultShownedTimesleProjects |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

### 校样批准

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 审批者ID | 审批人 |   |   |   |   |   |
| documentVersionID | documentVersion |   |   |   |   |   |
| ID¹ |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹标记已添加：NOT_FILTERABLE

### QueueDef

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| requestorCoreAction¹ |   |   |   |   |   |   |
| requestorForbiddenActions¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

### 费率

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| name |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### ReservedTime

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| extRefID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### ResourceManager

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| projectPriority |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   | allTasksOnIterations  |   |
| backlogParent | 看板板 |   |   |   | defaultShownedTimeskeTasks |   |
| kanbanBoardID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

### 团队

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 敏捷方法 |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| teamStoryBoardIssueStatuses |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 模板

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 模板任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

更新

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| updateType¹ | `updateEndorsement` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

### 用户

|   |   | 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | userGroups |   |   |   |   |   |   |
|   |   | userRoles |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 用户说明

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

### 工作

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   |   |   |
| backlogOrder² | 看板板  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改\
²添加了标记：动态、延迟读取和不分组
