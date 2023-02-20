---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 在任务列表中修改多个用户分配
description: 在管理任务分配时，您可以使用任务列表中的批量编辑功能同时修改多个任务的分配。
author: Alina
feature: Work Management
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 0%

---

# 在任务列表中修改多个用户分配

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

在管理任务分配时，您可以使用任务列表中的批量编辑功能同时修改多个任务的分配。

本文是指修改任务列表中多个任务的多个用户分配。 另请参阅以下文章，了解如何修改其他区域中多个任务的分配：

* 有关使用工作负载平衡器分配任务的信息，请参阅 [工作负载平衡器中分配工作的概述](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

有关将任务分配给列表中的一个资源的信息，请参阅 [分配任务](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## 访问要求

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目和任务的访问权限</p> <p>查看或更高权限用户</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>对任务贡献或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration&nbsp;Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration&nbsp;Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## 修改多个任务的分配

1. 转到包含要修改分配的任务的列表。
1. （可选）创建过滤器，以仅显示分配给要修改的被分派人的任务。

   例如，如果您的项目包含特定角色作为多个任务的默认代理人，则可以创建一个过滤器以仅显示具有该角色作为代理人的任务。 然后，您可以将角色替换为特定用户。

   有关创建过滤器的信息，请参阅 [创建或编辑过滤器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. 要筛选角色，请选择 **分配角色**，然后单击 **ID**.

   >[!TIP]
   >
   >请勿使用 **已分配给** 字段。 这将只查找任务的主所有者，而不查找可分配给任务的任何角色。

   或

   要筛选用户，请选择 **分配用户、** 然后单击 **ID。**

   >[!TIP]
   >
   >请勿使用 **已分配给** 字段。 这将仅查找任务的主所有者，而不查找可分配给任务的任何用户。

1. 选择要修改其分配的任务，然后单击 **编辑** 图标 ![](assets/edit-icon.png).

   此时将显示“编辑任务”页。 您编辑的项目将显示在页面的左上角。

1. 转到 **分配** 中。
1. 执行下列操作之一以添加或删除受分配者：

   >[!IMPORTANT]
   >
   >删除受分配者会影响任务小时数和分配百分比。 有关更多信息，请参阅 [删除受分配者如何影响任务小时数和分配百分比](#how-removing-assignees-affects-task-hours-and-allocation-percentages) 在本文中。

   * 要添加新的被分派人，请执行以下操作：

      1. 在 **分配** 选择 **被分派人**.

         此时将显示所有选定任务中通用的信息。 例如，如果将同一用户分配到所有任务，则该用户将显示在 **被分派人** 列。 如果所选任务中的信息不常见，则不显示任何信息。

      1. 开始键入用户、角色或团队的名称，然后在列表中显示时选择该名称。 分配将被添加，且不会替换选定任务上的当前分配。
      >[!TIP]
      >
      > * 您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
      >   
      > * 添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分名称相同的用户。 用户必须至少与一个作业角色关联，才能在您添加时查看该角色。

         > 
         >   如果在停用用户、作业角色或团队之前已分配它们，则它们仍会被分配到工作项。 在这种情况下，我们建议执行以下操作：
         >   
         >     * 将工作项重新分配给活动资源。
         >     * 将已停用团队中的用户与活动团队相关联，并将工作项重新分配给活动团队。



   * 要删除单个受分配人，请执行以下操作：

      1. 单击 **X图标** 如果要删除的被分派人名称旁边(如果被分派人显示在“分配”(Assignments)列表中)。

         或

         （视情况而定）如果要删除的代理人未显示在“工作总揽”部分中，因为该代理人只被分配到您选择的某些任务，请单击 **删除被分派人** 然后开始键入要删除的被分派人的名称，然后在该名称出现在下拉列表中时单击该名称。
   * 要删除所有现有受分配者，请执行以下操作：

      1. 单击 **删除所有现有的受分配人**，然后单击 **是，删除所有受分配人**.

         这不仅会删除常见的受分配人（在编辑对话框中显示的受分配人），还会删除所有选定任务上的所有受分配人。
      将用户从任务中删除可能会影响任务小时数和分配百分比。

      有关更多信息，请参阅 [修改任务分配概述](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).





1. （可选）为受分配者修改以下任意选项：

   * （视情况而定） **分配%或小时数**:指定新的分配百分比或小时数。

      >[!NOTE]
      >
      >仅当所有正在编辑的任务的持续时间类型相同时，才能修改此选项。 当持续时间类型为计算工作或工作驱动时，您可以更新分配百分比。 当持续时间类型为“简单”时，您可以更新“小时”。 有关持续时间类型的信息，请参阅 [任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
      如果字段为空，则表示值在各任务中不同；但是，您仍然能够对其进行修改。

   * **任务所有者**:选择此选项，使被分派人成为所有正在编辑的任务的所有者。
   * **被分派人的角色**:从下拉列表中选择一个角色。 如果未选择，Adobe Workfront会自动选择用户的主要角色。

1. 单击 **保存更改。**
