---
content-type: api
navigation-topic: api-navigation-topic
title: API版本8中的新增功能
description: 这是API版本9的新增资源列表。 有关已对版本8的资源进行的更新的列表，请访问API版本8的更新
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
TQID: https://experienceleague.adobe.com/bKFAN--rVO1yxgFLiyhXolgUBajVGYQxM7pBUuqy3v8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 269
ht-degree: 39%

---

# API版本8中的新增功能

## 新资源

这是API版本9的新增资源列表。 有关已对版本8的资源进行的更新的列表，请访问[对API版本8](../../wf-api/api/new-api-version-8-updates.md)的更新

**AgileWork**

| 字段 | 参考 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| backlogOrder | 客户 |   |   | bulkcopy  |   | 复制 |
| 颜色 | 迭代  |   |   |   |   | 计数 |
| 客户ID | lastUpdatedBy |   |   |   |   | 删除 |
| 预估 | op任务 |   |   |   |   | 编辑 |
| ID | 项目 |   |   |   |   | GET  |
| isReady | 情节提要父级 |   |   |   |   | 报告 |
| 迭代标识 | 任务 |   |   |   |   | SEARCH |
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

{style="table-layout:auto"}

### APIVersionMetadata

| 字段 | 参考 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 弃用版本 |   |   |   |   |   | 计数  |
| removalRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**KanbanBoard**

| 字段 | 参考 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 添加 |
| name |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | 删除 |
|   |   |   |   |   |   | 编辑 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ProofApprovalStatus

| 字段 | 参考 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**ProofFileMetadata**

| 字段 | 参考 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| documentVersionID | 文档版本 |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| 文件名 |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**ResourceBudgetedHour**

| 字段 | 参考 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 添加 |
| budgetedHours |   |   |   |   |   | 计数 |
| plannedBudgetedHours |   |   |   |   |   | 删除 |
| projectID |   |   |   |   |   | 编辑 |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ResourcePlannerFilter

| 字段 | 参考 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 添加 |
| name |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | 删除 |
|   |   |   |   |   |   | 编辑 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**富文本注释**

| 字段 | 参考 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### 订阅

| 字段 | 参考 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | 订阅者 | 添加 |
|   |   |   |   | removeSubscribers |   | 计数  |
|   |   |   |   | 订阅次数 |   | 删除 |
|   |   |   |   | 取消订阅 |   | GET |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### 用户角色

| 字段 | 参考 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| roleID | 角色 |   |   |   |   |   |
| timePercentage | 用户 |   |   |   |   |   |
| userID |   |   |   |   |   |   |
