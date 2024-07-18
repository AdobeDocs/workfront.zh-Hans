---
content-type: api
navigation-topic: api-navigation-topic
title: API版本8的更新
description: 查看API版本8的更新。
author: Becky
feature: Workfront API
role: Developer
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 31%

---

# API版本8的更新

## 已更新的资源

以下现有资源已使用此版本的Adobe Workfront API进行了更新。 要查看版本8的新资源，请参阅[API版本8](../../wf-api/api/new-api-version-8.md)的新增功能。 对资源所做的更改按以下方式表示：

* 添加内容只会列出
* 删除以删除线文本指示
* 更改会记录在表后面的注释中

### Accessrequest

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 操作<sup>1</sup>  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

### 访问规则<sup>1</sup> 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| coreAction<sup>2</sup>  |   |   |   |   |   |   |
| forbiddenActions<sup>2</sup> |   |   |   |   |   |   |
| secondaryActions<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

已移除<sup>1</sup>标记：可报告\
<sup>2</sup>对可能值的更改

### 审批

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  | resourcePools |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改\
<sup>2</sup>已添加标志：动态、LAZY_READ和NOT_GROUPABLE

### 任务

|   |   |   |   | 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnTasks | getAssignAssignmentsForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignAssignmentsForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style="table-layout:auto"}

### 客户

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |   |   |   | Getpackagingoptionvalue |   |   |
| proofPlan<sup>1</sup> |   |   |   | isPackagingOptionEnabled |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

### 客户首选项

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 名称<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

### 文档审批

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

已添加<sup>1</sup>标志： NOT_FILTERABLE

### 文档版本

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| activeProofStages |   |   |   |   |   |   |

{style="table-layout:auto"}

### 组

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   | 所有者 |   |   |   |   |

{style="table-layout:auto"}

### 小时类型

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| appGlobalID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

已添加<sup>1</sup>标志： NOT_FILTERABLE

### 迭代

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   |   |   | 移动故事 |   |   |

{style="table-layout:auto"}

### 类似

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style="table-layout:auto"}

### 注释

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| auditType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

### Op 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   | defaultShownTimesheetIssues  |   |
| backlogOrder | 迭代 |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| 预估 |   |   |   |   |   |   |
| 迭代标识 |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

### 项目组合

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

### 项目群

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

### 项目

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   | resourcePools |   |   | defaultShownTimesheetProjects |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

### ProofApproval

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| approverID | 审批者 |   |   |   |   |   |
| documentVersionID | 文档版本 |   |   |   |   |   |
| ID<sup>1</sup> |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style="table-layout:auto"}

已添加<sup>1</sup>标志： NOT_FILTERABLE

### QueueDef

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| requestorCoreAction<sup>1</sup> |   |   |   |   |   |   |
| requestorForbiddenActions<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

### 费率

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| name |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style="table-layout:auto"}

### 保留时间

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| extRefId |   |   |   |   |   |   |

{style="table-layout:auto"}

### 资源管理器

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 项目优先级 |   |   |   |   |   |   |

{style="table-layout:auto"}

### 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   | allTasksOnIterations  |   |
| backlogParent | kanbanBoard |   |   |   | defaultShownTimesheetTasks |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

### 团队

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 敏捷方法 |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| teamStoryBoardIssueStatuses |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style="table-layout:auto"}

### 模板

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style="table-layout:auto"}

### TemplateTask

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

更新

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> | `updateEndorsement` |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

### 用户

|   |   | 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | 用户组 |   |   |   |   |   |   |
|   |   | 用户角色 |   |   |   |   |   |   |

{style="table-layout:auto"}

### 用户注释

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

### 工作

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改\
<sup>2</sup>已添加标志：动态、LAZY_READ和NOT_GROUPABLE
