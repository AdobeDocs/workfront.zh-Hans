---
content-type: api
navigation-topic: api-navigation-topic
title: API版本11中的新增功能
description: ReportableBugedHour已作为报表资源添加到Adobe Workfront API。 它具有BudgetedHour中缺少的引用字段、核心字段和默认字段。
author: Becky
feature: Workfront API
role: Developer
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '3573'
ht-degree: 2%

---

# API版本11中的新增功能

* [已添加资源](#added-resources)
* [已删除资源](#removed-resources)
* [已修改的资源](#modified-resources)

## 已添加资源 {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [ReportableBudgetedHour](#reportablebudgetedhour)

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasaccessrule">LoginAsAccessRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessExpirationDate</li> 
     <li style="font-weight: bold;">访问器ID</li> 
     <li style="font-weight: bold;">客户ID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">访问器</li> 
     <li style="font-weight: bold;">客户</li> 
     <li style="font-weight: bold;">用户  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">对象代码</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasadditionalrule">LoginAsAdditionalRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">客户ID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">对象ID</li> 
     <li style="font-weight: bold;">对象代码  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">客户  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">对象代码</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginassettings">LoginAsSettings</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">客户ID</li> 
     <li style="font-weight: bold;">licenseType</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">restrictedLoginAs  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">客户  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>收藏集字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">其他规则</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">对象代码</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ReportableBudgetedHour {#reportablebudgetedhour}

ReportableBugedHour已作为报表资源添加到Adobe Workfront API。 它具有BudgetedHour中缺少的引用字段、核心字段和默认字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>分配日期是您在资源规划者中为其预算小时数的周的第一天（星期日）。</p> </li> 
     <li> <p style="font-weight: bold;">budgetedHours </p> <p>预算小时数是资源管理器为资源在项目上需要完成的工作预算的时数</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>分配给特定可报告预算小时对象的唯一Workfront ID。</p> </li> 
     <li style="font-weight: bold;">plannedBudgetedHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>分配给特定项目的唯一Workfront ID。</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>分配给特定工作角色的唯一Workfront ID。</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>分配给特定用户的唯一Workfront ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">项目</p> <p>ReportableBudgetedHour关联的项目。</p> </li> 
     <li> <p style="font-weight: bold;">角色</p> <p>与ReportableBudgetedHour关联的工作角色。</p> </li> 
     <li> <p style="font-weight: bold;">用户</p> <p>ReportableBudgetedHour关联的用户。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">name</li> 
     <li style="font-weight: bold;">对象代码</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>默认字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">name</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>运营</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">计数</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">报告 </li> 
     <li style="font-weight: bold;">SEARCH</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 已删除资源 {#removed-resources}

未删除API v11的资源。

## 已修改的资源 {#modified-resources}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </li> 
     <li><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </li> 
     <li><a href="#accessrule" class="MCXref xref">访问规则</a> </li> 
     <li><a href="#approval" class="MCXref xref">审批</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">批准路径</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">工作</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">基线任务</a> </li> 
     <li><a href="#category" class="MCXref xref">类别</a> </li> 
     <li><a href="#company" class="MCXref xref">公司</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">客户</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">客户首选项</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">文档</a> </li> 
     <li><a href="#iteration" class="MCXref xref">迭代</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">布局模板</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">里程碑路径</a> </li> 
     <li><a href="#note" class="MCXref xref">注释</a> </li> 
     <li><a href="#optask" class="MCXref xref">Op任务</a> </li> 
     <li><a href="#parameter" class="MCXref xref">参数</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">Portfolio</a> </li> 
     <li><a href="#program" class="MCXref xref">计划</a> </li> 
     <li><a href="#project" class="MCXref xref">项目</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">校对审批</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">保留时间</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">ResourcePlannerFilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">风险</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">计划报告</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">记分卡问题</a> </li> 
     <li><a href="#task" class="MCXref xref">任务</a> </li> 
     <li><a href="#team" class="MCXref xref">团队</a> </li> 
     <li><a href="#template" class="MCXref xref">模板</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">模板分配</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">模板任务</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">时间表</a> </li> 
     <li><a href="#update" class="MCXref xref">更新</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">用户注释</a> </li> 
     <li><a href="#work" class="MCXref xref">工作</a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevelPermissions {#accesslevelpermissions}

AccessLevelPermissions对象表示一组权限。 然后，这组权限可以与访问级别关联。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p>以下字段添加了可能的值BUDGETING_INFORMATION。 这允许具有权限的用户在规划者中编辑优先级和预算小时数。</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">禁止操作</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Accessrequest {#accessrequest}

如果用户无权访问Workfront中他们需要的对象，则可以请求对该对象的访问权限。 AccessRequest对象表示此请求。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">操作</p> <p>添加了可能的值BUDGETING_INFORMATION。 这允许具有权限的用户在规划者中编辑优先级和预算小时数。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 访问规则 {#accessrule}

AccessRule对象表示自定义访问级别中的规则集，该规则集确定用户如何共享他们创建的项目。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p>以下字段添加了可能的值BUDGETING_INFORMATION。 这允许具有权限的用户在规划者中编辑优先级和预算小时数。</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">禁止操作</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 审批 {#approval}

给定工作项，如任务、文档或时间表，可能要求主管或其他用户签发该工作项。 审批对象表示在工作项上注销的操作。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接字段<p style="font-weight: normal;">以下字段添加了验证器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 这些验证器指定相关对象的日期不能在1900年之前或2200年之后设置。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">约束日期</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">向公共API添加了以下字段，以提高计算EAC（完工估算）的透明度。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">预算执行工作成本(BCWP)也称为实现值，是一个项目绩效指标，它表示计算此指标时实际完成的任务的预算成本。 对于任务，BCWP =实际完成百分比x任务预算。 对于项目，BCWP = SUM（所有父任务和单个任务的BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">计划工作预算成本(BCWS)也称为计划值，是一个项目性能量度，表示计算此量度时应该完成的任务的预算成本。 对于任务，BCWS =计划完成百分比x任务预算。 对于项目，BCWS = SUM（所有父任务和单个任务的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">以下字段添加了可能的值ET。 此值表示经过的月时间单位，该值是指不考虑周末或节假日时的月。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">工作单位</li>
    </ul><p style="font-weight: normal;">以下字段添加了标记CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">项目净值</li>
    </ul><p style="font-weight: normal;">以下字段已从审批对象中删除。</p>
    <ul>
     <li style="font-weight: bold;">保留时间ID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">以下字段已添加到批准对象。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedtime</p> <p style="font-weight: normal;">从审批对象中移除  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>收藏集字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">已添加到批准对象。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 批准路径 {#approvalpath}

ApprovalPath对象是批准流程中的分支。 批准路径基于与批准流程关联的对象的状态。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">添加了可能的值ET。 此值表示经过的月时间单位，该值是指不考虑周末或节假日时的月。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

ApprovalProcess对象是可以与项目、任务或问题关联的多步批准。

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

### 任务 {#assignment}

任务对象表示工作项与分配给该工作项的用户、团队或组之间的连接。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>工作单位 </p> <p style="font-weight: normal;">添加了可能的值ET。 此值表示经过的月时间单位，该值是指不考虑周末或节假日时的月。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 基线任务 {#baselinetask}

基线是给定时刻项目性能的快照。 它们存储有关项目的关键信息，如关键日期、进度、成本和收入值。 创建基线时，也会在该基线的基线任务中捕获任务信息。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">添加了可能的值ET。 此值表示经过的月时间单位，该值是指不考虑周末或节假日时的月。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 类别 {#category}

Category对象是自定义表单。 您可以为此对象生成报表，也可以将其显示在其他对象报表中。

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

### 公司 {#company}

Company对象表示由人员集合组成的组织。 公司与用户或项目相关联。

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

### CustomEnum {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>操作</td> 
   <td> <p style="font-weight: normal;">已将以下操作添加到CustomEnum对象</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查询</td> 
   <td> <p>已将以下查询添加到CustomEnum对象</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">项目完成情况</li> 
     <li style="font-weight: bold;">taskConditions</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客户 {#customer}

Customer对象表示一个使用Workfront实例的组织。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumType</p> <p style="font-weight: normal;">添加了可能的值： </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ（项目完成情况）</li> 
       <li style="font-weight: normal;">CONDITION_TASK（任务条件）</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK（问题条件）  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Reference Fields</td> 
    <td> 
     <ul> 
      <li style="font-weight: bold;"> <p>loginAsSettings</p> <p style="font-weight: normal;">Added. &nbsp;</p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td>操作</td> 
   <td> <p style="font-weight: normal;">已将以下操作添加到Customer对象</p> 
    <ul> 
     <li style="font-weight: bold;">Goalenabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客户首选项 {#customerpreferences}

CustomerPreferences对象表示客户为其Workfront实例设置的首选项集。

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">添加了可能的值：</p> 
      <ul> 
       <li style="font-weight: normal;">password：password.eauthPolicy （密码复杂性要求）</li> 
       <li style="font-weight: normal;"> password：password.minimumLength （最小密码长度）</li> 
       <li style="font-weight: normal;">password：mobileSessionTimeout（移动会话超时）</li> 
       <li style="font-weight: normal;"> project.mgmt：default.project.usertimeoff（用户休息时间）</li> 
       <li style="font-weight: normal;">时间表：default.timesheet.manualrole（手动控制角色）</li> 
       <li style="font-weight: normal;">proof：defaultNonRecipientRole (config.proofhq.defaultnonrecipientrole) </li> 
       <li style="font-weight: normal;">proof：defaultNonRecipientGuestRole (config.proofhq.defaultnonrecipientguestrole)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup {#docmetadatalinkgroup}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>操作</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>getMetadataDetailsForDocument</p> <p style="font-weight: normal;">已添加</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 文档 {#document}

Document对象表示文件（如书面材料、图像或其他形式的信息）。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>操作</td> 
   <td> <p>已将以下操作添加到Document对象。</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofStages</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 迭代 {#iteration}

小版本对象表示单个敏捷小版本。 迭代是离散的时间段，用于规划和完成Agile故事。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p>以下字段已添加到“小版本”对象。</p> 
    <ul> 
     <li style="font-weight: bold;">originaltotalpoints</li> 
     <li style="font-weight: bold;">完成点数</li> 
     <li style="font-weight: bold;">totalPoint  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 布局模板 {#layout-template}

布局模板对象表示布局元素的特定排列，例如主菜单、导航面板或“主页”区域。 可以将布局模板分配给用户、团队、组或工作角色。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">此字段已添加，并且是一个布尔参数。如果布局模板设置为在工作列表和日历中显示到期日期的时间戳，则值为true；如果设置为隐藏时间戳，则值为false。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>默认字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps</p> <p style="font-weight: normal;">已添加</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 里程碑路径 {#milestonepath}

里程碑是表示它是项目关键点的任务指示标记。 通常用于表示重大事件，例如项目某一阶段的完成或一组关键活动。 MilestonePath对象是里程碑的集合。

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

### 注释 {#note}

Note对象是对Workfront对象所做的注释或更新。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p>以下字段已添加到Note对象中。</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>收藏集字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>赞</p> <p style="font-weight: normal;">已添加</p> </li> 
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
   <td colspan="2">直接字段<p style="font-weight: normal;">以下字段添加了验证器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 这些验证器指定相关对象的日期不能在1900年之前或2200年之后设置。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">以下字段已添加到OpTask。</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">Kanban Board对象的唯一Workfront ID。</p></li>
     <li style="font-weight: bold;"><p>percentcomplete</p><p style="font-weight: normal;">完成百分比是一个参数，它将返回问题的完成数量（百分比）。</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">工作  </li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>收藏集字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">已添加</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>搜索字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>工作</p> <p style="font-weight: normal;">已删除</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>默认字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>percentcomplete</p> <p style="font-weight: normal;">已添加</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>操作</td> 
   <td> <p>已将以下操作添加到OpTask对象</p> 
    <ul> 
     <li style="font-weight: bold;">批量移动</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 参数 {#parameter}

Parameter对象是一个自定义字段。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>显示类型</p> <p style="font-weight: normal;">添加的可能值TYAH（预输入）。</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">此字段已添加并引用引用引用对象的对象代码。 可以在<a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>中找到所有对象的对象代码。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 项目组合 {#portfolio}

Portfolio对象是争夺相同资源（通常是资金或人员来完成这些资源）的项目集合。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>描述</p> <p style="font-weight: normal;">添加了验证器MAX_LENGTH ，它指定说明的长度不超过4000个字符。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 项目群 {#program}

项目群对象是项目组合中的子集，其中的相似项目可以分组在一起。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>描述</p> <p style="font-weight: normal;">添加了验证器MAX_LENGTH ，它指定说明的长度不超过4000个字符。</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">此字段已添加，并且是一个布尔参数，如果对象处于活动状态，则该参数的值为true ；否则为false。 设置为“活动”的对象会显示在下拉菜单和预输入字段中，并可附加到其他对象。 未设置为“活动”的对象在下拉菜单和要附加到其他对象的前置键入字段中不可见。  </p> </li> 
     <li style="font-weight: bold;"> <p>name </p> <p style="font-weight: normal;">添加了验证器MAX_LENGTH ，它指定名称的长度不超过255个字符。  </p> </li> 
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

### 项目 {#project}

项目是Workfront中的工作项，是Workfront帮助人们完成工作方式中的主要构建基块。 Project对象表示一组具有通用、特定目标的任务。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接字段<p style="font-weight: normal;">以下字段添加了验证器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 这些验证器指定相关对象的日期不能在1900年之前或2200年之后设置。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">向公共API添加了以下字段，以提高计算EAC（完工估算）的透明度。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">预算执行工作成本(BCWP)也称为实现值，是一个项目绩效指标，它表示计算此指标时实际完成的任务的预算成本。 对于任务，BCWP =实际完成百分比x任务预算。 对于项目，BCWP = SUM（所有父任务和单个任务的BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">计划工作预算成本(BCWS)也称为计划值，是一个项目性能量度，表示计算此量度时应该完成的任务的预算成本。 对于任务，BCWS =计划完成百分比x任务预算。 对于项目，BCWS = SUM（所有父任务和单个任务的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">以下字段添加了标记CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">项目净值</li>
    </ul><p style="font-weight: normal;">以下字段已从Project对象中删除。</p>
    <ul>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>收藏集字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">已添加</p> </li> 
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
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isWaitingDecision</p> <p style="font-weight: normal;">此字段已添加，并且是一个布尔参数，如果验证等待决定，则值为true；如果验证等待决定，则值为false。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef对象表示队列，这是一个已发布到技术支持区域以允许用户向其提交问题的项目。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p>以下字段添加了可能的值BUDGETING_INFORMATION。 这允许具有权限的用户在规划者中编辑优先级和预算小时数。</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### 保留时间 {#reservedtime}

ReservedTime对象表示在用户个人时间中指定的天数，表示用户将无法工作。

ReservedTime资源已添加标志REPORTABLE。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p>以下字段删除了标记NOT_GROUPABLE。</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefId</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>以下字段已从ReservedTime对象中删除。</p> 
    <ul> 
     <li style="font-weight: bold;">taskID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>任务</p> <p style="font-weight: normal;">已删除  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>运营</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>编辑</p> <p style="font-weight: normal;">已添加</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ResourcePlannerFilter {#resourceplannerfilter}

ResourcePlannerFilter对象是一组规则，用于确定哪些项目将显示在资源规划者中。

ResourcePlannerFilter资源添加了标记SHARABLE。 没有对该对象进行其他更改。

### 风险 {#risk}

风险对象表示可能会阻止项目按时完成或在预算内完成的可能事件。 在规划阶段的项目会增加风险，以在批准任何工作之前确定潜在的障碍。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p>向Risk对象添加了以下字段：</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredById</p> <p style="font-weight: normal;">最初创建对象的用户的ID。</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>用户在Workfront中提交对象的日期。</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>Last Update Date参数将返回对象上次更新的日期，</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>上次更新者ID是一个参数，它将返回上次更新对象的用户的用户ID。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> <p style="font-weight: normal;">已将以下引用字段添加到RIsk对象。</p> 
    <ul> 
     <li style="font-weight: bold;">输入者</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 计划报告 {#scheduledreport}

ScheduledReport对象表示已配置为计划提交的报表。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">添加了以下可能值：</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 记分卡问题 {#scorecardquestion}

ScoreCardQuestion对象表示已添加到记分卡的问题。 这些问题通常由Portfolio经理决定，这些问题的答案让经理能够了解项目与项目组合目标的符合程度。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>显示类型</p> <p style="font-weight: normal;">可能附加值TYAH（预输入）  </p> </li> 
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
   <td colspan="2">直接字段<p style="font-weight: normal;">以下字段添加了验证器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 这些验证器指定相关对象的日期不能在1900年之前或2200年之后设置。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">约束日期</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">向公共API添加了以下字段，以提高计算EAC（完工估算）的透明度。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">预算执行工作成本(BCWP)也称为实现值，是一个项目绩效指标，它表示计算此指标时实际完成的任务的预算成本。 对于任务，BCWP =实际完成百分比x任务预算。 对于项目，BCWP = SUM（所有父任务和单个任务的BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">计划工作预算成本(BCWS)也称为计划值，是一个项目性能量度，表示计算此量度时应该完成的任务的预算成本。 对于任务，BCWS =计划完成百分比x任务预算。 对于项目，BCWS = SUM（所有父任务和单个任务的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">以下字段添加了可能的值ET。 此值表示经过的月时间单位，该值是指不考虑周末或节假日时的月。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">工作单位</li>
    </ul><p style="font-weight: normal;">以下字段已从Task对象中删除。</p>
    <ul>
     <li style="font-weight: bold;">保留时间ID</li>
    </ul><p style="font-weight: normal;">以下字段已添加到Task对象。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedtime</p> <p style="font-weight: normal;">已删除  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>收藏集字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">已添加</p> </li> 
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
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">此字段已添加到Team对象。 Agile评估类型确定如何评估文章的工作负载。 如果以小时数进行估计，则这是添加到故事的已计划小时数。 如果以点为单位进行估计，则每个点都将根据点的设置方式向文章添加若干已计划小时数（默认值为8小时）。 Agile评估类型的可能值包括：</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS（故事点）</li> 
       <li style="font-weight: normal;">小时（小时）</li> 
       <li style="font-weight: normal;">LEGACY_POINTS（小时作为点）  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 模板 {#template}

Template对象表示项目的模式。 可通过模板创建项目以节省时间。 模板包含团队和任务，在使用模板时，这些团队和任务将被复制到项目中。

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
   <td>收藏集字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>所有优先级</p> <p style="font-weight: normal;">已添加</p> </li> 
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

### 模板分派 {#templateassignment}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A TemplateAssignment object represents the connection between a Template and the User, Team, or Group it is assigned to.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>工作单位</p> <p style="font-weight: normal;">添加了可能的值ET。 此值表示经过的月时间单位，该值是指不考虑周末或节假日时的月。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

TemplateTask对象表示属于Template一部分的Task。 模板任务将成为使用模板的项目中的任务。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p style="font-weight: normal;">以下字段添加了可能的值ET。 此值表示经过的月时间单位，该值是指不考虑周末或节假日时的月。</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">工作单位</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>收藏集字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>所有优先级</p> <p style="font-weight: normal;">已添加</p> </li> 
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
   <td>核心字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>对象代码</p> <p style="font-weight: normal;">已删除</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 更新 {#update}

可以更新Workfront中的工作项以通知用户当前状态。 Update对象表示这些更新之一。 更新可由用户输入或由Workfront系统创建。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">添加了可能的值referenceObjectCustomData (enum.updatetypeenum.referenceobjectcustomdata)  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查询</td> 
   <td> <p style="font-weight: normal;">以下查询已添加到Update对象。</p> 
    <ul> 
     <li style="font-weight: bold;">objectUpdatesMobile</li> 
     <li style="font-weight: bold;">updateThreadMobile</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user">User</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A User object represents a person with an account in Workfront that can log in and interact with the system.</p>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>收藏集字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>loginAsAccessRules</p> <p style="font-weight: normal;">已添加</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>操作</td> 
   <td> <p style="font-weight: normal;">已将以下操作添加到User对象。</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUserAdmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查询</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmin</p> <p style="font-weight: normal;">已添加</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 用户注释 {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>操作</td> 
   <td> <p style="font-weight: normal;">已将以下操作添加到User对象。</p> 
    <ul> 
     <li style="font-weight: bold;">acknowledgeMyNotifications</li> 
     <li style="font-weight: bold;">unacknowledgedAllObjectsTypeCount  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查询</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>myAllObjectTypesUnreadNotifications</p> <p style="font-weight: normal;">已添加</p> </li> 
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
   <td colspan="2">直接字段<p style="font-weight: normal;">以下字段添加了验证器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 这些验证器指定相关对象的日期不能在1900年之前或2200年之后设置。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">约束日期</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">向公共API添加了以下字段，以提高计算EAC（完工估算）的透明度。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">预算执行工作成本(BCWP)也称为实现值，是一个项目绩效指标，它表示计算此指标时实际完成的任务的预算成本。 对于任务，BCWP =实际完成百分比x任务预算。 对于项目，BCWP = SUM（所有父任务和单个任务的BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">计划工作预算成本(BCWS)也称为计划值，是一个项目性能量度，表示计算此量度时应该完成的任务的预算成本。 对于任务，BCWS =计划完成百分比x任务预算。 对于项目，BCWS = SUM（所有父任务和单个任务的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">以下字段添加了可能的值ET。 此值表示经过的月时间单位，该值是指不考虑周末或节假日时的月。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">工作单位</li>
    </ul><p style="font-weight: normal;">以下字段已从工作对象中删除。</p>
    <ul>
     <li style="font-weight: bold;">保留时间ID</li>
    </ul><p style="font-weight: normal;">以下字段已添加到工作对象。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedtime</p> <p style="font-weight: normal;">已删除  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>收藏集字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">已添加</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
