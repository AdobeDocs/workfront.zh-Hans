---
content-type: api
navigation-topic: api-navigation-topic
title: API版本6的新增功能
description: API版本6的新增功能
author: John
feature: Workfront API
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 2ec05c03a5bfa842008870ca47fb617b81fd6ebd
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 42%

---

# API版本6的新增功能

## 新建对象

### 资源管理器

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID | 客户 |   |   |   |   | 添加 |
| customerID | 项目 |   |   |   |   | 计数 |
| projectID | resourceManager |   |   |   |   | 删除 |
| resourceManagerID | 模板 |   |   |   |   | 获取 |
| templateID |   |   |   |   |   | 报告  |
|   |   |   |   |   |   | 搜索  |


### Ews

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | 上传 |   |
| 句柄 |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### 自定义标签

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | 添加 |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | 计数 |
|   |   |   |   | removeCustomLabel |   | 删除 |
|   |   |   |   |   |   | 获取 |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | 搜索 |


## 更新的对象

对现有对象的更改：只列出了“添加”，“移除”具有“删除”，对现有的更改在表后面附加了注释

### 更新

 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| updateType¹ |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID² |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

² hasFilters属性更改为true

 

### 审批

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate¹ |   |   |   |   |   |   |
| isOriginalPlanedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹添加了日期验证

²添加了NOT_FILTERABLE标记

 

### 批准流程

|   | 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|---|
|  |  | `attachedApprovalPaths` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 批准步骤

 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| approvalType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

 

### 批准路径¹

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | 添加 |
| approvedStatusLabel |   |   |   |   |   | 计数 |
| 备注 |   |   |   |   |   | 删除 |
| enteredByID |   |   |   |   |   | 编辑 |
| entryDate |   |   |   |   |   | 获取 |
| globalPathID |   |   |   |   |   | 报告 |
| isPrivate |   |   |   |   |   | 搜索 |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| name² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹更改为可报告

²添加了最大长度验证器

 

### 工作服务对象

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| constraintDate¹ |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired² |   |   |   | workItemStatusLabels  |   |   |

{style=&quot;table-layout:auto&quot;}

¹添加了日期验证

²添加了不可过滤标记(_F)

 

### 分配

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 基线 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹添加了不可过滤标记(_F)

 

### 基线任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹添加了不可过滤标记(_F)

 

### 开票记录

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| billingDate¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹添加了NO_TIME字段标记

### 燃耗事件 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style=&quot;table-layout:auto&quot;}

 

### 类别 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style=&quot;table-layout:auto&quot;}

 

自定义枚举 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatusses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatuss |   |
|   |   |   |   |   | taskGroupStatusses |   |

{style=&quot;table-layout:auto&quot;}

 

文档 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

汇率 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| rate¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹更改了8到9的PRECISION验证器

 

### 集成

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 日志条目

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| changeType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

 

### Optask（问题）¹ 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹标记为可恢复

²添加了不可过滤标记(_F)

 

### 项目¹ 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlanedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| 工作 |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹标记为可恢复和资源_可管理

²添加了不可过滤标记(_F)

 

### 任务¹

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| constraintDate² |   |   |   |   |   |   |
| workRequired³ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹标记为可恢复

²添加了AT_DATE_YEAR_BEFORE验证器

³添加了不可过滤标记(_F)

 

### 团队

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 模板¹ 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹标记为可恢复和资源_可管理

### 模板任务¹ 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹标记为可恢复

²添加了不可过滤标记(_F)

 

### 用户

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| myInfo¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ MAX_LENGTH违规者

 

### 用户说明

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| eventType¹ |   |   |   |   | myNotifications² |   |

{style=&quot;table-layout:auto&quot;}

¹可能值已更改

²已将过滤器更改为 `[true]`

 

### 公告

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
