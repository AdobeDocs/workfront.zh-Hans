---
product-area: projects
navigation-topic: manage-projects
title: 重新计算项目时间表
description: 重新计算时间表使经理能够了解与项目相关的不同因素如何影响项目时间表。 项目的时间表是指计划和预计日期。
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: 3dfb30646e8a967264f7e562441a52a059d73d32
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 0%

---

# 重新计算项目时间表

<!--Audited: 06/2025-->

重新计算时间表使经理能够了解与项目相关的不同因素如何影响项目时间表。 项目的时间表是指计划和预计日期。

对计划、人员休息时间以及项目范围之外的其他项目进行更改不会立即影响项目时间线。 重新计算时间线时，项目时间线会受到影响。 在重新计算之前，外部影响不会对您的项目生效。

本文介绍了时间线重新计算的方式。

如果没有参与项目工作的任何用户的特殊访问权限，则会自动重新计算时间线。 此外，您可以手动重新计算时间线。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>新增：标准 </p> 
   或
   <p>当前：计划 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目的访问权限</p> <p>系统管理员重新计算系统中所有项目的时间表</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 自动重新计算

默认情况下，当项目范围每天或每晚更改时，项目时间表会自动重新计算。 Workfront管理员通过管理“设置”的“项目首选项”区域中的“时间表”设置，确定是每晚自动计算时间表，还是每次范围更改时自动计算时间表。 有关详细信息，请参阅[配置项目的时间表重新计算](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)。

>[!NOTE]
>
>如果项目的时间表超过15年，则会禁用该项目的自动重新计算，并且您只能选择手动更新类型。 如果将项目日期更改为少于15年，则必须先手动重新计算时间线，然后才能自动计算。

* [项目时间线的自动重新计算](#automatic-recalculation-of-project-timelines)
* [触发自动重新计算项目时间线的操作](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)


>[!IMPORTANT]
>
>对于预览和自定义刷新沙盒环境，将禁用夜间重新计算，并且不会自动重新计算项目时间线。 您必须手动重新计算预览和自定义刷新沙盒环境的项目时间线。

### 项目时间线的自动重新计算 {#automatic-recalculation-of-project-timelines}

Workfront仅对满足以下所有条件的项目每天重新计算时间线：

* 具有当前状态。
* 项目更新类型设置为“自动”或“自动”和“更改时”。

  有关信息，请参阅[项目更新类型概述](../../../manage-work/projects/planning-a-project/project-update-type-overview.md)。

* 上次更新日期为过去3个月内。 Workfront管理员可以更改此默认功能。 有关详细信息，请参阅[配置项目的时间表重新计算](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)。

* 项目时间线的上次计算日期不在当前日历日期内。 这意味着项目时间轴的最后计算日期在当天的00:00之前。

您可以配置项目时间线的更新频率。 更新项目时间表时，会根据对项目所做的更改重新计算时间表。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

有关信息，请参阅[选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md)。

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

### 触发自动重新计算项目时间线的操作 {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

项目周期中的各种范围更改会自动重新计算项目时间线，包括以下操作：

* 正在更新任务状态。
* 将任务移动到其他项目。
* 更新任务的计划日期或计划完成日期。
* 更新任务的持续时间类型、任务限制或任务受分配人数量。
* 更新任务前置任务关系。
* 将批准添加到任务，该任务还会将时间添加到任务的规划完成日期。\
  有关审批设置的详细信息，请参阅[配置全局审批设置](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)。

## 手动重新计算 {#manual-recalculation}

作为项目所有者，您可以手动重新计算各个项目的时间表。 Workfront管理员可以在Workfront中手动重新计算所有时间线。

* [重新计算单个项目或批量项目的时间表](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [在“编辑项目”框中批量手动重新计算时间线](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [重新计算系统中所有项目的时间线(仅限Workfront管理员)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### 重新计算单个项目或批量项目的时间表 {#recalculate-timelines-for-individual-projects-or-in-bulk}

您可以在Workfront中从项目页面、项目列表或报表重新计算项目的时间表。

1. 转到要重新计算时间线的项目，然后单击项目名称左侧的&#x200B;**更多**&#x200B;图标![更多菜单](assets/qs-more-menu.png)。

   或

   转到项目列表或报告并选择一个或多个项目，然后单击列表顶部的&#x200B;**更多**&#x200B;图标![更多菜单](assets/qs-more-menu.png)。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >根据项目的复杂性，我们建议不要在批量重新计算其时间表时选择大量项目以确保最佳性能。 某些因素可能会使项目过于复杂，例如多个依赖项或分配，或者大量自定义字段。

1. 单击&#x200B;**重新计算时间线**。 此时会重新计算时间线，并在屏幕上显示一条成功消息。

   >[!TIP]
   >
   >在时间表重新计算完成之前，某些计划日期或预计日期可能显示为灰色。 这意味着重新计算尚未完成，并且日期可能会发生更改。

### 在编辑项目框中手动批量重新计算时间线 {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

您可以通过批量编辑多个项目来手动重新计算这些项目的时间线。

>[!TIP]
>
>根据项目的复杂性，我们建议在批量编辑项目时不要选择大量项目以确保最佳性能。 某些因素可能会使项目过于复杂，例如多个依赖项或分配，或者大量自定义字段。

1. 转到项目列表。
1. 选择列表中的多个项目，然后单击&#x200B;**编辑**。
1. 单击&#x200B;**设置**，然后选择&#x200B;**重新计算时间线**。

1. 单击&#x200B;**保存更改**。

### 重新计算系统中所有项目的时间线(仅限Workfront管理员) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Workfront管理员可以运行重新计算时间表诊断以立即重新计算Workfront系统中的所有时间表。 这使所有项目经理能够立即查看外部更改对计划和计划日期的影响。

有关重新计算整个Workfront站点时间线的更多信息，请参阅[配置项目的时间线重新计算](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)中的重新计算整个Workfront实例的时间线一节。

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
