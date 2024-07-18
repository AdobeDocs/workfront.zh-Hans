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
source-wordcount: '538'
ht-degree: 34%

---

# API版本6中的新增功能

## 新建对象

### 资源管理器

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID | 客户 |   |   |   |   | 添加 |
| 客户ID | 项目 |   |   |   |   | 计数 |
| projectID | 资源管理器 |   |   |   |   | 删除 |
| resourceManagerID | 模板 |   |   |   |   | Get |
| templateID |   |   |   |   |   | 报表  |
|   |   |   |   |   |   | Search  |


### Ews

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 文件名 |   |   |   |   | 上传 |   |
| 句柄 |   |   |   |   |   |   |
| 对象代码 |   |   |   |   |   |   |


### 自定义标签

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
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

 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

<sup>2</sup> hasFilters属性已更改为true

 

### 审批

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| completedHours |   | 资源管理器 | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| 工作必需<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

已添加<sup>1</sup>日期验证

已添加<sup>2</sup> NOT_FILTERABLE标志

 

### 审批流程

|   | 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### 审批步骤

 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

 

### 审批路径<sup>1</sup>

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | 添加 |
| approvedStatusLabs |   |   |   |   |   | 计数 |
| 注释 |   |   |   |   |   | 删除 |
| enteredById |   |   |   |   |   | 编辑 |
| entryDate |   |   |   |   |   | Get |
| globalPathID |   |   |   |   |   | 报告 |
| isPrivate |   |   |   |   |   | 搜索 |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| 名称<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>已更改为可报告

<sup>2</sup>已添加最大长度验证器

 

### 工作服务对象

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| 工作必需<sup>2</sup> |   |   |   | workitemstatusLabels  |   |   |

{style="table-layout:auto"}

已添加<sup>1</sup>日期验证

已添加<sup>2</sup> Not_Filterable标志

 

### 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProject |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignuserfromprojects |   |   |

{style="table-layout:auto"}

 

### 基线 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 工作必需<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

已添加<sup>1</sup> Not_Filterable标志

 

### 基线任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 工作必需<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

已添加<sup>1</sup> Not_Filterable标志

 

### 账单记录

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>添加了NO_TIME字段标志

### 燃尽事件 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### 类别 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

自定义枚举 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatures |   |
|   |   |   |   |   | taskGroupStatures |   |

{style="table-layout:auto"}

 

文档 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

汇率 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 费率<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>已将PRECISION验证器更改为8到9

 

### 集成

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 日志条目

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

 

### Optask （问题）<sup>1</sup> 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 工作必需<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>标记为可恢复

已添加<sup>2</sup> Not_Filterable标志

 

### 项目<sup>1</sup> 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | 资源管理器 | resourceManagerIDs  |   |   |   |
| originalworkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| 工作 |   |   |   |   |   |   |
| 所需工作 |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>标记为可恢复且资源可管理

已添加<sup>2</sup> Not_Filterable标志

 

### 任务<sup>1</sup>

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| 工作必需<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>标记为可恢复

<sup>2</sup> AT_DATE_YEAR_BEFORE验证器已添加

已添加<sup>3</sup> Not_Filterable标志

 

### 团队

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### 模板<sup>1</sup> 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   | 资源管理器 | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>标记为可恢复且资源可管理

### 模板任务<sup>1</sup> 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 工作必需<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>标记为可恢复

已添加<sup>2</sup> Not_Filterable标志

 

### 用户

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>个MAX_LENGTH违规者

 

### 用户注释

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup>可能的值已更改

<sup>2</sup>的筛选器已更改为`[true]`

 

### 公告

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
