---
product-area: projects
navigation-topic: manage-issues
title: 修改列表中多个问题的用户分配
description: 修改列表中多个问题的用户分配
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 0358e79bd606d0035959bba2a47256456b529b18
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 1%

---

# 修改列表中多个问题的用户分配

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

您可以同时将用户分配修改为多个问题。 有关编辑问题或一次分配一个问题的信息，另请参阅以下文章：

* [编辑问题](../../../manage-work/issues/manage-issues/edit-issues.md)
* [分配问题](../../../manage-work/issues/manage-issues/assign-issues.md)

有关分配问题的一般信息，请参阅[修改问题分配的概述](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)。

>[!NOTE]
>
>您必须至少具有问题的Contribute权限，才能为该问题分配工作。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td> <p>标准</p>
   <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>编辑对问题的访问权限</p> <p>查看或更高权限的项目和任务以分配一个问题</p> </td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td> <p>管理问题的权限</p> <p>分配多个问题时，向问题所在的项目或任务分配Contribute权限或更高。</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:  drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of  reasons, including the following:</p>
<ul>
<li>Users join or leave  your team</li>
<li>A user takes a vacation that extends beyond the issue  due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## 修改多个问题的分配

1. 转到问题列表，其中包含要修改其分配的问题。
1. （可选）创建一个过滤器，以仅显示分配给要修改的被分派人的问题。

   例如，您可以创建一个过滤器，以仅显示具有作为被分配人的特定角色的问题。  然后，您可以使用特定用户替换角色。 执行以下操作：

   1. 单击&#x200B;**筛选器**&#x200B;下拉列表，然后单击&#x200B;**新建筛选器**。

   1. 在第一个字段中，开始键入&#x200B;**任务角色**，然后从列表中选择&#x200B;**任务角色：名称**。
   1. 从修饰符下拉菜单中选择&#x200B;**是**&#x200B;的任一项，然后开始键入角色的名称，并在角色显示在列表中时将其选定。 您可以键入多个角色。

      >[!TIP]
      >
      >不要使用&#x200B;**分配给**，因为此字段仅引用问题所有者，而不引用所有被分配人。

      问题列表会自动根据您的筛选条件进行筛选。
   1. （可选）单击&#x200B;**另存为新项**，然后单击&#x200B;**保存**。

1. 选择要修改分配的问题，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/qs-edit-icon.png)。

   此时将显示&#x200B;**编辑问题**。 所选的项目数显示在页面的左上角。

1. 单击左侧面板中的&#x200B;**工作**，然后单击要删除的工作负责人旁边的&#x200B;**x**&#x200B;图标。

   >[!TIP]
   >
   >只有分配到所有选定问题的被分配者才会显示在&#x200B;**工作总揽**&#x200B;区域。

   ![批量编辑问题中的分配区域](assets/assignments-area-on-bulk-edit-issues.png)

1. 开始键入用户、角色或团队的名称，以将受分配人添加到所有已选问题。

   >[!TIP]
   >
   >您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
   >
   >如果在停用用户、工作角色或团队之前已分配用户、工作角色或团队，则它们仍会分配给工作项。 在这种情况下，我们建议执行以下操作：
   >
   >* 将工作项重新分配给活动资源。
   >* 将已停用团队中的用户与活动团队关联，并将工作项重新分配给活动团队。

   添加的被分配人将添加到现有被分配人。 它们不会替换每个选定问题的现有问题。

1. （可选）单击&#x200B;**分配给我**&#x200B;以将所有问题分配给您自己。
1. 单击&#x200B;**保存**。


   <!--Old functionality for assignments for issues - before November 2025:
   1. (Conditional) In the Production environment, do the following: 
   1. Go to the **Assignments** section, then select **Assignee**.
      ![Assignments area](assets/classic-assignmens-area-on-edit-box-350x119.png)
   1. Do one of the following:
      1. To add a new assignee:
         1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected issues.
         >[!TIP]
         >
         >You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
         >
         >If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
         >
         >* Reassign the work item to active resources.
         >* Associate the users in a deactivated team with an active team and reassign the work item to the active team.
          Information that is common across all issues selected displays. For example, if the same user is assigned to all issues, that user displays in the **Assignee**  column. If information is not common across the issues selected, no information displays.
      1. To remove individual assignees:
         1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.
            Or
            If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the issues that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.
         1. Click  **Remove Assignee** again to add another assignee to remove.
      1. To remove all existing assignees:
         1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.
            This removes not only common assignees (assignees that are displayed in the edit  dialog box), but also all assignees on all the selected issues.
         1. (Optional) Modify any of the following options for the assignees you selected to associate with the issues:
          * **Issue Owner:**  Select the radio button to indicate which assignee is designated as the Issues Owner. If left unselected, Adobe Workfront designates the first assignee as the Issue Owner. This is not available for team assignments. 
            * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Workfront automatically selects the Primary Role of the user.
      1. Click **Save Changes**.-->




