---
product-area: projects
navigation-topic: manage-projects
title: 重新计算项目时间表
description: 重新计算时间表允许经理查看与项目相关的不同因素如何影响项目的时间表。 项目的时间表是指计划日期和预计日期。
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# 重新计算项目时间表

重新计算时间表允许经理查看与项目相关的不同因素如何影响项目的时间表。 项目的时间表是指计划日期和预计日期。

对项目范围之外的计划、人员休假时间和其他项目进行更改不会立即影响项目时间表。 重新计算时间轴时，项目时间轴会受到影响。 在重新计算之前，外部影响不会对您的项目生效。

本文介绍了时间轴重新计算的方法。

## 访问要求

<!--drafted for P&P: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
自动时间轴重新计算会在没有参与项目工作的任何用户的特殊访问权限的情况下进行。

但是，您必须具有以下访问权限才能手动重新计算项目的时间轴：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p>系统管理员为系统中的所有项目重新计算时间表</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 自动重新计算

默认情况下，当项目范围发生更改时或每天晚上自动重新计算项目时间轴。 Workfront管理员通过管理“设置”的“项目首选项”区域中的“时间轴”设置，确定是每晚自动计算时间轴，还是每次更改范围时自动计算时间轴。 有关更多信息，请参阅 [为项目配置时间轴重新计算](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!NOTE]
>
>如果项目的时间轴超过15年，则会禁用该项目的自动重新计算。 对于超过15年的项目，您只能选择“手动”更新类型。 如果将项目日期更改为少于15年，则必须在自动计算时间轴之前一次手动重新计算时间轴。

* [自动重新计算项目时间表](#automatic-recalculation-of-project-timelines)
* [触发项目时间轴自动重新计算的操作](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)

### 自动重新计算项目时间表 {#automatic-recalculation-of-project-timelines}

Adobe Workfront每天只对满足以下所有条件的项目重新计算时间表：

* 状态为“当前”
* 项目的“更新类型”设置为“自动”或“自动”，并且“更改时”

   有关项目更新类型类型的信息，请参阅 [项目更新类型概述](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* 在过去三个月内拥有上次更新日期\
   Workfront管理员可以更改此默认功能，如 [为项目配置时间轴重新计算](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

* 项目时间轴的上次计算日期不在当前日历日内。 这意味着项目时间线的最后一个计算日期在当天00:00之前。

您可以配置更新项目时间轴的频率。 更新项目时间轴后，将根据对项目所做的更改重新计算时间轴。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

有关信息，请参阅 [选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click&nbsp; <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
<li value="3"> <p>Click<strong>Settings.</strong><br><img src="assets/screen-shot-2013-09-18-at-10.36.16-am-350x347.png" alt="" style="width: 350;height: 347;"></p> </li>
<li value="4">In the <strong>Update Type</strong> drop-down list, select from the following options:<br><strong>- Automatic and On Change:</strong> (Default setting) The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night. <br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed.
<div>
<p><img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"></p>
</div><br>This indicates that the recalculation is not yet finished, and the dates are subject to change. <br><strong>- Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.<br>You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br><strong>- Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on.<br><note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note><br><strong>- Manual Only:</strong> The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="#manual-recalculation" class="MCXref xref">Manual recalculation</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).<br>For more information about the project Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a><note type="note">
If the timeline of a project is longer than 15 years, the automatic recalculation is disabled. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically.
</note></li>
<li value="5">Click <strong>Save Changes.</strong></li>
</ol>
</div>
-->

### 触发项目时间轴自动重新计算的操作 {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

项目生命周期中的各种范围更改会自动重新计算项目时间轴，包括以下操作：

* 正在更新任务状态。
* 将任务移到其他项目。
* 更新任务的计划日期或计划完成日期。
* 更新任务的持续时间类型、任务约束或受分配者数量。
* 更新任务前置关系。
* 向任务添加批准，该批准还会向任务的计划完成日期添加时间。\
   有关批准设置的更多信息，请参阅 [配置全局批准设置](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## 手动重新计算 {#manual-recalculation}

作为项目所有者，您可以人工重新计算单个项目的时间轴。 Workfront管理员可以在Workfront中手动重新计算所有时间轴。

* [重新计算单个项目或批量项目的时间表](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [在“编辑项目”框中批量手动重新计算时间轴](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [重新计算系统中所有项目的时间表(仅限Workfront管理员)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### 重新计算单个项目或批量项目的时间表 {#recalculate-timelines-for-individual-projects-or-in-bulk}

您可以从项目页面或项目列表或报表重新计算Workfront中项目的时间轴。

1. 转到要重新计算时间轴的项目，然后单击 **更多** 图标 ![](assets/qs-more-menu.png) 项目名称的左侧

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   或

   转到项目列表或报表，选择一个或多个项目，然后单击 **更多** 图标 ![](assets/qs-more-menu.png) 列表顶部。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >根据项目的复杂性，我们建议在批量重新计算项目时间轴时不要选择大量项目，以确保获得最佳性能。 某些可能导致项目过于复杂的因素可能是多个依赖关系或分配，或大量自定义字段。

1. 单击 **重新计算时间轴**.

   重新计算时间轴后，您会看到一条消息，指示重新计算成功。

   >[!TIP]
   >
   >在时间轴重新计算完成之前，某些计划日期或预计日期可能会显示为灰显。 这意味着重新计算尚未完成，并且日期可能会发生更改。

### 在“编辑项目”框中批量手动重新计算时间轴 {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

您可以通过批量编辑多个项目的时间轴来手动重新计算这些项目的时间轴。

>[!TIP]
>
>根据项目的复杂性，我们建议在批量编辑项目时不要选择大量项目，以确保获得最佳性能。 某些可能导致项目过于复杂的因素可能是多个依赖关系或分配或大量自定义字段。

1. 转到项目列表。
1. 在列表中选择多个项目，然后单击 **编辑**.
1. 单击 **设置**，然后选择 **重新计算时间轴**.

1. 单击 **保存更改**.

### 重新计算系统中所有项目的时间表(仅限Workfront管理员) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Workfront管理员可以运行重新计算时间轴诊断，以立即重新计算Workfront系统中的所有时间轴。 这允许所有项目经理立即查看外部更改对计划日期和预计日期的影响。

有关重新计算整个Workfront站点的时间轴的更多信息，请参阅 [为项目配置时间轴重新计算](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Project Update Types</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to thisa rticle: /Content/Manage work/Projects/Planning a Project/project-update-type-overview.htm)</p>
<p>For information about how to update the project's Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>. </p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<p>You can select how each project calculates its timeline by choosing between the following Update Types:</p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<ul>
<li> <p><strong>Automatic and On Change:</strong>&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp; <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong>&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong>&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong>&nbsp;The project timeline is updated only&nbsp;when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in&nbsp;the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->
