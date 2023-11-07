---
content-type: api
navigation-topic: api-navigation-topic
title: API版本8中的新增功能
description: 这是API版本9的新增资源列表。 有关已对版本8的资源进行的更新的列表，请访问API版本8的更新
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 30%

---

# API版本8中的新增功能

## 新资源

这是API版本9的新增资源列表。 有关已对版本8的资源进行的更新的列表，请访问 [API版本8的更新](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
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

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| 弃用版本 |   |   |   |   |   | 计数  |
| removalRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**KanbanBoard**

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
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

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**ProofFileMetadata**

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| documentVersionID | 文档版本 |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| 文件名 |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**ResourceBudgetedHour**

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
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

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 添加 |
| name |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | 删除 |
|   |   |   |   |   |   | 编辑 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**RichTextNote**

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### 订阅

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | 订阅者 | 添加 |
|   |   |   |   | removeSubscribers |   | 计数  |
|   |   |   |   | 订阅次数 |   | 删除 |
|   |   |   |   | 取消订阅 |   | GET |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### 用户角色

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| roleID | 角色 |   |   |   |   |   |
| timePercentage | 用户 |   |   |   |   |   |
| userID |   |   |   |   |   |   |
