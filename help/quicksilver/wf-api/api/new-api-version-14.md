---
content-type: api
navigation-topic: api-navigation-topic
title: API版本14中的新增功能
description: Adobe Workfront于2021年9月9日发布了API版本14。 API版本14具有对版本14的以下更改。
author: Becky
feature: Workfront API
role: Developer
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 0%

---

# API版本14中的新增功能

Adobe Workfront于2021年9月9日发布了API版本14。 API版本14具有对版本14的以下更改。

## 已添加资源

没有为API版本14添加资源。

## 已删除资源

没有为API版本14删除资源。

## 已修改的资源

已为API版本14修改以下资源。

* [记帐记录（帐单）](#billingrecord-bill)
* [类别(CTGY)](#category-ctgy)
* [CustomEnum (CSTEM)](#customenum-cstem)
* [客户(CUST)](#customer-cust)
* [客户首选项(CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion (DOCV)](#documentversion-docv)
* [组（组）](#group-group)
* [NoteTag (NTAG)](#notetag-ntag)
* [项目（项目）](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [资源分配(RSALLO)](#resource-allocation-rsallo)
* [角色（角色）](#role-role)
* [模板(TMPL)](#template-tmpl)
* [时间表(TSHET)](#timesheet-tshet)

### 记帐记录(BILL) {#billingrecord-bill}

BillingRecord对象记录可记帐的收入、小时数或费用。 此信息可用于在外部会计系统中创建发票。

有关开票记录的详细信息，请参阅[创建开票记录](../../manage-work/projects/project-finances/create-billing-records.md)。

BillingRecord对象添加了标志&#x200B;**DATA_EXTENDIBLE**。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>类别ID</b> </p> <p>已添加。 类别是自定义表单。 添加此参数是为了支持向BillingRecord对象添加自定义Forms的功能。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">引用字段</td> 
   <td> 
    <ul> 
     <li> <p><b>类别</b> </p> <p>已添加。 类别是一种自定义表单。 添加此参数是为了支持向BillingRecord对象添加自定义表单的功能。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">收藏集字段</td> 
   <td> 
    <ul> 
     <li> <p><b>对象类别</b> </p> <p>已添加。 这表示与BillingRecord对象关联的类别（自定义表单）集合。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>已添加。 此操作重新计算自定义表单字段中的表达式。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 类别(CTGY) {#category-ctgy}

Category对象是自定义表单。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>添加的可能值：</p> 
      <ul> 
       <li> <p> 帐单(BillingRecord)</p> </li> 
      </ul> <p>添加此值是为了支持向BillingRecord对象添加自定义表单的功能。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>此操作接受参数objID和objCode并返回布尔值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum (CSTEM) {#customenum-cstem}

CustomEnum对象有助于将状态代码转换为人类可读的文本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">查询</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>已添加。 此查询支持创建和管理组和子组的状态。 </p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">管理组状态</a>。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客户（客户） {#customer-cust}

Customer对象表示一个使用Workfront实例的组织。

这是一个内部对象。

### 客户首选项(CUSTPR) {#customerpreferences-custpr}

CustomerPreferences对象表示客户为其Workfront实例设置的首选项集。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><b>名称</b> </p> <p>添加的可能值：</p> 
      <ul> 
       <li> <p>允许用户在更新中添加图像(updates：images.toggle)</p> </li> 
      </ul> <p>此参数支持将图像添加到工作项更新的功能。 </p> <p>有关详细信息，请参阅<a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a>。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

DocumentVersion对象表示文件的特定版本（如书面材料、图像或其他形式的信息）。

有关文档版本的详细信息，请参阅[上载文档的新版本](../../documents/managing-documents/upload-new-document-version.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>已添加。 此字段记录来自Workfront Proof的上次回调的日期和时间（如果版本与验证关联）。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 组（组） {#group-group}

组对象表示一组用户和团队。 组通常代表部门结构。

有关组的详细信息，请参阅Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md)中的[组与团队。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>已添加。 此操作获取一个groupID数组，并将这些组作为子组添加到指定组。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NoteTag (NTAG) {#notetag-ntag}

NoteTag对象表示在工作项的更新中为用户或团队添加标签的行为。

有关在更新中标记的详细信息，请参阅[在更新中标记其他人](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">运营</td> 
   <td> <p>向NoteTag对象添加了以下操作：</p> 
    <ul> 
     <li> <p><b>计数</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>报告</b> </p> </li> 
     <li> <p><b>搜索</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 项目（项目） {#project-proj}

项目是Workfront中的工作项，是Workfront帮助人们完成工作方式中的主要构建基块。 Project对象表示一组具有通用、特定目标的任务。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>已添加。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

QueueDef对象表示队列，这是一个已发布到技术支持区域以允许用户向其提交问题的项目。

有关请求队列的详细信息，请参阅[创建请求队列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>已添加。 此操作支持通过使用请求队列和主题组中的路径来查找请求的功能。</p> <p>有关按路径搜索请求队列的详细信息，请参阅<a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">创建和提交Workfront请求</a>中的<a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">在Adobe Workfront Web应用中创建请求并生成草稿</a>。</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### 资源分配(RSALLO) {#resource-allocation-rsallo}

资源分配对象表示给定项目所需的资源估计。 此对象仅在旧版资源规划者中使用。 对于新资源规划者中的相应字段，请使用预算小时数(BGHR)。

资源分配对象删除了标志&#x200B;**REPORTABLE**。

### 角色(ROLE) {#role-role}

角色对象（工作角色）表示用户可能填充的功能能力或技能集，如Designer或产品经理。

有关工作角色的信息，请参阅[工作角色概述](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">已添加。 这是一个布尔参数，如果对象处于Active状态，则该参数的值为true ；否则为false。 设置为“活动”的对象会显示在下拉菜单和预输入字段中，并可附加到其他对象。</p> </li> 
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

### 模板（模板） {#template-tmpl}

Template对象表示项目的模式。 可使用模板创建项目以节省时间。 模板包含团队和任务，这些团队和任务将被复制到从该模板创建的任何项目中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">已添加。 添加此字段是为了支持将组与模板关联的能力。</p> <p style="font-weight: normal;">有关详细信息，请参阅<a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">编辑项目模板</a>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>组</p> <p style="font-weight: normal;">已添加。 添加此字段是为了支持将组与模板关联的能力。</p> <p style="font-weight: normal;">有关详细信息，请参阅<a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">编辑项目模板</a>。</p> </li> 
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
