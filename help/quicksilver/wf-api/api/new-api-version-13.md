---
content-type: api
navigation-topic: api-navigation-topic
title: API版本13中的新增功能
description: Adobe Workfront于2021年4月22日发布了API版本13。 API版本13具有对版本12的以下更改。
author: Becky
feature: Workfront API
role: Developer
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 2%

---

# API版本13中的新增功能

Adobe Workfront于2021年4月22日发布了API版本13。 API版本13具有对版本12的以下更改。

## 已添加资源

没有为API版本13添加资源。

## 已删除资源

未删除API版本13的资源。

## 已修改的资源

已为API版本13修改以下资源。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">访问级别</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">燃尽事件</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">客户首选项</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">组</a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">日志条目</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">布局模板</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">Op任务</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">项目</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">校对审批</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">任务</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">团队</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">时间表</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">周期性工时表</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">用户委派</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">工作</a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 访问级别 {#accesslevel}

AccessLevel对象与用户相关联，并描述确定用户可以访问的AccessLevelPermissions集。

有关访问级别的详细信息，请参阅[访问级别的工作方式](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md)。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>描述</b> </p> <p>添加了验证器MAX_LENGTH ，它指定说明的长度不超过4000个字符。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

BreadCrumb对象表示Workfront工作项的父/子层次结构中的元素。 痕迹导航指示工作项如何适应Portfolio、项目、项目和任务的较大结构。

有关痕迹导航的更多信息，请参阅新Adobe Workfront体验中的[痕迹导航概述](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>可以在<a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>中找到对象代码。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 燃尽事件 {#burndownevent}

BurndownEvent对象表示更改小版本限制的对象。

有关燃尽的详细信息，请参阅[燃尽](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md)。

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

CustomerPreferences对象表示客户为其Workfront实例设置的首选项集。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">添加了可能的值：</p> 
      <ul> 
       <li style="font-weight: normal;">密码：aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> 密码：aemAADomain (config.general.aem.aadomain) </li> 
       <li style="font-weight: normal;">密码：aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">密码：aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">时间表：default.timesheet.restrict.timesheet.edit.owners.admins (config.timesheet.restrict.timesheet.edit.owners.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>操作</td> 
   <td> <p>向CustomerPreferences资源添加了以下操作。</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>设置工时表首选项</b> </p> <p>采用参数：</p> 
      <ul> 
       <li> <p>首选项（映射）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 文档版本 {#documentversion}

DocumentVersion对象表示文件的特定版本（如书面材料、图像或其他形式的信息）。

有关文档版本的详细信息，请参阅[上载文档的新版本](../../documents/managing-documents/upload-new-document-version.md)。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>添加的可能值：</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>添加了标志NOT_FILTERABLE</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 组  {#group}

组对象表示一组用户和团队。 组通常代表部门结构。

有关组的详细信息，请参阅Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md)中的[组与团队。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>操作</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>此操作返回组的父组（给定组为其子组的组）的数组。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 日志条目 {#journalentry}

JournalEntry对象可以设置为在修改特定对象字段时记录这些字段的相关信息。 将某个字段设置为记录为日志条目对象的一部分时，每次修改该字段时将创建相应的日志条目。

JournalEntry资源添加了标志REPORTABLE。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> <p>以下字段删除了标记NOT_GROUPABLE：</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>字段名称</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>以下字段添加了标记NOT_FILTERABLE：</p> 
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

Adobe Workfront管理员或组管理员可创建模板以自定义Adobe Workfront中的布局元素。 LayoutTemplate对象特定于Adobe Workfront Classic。

有关在新的Adobe Workfront Experience中表示布局模板的对象，请参阅[UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>描述</b> </p> <p>添加了验证器MAX_LENGTH ，它指定说明的长度不超过4000个字符。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 链接文件夹 {#linkedfolder}

LinkedFolder对象表示从外部文档提供商(如Google驱动器或Dropbox)链接的文件夹。

有关链接文件夹的详细信息，请参阅[链接来自外部应用程序的文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>添加的可能值：</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Op 任务 {#optask}

OpTask对象通常称为“问题”。 问题是一个工作项，它通常表示存在阻止任务或项目完成的问题。 问题也可以是技术支持请求。 变更单、请求和错误也是问题。

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

项目是Workfront中的工作项，是Workfront帮助人们完成工作方式中的主要构建基块。 Project对象表示一组具有通用、特定目标的任务。

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

### ProofApproval {#proofapproval}

ProofApproval对象表示直接连接到验证的审批。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> <p>以下字段已添加到ProofApproval资源。</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>决策日期</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef对象表示队列，这是一个已发布到技术支持区域以允许用户向其提交问题的项目。

有关请求队列的详细信息，请参阅[创建请求队列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><b>文档位置</b> </p> <p>已添加。 可能的值包括：</p> 
      <ul> 
       <li> <p>0（在自定义表单之后）</p> </li> 
       <li> <p>1（自定义表单前）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 任务 {#task}

Task对象表示作为实现最终目标（完成项目）的步骤而必须执行的工作项。

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

团队对象是可分配给工作项的用户的集合。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">此字段已添加，并且是一个布尔参数，如果对象处于活动状态，则该参数的值为true ；否则为false。 设置为“活动”的对象会显示在下拉菜单和预输入字段中，并可附加到其他对象。 未设置为“活动”的对象在下拉菜单和要附加到其他对象的前置键入字段中不可见。  </p> </li> 
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

工时表对象表示一个虚拟工时表，允许用户输入任务、项目和管理费用小时类型的实际工作小时数。

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

### 周期性工时表 {#timesheetprofile}

工时表对象表示一个虚拟工时表，允许用户输入任务、项目和管理费用小时类型的实际工作小时数。

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

### UIT模板 {#uitemplate}

Adobe Workfront管理员或组管理员可创建模板以自定义Adobe Workfront中的布局元素。 UITemplate对象特定于新的Adobe Workfront体验。

有关在Adobe Workfront Classic中表示布局模板的对象，请参阅[布局模板](#layouttemplate)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> <p>向UITemplate资源添加了以下操作。</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>采用参数：</p> 
      <ul> 
       <li> <p>overrideIfExists（布尔值）</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>采用参数：</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists（布尔值）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 用户委托 {#userdelegation}

UserDelegation对象表示在特定时间段内将工作从一个用户委派给另一个用户的行为。

UserDelegation对象添加了标志REPORTABLE。

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

Work对象是Task和OpTask都继承的公用接口，它们共享公用代码。

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
