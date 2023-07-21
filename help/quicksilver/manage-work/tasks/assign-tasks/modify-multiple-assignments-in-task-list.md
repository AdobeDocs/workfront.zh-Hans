---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 修改任务列表中的多个用户分配
description: 在管理任务分配时，可以使用任务列表中的批量编辑功能一次为多个任务同时修改它们。
author: Alina
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 0%

---

# 修改任务列表中的多个用户分配

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

在管理任务分配时，可以使用任务列表中的批量编辑功能一次为多个任务同时修改它们。

本文参考为任务列表中的多个任务修改多个用户分配。 另请参阅以下文章，了解如何修改其他区域中多个任务的分配：

* 有关使用工作负载均衡器分配任务的信息，请参见 [在工作负载均衡器中分配工作概述](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

有关将任务分配给列表中某个资源的信息，请参阅 [分配任务](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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
   <td> <p>编辑对项目和任务的访问权限</p> <p>查看或更高的用户访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>向任务分配或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

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
1. （可选）创建一个过滤器，以便仅显示分配给要修改的受让人的任务。

   例如，如果您的项目包含特定角色作为多个任务的默认被分配人，则可以创建一个过滤器，以仅显示以该角色作为被分配人的任务。 然后，您可以使用特定用户替换角色。

   有关创建过滤器的信息，请参见 [创建或编辑筛选器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. 要筛选角色，请选择 **任务角色**，然后单击 **ID**.

   >[!TIP]
   >
   >请勿使用 **分配给** 字段。 这仅查找任务的主要所有者，而不是可分配给他们的任何角色。

   或

   要筛选用户，请选择 **任务用户，** 然后单击 **ID。**

   >[!TIP]
   >
   >请勿使用 **分配给** 字段。 这仅查找任务的主要所有者，而不是可分配给他们的任何用户。

1. 选择要修改分配的任务，然后单击 **编辑** 图标 ![](assets/edit-icon.png).

   此时将显示“编辑任务”页。 您编辑的项目将显示在页面的左上角。

1. 转到 **指定任务** 部分。
1. 执行以下操作之一以添加或删除被分配人：

   >[!IMPORTANT]
   >
   >移除被分派人可能会影响任务小时数和分配百分比。 有关更多信息，请参阅部分 [移除被分配人如何影响任务小时数和分配百分比](#how-removing-assignees-affects-task-hours-and-allocation-percentages) 本文章中。

   * 要添加新的被分派人，请执行以下操作：

      1. 在 **指定任务** 部分，选择 **被分派人**.

         将显示所有选定任务中通用的信息。 例如，如果将同一用户分配到所有任务，则该用户将显示在 **被分派人** 列。 如果所选任务中的信息不常见，则不会显示任何信息。

      1. 开始键入用户、角色或团队的名称，然后在此名称显示在列表中时将其选定。 分配已添加，不会替换选定任务上的当前分配。


     >[!TIP]
     >
     > * 您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
     >   
     > * 添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分具有相同名称的用户。 用户必须与至少一个工作角色关联，才能在添加时查看该角色。 您必须在访问级别中启用“查看联系人信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅 [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     > 
     >   如果在停用用户、工作角色或团队之前分配了用户、工作角色或团队，则他们仍会分配到工作项。 在这种情况下，我们建议执行以下操作：
     >   
     >     * 将工作项重新分配给有效资源。
     >     * 将已停用团队中的用户与活动团队相关联，并将工作项重新分配给活动团队。


   * 要移除单个被分配人，请执行以下操作：

      1. 单击 **X图标** 如果被分派人显示在“工作总揽”列表中，则位于要删除的被分派人姓名旁边。

         或

         （视情况而定）如果要删除的被分配人由于仅分配给您选择的某些任务而未显示在“工作总揽”部分中，请单击 **移除被分派人** 开始键入要删除的被分配人的名称，然后在名称出现在下拉列表中时单击该名称。

   * 要删除所有现有被分配人，请执行以下操作：

      1. 单击 **移除所有现有被分配人**，然后单击 **是，删除所有被分配人**.

         这不仅会删除常见的被分配人（显示在“编辑”对话框中的被分配人），还会删除所有选定任务上的所有被分配人。

     从任务中删除用户可能会影响任务小时数和分配百分比。

     有关更多信息，请参阅 [修改任务分配的概览](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. （可选）为被分派人修改以下任意选项：

   * （视情况而定） **分配%或小时**：指定新的分配百分比或小时。

     >[!NOTE]
     >
     >仅当所有正在编辑的任务中的持续时间类型相同时，才能修改此选项。 当持续时间类型为已计算的工作或投入比驱动时，您可以更新分配%。 当持续时间类型为简单时，您可以更新小时数。 有关持续时间类型的信息，请参见 [任务工期和工期类型概览](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     如果该字段为空，则意味着该值在各任务中是不同的；但是，您仍然能够修改它。

   * **任务所有者**：选择此选项可让被分派人成为所有正在编辑任务的任务所有者。
   * **被分派人的角色**：从下拉列表中选择一个角色。 如果未选中，Adobe Workfront会自动选择用户的主要角色。

1. 单击 **保存更改。**
