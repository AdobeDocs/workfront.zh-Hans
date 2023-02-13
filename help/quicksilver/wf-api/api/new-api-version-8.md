---
content-type: api
navigation-topic: api-navigation-topic
title: API版本8的新增功能
description: 这是API版本9新增的资源列表。 有关已对版本8的资源进行的更新列表，请访问API版本8的更新
author: John
feature: Workfront API
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 32%

---

# API版本8的新增功能

## 新资源

这是API版本9新增的资源列表。 有关已对版本8的资源进行更新的列表，请访问 [API版本8的更新](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 积压订单 | 客户 |   |   | bulkCopy  |   | 复制 |
| 颜色 | 迭代  |   |   |   |   | 计数 |
| customerID | lastUpdatedBy |   |   |   |   | 删除 |
| 估计 | opTask |   |   |   |   | 编辑 |
| ID | 项目 |   |   |   |   | GET  |
| isReady | storyboardParent |   |   |   |   | 报表 |
| iterationID | 任务 |   |   |   |   | SEARCH |
| lastUpdateDate | 团队 |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| 类型 |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### APIVersionMetadata

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | 计数  |
| removalRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | 报表 |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**看板板**

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 添加 |
| name |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | 删除 |
|   |   |   |   |   |   | 编辑 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 报表 |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ProofApprovalStatus

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ProofFileMetadata**

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ResourceBudgetedHour**

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 添加 |
| budgededHours |   |   |   |   |   | 计数 |
| planedBudgededHours |   |   |   |   |   | 删除 |
| projectID |   |   |   |   |   | 编辑 |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | 报表 |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ResourcePlannerFilter

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 添加 |
| name |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | 删除 |
|   |   |   |   |   |   | 编辑 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 报表 |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**富文本注释**

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 报表 |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### 订阅

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | 订阅者 | 添加 |
|   |   |   |   | removeSubscribers |   | 计数  |
|   |   |   |   | 订阅 |   | 删除 |
|   |   |   |   | 取消订阅 |   | GET |
|   |   |   |   |   |   | 报表 |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### 用户角色

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| roleID | 角色 |   |   |   |   |   |
| timePercentage | 用户 |   |   |   |   |   |
| userID |   |   |   |   |   |   |
