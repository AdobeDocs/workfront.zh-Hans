---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 分配任务
description: 您可以将任务分配给用户、角色或团队，以指明负责完成任务的人员。 您可以一次将任务分配给多个资源。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '2027'
ht-degree: 1%

---

# 分配任务

<span class="preview">此页面上高亮显示的信息是指尚未普遍可用的功能。 它只能在“预览”环境中用于所有客户，或者在“生产”环境中用于启用快速版本的客户。</span>

<span class="preview">有关快速版本的信息，请参阅 [为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">有关当前版本的信息，请参阅 [2024年第三季度发行版概述](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

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

分配给任务的用户的数量和任务所有者的计划可以修改任务的计划日期，从而导致更改项目的时间表。 有关将多个用户分配给一项任务的影响的信息，请参阅 [修改任务分配的概览](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

除了本文之外，我们还建议您阅读以下文章，以了解有关分配任务的更多信息：

* [修改任务分配的概览](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [进行智能分配](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [创建高级工作](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [修改任务列表中的多个用户分配](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [计划项目概述](../../../manage-work/projects/planning-a-project/plan-project.md)
* [任务计划完成日期概览](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [设置项目计划完成日期](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [在工作负载均衡器中分配工作概述](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

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

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目和任务的访问权限</p> <p>查看或更高的用户访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>向任务分配或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 向工作角色、团队和用户进行多个分配的注意事项

将多个资源分配给工作项时，请考虑以下事项：

* 用户可以有多个与其配置文件关联的工作角色。 有关将用户与工作角色关联的信息，请参阅 [编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 如果将多个用户分配给任务或问题，则您选择的第一个用户会自动被指定为任务或问题的所有者。
有关更改此设置的说明，请参阅文章中有关“设为主要节点”选项的信息 [创建高级工作](create-advanced-assignments.md).

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
   <p>有关用户的主要角色和其他角色的信息，请参阅 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">编辑用户配置文件</a>.</p>
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
1. 单击 **分配给** 在 **指定任务** 任务或问题标题中的字段。

   或

   如果任务或问题已分配，则单击分配的名称。

   生产环境中的示例图像：
   ![](../assign-tasks/assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

   <span class="preview">“预览”环境中的示例图像：</span>
   ![分配](assets/assignments-box-in-task-header.png)

1. 执行下列操作之一：

   * 开始键入要分配的用户、角色或团队的名称，然后当该名称出现在列表中时单击它。


     >[!TIP]
     >
     >添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分具有相同名称的用户。 用户必须与至少一个工作角色关联，才能在添加时查看工作角色。
     >
     >您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅 [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     >
     ><span class="preview">添加工作角色分配时，您可以搜索工作角色或位置。 选择“系统/默认工作角色”以使用分配的默认开单费率，或者选择“费率卡工作角色”以使用费率卡中的开单费率。 有关费率卡的详细信息，请参阅 [管理费率卡](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


   * （视情况而定）单击 **建议的分配** 列表（如果显示此列表）。 有关更多信息，请参阅 [智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

   * 单击 **高级**

     有关如何进行高级工作分配的信息，请参见 [创建高级工作](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. 单击&#x200B;**保存**。
1. （可选且视情况而定）单击 **X图标** 在任务右侧面板中任务名称的旁边，用于移除任务（如果单击） **高级**.

## 在列表中分配任务

当任何任务字段在列表视图中可见时，您可以在列表或报表中分配任务。 这是分配任务的更快方式。 本文介绍了如何修改列表中一项任务的分配。 有关为列表中的多个任务修改多个分配的信息，请参见 [修改任务列表中的多个用户分配](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

根据视图中显示的字段，可以将以下实体分配给任务：

| 字段 | 分配的实体 |
|---|---|
| **分配给** | 分配一个用户 |
| **已指定** | 分配一个用户 |
| **分配** | 分配用户、工作角色或团队 |

要在列表中分配任务，请执行以下操作：

1. 转到任务列表，该列表中具有“任务负责人”、“任务分派”或“工作总揽”字段。
1. （可选）单击 **自动保存** 下拉菜单并从以下选项中进行选择：

   | 选项 | 选项说明 |
   |---|---| 
   | 自动保存 | 您对任务所做的更改会自动保存，并且您无法还原这些更改 |
   | 手动保存 | 您必须手动保存更改。 在保存更改之前，您可以还原这些更改。 |
   | 时间线规划 | 您必须手动保存更改。 在保存更改之前，您可以还原这些更改。 保存更改和所有项目依赖项比选择手动保存更快。 |

   有关在列表中编辑任务时保存任务的更多信息，请参阅 [编辑列表中的任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. 要分配任务，请执行下列操作之一：

   * 在 **分派给** 或 **已指定** 开始键入要分配给任务的活动用户的名称，然后在列表中显示该用户时单击该用户。
   * 在 **指定任务** 字段并开始键入要分配给任务的活动用户、工作角色或团队的名称，然后在列表中显示该名称时单击该名称。

     >[!TIP]
     >
     >添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分具有相同名称的用户。 用户必须与至少一个工作角色关联，才能在添加时查看工作角色。
     >
     >您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅 [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >
     ><span class="preview">添加工作角色分配时，您可以搜索工作角色或位置。 选择“系统/默认工作角色”以使用分配的默认开单费率，或者选择“费率卡工作角色”以使用费率卡中的开单费率。 有关费率卡的详细信息，请参阅 [管理费率卡](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


1. （视情况而定）当在 **指定任务** 字段中，单击 **人员** 图标，打开 **高级工作** 框并创建高级分配。

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   有关更多信息，请参阅 [创建高级工作](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >您不能从“分配至”或“已分配”字段进行高级分配。

1. 将任务负责人添加到任务后，按Enter键或单击页面上的任意位置保存更改（如果已选择“自动保存”）。 否则，请单击 **保存**.

## 将多个任务分配给用户

1. 转到要批量分配的任务的列表。
1. （视情况而定）确保 **自动保存** 如果您在项目下的任务列表中，则该选项为选中状态。

   >[!IMPORTANT]
   >
   >在项目中手动保存任务时，无法批量编辑任务。

1. 在任务列表中选择多个任务。
1. 单击 **编辑**.

   此 **编辑任务** 对话框打开。

1. 在 **指定任务** 区域，选择 **被分派人** 框中，然后开始键入要分配给所有任务的用户、工作角色或团队的名称。

   >[!IMPORTANT]
   >
   >如果已经分配了任何任务，您在此处指定的资源将添加到任务中，而不是替换任务上的现有资源。

1. （可选）选择 **任务所有者** 列，指明在将多个资源分配给任务时，哪个资源是任务的主要被分配人或所有者。 这不适用于团队。
1. （视情况而定）指定 **分配%** 对于分配给任务的每个资源（如果您选择的所有任务的工期类型均为“投入比导向”或“计算的工作分配”）。 这指示这些资源应在完成任务上花费多少时间。 这仅适用于用户和职位角色。

   或

   指定金额 **小时** 对于分配给任务的每个资源，如果您选择的所有任务的持续时间类型为“简单”。 所有资源的所有小时总数应等于任务的计划小时数。

   >[!IMPORTANT]
   >
   >如果所选任务具有不同的持续时间类型或所选任务具有不同的持续时间类型，则无法指定每个资源的分配百分比或小时数。

   有关任务的持续时间类型的信息，请参阅 [任务工期和工期类型概览](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. （可选）从中选择用户应在任务中履行的角色 **选择角色** 中的下拉菜单 **被分派人的角色** 列。 如果不选择角色，Workfront会自动选择用户的主要角色。

1. （可选）如果要从所有任务中删除现有被分配人，请执行下列操作之一：

   1. 开始键入要从任务中删除的用户、角色或团队的名称，然后当该名称出现在列表上时将其选中并单击 **移除被分派人** 以移除更多被分配人。
   1. 单击 **移除所有现有被分配人** 以从所有选定任务中移除所有被分配人。

1. 单击 **保存更改**.
1. （可选，视情况而定）当任务列表中显示“分配给”或“工作总揽”字段时，在任务的以下列之一中单击，然后单击 **X图标** ，以将其从任务中删除。

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


