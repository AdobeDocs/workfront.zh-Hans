---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 分派任务
description: 您可以将任务分配给用户、角色或团队，以指明负责完成任务的人员。 您可以一次将任务分配给多个资源。
author: Lisa
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '1617'
ht-degree: 2%

---

# 分配任务

<!--Audited: 10/2025-->

<!--remove production/ preview and old/ new experience references at prod-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md). 

</div>-->

您可以将任务分配给用户、工作角色或团队，以指明负责完成任务的人员。 您可以一次将任务分配给多个资源。

>[!TIP]
>
>您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
>
>如果在停用用户、工作角色或团队之前已分配用户、工作角色或团队，则它们仍会分配给工作项。 在这种情况下，我们建议执行以下操作：
>
>* 将工作项重新分配给活动资源。
>* 将已停用团队中的用户与活动团队关联，并将工作项重新分配给活动团队。
>

分配给任务的用户的数量和任务所有者的计划可以修改任务的计划日期，从而导致更改项目的时间表。 有关将多个用户分配到任务的影响的信息，请参阅[修改任务分配的概述](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)。

除了本文之外，我们还建议您阅读以下文章，以了解有关分配任务的更多信息：

* [修改任务分配的概述](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [进行智能分配](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [创建高级工作](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [修改任务列表中的多个用户分配](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [计划项目概述](../../../manage-work/projects/planning-a-project/plan-project.md)
* [任务计划完成日期概述](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [设置项目计划完成日期](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [在工作负载均衡器中分配工作概述](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td> <p>标准</p>
   <p>工作版或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>编辑对项目和任务的访问权限</p> <p>查看或更高的用户访问权限</p> </td> 
  </tr> 
  <tr> 
   <td>对象权限</td>
   <td>为任务分配或更高权限</td>
  </tr>
 </tbody>
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 向工作角色、团队和用户进行多个分配的注意事项

将多个资源分配给工作项时，请考虑以下事项：

* 用户可以有多个与其配置文件关联的工作角色。 有关将用户与工作角色关联的信息，请参阅[编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

* 如果将多个用户分配给任务或问题，则您选择的第一个用户会自动被指定为任务或问题的所有者。
有关更改此内容的说明，请参阅[创建高级工作](create-advanced-assignments.md)一文中有关“设为主要工作”选项的信息。

* 团队不能是任务或问题的主要被分配人。 在任务或问题中，只能将用户或工作角色指定为主要角色。

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* 项目中的任务和问题可能首先分配给一个或多个团队或工作角色。 当项目准备开始时，可能需要将它们也分配给用户：

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>团队</td>
   <td>如果将任务分配给团队并且还分配了用户，则该任务仍会分配给团队和用户，即使用户不是团队成员。</td>
  </tr>
  <tr>
   <td>工作角色</td>
   <td><p>如果将任务或问题分配给一个或多个角色，然后又分配了用户，则根据以下规则确定要与附加用户（如果有）关联的工作角色：</p>
     <ul>
      <li>如果只分配了一个工作角色，并且该工作角色与用户的主要角色（在其配置文件中配置）匹配，则任务或问题仅分配给该用户。</li>
      <li>如果分配了多个角色，并且其中至少一个角色与用户的其他角色之一匹配，则任务或问题会分配给用户（如果有多个匹配，则随机选择角色），以及分配的任何其他角色</li>
      <li>如果至少分配了一个工作角色，并且没有匹配用户的工作角色，则任务或问题会分配给该角色和用户。</li>
     </ul>
   <p>有关用户的主要角色和其他角色的信息，请参阅<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">编辑用户配置文件</a>。</p>
   </td> 
     </tr>
  </tbody>
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations for multiple user assignments and using schedules</h2>
<p>(NOTE: moved to the Modify task assignments overview standalone article)</p>
<p>You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. </p>
<p>When you assign multiple users to a task, your Workfront administrator <span>or a group administrator</span> determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: </p>
<ul>
<li> <p><strong>The Primary Assignee's schedule</strong>: this is the schedule associated with the user designated as the task Owner.</p> <p>For information about associating users with schedules, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li>
<li><strong>The Project's schedule</strong>: this is the schedule associated with the project. For adding a schedule to a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
</ul>
<p>For information about setting up which schedule a project uses in the case of multiple assignments, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p>
</div>
-->

## 分配单个任务

1. 转到要分配的任务。
1. 在任务标题的&#x200B;**工作**&#x200B;字段中单击&#x200B;**分配给**

   或

   如果任务已分配，则单击分配的名称。

   ![分配](assets/assignments-from-task-header-0825.png)

1. 执行下列操作之一：

   * 开始键入要分配的用户、工作角色或团队的名称，然后在名称出现在列表中时单击该名称。

     >[!TIP]
     >
     >添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分具有相同名称的用户。 用户必须与至少一个工作角色关联，才能在添加时查看工作角色。
     >
     >您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅[授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

   * （视情况而定）显示&#x200B;**用户和团队**&#x200B;或&#x200B;**工作角色**&#x200B;列表时，单击其中的一个名称。 有关详细信息，请参阅[智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md)。

     您可以开始键入要分配给任务的任何用户、团队或工作角色的名称，然后当该名称显示在列表中时将其选定。

   * 单击&#x200B;**高级**。

     有关如何进行高级分配的信息，请参阅[创建高级分配](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)。

1. 单击&#x200B;**保存**。
1. （可选且有条件）单击任务右侧面板中任务名称旁边的&#x200B;**X图标**&#x200B;可删除任务（如果您单击了&#x200B;**高级**）。

## 内联编辑任务时分配列表中的任务

当任何任务字段在列表视图中可见时，您可以在列表或报表中分配任务。 这是分配任务的更快方式。 本文介绍了如何修改列表中一项任务的分配。 有关修改列表中多个任务的多个分配的信息，请参阅[修改任务列表中的多个用户分配](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)。

根据视图中显示的字段，可以将以下实体分配给任务：

| 字段 | 分配的实体 |
|---|---|
| **分配给** | 分配一个用户 |
| **已分配** | 分配一个用户 |
| **分配** | 分配用户、工作角色或团队 |

要在列表中分配任务，请执行以下操作：

1. 转到任务列表，该列表中具有“任务负责人”、“任务分派”或“工作总揽”字段。
1. （可选）单击&#x200B;**自动保存**&#x200B;下拉菜单，然后从以下选项中选择：

   | 选项 | 选项说明 |
   |---|---|
   | 自动保存 | 您对任务所做的更改会自动保存，并且您无法还原这些更改 |
   | 手动保存 | 您必须手动保存更改。 在保存更改之前，您可以还原这些更改。 |
   | 时间线规划 | 您必须手动保存更改。 在保存更改之前，您可以还原这些更改。 保存更改和所有项目依赖项比选择手动保存更快。 |

   有关在列表中编辑任务时保存任务的详细信息，请参阅[在列表中编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)。

1. 要分配任务，请执行下列操作之一：

   * 在&#x200B;**分配给**&#x200B;或&#x200B;**分配的**&#x200B;字段中单击，并开始键入要分配给任务的活动用户的名称，然后在任务显示在列表中时单击该名称。
   * 单击&#x200B;**工作总揽**&#x200B;字段并开始键入要分配给任务的活跃用户、工作角色或团队的名称，然后当它显示在列表中时单击它。

     >[!TIP]
     >
     >添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分具有相同名称的用户。 用户必须与至少一个工作角色关联，才能在添加时查看工作角色。
     >
     >您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅[授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)

     <!--<span class="preview">When adding a job role assignment, you can search for the job role or location. Select a Job role to use the default billing rate for the assignment, or select a Rate Card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. （视情况而定）在“工作总揽”字段中，单击列表底部的&#x200B;**高级**&#x200B;或工作总揽框右上角的&#x200B;**人员图标** ![人员图标](assets/teams.png)以打开&#x200B;**高级工作总揽**&#x200B;框并创建高级工作总揽。

   有关详细信息，请参阅[创建高级工作](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)。

   >[!TIP]
   >
   >您不能从“分配至”或“已分配”字段进行高级分配。

1. 将任务负责人添加到任务后，按Enter键或单击页面上的任意位置保存更改（如果已选择“自动保存”）。 否则，请单击&#x200B;**保存**。

## 从列表批量分配多个任务

1. 转到要批量分配的任务的列表。
1. （视情况而定）如果您在项目下的任务列表中，请确保已选择&#x200B;**自动保存**&#x200B;选项。

   >[!IMPORTANT]
   >
   >在项目中手动保存任务时，无法批量编辑任务。

1. 在任务列表中选择多个任务。
1. 单击&#x200B;**编辑**。

   将打开&#x200B;**编辑任务**&#x200B;框。

1. 在&#x200B;**工作**&#x200B;区域，在提供的&#x200B;**搜索人员、角色或团队**&#x200B;字段中开始键入用户、团队或角色的名称，然后在用户、团队或角色显示在列表中时单击它们

   >[!IMPORTANT]
   >
   >如果已经分配了任何任务，您在此处指定的资源将添加到任务中，而不是替换任务上的现有资源。

1. 为所选任务指定以下字段：

   * 将鼠标悬停在分配名称上，然后单击&#x200B;**设为主要项**&#x200B;以指示哪个分配人是任务的所有者。
   * **持续时间类型**

     有关任务的持续时间类型的信息，请参阅[任务持续时间和持续时间类型概览](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

   * **持续时间**
   * **计划小时数**

     有关详细信息，请参阅[编辑任务](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md)。

1. （可选）如果要从所有任务中移除现有被分配人，请在&#x200B;**搜索人员、角色或团队**&#x200B;字段中单击其名称旁边的&#x200B;**x**。

1. 单击&#x200B;**保存**。
1. （可选且有条件）当任务列表中显示&#x200B;**分配给**&#x200B;或&#x200B;**工作总揽**&#x200B;字段时，单击其中一列的任务内容，然后单击被分配人名称旁边的&#x200B;**X图标**&#x200B;以将其从任务中删除。


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations about unassigning tasks</h2>
<p>(NOTE: moved this to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm)</p>
<p>You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.</p>
<p>For more information about removing assignments from tasks in bulk, see <a href="../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md" class="MCXref xref">Modify multiple user assignments in a task list</a>. </p>
<p>Consider the following when removing assignments from tasks: </p>
<ul>
<li>When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.</li>
<li>When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->


<!--Assigning multiple tasks in bulk from a list differs depending on which environment you choose. 

### Assign multiple tasks in bulk from a list in the Production environment

1. Go to a list of tasks that you want to assign in bulk. 
1. (Conditional) Ensure that the **Autosave** option is selected if you are on a list of tasks under a project.

   >[!IMPORTANT]
   >
   >You cannot edit tasks in bulk when saving tasks manually on a project.

1. Select several tasks in the tasks list. 
1. Click **Edit**.

   The **Edit Tasks** dialog box opens in the new experience.

1. Continue assigning the tasks using the new experience.

   For more information, see the section [Assign multiple tasks in bulk from a list in the new experience](#assign-multiple-tasks-in-bulk-from-a-list-in-the-new-experience) in this article.

1. (Optional) Click **Switch back to old experience** at the bottom of the **Edit Tasks** box to open the old experience.

1. (Conditional) Using the old experience, in the **Assignments** area, select the **Assignee** box, then start typing the name of a user, job role, or team that you want to assign to all the tasks.

   >[!IMPORTANT]
   >
   >If any of the tasks is already assigned, the resources you indicate here are added to the tasks instead of replacing the existing resources on the tasks. 

1. (Optional) Select the radio button in the **Task Owner** column to indicate which resource is the primary assignee or the Owner of the task, when you assign more than one resource to the task. This is not available for teams. 
1. (Conditional) Specify the **Allocation %** for each resource assigned to the task if all the tasks you selected have a Duration Type of Effort Driven or Calculated Assignment. This indicates how much of their time these resources should spend on completing the task. This is only available for users and job roles.

   Or

   Specify the amount of **Hours** for each resource assigned to the task if all the tasks you selected have a Duration Type of Simple. The total of all hours for all resources should equal the number of Planned Hours for the task.

   >[!IMPORTANT]
   >
   >You cannot specify the allocation percentage or the number of hours per resource if the tasks you selected have different Duration Types or of the tasks you selected have different Duration Types.

   For information about Duration Type on tasks, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Optional) Select a role that the user should fulfill on the task from the **Pick a role** drop-down menu in the **Assignee's Role** column when you assign users to tasks. If you do not select a role, Workfront automatically selects the user's Primary Role. 

1. (Optional) If you want to remove existing assignees from all tasks do one of the following:

   1. Start typing the name of a user, role, or team you want to remove from the task, then select it when it appears on the list and click **Remove Assignee** to remove more assignees.
   1. Click **Remove All Existing Assignees** to remove all assignees from all selected tasks.

1. Click **Save Changes**.
1. (Optional and conditional) When the Assigned to or the Assignments fields display in your list of tasks, click inside one of these columns for a task, then click the **X icon** next to the name of an assignee to remove it from the task.


#### Assign multiple tasks in bulk from a list in the new experience

1. Go to a list of tasks that you want to assign in bulk.
1. (Conditional) Ensure that the **Autosave** option is selected if you are on a list of tasks under a project.

   >[!IMPORTANT]
   >
   >You cannot edit tasks in bulk when saving tasks manually on a project.

1. Select several tasks in the tasks list. 
1. Click **Edit**.

   The **Edit Tasks** dialog box opens.

1. In the **Assignments** area, start typing the name of users, teams, or roles in the **Search people, roles, or teams** field provided, then click them when they display in the list

   Or 

   Click **Assign to me** to assign it to yourself.

   >[!IMPORTANT]
   >
   >If any of the tasks is already assigned, the resources you indicate here are added to the tasks instead of replacing the existing resources on the tasks.

1. Click inside the **Duration Type** field and choose a Duration Type. 

   For information about Duration Type on tasks, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Conditional) Depending on what **Duration Type** you selected, update the following fields: 

   * Duration
   * Planned Hours

      For more information, see [Edit tasks](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md). 

1. (Optional) If you want to remove existing assignees from all tasks, click the **x** next to their name in the **Search people, roles, or teams** field.

1. Click **Save**.
1. (Optional and conditional) When the **Assigned to** or the **Assignments** fields display in your list of tasks, click inside one of these columns for a task, then click the **X icon** next to the name of an assignee to remove it from the task.

<div class="preview">
### Assign multiple tasks in bulk from a list in the Preview environment
-->