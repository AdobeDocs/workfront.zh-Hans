---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 设置项目计划完成日期
description: 项目的计划完成日期是项目设置完成的日期。
author: Alina
feature: Work Management
exl-id: 996398c5-de92-445e-8e86-36b2efdcf6b5
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# 设置项目计划完成日期

项目的计划完成日期是项目设置完成的日期。

项目的计划起始日期和计划完成日期取决于项目任务的日期。 本文介绍了如何手动或自动设置项目的计划完成日期。 有关任务的计划完成日期的详细信息，请参阅 [任务计划完成日期概览](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

项目的计划完成日期可以人工设置，也可以自动设置，具体取决于您是从开始日期还是从完成日期开始计划项目。

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
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必须具有以下访问权限才能执行本文中的步骤：

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
   <td> <p>编辑对项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 人工设置项目的计划完成日期

在计划项目从完成日期开始时，您必须人工设置项目的计划完成日期。 

要从完成日期开始计划项目，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) ，然后单击 **项目**.

1. 单击 **新建项目** then **新建项目**.

   有关创建项目的更多信息，请参阅文章 [创建项目](../../../manage-work/projects/create-projects/create-project.md).

1. 选择 **项目详细信息** 在左侧面板中，单击 **编辑项目** 图标。

1. 在 **计划模式** 字段，选择 **完成日期**.

1. 指定 **计划完成日期** 的项目。
1. 单击 **保存更改**.

   开始向项目添加任务时， **计划开始日期** 根据所有任务的总持续时间计算项目的总持续时间。 

## 自动设置项目的计划完成日期

当您计划从开始日期开始的项目时，Adobe Workfront会自动计算项目的计划完成日期。 

要从开始日期计划项目，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) ，然后单击 **项目**.

1. 单击 **新建项目** then **新建项目**.

   有关创建项目的更多信息，请参阅文章 [创建项目](../../../manage-work/projects/create-projects/create-project.md).

1. 选择 **项目详细信息** 在左侧面板中，单击 **编辑项目** 图标。

1. 在 **计划模式** 字段，选择 **开始日期**.

1. 指定 **计划开始日期** 的项目。
1. 单击 **保存更改**.

   开始向项目添加任务时， **计划完成日期** 根据所有任务的总持续时间计算项目的总持续时间。 

   有关任务持续时间的详细信息，请参阅文章 [任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   项目的计划完成日期与项目上最后一个任务的计划完成日期一致。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>The Planned Completion Date of a task</h2>
<p>(NOTE: drafted because I created a new article, here: /Content/Manage work/Tasks/Task information/task-planned-completion-date.htm)</p>
<p>You can either specify the Planned Completion Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria.&nbsp;</p>
<ul>
<li><a href="#manually-set-the-planned-completion-date-of-a-task" class="MCXref xref">Manually set the Planned Completion Date of a task</a> </li>
<li><a href="#how-the-planned-completion-date-is-calculated-for-a-task" class="MCXref xref">How the Planned Completion Date is calculated for a task</a> </li>
</ul>
<p><strong>Manually set the Planned Completion Date of a task</strong></p>
<p>Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task.&nbsp;</p>
<p>You can manually set the Planned Completion Date&nbsp;when creating a task, as described in&nbsp;the article <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p>
<p>You can manually specify the Planned Completion Date when you select any of the following Task Constraints:&nbsp;</p>
<table border="1" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th> <p><strong>Task Constraint Type</strong> </p> </th>
<th> <p><strong>Effect of Manually Changing the Planned Completion Date</strong> </p> </th>
</tr>
</thead>
<tbody>
<tr>
<td> <p>Must Finish On</p> <p>Finish No Later Than</p> <p>Finish No Earlier Than</p> </td>
<td> <p><span class="s1">The Planned Start Date is adjusted in order to keep the Duration the same.</span> </p> </td>
</tr>
<tr>
<td> <p>Fixed Dates</p> </td>
<td> <p>The Duration is adjusted in order to keep the Planned Start Date the same.</p> </td>
</tr>
</tbody>
</table>
<p><strong>How the Planned Completion Date is calculated for a task</strong></p>
<p>When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task:</p>
<ul>
<li> <p>Task Constraint</p> <p>For more information about Task Constraints, see the article <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </li>
<li> <p>Task predecessor relationship</p> <p>For more information about task predecessors, see the article <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </li>
<li>Project Completion Date, when the project is scheduled from Completion Date.</li>
<li> <p>The time off schedule of the Primary&nbsp;Assignee of the task. </p> <p>When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the <strong>Consider user time off in task durations</strong> setting is selected for the <strong>User Time Off</strong> field. New projects inherit this setting from the Project&nbsp;Preferences area, but you can edit the setting at the project level. </p> <p>For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4. </p> <p>For information about the <strong>User Time Off</strong> preference, see the articles <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> or <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
</ul>
<p>When set automatically, the Planned Completion Date&nbsp;is determined based on the following calculation:&nbsp;</p>
<p><code>Planned Completion Date = Planned Start Date + Duration</code> </p>
<p>For example, if your task has a start date of September 16 and a duration of 10 days, the Planned Completion Date is September 26.</p> <note type="note">
&nbsp;The Update Type for the project must also be&nbsp;set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically&nbsp;adjusted.
<br>For more information about the Update Type, see the article
<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.
</note>
</div>
-->
