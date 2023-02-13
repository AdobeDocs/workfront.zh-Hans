---
content-type: api
navigation-topic: api-navigation-topic
title: API版本12的新增功能
description: Workfront于2020年11月12日发布了API版本12。 API版本12具有与版本11相比的以下更改
author: John
feature: Workfront API
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '2516'
ht-degree: 2%

---

# API版本12的新增功能

Workfront于2020年11月12日发布了API版本12。 API版本12具有与版本11相比的以下更改

## 添加了资源

以下资源是Workfront API版本12中的新增资源。

* [面包屑](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### 面包屑 {#breadcrumb}

BreadCrumb对象表示Adobe Workfront工作项的父/子层次结构中的元素。 痕迹导航指示工作项如何适合Portfolio、项目、项目和任务的更大结构。

有关Workfront中的痕迹导航的更多信息，请参阅 [新Adobe Workfront体验中的痕迹导航概述](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>操作</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">getObjectHierarchy</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RichTextParameterValue {#richtextparametervalue}

富文本字段现在可用于更多对象。 RichTextParameterValue对象已添加到Workfront以支持此可用性。

有关更多信息，请参阅 [Adobe Workfront API中的富文本字段](../../wf-api/general/rich-text-field-api.md).

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
     <li style="font-weight: bold;">ID</li> 
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

## 已删除的资源

未删除API版本12的资源。

## 修改的资源

已为Workfront API版本12修改以下资源。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">访问级别</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">访问规则</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">ActivityLog</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">公告附件</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">审批</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">日历节</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">公司</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">客户</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">客户首选项</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">文档</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">组 </a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">Op 任务</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">参数</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">项目组合</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">项目群</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">计划报表</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">任务</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">团队</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">模板任务</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">时间表</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">用户</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">工作 </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### 访问级别 {#accesslevel}

AccessLevel对象与用户相关联，并描述一组AccessLevelPermissions，这些AccessLevelPermissions决定用户可以访问哪些内容。

有关访问级别的更多信息，请参阅 [访问级别的工作方式](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Direct Fields</td>
   --> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">fieldAccessPrivileges</p>
      --> <!--
       <p style="font-weight: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Added the possible value CPJ (Copy). This allows Users with Planner Access Level to copy Projects.</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevelPermissions {#accesslevelpermissions}

AccessLevelPermissions对象表示访问、创建或修改Workfront对象的特定权限。 然后，这些权限可以与访问级别关联。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>添加了以下possibleValues:</p> 
      <ul> 
       <li> <p>PLANEDED_HOURS_CONTOURING </p> <p>具有包含此权限的访问级别的用户可以更新负载平衡器中的计划时间。</p> <p>有关更多信息，请参阅 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">管理用户分配时更新任务计划小时数</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作负载平衡器中管理用户分配</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> <p>具有包含此权限的访问级别的用户可以向自定义表单添加字段。</p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>具有包含此权限的访问级别的用户可以共享具有删除访问权限的全系统自定义字段。</p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定义字段和小组件的共享</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>添加了以下possibleValues:</p> 
      <ul> 
       <li> <p>PLANEDED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>添加了以下possibleValues:</p> 
      <ul> 
       <li> <p>PLANEDED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">OR</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value PLANNED_HOURS_CONTOURING, which allows a user to update planned hours in the Workload Balancer</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value ADD_TO_CUSTOM_FORMS, which allows a user to add fields to custom forms.</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value EDIT_SYSTEMWIDE, which allows a user to share a custom field system-wide with Delete access. </p>
    --> <!--
     <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <li> <p>coreAction</p> </li> 
      <li> <p>forbiddenActions</p> </li> 
      <li> <p>secondaryActions</p> </li> 
     </ul>
    --> </td> 
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
     <li> <p style="font-weight: bold;">操作</p> <p>添加了以下possibleValues:</p> 
      <ul> 
       <li> <p>PLANEDED_HOURS_CONTOURING </p> <p>具有包含此权限的访问级别的用户可以更新负载平衡器中的计划时间。</p> <p>有关更多信息，请参阅 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">管理用户分配时更新任务计划小时数</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作负载平衡器中管理用户分配</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> <p>具有包含此权限的访问级别的用户可以向自定义表单添加字段。</p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>具有包含此权限的访问级别的用户可以共享具有删除访问权限的全系统自定义字段。</p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定义字段和小组件的共享</a>.</p> </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>添加了以下possibleValues:</p> 
      <ul> 
       <li> <p>PLANEDED_HOURS_CONTOURING </p> <p>具有包含此权限的访问级别的用户可以更新负载平衡器中的计划时间。</p> <p>有关更多信息，请参阅 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">管理用户分配时更新任务计划小时数</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作负载平衡器中管理用户分配</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> <p>具有包含此权限的访问级别的用户可以向自定义表单添加字段。</p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>具有包含此权限的访问级别的用户可以共享具有删除访问权限的全系统自定义字段。</p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定义字段和小组件的共享</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>添加了以下possibleValues:</p> 
      <ul> 
       <li> <p>PLANEDED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>添加了以下possibleValues:</p> 
      <ul> 
       <li> <p>PLANEDED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ActivityLog {#activitylog}

ActivityLog对象是在给定Workfront校样帐户中发生的所有活动的完整列表。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>操作</p> </td> 
   <td> <p>从ActivityLog对象中删除了以下操作：</p> 
    <ul> 
     <li> <p><strong>添加</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 公告附件 {#announcementattachment}

AnnowtingAttachment对象表示已附加到Workfront公告的文件。

有关公告附件的更多信息，请参阅 [发送公告](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>添加了可能值：</p> 
      <ul> 
       <li> <p>qdoc(enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides(enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet(enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
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
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>积压订单</strong> </p> <p>删除了以下标记：</p> 
      <ul> 
       <li> <p>动态，</p> </li> 
       <li> <p>LAZY_READ，</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>添加了以下标记</p> 
      <ul> 
       <li> <p>自动加载(_L),</p> </li> 
       <li> <p>动态，</p> </li> 
       <li> <p>只读</p> </li> 
      </ul> </li> 
     <li> <p><strong>workWork</strong> </p> <p>添加了此字段，它表示用户完成任务所需的每日工作量是中、小，还是大。 可能的值包括：</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2（中）</p> </li> 
       <li> <p>3（大）</p> </li> 
      </ul> <p>有关Workfront中的工作精力的更多信息，请参阅 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作概述</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 日历节 {#calendarsection}

日历部分是日历报表。

有关日历报表的详细信息，请参阅 [日历报表概述](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p style="font-weight: normal;">CalendarSection对象中添加了以下字段，以支持在日历报表中使用自定义日期的新功能。 </p> <p style="font-weight: normal;">有关更多信息，请参阅 <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">在日历报表中使用自定义日期字段</a>.</p> 
    <ul> 
     <li> <p style="font-weight: normal;">customDate</p> </li> 
     <li> <p style="font-weight: normal;">customEndDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">customStartDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">ignoreActualDates</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 公司 {#company}

公司对象表示由人员集合组成的组织。

有关公司的更多信息，请参阅 [创建和编辑公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">与公司关联的组的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>组</p> <p style="font-weight: normal;">与公司关联的组。 将公司与群组关联后，群组管理员可以扩展对公司的群组访问权限和权限。</p> </li> 
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
  <tr> 
   <td>操作</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">此操作采用CustomerProductTypeEnum参数并返回一个布尔值，表示该客户是否拥有该产品的帐户。 </p> </li> 
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
       <li style="font-weight: normal;">password:zoomIntegrationEnabled（在更新流中启用缩放集成）</li> 
       <li style="font-weight: normal;"> password:quipIntegrationEnabled(config.general.quip.enabled)  </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">已添加</p> </li> 
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
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">删除了可能的值：</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP(Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>proofDecision</strong> </p> <p>已添加</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>操作</td> 
   <td> <p>以下操作已添加到文档对象。</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">此操作采用documentVersonID参数（字符串）并返回指示审阅人决策的映射。</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">此操作采用以下参数：</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID（字符串）</p> </li> 
       <li> <p>reviewerDecision（字符串）</p> </li> 
       <li> <p>注释（字符串）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 组  {#group}

组对象表示一组用户和团队。 团体通常代表部门结构。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">分配给组的业务主管的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>商业领袖</p> <p style="font-weight: normal;">分配给组的业务负责人。 业务领导者是为组做出业务决策的人。</p> <p style="font-weight: normal;">有关业务领导者的更多信息，请参阅 <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">业务领先者概述</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>操作</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>此操作采用以下参数：</p> 
      <ul> 
       <li> <p>userIDs(string[])</p> </li> 
       <li> <p>roleIDs(string[])</p> </li> 
       <li> <p>teamID（字符串）</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>此操作采用以下参数：</p> 
      <ul> 
       <li> <p>newMemberIDs(string[])</p> </li> 
       <li> <p>removedMemberDs(string[])</p> </li> 
      </ul> </li> 
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
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">删除了可能的值：</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP(Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Op 任务 {#optask}

OpTask对象通常称为问题。 问题是一个工作项，通常指示存在阻止完成任务或项目的问题。 问题也可以是帮助台请求。 更改订单、请求和错误也是问题。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>积压订单</strong> </p> <p>顺序指示任务或文章在敏捷积压工作中的位置。</p> <p>此字段删除了以下标记：
       <ul>
        <li>动态，</li>
        <li>LAZY_READ，</li>
        <li>NOT_GROUPABLE:</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> <p>这些操作添加了参数状态以支持新的“开始”按钮功能，当用户单击该按钮以表示他们已开始处理该项目时，该功能会更改工作项的状态。</p> <p>有关更多信息，请参阅 <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">将“Work On It（处理它）”按钮替换为“Start（开始）”按钮</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 参数 {#parameter}

参数对象是自定义字段。

参数资源添加了标志SHARABLE。

有关自定义字段的更多信息，请参阅 [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) in [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>添加了可能值：</p> 
      <ul> 
       <li> <p>富（富文本）</p> <p>有关更多信息，请参阅 <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API中的富文本字段</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>添加了可能值：</p> 
      <ul> 
       <li> <p>富（带格式的文本字段）</p> <p>有关更多信息，请参阅 <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API中的富文本字段</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>标签</strong> </p> <p>已添加</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">收藏集字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>accessRules</strong> </p> <p>已添加</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">默认字段</td> 
   <td> 
    <ul> 
     <li> <p class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><strong>标签</strong> </p> <p>已添加</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 项目组合 {#portfolio}

Portfolio对象是争夺相同资源（通常是资金或人员）的项目集合。

有关组合的更多信息，请参阅 [PortfolioAdobe Workfront概述](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">与组合关联的组的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>组</p> <p style="font-weight: normal;">与组合关联的组。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 项目群 {#program}

项目组合中的项目是项目对象的子集，可以将相似项目组合在一起。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">与程序关联的组的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>组</p> <p style="font-weight: normal;">与程序关联的组。 </p> </li> 
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
     <li><strong>requestorCoreAction</strong> <p>添加了以下possibleValues:</p> 
      <ul> 
       <li> <p>PLANEDED_HOURS_CONTOURING </p> <p>具有包含此权限的访问级别的用户可以更新负载平衡器中的计划时间。</p> <p>有关更多信息，请参阅 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">管理用户分配时更新任务计划小时数</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作负载平衡器中管理用户分配</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> <p>具有包含此权限的访问级别的用户可以向自定义表单添加字段。</p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>具有包含此权限的访问级别的用户可以共享具有删除访问权限的全系统自定义字段。</p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定义字段和小组件的共享</a></p> </li> 
      </ul> <li> <p><strong>requestorForbiddenActions</strong> </p> <p>添加了以下possibleValues:</p> 
       <ul> 
        <li> <p>PLANEDED_HOURS_CONTOURING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS。 </p> </li> 
        <li> <p>EDIT_SYSTEMWIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 计划报表 {#scheduledreport}

ScheduledReport对象表示已配置为计划提交的报表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>格式</strong> </p> <p>添加了可能值：</p> 
      <ul> 
       <li> <p>qdoc(enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides(enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet(enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

ScoreCardQuestion对象表示已添加到记分卡中的问题。 这些问题通常由Portfolio经理确定，他们的回答使经理能够了解项目与项目组合目标的一致程度。

有关记分卡问题的更多信息，请参阅 [创建记分卡](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">添加了可能的值RICH（带格式的文本字段） </p> <p style="font-weight: normal;">有关更多信息，请参阅 <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API中的富文本字段</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 任务 {#task}

任务对象表示一个工作项，必须将该工作项作为实现最终目标（完成项目）的步骤来执行。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>workWork</strong> </p> <p>添加了此字段，它表示用户完成任务所需的每日工作量是中、小，还是大。 可能的值包括：</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2（中）</p> </li> 
       <li> <p>3（大）</p> </li> 
      </ul> <p>有关Workfront中的工作精力的更多信息，请参阅 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作概述</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> <p>这些操作添加了参数状态以支持新的“开始”按钮功能，当用户单击该按钮以表示他们已开始处理该项目时，该功能会更改工作项的状态。</p> <p>有关更多信息，请参阅 <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">将“Work On It（处理它）”按钮替换为“Start（开始）”按钮</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 团队 {#team}

Team对象是可分配给工作项的用户集合。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> <p>向团队资源中添加了以下字段：</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>此字段表示已完成的卡在看板板上保留的天数。</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>此字段将团队与组关联。 这将团队标识为组的一部分，并允许组管理员管理团队。</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>这是一个布尔参数，用于指示团队的“Work on It”（处理它）按钮是否已配置为“Start”（开始）按钮。 当团队成员单击“开始”按钮以开始处理工作项时，该项目的状态将从“新建”更改为在团队设置中配置的状态。</p> </li> 
     <li> <p>以下字段允许您在单个工作项上为“开始”按钮指定自定义状态。</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuss</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatus</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuss</strong> </p> <p><strong>workOnItTaskStatuss</strong> </p> </li> 
      </ul> <p>有关“开始”按钮的详细信息，请参阅 <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">将“Work On It（处理它）”按钮替换为“Start（开始）”按钮</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">引用字段</td> 
   <td> <p>向团队资源中添加了以下字段：</p> 
    <ul> 
     <li> <p><strong>组</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 模板任务 {#templatetask}

TemplateTask对象表示作为模板一部分的任务。 模板任务在使用模板的项目中成为任务。

有关模板任务的详细信息，请参阅 [编辑模板任务](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>workWork</strong> </p> <p>添加了此字段，它表示用户完成任务所需的每日工作量是中、小，还是大。 可能的值包括：</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2（中）</p> </li> 
       <li> <p>3（大）</p> </li> 
      </ul> <p>有关Workfront中的工作精力的更多信息，请参阅 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作概述</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 时间表 {#timesheet}

时间表对象表示一个虚拟工时记录卡，它允许用户输入为任务、项目和间接费用小时类型工作的实际小时数。

有关工时单的详细信息，请参阅 [工时单概述](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">核心字段</td> 
   <td> <p>已从时间表资源中删除以下字段：</p> 
    <ul> 
     <li> <p><strong>objoce</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 更新

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>updateType</strong> </p> <p>添加了以下可能值：</p> 
      <ul> 
       <li> <p>initiativeAdd(enum.updatetypeenum.initiativeadd)</p> </li> 
       <li> <p>initiativeEdit(enum.updatetypeenum.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">有关计划的更多信息，请参阅 <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">方案规划器中的方案概述</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 用户 {#user}

User对象表示在Workfront中具有可登录并与系统交互的帐户的人员。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> <p>向用户资源添加了以下字段：</p> 
    <ul> 
     <li> <p><strong>actualDecavilationDate</strong> </p> <p>这表示用户被停用的日期和时间。</p> <p>有关已停用用户的更多信息，请参阅 <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新激活用户</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>此字段显示用户对Workfront Target的访问权限。 可能的值包括：</p> 
      <ul> 
       <li> <p>无权访问</p> </li> 
       <li> <p>查看</p> </li> 
       <li> <p>编辑</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> <p>向用户资源添加了以下操作：</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>此操作采用以下参数</p> 
      <ul> 
       <li> <p>id（字符串）</p> </li> 
       <li> <p>objCode（字符串）</p> </li> 
      </ul> </li> 
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
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>积压订单</strong> </p> <p>顺序指示任务或文章在敏捷积压工作中的位置。</p> <p>此字段删除了以下标记：</p> 
      <ul> 
       <li> <p>动态，</p> </li> 
       <li> <p>LAZY_READ，</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>此字段添加了以下标记：</p> 
      <ul> 
       <li> <p>自动加载(_L),</p> </li> 
       <li> <p>动态，</p> </li> 
       <li> <p>只读</p> </li> 
      </ul> </li> 
     <li> <p><strong>workWork</strong> </p> <p>添加了此字段，它表示用户完成任务所需的每日工作量是中、小，还是大。 可能的值包括：</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2（中）</p> </li> 
       <li> <p>3（大）</p> </li> 
      </ul> <p>有关Workfront中的工作精力的更多信息，请参阅 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作概述</a>.</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
