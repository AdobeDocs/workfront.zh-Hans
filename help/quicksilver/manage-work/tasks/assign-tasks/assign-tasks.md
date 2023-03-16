---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 分配任务
description: 您可以向用户、角色或团队分配任务，以指示谁负责完成任务。 您可以一次将任务分配给多个资源。
author: Alina
feature: Work Management
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '1789'
ht-degree: 1%

---

# 分配任务

您可以向用户、作业角色或团队分配任务，以指明谁负责完成任务。 您可以一次将任务分配给多个资源。

>[!TIP]
>
>您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
>
>如果在停用用户、作业角色或团队之前已分配它们，则它们仍会被分配到工作项。 在这种情况下，我们建议执行以下操作：
>
>* 将工作项重新分配给活动资源。
>* 将已停用团队中的用户与活动团队相关联，并将工作项重新分配给活动团队。
>


分配给任务的用户数和任务所有者的计划可以修改任务的计划日期，从而更改项目的时间表。 有关为任务分配多个用户的影响的信息，请参阅 [修改任务分配概述](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

除了本文之外，我们建议您阅读以下文章以了解有关分配任务的更多信息：

* [修改任务分配概述](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [进行智能分配](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [创建高级分配](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [在任务列表中修改多个用户分配](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [计划项目概述](../../../manage-work/projects/planning-a-project/plan-project.md)
* [任务计划完成日期概览](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [设置项目计划完成日期](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [工作负载平衡器中分配工作的概述](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## 访问要求

<!--drafted for P&P - replace table below with this:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>View or higher access to Users</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目和任务的访问权限</p> <p>查看或更高权限用户</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>对任务贡献或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 对工作角色、团队和用户进行多种分配的注意事项

在为工作项分配多个资源时，请考虑以下事项：

* 用户可以拥有与其配置文件关联的多个作业角色。 有关将用户与作业角色关联的信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 如果为任务或问题分配多个用户，则您选择的第一个用户将自动指定为任务或问题的所有者。
有关更改此选项的说明，请参阅文章中有关“设为主要”选项的信息 [创建高级分配](create-advanced-assignments.md).

* 团队不能是任务或问题上的主要代理人。 在任务或问题上，只能将用户或作业角色指定为主角色。

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* 项目中的任务和问题可能会首先分配给一个或多个团队或作业角色。 当项目准备就绪后，可能还需要将它们分配给用户：

   <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>团队</td>
   <td>如果您为团队分配任务，并且还为用户分配了任务，则该任务仍会分配给团队和用户，即使用户不是团队的成员也是如此。</td>
  </tr>
  <tr>
   <td>职位角色</td>
   <td><p>如果您将任务或问题分配给一个或多个角色，然后又分配了一个用户，则会根据以下规则确定要与附加用户关联的作业角色（如果有）：</p>
     <ul>
      <li>如果只分配了一个作业角色，并且该角色与用户的主角色（在其配置文件中配置）匹配，则该任务或问题将仅分配给该用户。</li>
      <li>如果分配了多个角色，并且其中至少一个角色与用户的其他角色之一匹配，则任务或问题会被分配给用户（如果存在多个匹配，则随机选择角色），以及分配的任何其他角色</li>
      <li>如果至少分配了一个作业角色，并且与用户的作业角色没有匹配，则任务或问题将分配给角色或角色以及用户。</li>
     </ul>
   <p>有关用户的主要角色和其他角色的信息，请参阅 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">编辑用户的配置文件</a>.</p>
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
1. 单击 **分配给** 在 **分配** 字段。

   或

   如果已分配任务或问题，请单击分配的名称。

![](../assign-tasks/assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. 执行下列操作之一：

   * 开始键入要分配的用户、角色或团队的名称，然后在列表中显示该名称时单击该名称。


      >[!TIP]
      >
      >添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分名称相同的用户。 用户必须至少与一个作业角色关联，才能在您添加时查看该角色。


   * （视情况而定）单击 **建议的分配** 列表（如果显示此列表）。 有关更多信息，请参阅 [智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

   * 单击 **高级**

      有关如何进行高级分配的信息，请参阅 [创建高级分配](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. 单击&#x200B;**保存**。
1. （可选并视情况而定）单击 **X图标** 单击任务右侧面板中用于删除分配的分配名称旁边的 **高级**.

## 在列表中分配任务

当列表视图中显示任何分配字段时，您可以在列表或报表中分配任务。 这是分配任务的更快方式。 本文介绍了如何修改列表中某个任务的分配。 有关在列表中为多个任务修改多个分配的信息，请参阅 [在任务列表中修改多个用户分配](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

根据视图中显示的字段，您可以为任务分配以下实体：

| 字段 | 已分配的实体 |
|---|---|
| **分配给** | 分配一个用户 |
| **已分派** | 分配一个用户 |
| **分配** | 分配用户、工作角色或团队 |

要在列表中分配任务，请执行以下操作：

1. 转到视图中具有“已分配至”、“已分配”或“分配”字段的任务列表。
1. （可选）单击 **自动保存** 下拉菜单，然后从以下选项中选择：

   | 选项 | 选项描述 |
   |---|---| 
   | 自动保存 | 您对任务所做的更改会自动保存，您无法还原它们 |
   | 手动保存 | 您必须手动保存更改。 您可以在保存更改之前还原这些更改。 |
   | 时间线规划 | 您必须手动保存更改。 您可以在保存更改之前还原这些更改。 保存更改和所有项目依赖项的速度比选择“手动保存”时要快。 |

   有关在列表中编辑任务时保存任务的详细信息，请参阅 [在列表中编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. 要分配任务，请执行以下操作之一：

   * 在 **分配给** 或 **已分配** 字段，然后开始键入要分配给任务的活动用户的名称，然后在任务显示在列表中时单击该名称。
   * 在 **分配** 字段，然后开始键入要分配给任务的活动用户、作业角色或团队的名称，然后在列表中显示时单击该名称。

      >[!TIP]
      >添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分名称相同的用户。 用户必须至少与一个作业角色关联，才能在您添加时查看该角色。
      >
      >
   >

1. （视情况而定）在 **分配** 字段，单击 **人员** 图标以打开 **高级分配** 框中创建高级分配。

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   有关更多信息，请参阅 [创建高级分配](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   您不能从“已分配给”或“已分配”字段进行高级分配。

1. 在将受分配人添加到任务后，按Enter键或单击页面上的任意位置，以保存所做更改（如果选择了“自动保存”）。 否则，请单击 **保存**.

## 为用户分配多个任务

1. 转到要批量分配的任务列表。
1. （视情况而定）确保 **自动保存** 选项。

   >[!IMPORTANT]
   在项目上手动保存任务时，无法批量编辑任务。

1. 在任务列表中选择多个任务。
1. 单击 **编辑**.

   的 **编辑任务** 对话框。

1. 在 **分配** 区域，选择 **被分派人** 框中，然后开始键入要分配给所有任务的用户、作业角色或团队的名称。

   >[!IMPORTANT]
   如果已分配任何任务，则您在此处指示的资源将添加到任务中，而不是替换任务中的现有资源。

1. （可选）选择 **任务所有者** 列来指示在向任务分配多个资源时，哪个资源是主要任务接受者或任务的所有者。 这不适用于团队。
1. （视情况而定）指定 **分配%** 对于分配给任务的每个资源，如果您选择的所有任务都具有持续时间类型“工作驱动”或“计算分配”。 这表示这些资源在完成任务上应花费的时间。 此设置仅适用于用户和作业角色。

   或

   指定 **小时** 对于分配给任务的每个资源，如果您选择的所有任务的持续时间类型都为“简单”。 所有资源的所有小时总数应等于任务的计划小时数。

   >[!IMPORTANT]
   如果您选择的任务具有不同的持续时间类型或您选择的任务具有不同的持续时间类型，则无法指定每个资源的分配百分比或小时数。

   有关任务的持续时间类型的信息，请参阅 [任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. （可选）从 **选择角色** 下拉菜单(位于 **被分派人的角色** 列。 如果未选择角色，Workfront会自动选择用户的主角色。

1. （可选）如果要从所有任务中删除现有任务分配者，请执行以下操作之一：

   1. 开始键入要从任务中删除的用户、角色或团队的名称，然后在列表中显示该名称时将其选中，并单击 **删除被分派人** 以删除更多受分配者。
   1. 单击 **删除所有现有的受分配人** 从所有选定任务中删除所有受分配者。

1. 单击 **保存更改**.
1. （可选和视情况而定）当任务列表中显示“已分配给”或“分配”字段时，在任务的这些列之一中单击，然后单击 **X图标** 将其从任务中删除的被分派人名称旁边。

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


