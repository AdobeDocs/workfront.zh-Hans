---
content-type: api
navigation-topic: api-navigation-topic
title: API版本11的新增功能
description: ReporableBudgedHour已作为报告资源添加到Adobe Workfront API中。 它具有参考字段、核心字段和默认字段，这些字段在BudgetedHour中不存在。
author: John
feature: Workfront API
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '3600'
ht-degree: 2%

---

# API版本11的新增功能

* [添加了资源](#added-resources)
* [已删除的资源](#removed-resources)
* [修改的资源](#modified-resources)

## 添加了资源 {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [ReporableBudgededHour](#reportablebudgetedhour)

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
     <li style="font-weight: bold;">accessorID</li> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">存取器</li> 
     <li style="font-weight: bold;">客户</li> 
     <li style="font-weight: bold;">用户  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
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
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">objID</li> 
     <li style="font-weight: bold;">objObjCode  </li> 
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
     <li style="font-weight: bold;">objCode</li> 
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
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">licenseTypes</li> 
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
     <li style="font-weight: bold;">additionalRules</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ReporableBudgededHour {#reportablebudgetedhour}

ReporableBudgedHour已作为报告资源添加到Adobe Workfront API中。 它具有参考字段、核心字段和默认字段，这些字段在BudgetedHour中不存在。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>分配日期是您在资源计划员中为小时编制预算的一周的第一天（星期日）。</p> </li> 
     <li> <p style="font-weight: bold;">budgededHours </p> <p>预算小时数是资源管理者在项目上需要完成的工作预算的小时数</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>分配给特定可报告预算小时对象的唯一Workfront ID。</p> </li> 
     <li style="font-weight: bold;">planedBudgededHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>分配给特定项目的唯一Workfront ID。</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>分配给特定作业角色的唯一Workfront ID。</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>分配给特定用户的唯一Workfront ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">项目</p> <p>与ReporableBudgetedHour关联的项目。</p> </li> 
     <li> <p style="font-weight: bold;">角色</p> <p>ReporableBudgetedHour与之关联的职务角色。</p> </li> 
     <li> <p style="font-weight: bold;">用户</p> <p>与ReporableBudgetedHour关联的用户。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">name</li> 
     <li style="font-weight: bold;">objCode</li> 
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
   <td>操作</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">计数</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">报表 </li> 
     <li style="font-weight: bold;">SEARCH</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 已删除的资源 {#removed-resources}

未删除API v11的资源。

## 修改的资源 {#modified-resources}

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
     <li><a href="#approvalpath" class="MCXref xref">ApprovalPath</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">分配</a> </li> 
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
     <li><a href="#optask" class="MCXref xref">Op 任务</a> </li> 
     <li><a href="#parameter" class="MCXref xref">参数</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">项目组合</a> </li> 
     <li><a href="#program" class="MCXref xref">项目群</a> </li> 
     <li><a href="#project" class="MCXref xref">项目</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">校样批准</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">ReservedTime</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">ResourcePlannerFilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">风险</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">计划报表</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">任务</a> </li> 
     <li><a href="#team" class="MCXref xref">团队</a> </li> 
     <li><a href="#template" class="MCXref xref">模板</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">模板分配</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">模板任务</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">时间表</a> </li> 
     <li><a href="#update" class="MCXref xref">更新</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">用户说明</a> </li> 
     <li><a href="#work" class="MCXref xref">工作 </a> </li> 
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
   <td> <p>以下字段添加了可能的值BUDGETING_INFORMATION。 这允许具有权限的用户在计划员中编辑优先级和预算小时数。</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

如果用户无权访问其所需的Workfront中的对象，则他们可以请求访问该对象。 AccessRequest对象表示此请求。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">操作</p> <p>添加了可能的值BUDGETING_INFORMATION。 这允许具有权限的用户在计划员中编辑优先级和预算小时数。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 访问规则 {#accessrule}

AccessRule对象表示自定义访问级别中的规则集，用于确定用户如何共享他们创建的项目。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p>以下字段添加了可能的值BUDGETING_INFORMATION。 这允许具有权限的用户在计划员中编辑优先级和预算小时数。</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 审批 {#approval}

给定工作项（如任务、文档或时间表）可能要求主管或其他用户在工作项上签名。 “批准”对象表示在工作项上注销的操作。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接字段<p style="font-weight: normal;">以下字段添加了AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR的验证器。 这些验证程序指定，不能在1900年之前或2200年之后设置关联对象上的日期。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">planedCompletionDate</li>
     <li style="font-weight: bold;">planedStartDate</li>
    </ul><p style="font-weight: normal;">为了在计算EAC（完成时估计）时提高透明度，向公共API添加了以下字段。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">“已得值，已执行的预算工作成本(BCWP)”也称为“已得值”(Reared Value， Budgeted Work of Performed Cost， BCWP)”（项目绩效量度），它表示在计算此量度时实际完成的任务金额的预算成本。 对于任务，BCWP =实际完成百分比x任务预算。 对于项目，BCWP =所有父任务和单个任务的SUM（BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">“已计划的工作成本(BCWS)”也称为“计划值”，它是一个项目绩效量度，它表示在计算此量度时应已完成的任务量的预算成本。 对于任务，BCWS =计划完成百分比x任务预算。 对于项目，BCWS = SUM（所有父任务和单个任务的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">以下字段添加了可能的值ET。 此值表示“已用月份”的时间单位，指与周末或节假日无关的月份。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">以下字段添加了标志CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgededCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">从Approval对象中删除了以下字段。</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
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
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">从批准对象中删除  </p> </li> 
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

### ApprovalPath {#approvalpath}

ApprovalPath对象是批准流程中的一个分支。 审批路径基于审批流程所关联对象的状态。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">添加了可能的值ET。 此值表示“已用月份”的时间单位，指与周末或节假日无关的月份。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

ApprovalProcess对象是一个多步审批，可与项目、任务或问题关联。

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

### 分配 {#assignment}

分配对象表示工作项与被分配用于处理该工作项的用户、团队或组之间的连接。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">添加了可能的值ET。 此值表示“已用月份”的时间单位，指与周末或节假日无关的月份。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 基线任务 {#baselinetask}

基线是项目在给定时间内性能的快照。 它们存储有关项目的关键信息片段，如关键日期、进度、成本和收入值。 创建基线时，还会在该基线的基线任务上捕获任务信息。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">添加了可能的值ET。 此值表示“已用月份”的时间单位，指与周末或节假日无关的月份。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 类别 {#category}

类别对象是自定义表单。 您可以为此对象生成报表，也可以在其他对象报表中显示该报表。

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

### 公司 {#company}

公司对象表示由人员集合组成的组织。 公司与用户或项目关联。

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
   <td> <p style="font-weight: normal;">以下操作已添加到CustomEnum对象</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查询</td> 
   <td> <p>以下查询已添加到CustomEnum对象</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客户 {#customer}

Customer对象表示使用Workfront实例的组织。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">添加了可能值： </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ（项目条件）</li> 
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
   <td> <p style="font-weight: normal;">以下操作已添加到Customer对象</p> 
    <ul> 
     <li style="font-weight: bold;">goalsEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客户首选项 {#customerpreferences}

CustomerPreferences对象表示客户为其Workfront实例设置的一组首选项。

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
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">添加了可能值：</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy（密码复杂性要求）</li> 
       <li style="font-weight: normal;"> password:password.minimumLength（最小密码长度）</li> 
       <li style="font-weight: normal;">password:mobileSessionTimeout（移动设备会话超时）</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff（用户时间关闭）</li> 
       <li style="font-weight: normal;">时间表：default.timeske.manualrole（手动控制角色）</li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientRole(config.proofhq.defaultnonrecipiententrole) </li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientGuestRole(config.proofhq.defaultnonrecipientguestrole)  </li> 
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

文档对象表示文件（如书面材料、图像或其他信息形式）。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>操作</td> 
   <td> <p>以下操作已添加到文档对象。</p> 
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

迭代对象表示单个敏捷迭代。 迭代是用于计划和完成敏捷故事的离散时间段。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p>以下字段已添加到迭代对象。</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">已完成点数</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 布局模板 {#layout-template}

布局模板对象表示布局元素的特定排列，如主菜单、导航面板或“主页”区域。 布局模板可以分配给用户、团队、组或作业角色。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">此字段已添加，是一个布尔参数，如果布局模板设置为在工作列表和日历中显示到期日期的时间戳，则该参数的值为true；如果设置为隐藏时间戳，则该参数为false。  </p> </li> 
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

里程碑是任务上的标记，指示它是项目中的关键点。 通常用于表示重大事件，如项目某一阶段或一组关键活动的完成情况。 MilestonePath对象是里程碑的集合。

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

### 注释 {#note}

Note对象是对Workfront对象进行的注释或更新。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p>以下字段已添加到Note对象。</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>收藏集字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>称赞</p> <p style="font-weight: normal;">已添加</p> </li> 
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
   <td colspan="2">直接字段<p style="font-weight: normal;">以下字段添加了AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR的验证器。 这些验证程序指定，不能在1900年之前或2200年之后设置关联对象上的日期。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">planedCompletionDate</li>
     <li style="font-weight: bold;">planedStartDate</li>
    </ul><p style="font-weight: normal;">向OpTask中添加了以下字段。</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">看板板对象的唯一Workfront ID。</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">“完成百分比”是一个参数，它将以百分比形式返回已完成的问题量。</p></li>
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
     <li style="font-weight: bold;"> <p>percentComplete</p> <p style="font-weight: normal;">已添加</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>操作</td> 
   <td> <p>向OpTask对象添加了以下操作</p> 
    <ul> 
     <li style="font-weight: bold;">bulkMove</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 参数 {#parameter}

参数对象是自定义字段。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">添加了可能的值TYAH(Typeahead)。</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">添加了此字段，它引用引用对象的对象代码。 所有对象的对象代码均可在 <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 项目组合 {#portfolio}

Portfolio对象是争夺相同资源（通常是资金或人员）的项目集合。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>描述</p> <p style="font-weight: normal;">添加了验证器MAX_LENGTH ，它指定描述的长度不超过4000个字符。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 项目群 {#program}

Program对象是组合中的一个子集，可以将相似项目组合在一起。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>描述</p> <p style="font-weight: normal;">添加了验证器MAX_LENGTH ，它指定描述的长度不超过4000个字符。</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">添加了此字段，它是一个布尔参数，如果对象处于活动状态，则值为true；如果对象不活动，则为false。 设置为“活动”(Active)的对象显示在下拉菜单和提前键入字段中，并可附加到其他对象。 未设置为“活动”(Active)的对象在下拉菜单和要附加到其他对象的提前键入字段中不可见。  </p> </li> 
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

项目是Workfront内的工作项，是Workfront帮助人们工作方式的主要构建基块。 项目对象表示一组具有相同特定目标的任务。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接字段<p style="font-weight: normal;">以下字段添加了AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR的验证器。 这些验证程序指定，不能在1900年之前或2200年之后设置关联对象上的日期。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">planedCompletionDate</li>
     <li style="font-weight: bold;">planedStartDate</li>
    </ul><p style="font-weight: normal;">为了在计算EAC（完成时估计）时提高透明度，向公共API添加了以下字段。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">“已得值，已执行的预算工作成本(BCWP)”也称为“已得值”(Reared Value， Budgeted Work of Performed Cost， BCWP)”（项目绩效量度），它表示在计算此量度时实际完成的任务金额的预算成本。 对于任务，BCWP =实际完成百分比x任务预算。 对于项目，BCWP =所有父任务和单个任务的SUM（BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">“已计划的工作成本(BCWS)”也称为“计划值”，它是一个项目绩效量度，它表示在计算此量度时应已完成的任务量的预算成本。 对于任务，BCWS =计划完成百分比x任务预算。 对于项目，BCWS = SUM（所有父任务和单个任务的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">以下字段添加了标志CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgededCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">以下字段已从项目对象中删除。</p>
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

### 校样批准 {#proofapproval}

ProofApproval对象表示直接连接到校样的批准。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isAwaitingDecision</p> <p style="font-weight: normal;">此字段已添加，是一个布尔参数，如果校样正在等待决策，则值为true；如果校样未等待决策，则值为false。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef对象表示队列，该队列是已发布到“帮助台”区域以允许用户向其提交问题的项目。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p>以下字段添加了可能的值BUDGETING_INFORMATION。 这允许具有权限的用户在计划员中编辑优先级和预算小时数。</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### ReservedTime {#reservedtime}

ReservedTime对象表示在用户的个人时间上指定的天数，表示用户将无法工作。

ReservedTime资源添加了标记REPOURABLE。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p>以下字段删除了标志NOT_GROUPABLE。</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>从ReservedTime对象中删除了以下字段。</p> 
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
   <td>操作</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>编辑</p> <p style="font-weight: normal;">已添加</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ResourcePlannerFilter {#resourceplannerfilter}

ResourcePlannerFilter对象是一组规则，用于确定将在资源计划器中显示哪些物料。

ResourcePlannerFilter资源添加了标志SHARABLE。 对象没有其他更改。

### 风险 {#risk}

“风险”对象表示可能的事件，可能会阻止项目按时或在预算内完成。 在规划阶段的项目中增加风险，以在批准任何工作之前找出潜在障碍。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p>在Risk对象中添加了以下字段：</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredByID</p> <p style="font-weight: normal;">最初创建对象的用户的ID。</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>用户在Workfront中提交对象的日期。</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>Last Update（上次更新日期）参数将返回对象进行上次更新的日期，</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Last Updated By ID是一个参数，它将返回更新对象的上一个用户的用户ID。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> <p style="font-weight: normal;">向RIsk对象添加了以下引用字段。</p> 
    <ul> 
     <li style="font-weight: bold;">enteredBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 计划报表 {#scheduledreport}

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

### ScoreCardQuestion {#scorecardquestion}

ScoreCardQuestion对象表示已添加到记分卡中的问题。 这些问题通常由Portfolio经理确定，他们的回答使经理能够了解项目与项目组合目标的一致程度。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">添加了可能的值TYAH(Typeahead)  </p> </li> 
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
   <td colspan="2">直接字段<p style="font-weight: normal;">以下字段添加了AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR的验证器。 这些验证程序指定，不能在1900年之前或2200年之后设置关联对象上的日期。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">planedCompletionDate</li>
     <li style="font-weight: bold;">planedStartDate</li>
    </ul><p style="font-weight: normal;">为了在计算EAC（完成时估计）时提高透明度，向公共API添加了以下字段。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">“已得值，已执行的预算工作成本(BCWP)”也称为“已得值”(Reared Value， Budgeted Work of Performed Cost， BCWP)”（项目绩效量度），它表示在计算此量度时实际完成的任务金额的预算成本。 对于任务，BCWP =实际完成百分比x任务预算。 对于项目，BCWP =所有父任务和单个任务的SUM（BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">“已计划的工作成本(BCWS)”也称为“计划值”，它是一个项目绩效量度，它表示在计算此量度时应已完成的任务量的预算成本。 对于任务，BCWS =计划完成百分比x任务预算。 对于项目，BCWS = SUM（所有父任务和单个任务的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">以下字段添加了可能的值ET。 此值表示“已用月份”的时间单位，指与周末或节假日无关的月份。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">从任务对象中删除了以下字段。</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">以下字段已添加到任务对象。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">已删除  </p> </li> 
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

Team对象是可分配给工作项的用户集合。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">此字段已添加到Team对象。 敏捷估计类型确定如何估计文章的工作负载。 如果以小时为单位进行估计，则为添加到文章的计划小时数。 如果以点为单位进行估计，则每个点将根据点的设置方式（默认为8小时）在文章中添加多个计划小时数。 敏捷估计类型的可能值包括：</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS（文章点）</li> 
       <li style="font-weight: normal;">小时（小时）</li> 
       <li style="font-weight: normal;">LEGACY_POINTS（小时作为点）  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 模板 {#template}

模板对象表示项目的模式。 可以从模板创建项目以节省时间。 模板包含团队和任务，在使用模板时，这些组和任务将被复制到项目中。

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
   <td>收藏集字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriires</p> <p style="font-weight: normal;">已添加</p> </li> 
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

### 模板分配 {#templateassignment}

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
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">添加了可能的值ET。 此值表示“已用月份”的时间单位，指与周末或节假日无关的月份。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 模板任务 {#templatetask}

TemplateTask对象表示作为模板一部分的任务。 模板任务在使用模板的项目中成为任务。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p style="font-weight: normal;">以下字段添加了可能的值ET。 此值表示“已用月份”的时间单位，指与周末或节假日无关的月份。</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>收藏集字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriires</p> <p style="font-weight: normal;">已添加</p> </li> 
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
   <td>核心字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">已删除</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 更新 {#update}

可以更新Workfront中的工作项，以便让用户了解当前状态。 更新对象表示这些更新之一。 更新可由用户输入或由Workfront系统创建。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">添加了可能的值referenceObjectCustomData(enum.updatetypeenum.referenceobjectcustomdata)  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查询</td> 
   <td> <p style="font-weight: normal;">以下查询已添加到更新对象。</p> 
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
   <td> <p style="font-weight: normal;">向用户对象添加了以下操作。</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUserAdmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查询</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmins</p> <p style="font-weight: normal;">已添加</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 用户说明 {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>操作</td> 
   <td> <p style="font-weight: normal;">向用户对象添加了以下操作。</p> 
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

Work对象是Task和OpTask都可继承的通用接口，并在二者之间共享通用代码。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接字段<p style="font-weight: normal;">以下字段添加了AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR的验证器。 这些验证程序指定，不能在1900年之前或2200年之后设置关联对象上的日期。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">planedCompletionDate</li>
     <li style="font-weight: bold;">planedStartDate</li>
    </ul><p style="font-weight: normal;">为了在计算EAC（完成时估计）时提高透明度，向公共API添加了以下字段。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">“已得值，已执行的预算工作成本(BCWP)”也称为“已得值”(Reared Value， Budgeted Work of Performed Cost， BCWP)”（项目绩效量度），它表示在计算此量度时实际完成的任务金额的预算成本。 对于任务，BCWP =实际完成百分比x任务预算。 对于项目，BCWP =所有父任务和单个任务的SUM（BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">“已计划的工作成本(BCWS)”也称为“计划值”，它是一个项目绩效量度，它表示在计算此量度时应已完成的任务量的预算成本。 对于任务，BCWS =计划完成百分比x任务预算。 对于项目，BCWS = SUM（所有父任务和单个任务的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">以下字段添加了可能的值ET。 此值表示“已用月份”的时间单位，指与周末或节假日无关的月份。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">从Work对象中删除了以下字段。</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">以下字段已添加到Work对象。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">已删除  </p> </li> 
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
