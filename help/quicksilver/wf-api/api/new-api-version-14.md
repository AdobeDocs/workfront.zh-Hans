---
content-type: api
navigation-topic: api-navigation-topic
title: API版本14的新增功能
description: Adobe Workfront于2021年9月9日发布了API版本14。 API版本14具有以下与版本14相比的更改。
author: Becky
feature: Workfront API
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 2%

---

# API版本14的新增功能

Adobe Workfront于2021年9月9日发布了API版本14。 API版本14具有以下与版本14相比的更改。

## 添加了资源

未为API版本14添加任何资源。

## 删除的资源

未删除API版本14的资源。

## 修改的资源

已为API版本14修改以下资源。

* [帐单记录（帐单）](#billingrecord-bill)
* [类别(CTGY)](#category-ctgy)
* [CustomEnum(CSTEM)](#customenum-cstem)
* [客户(CUST)](#customer-cust)
* [客户首选项(CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion(DOCV)](#documentversion-docv)
* [组（组）](#group-group)
* [NoteTag(NTAG)](#notetag-ntag)
* [项目(PROJ)](#project-proj)
* [QueueDef(QUED)](#queuedef-qued)
* [资源分配(RSALLO)](#resource-allocation-rsallo)
* [角色（角色）](#role-role)
* [模板(TMPL)](#template-tmpl)
* [工时单(TSHET)](#timesheet-tshet)

### 帐单记录（帐单） {#billingrecord-bill}

BillingRecord对象记录可开单的收入、小时数或费用。 此信息可用于在外部会计系统中创建发票。

有关计费记录的详细信息，请参阅 [创建帐单记录](../../manage-work/projects/project-finances/create-billing-records.md).

BillingRecord对象添加了标记 **DATA_EXTENDIBLE**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>已添加. 类别是自定义表单。 添加此参数是为了支持将自定义Forms添加到BillingRecord对象的功能。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">引用字段</td> 
   <td> 
    <ul> 
     <li> <p><b>类别</b> </p> <p>已添加. 类别是自定义表单。 添加此参数是为了支持向BillingRecord对象添加自定义表单的功能。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">收藏集字段</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>已添加. 它表示与BillingRecord对象关联的类别（自定义表单）集合。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>已添加. 此操作将重新计算自定义表单字段中的表达式。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 类别(CTGY) {#category-ctgy}

类别对象是自定义表单。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>添加了可能值：</p> 
      <ul> 
       <li> <p> 帐单（帐单记录）</p> </li> 
      </ul> <p>此值是为了支持向BillingRecord对象添加自定义表单的功能。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectCreondInPendingApprovalStatus</b> </p> <p>此操作采用参数objID和objCode，并返回一个布尔值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum(CSTEM) {#customenum-cstem}

CustomEnum对象有助于将状态代码转换为人类可读的文本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">查询</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>已添加. 此查询支持为组和子组创建和管理状态的功能。 </p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">管理组状态</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客户(CUST) {#customer-cust}

Customer对象表示使用Workfront实例的组织。

这是内部对象。

### 客户首选项(CUSTPR) {#customerpreferences-custpr}

CustomerPreferences对象表示客户为其Workfront实例设置的一组首选项。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>添加了可能值：</p> 
      <ul> 
       <li> <p>允许用户在更新中添加图像（更新：images.toggle）</p> </li> 
      </ul> <p>此参数支持将图像添加到工作项更新中的功能。 </p> <p>有关更多信息，请参阅 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion(DOCV) {#documentversion-docv}

DocumentVersion对象表示文件的特定版本（如书面材料、图像或其他形式的信息）。

有关文档版本的更多信息，请参阅 [上传文档的新版本](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>已添加. 如果版本与校样关联，则此字段会记录Workfront校样中最后一个回调的日期和时间。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 组（组） {#group-group}

组对象表示一组用户和团队。 团体通常代表部门结构。

有关群组的更多信息，请参阅 [Adobe Workfront中的组与团队比较](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> 
    <ul> 
     <li> <p><b>addSublogums</b> </p> <p>已添加. 此操作会采用groupIDs数组，并将这些组作为子组添加到指定的组。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NoteTag(NTAG) {#notetag-ntag}

NoteTag对象表示在对工作项进行更新时标记用户或团队的行为。

有关更新中标记的更多信息，请参阅 [更新时标记其他人](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> <p>向NoteTag对象添加了以下操作：</p> 
    <ul> 
     <li> <p><b>计数</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>报表</b> </p> </li> 
     <li> <p><b>SEARCH</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 项目(PROJ) {#project-proj}

项目是Workfront内的工作项，是Workfront帮助人们工作方式的主要构建基块。 项目对象表示一组具有相同特定目标的任务。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>已添加.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef(QUED) {#queuedef-qued}

QueueDef对象表示Queue，该Queue是已发布到“帮助台”区域以允许用户向其提交问题的项目。

有关请求队列的更多信息，请参阅 [创建请求队列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>已添加. 此操作支持使用通过请求队列和主题组的路径来查找请求。</p> <p>有关按路径搜索请求队列的更多信息，请参阅 <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">在Workfront Web应用程序中创建请求并生成草稿</a> in <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">创建和提交Adobe Workfront请求</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### 资源分配(RSALLO) {#resource-allocation-rsallo}

“资源分配”对象表示给定项目所需资源的估计值。 此对象仅在旧版资源计划器中使用。 对于新资源计划员中的相应字段，请使用预算小时数(BGHR)。

资源分配对象删除了标记 **可报告**.

### 角色（角色） {#role-role}

角色对象（作业角色）表示用户可能填充的功能能力或技能集，如设计人员或产品经理。

有关作业角色的信息，请参阅 [作业角色概述](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">已添加. 如果对象处于活动状态，则此参数是一个布尔参数，如果对象处于活动状态，则其值为true；如果对象处于非活动状态，则为false。 设置为“活动”(Active)的对象显示在下拉菜单和提前键入字段中，并可附加到其他对象。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">默认字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">已添加</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 模板(TMPL) {#template-tmpl}

模板对象表示项目的模式。 可以从模板创建项目以节省时间。 模板包含团队和任务，这些团队和任务将复制到使用该模板创建的任何项目。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">已添加. 添加此字段是为了支持将组与模板关联的功能。</p> <p style="font-weight: normal;">有关更多信息，请参阅 <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">编辑项目模板</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>组</p> <p style="font-weight: normal;">已添加. 添加此字段是为了支持将组与模板关联的功能。</p> <p style="font-weight: normal;">有关更多信息，请参阅 <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">编辑项目模板</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Timesheet (TSHET)</strong></p>
<p>A&nbsp;Timesheet object represents a virtual timecard that allows users to enter actual hours worked for tasks, projects, and overhead hour types.</p>
<p>For more information, see <a href="../../timesheets/timesheets/timesheets-overview.md" class="MCXref xref">Timesheets overview</a>.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Core Fields</td>
<td>
<ul>
<li> <p><b>objCode</b> </p> <p>Removed.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
</div>
-->
