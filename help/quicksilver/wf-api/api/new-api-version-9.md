---
content-type: api
navigation-topic: api-navigation-topic
title: API版本9的新增功能
description: 这是API版本9的新资源列表，要查看对版本9的资源所做的更新列表，请访问API版本9的更新
author: John
feature: Workfront API
exl-id: 29d922f4-f4c6-45e5-b9fa-43e2068ec66d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 25%

---

# API版本9的新增功能

## 新资源

这是API版本9的新资源列表，要查看对版本9的资源所做的更新列表，请访问 [API版本9的更新](../../wf-api/api/new-api-version-9-updates.md)

### 访问级别

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `accessRestrictions` | `customer` | `accessLevelPermissions` |  |  |  | `ADD` |
| `customerID` | `lastUpdatedBy` | `accessRulePreferences` |  |  |  | `COPY` |
| `description` |  |  |  |  |  | `COUNT` |
| `descriptionKey` |  |  |  |  |  | `DELETE` |
| `entryDate` |  |  |  |  |  | `EDIT` |
| `extRefID` |  |  |  |  |  | `GET` |
| `fieldAccessPrivileges` |  |  |  |  |  | `REPLACE` |
| `ID` |  |  |  |  |  | `REPORT` |
| `isAdmin` |  |  |  |  |  | `SEARCH` |
| `isUnsupportedWorkerLicense` |  |  |  |  |  |   |
| `lastUpdatedByID` |  |  |  |  |  |   |
| `lastUpdatedDate` |  |  |  |  |  |  |
| `licenseType` |  |  |  |  |  |  |
| `name` |  |  |  |  |  |  |
| `nameKey` |  |  |  |  |  |  |
| `securityModelType` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### AccessLevelPermissions

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `coreAction` |  |  |  |  |  |   |
| `forbiddenActions` |  |  |  |  |  |   |
| `ID` |  |  |  |  |  |   |
| `isAdmin` |  |  |  |  |  |   |
| `objObjCode` |  |  |  |  |  |  |
| `secondaryActions` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### AccessRulePreference

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `ID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### BudgededHour

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `allocationDate` |  |  |  |  |  | `ADD` |
| `budgetedHours` |  |  |  |  |  | `DELETE` |
| `GUID` |  |  |  |  |  | `GET` |
| `plannedBudgetedHours` |  |  |  |  |  | `SEARCH` |
| `projectID` |   |   |   |   |   |   |
| `roleID`  |   |   |   |   |   |   |
| `userID`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### CalendarPortalSection

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `calendarInfoID` | `customer` |  | `displayDescription` |  |  | `ADD` |
| `customerID` | `enteredBy` |  | `displayName` |  |  | `COPY` |
| `enteredByID` |  |  |  |  |  | `COUNT` |
| `entryDate` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `name` |  |  |  |  |  | `SEARCH` |
| `objID`  |   |   |   |   |   |   |
| `objObjCode`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 日历节

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `calendarID` | `customer` | `filters` |  | `getConcatenatedExpressionForm` |  | `ADD` |
| `calEvents` |  |  |  | `getPrettyExpressionForm` |  | `COUNT` |
| `color` |  |  |  |  |  | `DELETE` |
| `customerID` |  |  |  |  |  | `EDIT` |
| `duration` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `milestone` |  |  |  |  |  | `SEARCH` |
| `name`  |   |   |   |   |   |   |
| `plannedDate` |   |   |   |   |   |   |
| `startDate` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### ExternalSection

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `appGlobalID` | `customer` |  | `displayDescription` | `calculateURL` |  | `ADD` |
| `calculatedURL` | `enteredBy` |  | `displayName` | `calculateURLS` |  | `COPY` |
| `customerID` | `view` |  | `linkedCustomersMM` |  |  | `COUNT` |
| `description` |  |  | `linkedUsersMM` |  |  | `DELETE` |
| `descriptionKey` |  |  |  |  |  | `EDIT` |
| `enteredByID` |  |  |  |  |  | `GET` |
| `entryDate` |  |  |  |  |  | `REPORT` |
| `extRefID` |  |  |  |  |  | `SEARCH` |
| `frame`  |   |   |   |   |   |   |
| `friendlyURL`  |   |   |   |   |   |   |
| `globalUIKey`  |   |   |   |   |   |   |
| `height`  |   |   |   |   |   |   |
| `ID`  |   |   |   |   |   |   |
| `name`  |   |   |   |   |   |   |
| `nameKey`  |   |   |   |   |   |   |
| `objID`  |   |   |   |   |   |   |
| `objInterface`  |   |   |   |   |   |   |
| `objObjCode`  |   |   |   |   |   |   |
| `scrolling` |   |   |   |   |   |   |
| `url` |   |   |   |   |   |   |
| `viewID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

这份清单分成两半。 要查看下半部分，请参阅 [API版本9的新增功能（续）](../../wf-api/api/new-api-version-9-continue.md). 要查看版本9更新的列表，请访问 [API版本9的更新](../../wf-api/api/new-api-version-9-updates.md)
