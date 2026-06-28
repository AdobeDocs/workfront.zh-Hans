---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 使用工作负载均衡器批量分配工作
description: 您可以使用Adobe Workfront工作负载均衡器批量将资源分配给多个任务和问题。
author: Lisa
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
TQID: https://experienceleague.adobe.com/6QlIfRh94tpLTZF6x5LU2BueTjShzNsaKxb45CEylqA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: c33d85a1-be85-4290-854c-87408c10aa80
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 73c78912e15a03bfd09c127e39d94bf5af42b8e2
workflow-type: tm+mt
source-wordcount: 1242
ht-degree: 3%

---

# 使用工作负载均衡器批量分配工作

<!--Audited: 07/2024-->

您可以使用Adobe Workfront工作负载均衡器批量将资源分配给多个任务和问题。

有关使用工作负载均衡器将工作分配给用户的一般信息，请参阅[在工作负载均衡器中分配工作的概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td><p>“任一”</p></td>
  </tr>
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>在资源区域使用工作负载均衡器时进行规划；在使用团队或项目的工作负载均衡器时进行工作</p></td>
  </tr>
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>编辑对以下内容的访问权限：</p> 
    <ul> 
     <li>资源管理</li> 
     <li>项目</li> 
     <li>任务</li> 
     <li>问题</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>包含制定工作分派的项目、任务和问题的Contribute权限或更高版本</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在工作负载均衡器中进行批量分配的注意事项

* 您可以快速管理一个或多个项目中多个任务和问题的资源分配。 分配中的更改会立即在工作负载均衡器中可见。
* 您不能将资源分配给已完成的工作项或已完成项目上的项。
* 在批量分配工作角色和用户时，可以执行以下操作：

   * 替换所有有效组合中用户和角色之间的分配。
   * 从用户的所有工作项中取消分配用户。

**示例**

* 您负责为多个新项目分配用户。 项目最初从模板创建，并且工作角色已分配给项目中的各种任务。 您需要将特定用户Jackie Simms分配给当前分配给工作角色的所有任务。 您可以使用Replace函数将这些任务分配给Jackie Simms。
* 3个不同项目中的45个任务被分配给Jackie Simms。 Jackie离开了组织，现在您需要将其任务重新分配给另一个用户。 您可以使用“替换”功能将这些任务分配给新人员。
* 2个不同项目中的10个任务被分配给另一个用户Rick Kuvec。 您意识到我们错误地将Rick分派到了这些任务中，但是您不确定此时需要将其分派给谁。 您需要同时取消将Rick分配到所有任务。 您可以使用“取消分配”功能将Rick从这些任务中删除。

## 在工作负载均衡器中批量分配工作

1. 转到要分配工作的工作负载均衡器。

   您可以在项目或团队级别使用“资源”区域的工作负载均衡器将工作分配给用户。 有关工作负载均衡器在Workfront中的位置的更多信息，请参阅[找到工作负载均衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)。


1. 单击工作负载均衡器顶部的&#x200B;**批量分配** ![批量分配](assets/bulk-assignments-wb.png)。

   批量任务面板将在工作负载均衡器的右侧打开。

1. （视情况而定）如果您正在从资源区域或团队访问工作负载均衡器，请展开&#x200B;**项目：名称**&#x200B;下拉菜单，并使用筛选器修饰符选择要为其分配的一个或多个项目。 您可以按名称（这是默认选项）或状态选择项目。

   有关Workfront筛选器修饰符的信息，请参阅[筛选器和条件修饰符](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   >[!NOTE]
   >
   >在访问项目的工作负载均衡器时，默认情况下会选择项目名称。

   ![批量分配中的项目名称](assets/project-name-status-dropdown-bulk-assignments-wb.png)

1. （可选）单击&#x200B;**选择项目任务**&#x200B;以选择要为其分配的一个或多个任务，然后在&#x200B;**任务：名称**&#x200B;下拉菜单中，按“名称”（这是默认选项）或“状态”选择任务，并使用筛选器修饰符搜索特定任务。

   有关Workfront筛选器修饰符的信息，请参阅[筛选器和条件修饰符](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   >[!NOTE]
   >
   >您不能选择处于完成状态的任务。

   ![批量分配中的任务状态](assets/task-name-status-dropdown-bulk-assignments-wb.png)

   >[!TIP]
   >
   >如果要批量分配问题和任务，请将此选择留空。

1. （可选）单击其中一个选定条件旁边的&#x200B;**删除**&#x200B;图标![删除图标](assets/delete.png)

   或

   单击“批量任务”面板右上角的&#x200B;**全部清除**&#x200B;可删除所有选择。

1. 选择以下选项之一，然后继续执行以下所述的步骤：

   * [替换资源](#replace-user)
   * [取消分配资源](#unassign-user)

   >[!TIP]
   >
   >如果没有与选定过滤器匹配的项目，则这些选项将灰显。

<!--

### Assign user {#assign-user}

When you assign a user using Bulk Assignments in the Workload Balancer, the following things occur:

* A user is assigned to all work items currently assigned to a specified role within the selected projects.
* The user is not assigned to the following types of work items:

   * Items that are already assigned to a user.
   * Completed items.

* If the user you selected is not associated with the specified role, the role is replaced by the user in the user's Primary Role.

To assign a user to work items previously assigned to job roles:

1. Start assigning work items using Bulk Assignments in the Workload Balancer as described above and select **Assign**. 

1. In the **Role assignment** field, click the drop-down arrow to choose from a list of roles. Only roles currently assigned within the specified projects are displayed. This is a required field. 

   ![Role assignment](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. In the **User to assign** field, click the drop-down arrow to choose from a list of suggested users or to type another user's name.

   Select users from the following areas:

   * **Suggested Assignments**: Users who can fulfill the selected role and who match the criteria for Smart Assignments. For more information, see [Smart assignments overview](../../manage-work/tasks/assign-tasks/smart-assignments.md).
   * **Other Assignments**: All users in the system who can fulfill the selected role. 
   
      >[!TIP]
      >
      >Only the first 50 users are listed in the Other Assignments area.


   After selecting a user, Workfront displays a note about the number of items where the user you specified will be assigned and what job role they will replace.

   >[!TIP]
   >
   >All the roles of the user display in the list, under the user's name.


1. Click **Assign**.

   The specified roles are replaced with the users that you selected.

   You receive a confirmation about how many work items have had the selected role replaced with the selected user.

   ![Bulk assignment confirmation](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

-->

### 替换资源 {#replace-user}

您可以使用选定项目中的其他资源替换已分配给工作项的资源。

资源替换可以是：

* 角色与角色
* 具有用户的用户
* 具有角色的用户
* 具有用户的角色

在工作负载均衡器中使用批量分配将资源替换为其他资源时，出现以下情况：

* 替代资源被分配给选定项目中当前分配给原始资源的所有工作项。
* 新资源未分配给任何已标记为“完成”的工作项。
* 对于用户到用户的替换，如果与第一个用户关联的角色与第二个用户的任何角色都不匹配，则第二个用户将分配到其主要角色。

要将资源替换为其他资源，请执行以下操作：

1. 按如上所述在工作负载均衡器批量分配区域中选择工作项，然后选择&#x200B;**替换资源**。
1. 在&#x200B;**当前分配的资源**&#x200B;字段中，单击下拉箭头从资源列表中进行选择。 仅显示指定项目中当前分配给未完成工作项的资源。 这是必填字段。

   ![替换资源](assets/bulk-assignments-workload-balancer-replace-selected.png)

1. 在要分配的&#x200B;**资源**&#x200B;字段中，单击下拉箭头从建议资源列表中进行选择，或键入其他工作角色或用户名。 默认情况下，第一个列出的资源与智能分配的条件相匹配。 有关详细信息，请参阅[智能分配概述](../../manage-work/tasks/assign-tasks/smart-assignments.md)。

   Workfront显示一个注释，说明当前分配的资源将替换第二个资源的项目数。

1. 单击&#x200B;**替换**。

   选定项目或任务的所有工作项中的第一个资源被第二个资源替换。

   您将收到一个确认函，确认有多少工作项已将原始分配替换为所选的第二个资源。

### 取消分配资源 {#unassign-user}

您可以从选定项目中为其分配资源的所有工作项中取消分配资源。

在使用工作负载均衡器中的批量分配从用户的所有分配中取消分配用户时，出现以下情况：

* 指定的用户将从其分配到的所有工作项中删除。
* 如果未分配的用户与工作角色相关联，则移除用户后，工作角色仍会分配给工作项。

* 如果将指定的用户分配给已完成的工作项，则该用户仍会分配给这些工作项。

有关用户和工作角色分配的更多信息，请参阅在工作负载均衡器[&#128279;](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)中分配工作的概述。

要从选定项目中的工作项取消分配用户，或为其分配的选定任务或问题取消分配用户，请执行以下操作：

1. 按如上所述在工作负载均衡器批量分配区域中选择工作项，然后选择&#x200B;**取消分配资源**。

1. 在&#x200B;**要取消分配的用户**&#x200B;字段中，单击下拉箭头从用户列表中进行选择。 只有当前分配给指定项目中未完成工作项的用户才会显示。 这是必填字段。

   ![取消分配用户](assets/bulk-assignments-workload-balancer-unassign-selected.png)

   Workfront显示有关当前已分配用户将被取消分配的项目数的注释。

1. 单击&#x200B;**取消分配**。\
   您会收到有关已删除指定用户的工作项数的确认。




