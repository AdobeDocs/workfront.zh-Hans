---
content-type: api
navigation-topic: api-navigation-topic
title: API版本7中的新增功能
description: 收藏集
author: Becky
feature: Workfront API
role: Developer
exl-id: 8c575251-677b-474d-84aa-02b637ef7760
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 43%

---

# API版本7中的新增功能

## 新建对象

### 校对Bean

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 搜索 |
| 死线 |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style="table-layout:auto"}

### DocMetadataLink

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>字段</th> 
   <th>引用</th> 
   <th> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">收藏集</p> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">+++++++++++ </p> </th> 
   <th>搜索</th> 
   <th>操作</th> 
   <th>查询</th> 
   <th>运营</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ID</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>添加</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>计数 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>删除 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Get  </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>报表 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Search </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 添加 |
|   |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | 删除 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | 搜索 |

{style="table-layout:auto"}

### ProofApproval

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | 搜索 |

{style="table-layout:auto"}

 

### 资源分布

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 添加 |
|   |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | 删除 |
|   |   |   |   |   |   | 编辑 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | 搜索 |

{style="table-layout:auto"}

 

### 用户组

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| groupID | 组 |   |   |   |   |   |
| isOwner  | 用户  |   |   |   |   |   |
| userID  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 周期性工时表

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |  hourType |   |   |   | 添加 |
| name |   |   |   |   |   | 复制 |
|   |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | 删除 |
|   |   |   |   |   |   | 编辑 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | 搜索 |
|   |   |   |   |   |   | 替换 |

{style="table-layout:auto"}

 

### RsrcPool

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID | 客户 | 用户 |   |   |   | 添加 |
| 客户ID  | 输入者  |   |   |   |   | 计数 |
| 描述  | lastUpdatedBy  |   |   |   |   | 删除 |
| enteredById  |   |   |   |   |   | 编辑 |
| entryDate  |   |   |   |   |   | Get |
| extRefId  |   |   |   |   |   | 报告 |
| lastUpdateDate |   |   |   |   |   | 搜索 |
| lastUpdateByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### DocMetadataLinkGroup

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 计数 |
| 文章名称  |   |   |   |   |   | Get |
| pageID  |   |   |   |   |   | 报告 |
| url  |   |   |   |   |   | 搜索 |

{style="table-layout:auto"}

 

 

 

## 已更新对象

对现有对象的更改：只列出添加项，删除项具有删除线，对现有对象的更改在表后具有附加注释

### UpdateBean

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改 

 

### ApprovalServiceObject

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate<sup>1</sup> |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |    |

{style="table-layout:auto"}

 

### 访问规则<sup>1</sup>

<sup>1</sup>已标记为可报告

 

### 审批流程

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   | `AttachedApprovalPaths`  |   |   |   |   |

{style="table-layout:auto"}

  

### 审批路径<sup>1</sup>

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | `Add` |
|   |   |   |   |   |   | `Delete` |
|   |   |   |   |   |   | `Edit` |

{style="table-layout:auto"}

已移除<sup>1</sup>可报告标志

 

### 工作服务对象

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style="table-layout:auto"}

已添加<sup>1</sup>日期验证

已添加<sup>2</sup> Not_Filterable标志

 

### 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|  workPerDayList |   |   |   | assignUserToRoleOnProjects<sup>1</sup> |   |   |
|   |   |   |   | swapUsersOnProjects<sup>1</sup> |   |   |
|   |   |   |   | unassignUserFromProjects<sup>1</sup> |   |   |

{style="table-layout:auto"}

<sup>1</sup>已添加字段includeIssues

 

### 客户 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改 

 

### 自定义枚举 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| groupID  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 文档 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| checkOutTimestamp |   |   |   |  createProof |   |   |

{style="table-layout:auto"}

 

### 文档版本 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   |   |   |  getProofingTokens |   |   |

{style="table-layout:auto"}

 

### 组

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| isPublic |  布局模板 | 用户组  |   |   |   |   |
| 布局模板标识 |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>已将PRECISION验证器更改为8到9

 

### 小时类型

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   |   |   |   | defaultOpTaskHourType |   |
|   |   |   |   |   | defaultProjectHourType |   |
|   |   |   |   |   | defaultTaskHourType  |   |
|   |   |   |   |   | globalHourType  |   |
|   |   |   |   |   | objectHourTypes  |   |

{style="table-layout:auto"}

 

### 日志条目

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改

 

### Optask（问题）

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |  assignmultiple |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### 项目

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### QueueDef

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| allowedLegacyQueueTopicIDs |  |  |  | getQueueDefTree |   |   |

{style="table-layout:auto"}

 

### 队列主题

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |  queueTopicID |   |

{style="table-layout:auto"}

 

### 最新

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|   |   |   |   |  updateLastViewedObject |   |   |

{style="table-layout:auto"}

 

### 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   | assignmultiple  |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### TemplateTask

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| 工作必需<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>类型从Int更改为Double 

 

### 用户

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>字段</th> 
   <th>引用</th> 
   <th>收藏集</th> 
   <th>搜索</th> 
   <th>操作</th> 
   <th>查询</th> 
   <th>运营</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>
    <code>lastWhatsNew</code> </td> 
   <td> </td> 
   <td>
    <code>roles</code> </td> 
   <td> 角色</td> 
   <td>addMobileDevice</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;scheduleDeactivationDate&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">scheduleDeactivationDate</span></td> 
   <td> </td> 
   <td><span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;timesheetProfileHourTypes&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">timesheetProfileHourTypes</span> </td> 
   <td> </td> 
   <td>getAvailableActions</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>hasAnyAccess</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>isUserTerminalsActive</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>removeMobileDevice</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>showShouldProofHQNavButton</td> 
   <td> </td> 
   <td>  </td> 
  </tr> 
 </tbody> 
</table>

### 用户注释

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
| `acknowledgedmentIDs` |   |   |   |  unackknowledgeMany |   |   |
| 确认日期 |   |   |   |   |   |   |
| ackType |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### CustomerPrefObject

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 运营 |
|---|---|---|---|---|---|---|
|  name |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>对可能值的更改
