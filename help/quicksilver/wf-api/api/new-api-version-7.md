---
content-type: api
navigation-topic: api-navigation-topic
title: API版本7的新增功能
description: 收藏集
author: John
feature: Workfront API
exl-id: 8c575251-677b-474d-84aa-02b637ef7760
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 50%

---

# API版本7的新增功能

## 新建对象

### 校样Bean

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 搜索 |
| deadLine |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

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
   <th>操作</th> 
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
   <td>获取  </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>报告 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>搜索 </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 添加 |
|   |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | 删除 |
|   |   |   |   |   |   | 获取 |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | 搜索 |

{style=&quot;table-layout:auto&quot;}

### 校样批准

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | 获取 |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | 搜索 |

{style=&quot;table-layout:auto&quot;}

 

### 资源轮廓

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 添加 |
|   |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | 删除 |
|   |   |   |   |   |   | 编辑 |
|   |   |   |   |   |   | 获取 |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | 搜索 |

{style=&quot;table-layout:auto&quot;}

 

### 用户组

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| groupID | 组 |   |   |   |   |   |
| isOwner  | 用户  |   |   |   |   |   |
| userID  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 时间表配置文件

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |  hourTypes |   |   |   | 添加 |
| name |   |   |   |   |   | 复制 |
|   |   |   |   |   |   | 计数 |
|   |   |   |   |   |   | 删除 |
|   |   |   |   |   |   | 编辑 |
|   |   |   |   |   |   | 获取 |
|   |   |   |   |   |   | 报告 |
|   |   |   |   |   |   | 搜索 |
|   |   |   |   |   |   | 替换 |

{style=&quot;table-layout:auto&quot;}

 

### RsrcPool

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID | 客户 | 用户 |   |   |   | 添加 |
| customerID  | enteredBy  |   |   |   |   | 计数 |
| 描述  | lastUpdatedBy  |   |   |   |   | 删除 |
| enteredByID  |   |   |   |   |   | 编辑 |
| entryDate  |   |   |   |   |   | 获取 |
| extRefID  |   |   |   |   |   | 报告 |
| lastUpdateDate |   |   |   |   |   | 搜索 |
| lastUpdateByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### DocMetadataLinkGroup

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 计数 |
| articleName  |   |   |   |   |   | 获取 |
| pageID  |   |   |   |   |   | 报告 |
| url  |   |   |   |   |   | 搜索 |

{style=&quot;table-layout:auto&quot;}

 

 

 

## 更新的对象

对现有对象的更改：只列出了“添加”，“移除”具有“删除”，对现有的更改在表后面附加了注释

### UpdateBean

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| updateType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改 

 

### ApprovalServiceObject

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate¹ |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |    |

{style=&quot;table-layout:auto&quot;}

 

### AccessRule¹

¹标记为可报告

 

### 批准流程

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   | `AttachedApprovalPaths`  |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

  

### 批准路径¹

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | `Add` |
|   |   |   |   |   |   | `Delete` |
|   |   |   |   |   |   | `Edit` |

{style=&quot;table-layout:auto&quot;}

¹已删除可报告标志

 

### 工作服务对象

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹添加了日期验证

²添加了不可过滤标记(_F)

 

### 分配

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|  workPerDayList |   |   |   | assignUserToRoleOnProjects¹ |   |   |
|   |   |   |   | swapUsersOnProjects¹ |   |   |
|   |   |   |   | unassignUserFromProjects¹ |   |   |

{style=&quot;table-layout:auto&quot;}

¹添加了includeIssues字段

 

### 客户 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| bizRuleExclusions¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改 

 

### 自定义枚举 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| groupID  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 文档 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| checkOutTimestamp |   |   |   |  createProof |   |   |

{style=&quot;table-layout:auto&quot;}

 

### DocumentVersion 

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |  getProofingTokens |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 组

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| isPublic |  layoutTemplate | userGroups  |   |   |   |   |
| layoutTemplateID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹更改了8到9的PRECISION验证器

 

### HourType

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |   | defaultOpTaskHourType |   |
|   |   |   |   |   | defaultProjectHourType |   |
|   |   |   |   |   | defaultTaskHourType  |   |
|   |   |   |   |   | globalHourTypes  |   |
|   |   |   |   |   | objectHourTypes  |   |

{style=&quot;table-layout:auto&quot;}

 

### 日志条目

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| changeType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改

 

### Optask（问题）

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |  assignMultiple |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

 

### 项目

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

 

### QueueDef

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| allowedLegacyQueueTopicIDs |  |  |  | getQueueDefTree |   |   |

{style=&quot;table-layout:auto&quot;}

 

### QueueTopic

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |  queueTopicID |   |

{style=&quot;table-layout:auto&quot;}

 

### 最新

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |  updateLastViewedObject |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   | assignMultiple  |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 模板任务

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹类型从Int更改为Double 

 

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
   <th>操作</th> 
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
   <td> <span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;scheduleDeactivationDate&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">scheduleDecavilationDate</span></td> 
   <td> </td> 
   <td><span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;timesheetProfileHourTypes&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">timeskeleProfileHourTypes</span> </td> 
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
   <td>isUserTermonicalActive</td> 
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

### 用户说明

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
| `acknowledgedmentIDs` |   |   |   |  unackknowledgeMany |   |   |
| ackDate |   |   |   |   |   |   |
| ackType |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

 

### CustomerPrefObject

| 字段 | 引用 | 收藏集 | 搜索 | 操作 | 查询 | 操作 |
|---|---|---|---|---|---|---|
|  name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹对可能值的更改
