---
content-type: api
navigation-topic: api-navigation-topic
title: API版本10中的新增功能
description: 已更新的资源
author: Becky
feature: Workfront API
role: Developer
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 39%

---

# API版本10中的新增功能

* [新资源](#new-resources)
* [已更新资源](#updated-resources)
* [已删除资源](#removed-resources)

## 新资源 {#new-resources}

### 活动日志

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | 添加 |
|   |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### 日历条目

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 添加 |
|   |   |   |   |   |   | 计数  |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | 编辑  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 报告  |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### CalendarEntryExternalReference

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 报告  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### ExternalAuthToken

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 添加 |
|   |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | 编辑  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 报告  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### LicenseTypeGroupLimit

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 客户ID | 客户 |   |   |   |   |   |
| groupID | 组 |   |   |   |   |   |
| planlimit |   |   |   |   |   |   |
| usedLicenses |   |   |   |   |   |   |
| 工作限制 |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserHomeCalendarPreference

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 客户ID | 客户 |   |   |   |   | 添加 |
| edTime | 用户 |   |   |   |   | 计数 |
| firstDayOfWeek |   |   |   |   |   | 删除 |
| ID |   |   |   |   |   | 编辑 |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | 报告 |
| userID |   |   |   |   |   | SEARCH |
| 工作日期 |   |   |   |   |   |   |

{style="table-layout:auto"}

**已更新资源**

以下现有资源已使用此版本的Workfront API进行了更新。 对资源所做的更改如下所示：

* 添加内容只会列出
* 删除以删除线文本指示
* 更改在表后面的注释中列出

### 审批

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval `<sup>1</sup>`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetedCost  |   |   |   |   |   |   |
| 项目净值  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost  |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup> Type changed from null to boolean`

### 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| assignmentPercent `<sup>1</sup>` |   |   |   |   |   |   |
| viewedByAssignedToUser |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup>`已添加验证器LESS_THAN_EQUAL

### BudgetedHour

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 客户首选项

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 名称`<sup>1</sup>` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对possibleValues的更改

### DocMetadataLinkGroup

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style="table-layout:auto"}

### 文档

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |   |   |   |   |   |

{style="table-layout:auto"}

### 文档请求

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

文档版本

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| externalIntegrationType <sup>1</sup> |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对possibleValues的更改

费用

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 组

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style="table-layout:auto"}

### 链接文件夹

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| externalIntegrationType<sup>1</sup> |  |  |  |  |   |   |

{style="table-layout:auto"}

<sup>1</sup>对possibleValues的更改

### Op 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| priorityColor |   |  | pendingApproval<sup>1</sup> |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>类型从null更改为布尔值

### 门户部分

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |  |   | groupIDs |   |   |   |

{style="table-layout:auto"}

### 项目组合

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 项目组合净值 |   |   |   |  |  |   |
| 项目组合Roi |   |   |   |   |   |   |

{style="table-layout:auto"}

### 项目

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| 项目净值 |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style="table-layout:auto"}

### ProofApproval

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| approverDecision |   |   |   |   |   |   |

{style="table-layout:auto"}

### 费率

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| rateValue <sup>1</sup> |  |  |  |  |  |   |

{style="table-layout:auto"}

<sup>1</sup>已添加验证方货币

### 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 团队

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| hoursPerPoint <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>已添加验证器LESS_THAN

### 团队分派

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 团队任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 时间表

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### 更新

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| updateType `<sup>1</sup>` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style="table-layout:auto"}

<sup>1</sup>更改了possibleValues

### 用户

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   | accesslevel  |   |   |   |   |   |

{style="table-layout:auto"}

### 用户注释

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| eventType <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>更改了possibleValues

### 工作

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval <sup>1</sup>  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>类型从null更改为布尔值

## 已删除资源 {#removed-resources}

### ResourceBudgetedHour

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 添加  |
| budgetedHours |   |   |   |   |   | 计数  |
| ID |   |   |   |   |   | DELETE  |
| plannedBudgetedHours |   |   |   |   |   | 编辑  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | 报告  |
| userID |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

 

 

 
