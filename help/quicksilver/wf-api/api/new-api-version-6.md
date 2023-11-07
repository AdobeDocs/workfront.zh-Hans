---
content-type: api
navigation-topic: api-navigation-topic
title: API版本6中的新增功能
description: API版本6中的新增功能
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 38%

---

# API版本6中的新增功能

## 新建对象

### 资源管理器

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID | 客户 |   |   |   |   | 添加 |
| 客户ID | 项目 |   |   |   |   | 计数 |
| projectID | 资源管理器 |   |   |   |   | 删除 |
| resourceManagerID | 模板 |   |   |   |   | Get |
| templateID |   |   |   |   |   | 报告  |
|   |   |   |   |   |   | 搜索  |


### Ews

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 文件名 |   |   |   |   | 上传 |   |
| 句柄 |   |   |   |   |   |   |
| 对象代码 |   |   |   |   |   |   |


### 自定义标签

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabel | 添加 |
|   |   |   |   | inUseByOtherLayoutTemplate | user自定义标签 | 计数 |
|   |   |   |   | removeCustomLabel |   | 删除 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | 搜索 |


## 已更新对象

对现有对象的更改：只列出添加项，删除项具有删除线，对现有对象的更改在表后具有附加注释

### 更新

 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> 对可能值的更改

<sup>2</sup> hasFilters属性已更改为true

 

### 审批

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| completedHours |   | 资源管理器 | resourceManagerIDs |   |   |   |
| 约束日期<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| 所需工作<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 已添加日期验证

<sup>2</sup> 已添加NOT_FILTERABLE标志

 

### 批准流程

|   | 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### 审批步骤

 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 对可能值的更改

 

### 批准路径<sup>1</sup>

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | 添加 |
| approvedStatusLabs |   |   |   |   |   | 计数 |
| 备注 |   |   |   |   |   | 删除 |
| enteredById |   |   |   |   |   | 编辑 |
| entryDate |   |   |   |   |   | Get |
| globalPathID |   |   |   |   |   | 报告 |
| isPrivate |   |   |   |   |   | 搜索 |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| name<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 更改为可报告

<sup>2</sup> 添加了最大长度验证器

 

### 工作服务对象

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 约束日期<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| 所需工作<sup>2</sup> |   |   |   | workitemstatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup> 已添加日期验证

<sup>2</sup> 已添加Not_Filterable标志

 

### 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProject |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignuserfromprojects |   |   |

{style="table-layout:auto"}

 

### 基线 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 所需工作<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 已添加Not_Filterable标志

 

### 基线任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 所需工作<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 已添加Not_Filterable标志

 

### 开票记录

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 添加了NO_TIME字段标志

### 燃尽事件 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### 类别 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

自定义枚举 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatures |   |
|   |   |   |   |   | taskGroupStatures |   |

{style="table-layout:auto"}

 

文档 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

汇率 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 费率<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 将PRECISION验证器更改为8到9

 

### 集成

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 日志条目

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 对可能值的更改

 

### Optask（问题）<sup>1</sup> 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 所需工作<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 标记为可恢复

<sup>2</sup> 已添加Not_Filterable标志

 

### 项目<sup>1</sup> 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | 资源管理器 | resourceManagerIDs  |   |   |   |
| originalworkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| 工作 |   |   |   |   |   |   |
| 所需工作 |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 标记为“可恢复”和“资源可管理”

<sup>2</sup> 已添加Not_Filterable标志

 

### 任务<sup>1</sup>

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 约束日期<sup>2</sup> |   |   |   |   |   |   |
| 所需工作<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 标记为可恢复

<sup>2</sup> 已添加AT_DATE_YEAR_BEFORE验证器

<sup>3</sup> 已添加Not_Filterable标志

 

### 团队

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### 模板<sup>1</sup> 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   | 资源管理器 | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 标记为“可恢复”和“资源可管理”

### 模板任务<sup>1</sup> 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 所需工作<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 标记为可恢复

<sup>2</sup> 已添加Not_Filterable标志

 

### 用户

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> MAX_LENGTH违规者

 

### 用户注释

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 事件类型<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> 可能的值已更改

<sup>2</sup> 已将筛选器更改为 `[true]`

 

### 公告

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
