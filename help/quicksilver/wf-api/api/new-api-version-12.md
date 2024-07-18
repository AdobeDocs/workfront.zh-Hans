---
content-type: api
navigation-topic: api-navigation-topic
title: API版本12中的新增功能
description: Workfront于2020年11月12日发布了API版本12。 API版本12具有对版本11的以下更改
author: Becky
feature: Workfront API
role: Developer
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2475'
ht-degree: 1%

---

# API版本12中的新增功能

Workfront于2020年11月12日发布了API版本12。 API版本12具有对版本11的以下更改

## 已添加资源

Workfront API版本12中新增了以下资源。

* [BreadCrumb](#breadcrumb)
* [RtfParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

BreadCrumb对象表示Adobe Workfront工作项的父/子层次结构中的元素。 痕迹导航指示工作项如何适应Portfolio、项目、项目和任务的较大结构。

有关Workfront中的痕迹导航的更多信息，请参阅新Adobe Workfront体验中的[痕迹导航概述](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

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

### RtfParameterValue {#richtextparametervalue}

富文本字段现在可用于更多对象。 已将RichTextParameterValue对象添加到Workfront以支持此可用性。

有关详细信息，请参阅Adobe Workfront API中的[富文本字段](../../wf-api/general/rich-text-field-api.md)。

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
     <li style="font-weight: bold;">对象代码</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 已删除资源

未删除API版本12的资源。

## 已修改的资源

为Workfront API版本12修改了以下资源。

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
     <li> <p><a href="#activitylog" class="MCXref xref">活动日志</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">AnnouncementAttachment</a> </p> </li> 
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
     <li> <p><a href="#group" class="MCXref xref">组</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">Op任务</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">参数</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">Portfolio</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">计划</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">计划报告</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">记分卡问题</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">任务</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">团队</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">模板任务</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">时间表</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">用户</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">工作</a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### 访问级别 {#accesslevel}

AccessLevel对象与用户相关联，并描述确定用户可以访问的AccessLevelPermissions集。

有关访问级别的详细信息，请参阅[访问级别的工作方式](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md)。

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

AccessLevelPermissions对象表示访问、创建或修改Workfront对象的特定权限。 然后，可将这些权限与访问级别关联。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>添加了以下possibleValues：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>具有包括此权限的访问级别的用户可以在工作负载均衡器中更新计划的小时数。</p> <p>有关详细信息，请参阅<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">管理工作负载均衡器</a>中的管理用户分配</a>中的<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">更新任务规划小时数。</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>具有包含此权限的访问级别的用户可以将字段添加到自定义表单。</p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>中的<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a>。</p> </li> 
       <li> <p>EDIT_SYSTEM范围 </p> <p>具有包含此权限的访问级别的用户可以在系统范围内使用“删除”权限共享自定义字段。</p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定义字段和小部件的共享</a>。</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>添加了以下possibleValues：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEM范围 </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>添加了以下possibleValues：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEM范围 </p> </li> 
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
     <li> <p style="font-weight: bold;">操作</p> <p>添加了以下possibleValues：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>具有包括此权限的访问级别的用户可以在工作负载均衡器中更新计划的小时数。</p> <p>有关详细信息，请参阅<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">管理工作负载均衡器</a>中的管理用户分配</a>中的<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">更新任务规划小时数。</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>具有包含此权限的访问级别的用户可以将字段添加到自定义表单。</p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>中的<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a>。</p> </li> 
       <li> <p>EDIT_SYSTEM范围 </p> <p>具有包含此权限的访问级别的用户可以在系统范围内使用“删除”权限共享自定义字段。</p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定义字段和小部件的共享</a>。</p> </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>添加了以下possibleValues：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>具有包括此权限的访问级别的用户可以在工作负载均衡器中更新计划的小时数。</p> <p>有关详细信息，请参阅<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">管理工作负载均衡器</a>中的管理用户分配</a>中的<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">更新任务规划小时数。</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>具有包含此权限的访问级别的用户可以将字段添加到自定义表单。</p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>中的<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a>。</p> </li> 
       <li> <p>EDIT_SYSTEM范围 </p> <p>具有包含此权限的访问级别的用户可以在系统范围内使用“删除”权限共享自定义字段。</p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定义字段和小部件的共享</a>。</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>添加了以下possibleValues：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEM范围 </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>添加了以下possibleValues：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEM范围 </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 活动日志 {#activitylog}

ActivityLog对象是在给定Workfront Proof帐户中发生的所有活动的完整列表。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>运营</p> </td> 
   <td> <p>以下操作已从ActivityLog对象中删除：</p> 
    <ul> 
     <li> <p><strong>添加</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 公告附件 {#announcementattachment}

AnnouncementAttachment对象表示已附加到Workfront公告的文件。

有关公告附件的详细信息，请参阅[发送公告](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>文件扩展名</strong> </p> <p>添加了可能的值：</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
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
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>删除了以下标志：</p> 
      <ul> 
       <li> <p>动态，</p> </li> 
       <li> <p>延迟读取，</p> </li> 
       <li> <p>NOT_GROUP</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>添加了以下标志</p> 
      <ul> 
       <li> <p>AUTO_LOAD</p> </li> 
       <li> <p>动态，</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>工作投入</strong> </p> <p>添加了此字段，表示用户完成任务需要花费少量、中量或大量的每日工作量。 可能的值包括：</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 （大）</p> </li> 
      </ul> <p>有关Workfront中工作投入的详细信息，请参阅<a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作投入概述</a>。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 日历节 {#calendarsection}

日历部分是一个日历报告。

有关日历报告的详细信息，请参阅[日历报告概述](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> <p style="font-weight: normal;">向CalendarSection对象中添加了以下字段，以支持在日历报表中使用自定义日期的新功能。 </p> <p style="font-weight: normal;">有关详细信息，请参阅<a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">在日历报告中使用自定义日期字段</a>。</p> 
    <ul> 
     <li> <p style="font-weight: normal;">customdate</p> </li> 
     <li> <p style="font-weight: normal;">customEndDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">customStartDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">ignoreActualDates</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 公司 {#company}

Company对象表示由人员集合组成的组织。

有关公司的详细信息，请参阅[创建和编辑公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">公司关联的组的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>组</p> <p style="font-weight: normal;">公司关联的组。 将公司与组关联允许组管理员将组访问权限扩展到公司。</p> </li> 
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
  <tr> 
   <td>操作</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>产品已启用</strong> </p> <p style="font-weight: normal;">此操作采用CustomerProductTypeEnum参数并返回一个布尔值，指示该客户是否拥有该产品帐户。 </p> </li> 
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
       <li style="font-weight: normal;">password：zoomIntegrationEnabled（在更新流中启用缩放集成）</li> 
       <li style="font-weight: normal;"> 密码：quipIntegrationEnabled (config.general.quip.enabled)  </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">已添加</p> </li> 
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
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">删除了可能的值：</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>proofDecision</strong> </p> <p>已添加</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>操作</td> 
   <td> <p>已将以下操作添加到Document对象。</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">此操作采用documentVersonID参数（字符串）并返回一个指示审阅人决策的映射。</p> </li> 
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

组对象表示一组用户和团队。 组通常代表部门结构。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>业务领导者ID</p> <p style="font-weight: normal;">分配给组的业务负责人ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>业务领导者</p> <p style="font-weight: normal;">分配给组的业务负责人。 业务负责人是为组制定业务决策的人员。</p> <p style="font-weight: normal;">有关商业领袖的详细信息，请参阅<a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">商业领袖概述</a>。<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>操作</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>此操作采用以下参数：</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (string[])</p> </li> 
       <li> <p>teamID（字符串）</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>此操作采用以下参数：</p> 
      <ul> 
       <li> <p>newMemberIDs (string[])</p> </li> 
       <li> <p>removedMemberDs (string[])</p> </li> 
      </ul> </li> 
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
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">删除了可能的值：</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Op 任务 {#optask}

OpTask对象通常称为“问题”。 问题是一个工作项，它通常表示存在阻止任务或项目完成的问题。 问题也可以是技术支持请求。 变更单、请求和错误也是问题。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>直接字段</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>顺序指示任务或故事在敏捷积压中的位置。</p> <p>此字段删除了以下标志：
       <ul>
        <li>动态，</li>
        <li>延迟读取，</li>
        <li>NOT_GROUPABLE：</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> <p>这些操作添加参数状态以支持新的“开始”按钮功能，当用户单击按钮以指示他们已开始处理工作项时，该功能会更改工作项的状态。</p> <p>有关详细信息，请参阅<a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">将处理此项按钮替换为开始按钮</a>。</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 参数 {#parameter}

Parameter对象是一个自定义字段。

Parameter资源添加了标记SHARABLE。

有关自定义字段的详细信息，请参阅[创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)中的[创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>数据类型</strong> </p> <p>添加的可能值：</p> 
      <ul> 
       <li> <p>RTF（富文本）</p> <p>有关详细信息，请参阅Adobe Workfront API中的<a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">富文本字段</a>。</p> </li> 
      </ul> </li> 
     <li> <p><strong>显示类型</strong> </p> <p>添加的可能值：</p> 
      <ul> 
       <li> <p>RTF（带格式的文本字段）</p> <p>有关详细信息，请参阅Adobe Workfront API中的<a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">富文本字段</a>。</p> </li> 
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

Portfolio对象是争夺相同资源（通常是资金或人员来完成这些资源）的项目集合。

有关项目组合的详细信息，请参阅Adobe Workfront中的[Portfolio概述](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md)。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">与项目组合关联的组的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>组</p> <p style="font-weight: normal;">项目组合关联的组。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 项目群 {#program}

项目群对象是项目组合中项目的子集，其中类似的项目可以分组在一起。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">与项目关联的组的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>引用字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>组</p> <p style="font-weight: normal;">与项目关联的组。 </p> </li> 
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
     <li><strong>requestorCoreAction</strong> <p>添加了以下possibleValues：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>具有包括此权限的访问级别的用户可以在工作负载均衡器中更新计划的小时数。</p> <p>有关详细信息，请参阅<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">管理工作负载均衡器</a>中的管理用户分配</a>中的<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">更新任务规划小时数。</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>具有包含此权限的访问级别的用户可以将字段添加到自定义表单。</p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>中的<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a>。</p> </li> 
       <li> <p>EDIT_SYSTEM范围 </p> <p>具有包含此权限的访问级别的用户可以在系统范围内使用“删除”权限共享自定义字段。</p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定义字段和小部件的共享</a></p> </li> 
      </ul> <li> <p><strong>requestorForbiddenActions</strong> </p> <p>添加了以下possibleValues：</p> 
       <ul> 
        <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
        <li> <p>EDIT_SYSTEM范围 </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 计划报告 {#scheduledreport}

ScheduledReport对象表示已配置为计划提交的报表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>格式</strong> </p> <p>添加了可能的值：</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 记分卡问题 {#scorecardquestion}

ScoreCardQuestion对象表示已添加到记分卡的问题。 这些问题通常由Portfolio经理决定，这些问题的答案让经理能够了解项目与项目组合目标的符合程度。

有关记分卡问题的详细信息，请参阅[创建记分卡](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>显示类型</p> <p style="font-weight: normal;">添加的可能值RTF（带格式的文本字段） </p> <p style="font-weight: normal;">有关详细信息，请参阅Adobe Workfront API中的<a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">富文本字段</a>。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 任务 {#task}

Task对象表示作为实现最终目标（完成项目）的步骤而必须执行的工作项。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>工作投入</strong> </p> <p>添加了此字段，表示用户完成任务需要花费少量、中量或大量的每日工作量。 可能的值包括：</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 （大）</p> </li> 
      </ul> <p>有关Workfront中工作投入的详细信息，请参阅<a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作投入概述</a>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> <p>这些操作添加参数状态以支持新的“开始”按钮功能，当用户单击按钮以指示他们已开始处理工作项时，该功能会更改工作项的状态。</p> <p>有关详细信息，请参阅<a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">将处理此项按钮替换为开始按钮</a>。</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 团队 {#team}

团队对象是可分配给工作项的用户的集合。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> <p>已将以下字段添加到团队资源：</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>此字段表示已完成信息卡在Kanban展示板上剩余的天数。</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>此字段将团队与组相关联。 这会将团队标识为组的一部分，并允许组管理员管理团队。</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>这是一个布尔参数，指示团队的“处理此项工作”按钮是否已配置为“开始”按钮。 当团队成员单击“开始”按钮开始处理工作项目时，项目的状态将从“新建”更改为团队设置中配置的状态。</p> </li> 
     <li> <p>以下字段允许您为各个工作项上的“开始”按钮指定自定义状态。</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuses</strong> </p> <p><strong>workOnItTaskStatuses</strong> </p> </li> 
      </ul> <p>有关“开始”按钮的详细信息，请参阅<a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">将处理它按钮替换为“开始”按钮</a>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">引用字段</td> 
   <td> <p>以下字段已添加到团队资源：</p> 
    <ul> 
     <li> <p><strong>组</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

TemplateTask对象表示属于Template一部分的Task。 模板任务将成为使用模板的项目中的任务。

有关模板任务的详细信息，请参阅[编辑模板任务](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>工作投入</strong> </p> <p>添加了此字段，表示用户完成任务需要花费少量、中量或大量的每日工作量。 可能的值包括：</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 （大）</p> </li> 
      </ul> <p>有关Workfront中工作投入的详细信息，请参阅<a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作投入概述</a>。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 时间表 {#timesheet}

工时表对象表示一个虚拟工时表，允许用户输入任务、项目和管理费用小时类型的实际工作小时数。

有关时间表的详细信息，请参阅[时间表概述](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">核心字段</td> 
   <td> <p>以下字段已从时间表资源中删除：</p> 
    <ul> 
     <li> <p><strong>objcode</strong> </p> </li> 
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
       <li> <p>initiativeAdd (enum.updatetypeenum.initiativeadd)</p> </li> 
       <li> <p>initiativeEdit (enum.updatetypeenum.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">有关计划的详细信息，请参阅Scenario Planner</a>中的<a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">计划概述。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 用户 {#user}

User对象表示在Workfront中拥有帐户的人员，该帐户可以登录并与系统交互。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接字段</td> 
   <td> <p>以下字段已添加到用户资源：</p> 
    <ul> 
     <li> <p><strong>actualDeactivationDate</strong> </p> <p>这表示停用用户的日期和时间。</p> <p>有关已停用用户的详细信息，请参阅<a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新激活用户</a>。</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>此字段显示用户对Workfront目标的访问权限。 可能的值包括：</p> 
      <ul> 
       <li> <p>无权访问</p> </li> 
       <li> <p>查看</p> </li> 
       <li> <p>编辑</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> <p>以下操作已添加到User资源：</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>此操作采用以下参数</p> 
      <ul> 
       <li> <p>ids（字符串）</p> </li> 
       <li> <p>objCode（字符串）</p> </li> 
      </ul> </li> 
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
   <td>直接字段</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>顺序指示任务或故事在敏捷积压中的位置。</p> <p>此字段删除了以下标志：</p> 
      <ul> 
       <li> <p>动态，</p> </li> 
       <li> <p>延迟读取，</p> </li> 
       <li> <p>NOT_GROUP</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>此字段添加了以下标记：</p> 
      <ul> 
       <li> <p>AUTO_LOAD</p> </li> 
       <li> <p>动态，</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>工作投入</strong> </p> <p>添加了此字段，表示用户完成任务需要花费少量、中量或大量的每日工作量。 可能的值包括：</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 （大）</p> </li> 
      </ul> <p>有关Workfront中工作投入的详细信息，请参阅<a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作投入概述</a>。</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
