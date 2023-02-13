---
content-type: api
navigation-topic: api-navigation-topic
title: API版本10的新增功能
description: 更新的资源
author: John
feature: Workfront API
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 46%

---

# API版本10的新增功能

* [新资源](#new-resources)
* [更新的资源](#updated-resources)
* [已删除的资源](#removed-resources)

## 新资源 {#new-resources}

### ActivityLog

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | 添加 |
|   |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### 日历条目

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 添加 |
|   |   |   |   |   |   | 计数  |
|   |   |   |   |   |   | 删除  |
|   |   |   |   |   |   | 编辑  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 报表  |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### CalendarEntryExternalReference

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 报表  |
|   |   |   |   |   |   | SEARCH  |

{style=&quot;table-layout:auto&quot;}

### ExternalAuthToken

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 添加 |
|   |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | 删除  |
|   |   |   |   |   |   | 编辑  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 报表  |
|   |   |   |   |   |   | SEARCH  |

{style=&quot;table-layout:auto&quot;}

### LicenseTypeGroupLimit

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| customerID | 客户 |   |   |   |   |   |
| groupID | 组 |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedLicenses |   |   |   |   |   |   |
| 工作限制 |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### UserHomeCalendarPreference

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| customerID | 客户 |   |   |   |   | 添加 |
| edTime | 用户 |   |   |   |   | 计数 |
| firstDayOfWeek |   |   |   |   |   | 删除 |
| ID |   |   |   |   |   | 编辑 |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | 报表 |
| userID |   |   |   |   |   | SEARCH |
| workDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**更新的资源**

以下现有资源已使用此版本的Workfront API进行更新。 对资源所做的更改如下所示：

* 添加内容仅列出
* 删除使用删除线文本进行指示
* 更改列在表后面的注释中

### 审批

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval `¹`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgededCost  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgededLaborCost  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

`¹ Type changed from null to boolean`

### 分配

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| assignmentPercent `¹` |   |   |   |   |   |   |
| viewedByAssignedToUser |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

`¹`添加了验证器LESS_THAN_EQUAL

### BudgededHour

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 客户首选项

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| name `¹` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对possibleValues的更改

### DocMetadataLinkGroup

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style=&quot;table-layout:auto&quot;}

### 文档

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### DocumentRequest

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

DocumentVersion

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| externalIntegrationType ¹ |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对possibleValues的更改

费用

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 组

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style=&quot;table-layout:auto&quot;}

### LinkedFolder

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| externalIntegrationType¹ |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹对possibleValues的更改

### Op 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| priorityColor |  |  | pendingApproval¹ |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹类型从null更改为布尔值

### PortalSection

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|  |  |  | groupIDs |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 项目组合

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| portfolioNetValue |  |  |  |  |  |  |
| portfolioRoi |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 项目

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| projectBudgededCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgededLaborCost |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 校样批准

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 审批者决策 |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 费率

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| rateValue ¹ |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹添加了验证器货币

### 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 团队

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| hoursPerPoint ¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹添加了验证器LESS_THAN

### TeamAssignment

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### TeamTask

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 时间表

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 更新

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| updateType `¹` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style=&quot;table-layout:auto&quot;}

¹对possibleValues的更改

### 用户

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 用户说明

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| eventType ¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对possibleValues的更改

### 工作

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval ¹  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹类型从null更改为布尔值

## 已删除的资源 {#removed-resources}

### ResourceBudgetedHour

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 添加  |
| budgededHours |   |   |   |   |   | 计数  |
| ID |   |   |   |   |   | 删除  |
| planedBudgededHours |   |   |   |   |   | 编辑  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | 报表  |
| userID |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

 

 

 
