---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 修改任务列表中的多个用户分配
description: 在管理任务分配时，可以使用任务列表中的批量编辑功能一次为多个任务同时修改它们。
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 3%

---

# 修改任务列表中的多个用户分配

<!--Audited: 11/2025-->

<!--remove the old/new experience references when the toggles are removed-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).  

</div>-->

在管理任务分配时，可以使用任务列表中的批量编辑功能一次为多个任务同时修改它们。

本文参考为任务列表中的多个任务修改多个用户分配。 另请参阅以下文章，了解如何修改其他区域中多个任务的分配：

* 有关使用工作负载均衡器分配任务的信息，请参阅[在工作负载均衡器中分配工作的概述](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)。

有关将任务分配给列表中一个资源的信息，请参阅[分配任务](../../../manage-work/tasks/assign-tasks/assign-tasks.md)。

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
   <td>向任务分配或更高权限</td>
  </tr>
 </tbody>
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

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
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
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
1. （可选）创建一个过滤器，以便仅显示分配给要修改的被分配人的任务。

   例如，如果项目包含特定角色作为多个任务的默认任务接受者，则可以创建一个过滤器，以仅显示以该角色作为任务接受者的任务。 然后，您可以使用特定用户替换角色。

   有关创建筛选器的信息，请参阅[创建或编辑筛选器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)。


1. 要筛选角色，请选择&#x200B;**分配角色**，然后单击&#x200B;**ID**。

   >[!TIP]
   >
   >不要使用&#x200B;**分配给**&#x200B;字段。 这仅查找任务的主要所有者，而不是可分配给他们的任何角色。

   或

   要筛选用户，请选择&#x200B;**任务用户，**，然后单击&#x200B;**ID。**

   >[!TIP]
   >
   >不要使用&#x200B;**分配给**&#x200B;字段。 此操作仅查找任务的主要所有者，而不是查找可分配给任务的任何用户。

1. 选择要修改分配的任务，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。

   1. 要添加或移除被分配人，请执行下列操作之一：

      * 要添加被分配人，请在&#x200B;**搜索人员、角色或团队**&#x200B;字段中开始键入被分配人的姓名，然后当他们显示在列表中时选择他们。

        新被分配人会添加到选定任务上的现有被分配人。
      * 要删除被分配人，请在&#x200B;**删除被分配人**&#x200B;框中单击被分配人的姓名

        或

        单击&#x200B;**删除所有现有被分配人**。

        将从所有选定任务中删除被分配人。

        从任务中移除用户可能会影响任务小时数和分配百分比。

        有关详细信息，请参阅[修改任务分配的概述](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)。


        >[!TIP]
        >
        >* 您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
        >   
        >* 添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分具有相同名称的用户。 用户必须与至少一个工作角色关联，才能在添加时查看工作角色。 您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅[授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。
        > 
        >   如果在停用用户、工作角色或团队之前已分配用户、工作角色或团队，则它们仍会分配给工作项。 在这种情况下，我们建议执行以下操作：
        >   
        >* 将工作项重新分配给活动资源。
        >* 将已停用团队中的用户与活动团队关联，并将工作项重新分配给活动团队。


   1. （可选）修改受让人的以下任意选项：

      * （视情况而定） **分配%或小时数**：指定新的分配百分比或小时数。

      >[!NOTE]
      >
      >仅当所有正在编辑的任务的“持续时间类型”相同时，才能修改此选项。 当持续时间类型为已计算的工作或投入比驱动时，您可以更新分配%。 当持续时间类型为简单时，您可以更新小时数。 有关持续时间类型的信息，请参阅[任务持续时间和持续时间类型概览](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。
      >
      >
      >如果字段为空，则意味着值在各任务中是不同的；但是，您仍然能够修改它。

      * **设为主要**：将鼠标悬停在所选任务上并选择此选项，以使被分派人成为正在编辑的所有任务的所有者。
      * **被分派人的角色**：从下拉列表中选择一个角色。 如果保持未选中状态，Adobe Workfront将自动选择用户的主要角色。
      * **持续时间类型**
      * **持续时间**
      * **计划小时数**

   1. 单击&#x200B;**保存**。

<!-- temporary content - for Assignments redesign:

Editing assignments on tasks differs depending on which environment you choose. 

1. (Conditional) If you are using the Production environment to assign tasks, the **Edit Tasks** box opens in the new experience. Do the following in the Production environment: 

   1. To add or remove assignees, do one of the following:

      * To add assignees, start typing the name of an assignee in the **Search people, roles, or teams** field, then select them when they display in the list. 
      * To remove assignees, click the **x** icon to the right of their name. Only assignees that are common to all tasks display in the list. 
      * Click Assign to me to assign the selected tasks to yourself.

   1. (Conditional) When using the new experience, click **Save**.

   1. (Optional) Click **Switch to old experience** at the bottom of the **Edit Tasks** box.
      
      The **Edit Tasks** box opens in the old experience.

   1. (Conditional) In the old experience, do the following to modify the assignees:

      1. Go to the **Assignments** section.

         >[!IMPORTANT]
         >
         >Removing assignees can affect the task hours and allocation percentages. For more information, see the section [How removing assignees affects task hours and allocation percentages](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in this article.

      1. Do one of the following to add or remove assignees:

         * To add a new assignee:

            1. In the **Assignments** section, select **Assignee**.

               Information that is common across all tasks selected displays. For example, if the same user is assigned to all tasks, that user displays in the **Assignee** column. If information is not common across the tasks selected, no information displays.
            
            1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected tasks.

            >[!TIP]
            >
            > * You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
            >   
            > * When adding a user assignment, notice the avatar, the user's Primary Role, or their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them. You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
            > 
            >   If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
            >   
            >     * Reassign the work item to active resources.
            >     * Associate the users in a deactivated team with an active team and reassign the work item to the active team.


         * To remove individual assignees:

            1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.

               Or

               (Conditional) If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the tasks that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.

         * To remove all existing assignees:

            1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.

               This removes not only common assignees (assignees that are displayed in the edit dialog box), but also all assignees on all the selected tasks.

            Removing users from tasks can affect task hours and allocation percentages.
            
            For more information, see [Overview of modifying task assignments](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

      1. (Optional) Modify any of the following options for assignees:

         * (Conditional) **Allocation % or Hours**: Specify a new allocation percentage or hours.

         >[!NOTE]
         >
         >This option can be modified only if the Duration Type is the same across all tasks that are being edited. When the Duration Type is Calculated Work or Effort Driven you can update the Allocation %. When the Duration Type is Simple you can update the Hours. For information about Duration Type, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
         >
         >
         >If the field is blank, this means that the value is different across tasks; however, you are still able to modify it.

         * **Task Owner**: Select this option to make the assignee the owner of the task for all tasks being edited.
         * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Adobe Workfront automatically selects the Primary Role of the user. 

      1. Click **Save Changes.**
        

1. <span class="preview">(Conditional) If you are using the Preview environment to assign tasks, the **Edit Tasks** box opens. Do the following in the Preview environment: </span>

   <div class="preview">-->





