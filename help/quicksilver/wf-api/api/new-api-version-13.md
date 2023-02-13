---
content-type: api
navigation-topic: api-navigation-topic
title: API版本13的新增功能
description: Adobe Workfront于2021年4月22日发布了API版本13。 API版本13的版本12具有以下更改。
author: John
feature: Workfront API
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 2%

---

# API版本13的新增功能

Adobe Workfront于2021年4月22日发布了API版本13。 API版本13的版本12具有以下更改。

## 添加了资源

未为API版本13添加任何资源。

## 删除的资源

未删除API版本13的资源。

## 修改的资源

已为API版本13修改以下资源。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">访问级别</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">面包屑</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">客户首选项</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">组 </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">日记帐分录</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">布局模板</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">Op 任务</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">项目</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">校样批准</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">任务</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">团队</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">时间表</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">时间表配置文件</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">用户委派</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">工作 </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 访问级别 {#accesslevel}

AccessLevel对象与用户相关联，并描述一组AccessLevelPermissions，这些AccessLevelPermissions决定用户可以访问哪些内容。

有关访问级别的更多信息，请参阅 [访问级别的工作方式](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>描述</b> </p> <p>添加了验证器MAX_LENGTH ，它指定描述的长度不超过4000个字符。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 面包屑 {#breadcrumb}

BreadCrumb对象表示Workfront工作项的父/子层次结构中的元素。 痕迹导航指示工作项如何适合Portfolio、项目、项目和任务的更大结构。

有关痕迹导航的更多信息，请参阅 [新Adobe Workfront体验中的痕迹导航概述](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>对象代码可在 <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

BurndownEvent对象表示更改小版本的束的对象。

有关燃耗的详细信息，请参阅 [燃耗](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> <p>以下字段删除了标记NOT_GROUPABLE </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客户首选项 {#customerpreferences}

CustomerPreferences对象表示客户为其Workfront实例设置的一组首选项。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">添加了可能值：</p> 
      <ul> 
       <li style="font-weight: normal;">密码：aemAPIKey(config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> password:aemAADomain(config.general.aem.aadomain) </li> 
       <li style="font-weight: normal;">password:aemIntegrationEnabled(config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">password:aemHost(config.general.aem.host)</li> 
       <li style="font-weight: normal;">timetime:default.timeske.restrict.timeske.edit.owners.admins(config.timeske.restrict.timeske.edit.owners.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>操作</td> 
   <td> <p>以下操作已添加到CustomerPreferences资源中。</p> 
    <ul> 
     <li> <p><b>getTimeskePreferences</b> </p> </li> 
     <li> <p><b>setTimeskePreferences</b> </p> <p>采用参数：</p> 
      <ul> 
       <li> <p>首选项（映射）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

DocumentVersion对象表示文件的特定版本（如书面材料、图像或其他形式的信息）。

有关文档版本的更多信息，请参阅 [上传文档的新版本](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>添加了可能值：</p> 
      <ul> 
       <li> <p>AEM(Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>添加了标记NOT_FILTERABLE</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 组  {#group}

组对象表示一组用户和团队。 团体通常代表部门结构。

有关群组的更多信息，请参阅 [Adobe Workfront中的组与团队比较](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>操作</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>此操作会返回组父组（给定组是的子组）的数组。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 日记帐分录 {#journalentry}

JournalEntry对象可设置为在修改特定对象字段时记录有关这些字段的信息。 将字段设置为作为“日记帐分录”对象的一部分进行记录时，每次修改该字段时，都会创建相应的“日记帐分录”。

JournalEntry资源添加了标志REPOURABLE。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> <p>以下字段删除了标记NOT_GROUPABLE:</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>以下字段添加了标记NOT_FILTERABLE:</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>subObjID</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>topObjID</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 布局模板 {#layouttemplate}

Adobe Workfront管理员或组管理员可以创建模板以自定义Adobe Workfront中的布局元素。 LayoutTemplate对象特定于Adobe Workfront Classic。

有关表示新Adobe Workfront体验中布局模板的对象，请参阅 [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>描述</b> </p> <p>添加了验证器MAX_LENGTH ，它指定描述的长度不超过4000个字符。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

LinkedFolder对象表示从外部文档提供程序链接的文件夹，如Google驱动器或Dropbox。

有关链接文件夹的更多信息，请参阅 [从外部应用程序链接文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>添加了可能值：</p> 
      <ul> 
       <li> <p>AEM(Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Op 任务 {#optask}

OpTask对象通常称为问题。 问题是一个工作项，通常指示存在阻止完成任务或项目的问题。 问题也可以是帮助台请求。 更改订单、请求和错误也是问题。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>搜索字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 项目 {#project}

项目是Workfront内的工作项，是Workfront帮助人们工作方式的主要构建基块。 项目对象表示一组具有相同特定目标的任务。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertedOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 校样批准 {#proofapproval}

ProofApproval对象表示直接连接到校样的批准。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> <p>以下字段已添加到ProofApproval资源中。</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>DecisionDate</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef对象表示队列，该队列是已发布到“帮助台”区域以允许用户向其提交问题的项目。

有关请求队列的更多信息，请参阅 [创建请求队列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>已添加. 可能的值包括：</p> 
      <ul> 
       <li> <p>0（在自定义表单之后）</p> </li> 
       <li> <p>1（自定义表单之前）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 任务 {#task}

任务对象表示一个工作项，必须将该工作项作为实现最终目标（完成项目）的步骤来执行。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>搜索字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 团队 {#team}

Team对象是可分配给工作项的用户集合。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">添加了此字段，它是一个布尔参数，如果对象处于活动状态，则值为true；如果对象不活动，则为false。 设置为“活动”(Active)的对象显示在下拉菜单和提前键入字段中，并可附加到其他对象。 未设置为“活动”(Active)的对象在下拉菜单和要附加到其他对象的提前键入字段中不可见。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>默认字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">已添加</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 时间表 {#timesheet}

时间表对象表示一个虚拟工时记录卡，它允许用户输入为任务、项目和间接费用小时类型工作的实际小时数。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>已添加</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心字段</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>已删除</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 时间表配置文件 {#timesheetprofile}

时间表对象表示一个虚拟工时记录卡，它允许用户输入为任务、项目和间接费用小时类型工作的实际小时数。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>已添加</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>默认字段</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>已添加</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UITemplate {#uitemplate}

Adobe Workfront管理员或组管理员可以创建模板以自定义Adobe Workfront中的布局元素。 LayoutTemplate对象特定于新的Adobe Workfront体验。

有关在Adobe Workfront Classic中表示布局模板的对象，请参阅 [布局模板](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> <p>在UITemplate资源中添加了以下操作。</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>采用参数：</p> 
      <ul> 
       <li> <p>overrideIfExists（布尔值）</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>采用参数：</p> 
      <ul> 
       <li> <p>layoutTemplateIDs(string[])</p> </li> 
       <li> <p>overrideIfExists（布尔值）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 用户委派 {#userdelegation}

UserDelegation对象表示将工作从一个用户委派到另一个用户一段特定时间的行为。

UserDelegation对象添加了标记REPOURABLE。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> <p>以下字段删除了标记NOT_GROUPABLE</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">默认字段</td> 
   <td> <p>添加了以下字段：</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 工作  {#work}

Work对象是Task和OpTask都可继承的通用接口，并在二者之间共享通用代码。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>搜索字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
