---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 使用工作负载均衡器批量分配工作
description: 您可以使用Adobe Workfront工作负载均衡器批量将资源分配给多个任务和问题。
author: Lisa
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 1%

---

# 使用工作负载均衡器批量分配工作

<!--Audited: 07/2024-->

您可以使用Adobe Workfront工作负载均衡器批量将资源分配给多个任务和问题。

有关使用工作负载均衡器将工作分配给用户的一般信息，请参阅[在工作负载均衡器中分配工作的概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划，在资源区域使用工作负载均衡器时；</br>
       工作，使用团队或项目的工作负载均衡器时</p></td>
  </tr>
  <tr> 
   <td role="rowheader">访问级别配置</td> 
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
   <td role="rowheader">对象权限</td> 
   <td>Contribute对项目、任务和问题（包括制定工作）的权限或更高</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在工作负载均衡器中进行批量分配的注意事项

* 您可以快速管理一个或多个项目中多个任务和问题的用户分配。 分配中的更改会立即在工作负载均衡器中可见。
* 您不能将资源分配给已完成的工作项或已完成项目上的项。
* 在批量分配用户时，可以执行以下操作：

   * 将用户分配给当前分配给工作角色的所有工作项。
   * 替换用户之间的用户分配。
   * 从用户的所有工作项中取消分配用户。

**示例**

* 您负责为多个新项目分配用户。 项目最初从模板创建，并且工作角色已分配给项目中的各种任务。 您需要将特定用户Jackie Simms分配给当前分配给工作角色的所有任务。 您可以使用“分配”功能将这些任务分配给Jackie Simms。
* 3个不同项目中的45个任务被分配给Jackie Simms。 Jackie离开了组织，现在您需要将其任务重新分配给另一个用户。 您可以使用“替换”功能将这些任务分配给新人员。
* 2个不同项目中的10个任务被分配给另一个用户Rick Kuvec。 您意识到我们错误地将Rick分派到了这些任务中，但是您不确定此时需要将其分派给谁。 您需要同时取消将Rick分配到所有任务。 您可以使用“取消分配”功能将Rick从这些任务中删除。

## 在工作负载均衡器中批量分配工作

1. 转到要分配工作的工作负载均衡器。

   您可以在项目或团队级别使用“资源”区域的工作负载均衡器将工作分配给用户。 有关工作负载均衡器在Workfront中的位置的更多信息，请参阅[找到工作负载均衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)。


1. 单击工作负载均衡器顶部的&#x200B;**批量分配** ![](assets/bulk-assignments-wb.png)。

   批量任务面板将在工作负载均衡器的右侧打开。

1. （视情况而定）如果您正在从资源区域或团队访问工作负载均衡器，请展开&#x200B;**项目：名称**&#x200B;下拉菜单，并使用筛选器修饰符选择要为其分配的一个或多个项目。 您可以按名称（这是默认选项）或状态选择项目。

   有关Workfront筛选器修饰符的信息，请参阅[筛选器和条件修饰符](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   >[!NOTE]
   >
   >在访问项目的工作负载均衡器时，默认情况下会选择项目名称。

   ![](assets/project-name-status-dropdown-bulk-assignments-wb-nwe-350x133.png)

1. （可选）单击&#x200B;**选择项目任务**&#x200B;以选择要为其分配的一个或多个任务，然后在&#x200B;**任务：名称**&#x200B;下拉菜单中，按“名称”（这是默认选项）或“状态”选择任务，并使用筛选器修饰符搜索特定任务。

   有关Workfront筛选器修饰符的信息，请参阅[筛选器和条件修饰符](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   >[!NOTE]
   >
   >您不能选择处于完成状态的任务。

   ![](assets/task-name-status-dropdown-bulk-assignments-wb-nwe-350x102.png)

   >[!TIP]
   >
   >如果要批量分配问题和任务，请将此选择留空。

1. （可选）单击其中一个选定条件旁边的&#x200B;**删除**&#x200B;图标![](assets/delete.png)

   或

   单击“批量任务”面板右上角的&#x200B;**全部清除**&#x200B;可删除所有选择。

1. 选择以下选项之一，然后继续执行以下所述的步骤：

   * [分配用户](#assign-user)
   * [替换用户](#replace-user)
   * [取消分配用户](#unassign-user)

   >[!TIP]
   >
   >如果没有与选定过滤器匹配的项目，则这些选项将灰显。

### 分配用户 {#assign-user}

在工作负载均衡器中使用批量分配分配来分配用户时，出现以下情况：

* 用户被分配到选定项目中当前分配给指定角色的所有工作项。
* 用户未分配到以下类型的工作项：

   * 已分配给用户的项目。
   * 已完成项目。

* 如果您选择的用户未与指定的角色关联，则该角色将由用户的主要角色中的用户替换。

要将用户分配给先前分配给工作角色的工作项，请执行以下操作：

1. 开始使用工作负载均衡器中的批量分配来分配工作项（如上所述），然后选择&#x200B;**分配**。

1. 在&#x200B;**角色分配**&#x200B;字段中，单击下拉箭头从角色列表中进行选择。 仅显示指定项目中当前分配的角色。 这是必填字段。

   ![](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. 在&#x200B;**要分配的用户**&#x200B;字段中，单击下拉箭头从建议的用户列表中进行选择或键入其他用户的名称。

   从以下区域选择用户：

   * **建议分配**：满足所选角色且符合智能分配条件的用户。 有关详细信息，请参阅[智能分配概述](../../manage-work/tasks/assign-tasks/smart-assignments.md)。
   * **其他分配**：系统中可以履行所选角色的所有用户。

     >[!TIP]
     >
     >只有前50个用户列在“其他任务”区域。


   选择用户后，Workfront会显示有关为您指定的用户分配的项目数以及这些用户将替换的工作角色的注释。

   >[!TIP]
   >
   >用户的所有角色都显示在列表中，位于用户名的下方。


1. 单击&#x200B;**分配**。

   指定的角色将替换为您选择的用户。

   您将收到确认，确认有多少工作项已将所选角色替换为所选用户。

   ![](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

### 替换用户 {#replace-user}

您可以使用选定项目中的其他用户替换已分配给工作项的用户。

在工作负载均衡器中使用批量分配将用户替换为另一个用户时，出现以下情况：

* 替代用户被分配到当前分配给选定项目内原始用户的所有工作项。

* 新用户未分配到任何已标记为“完成”的工作项。
* 如果与第一个用户关联的角色与第二个用户的任何角色都不匹配，则第二个用户将分配到其“主要角色”。

要用其他用户替换用户，请执行以下操作：

1. 开始在工作负载均衡器中分配工作项（如上所述），然后选择&#x200B;**替换**。
1. 在&#x200B;**当前分配的用户**&#x200B;字段中，单击下拉箭头从用户列表中进行选择。 仅显示指定项目中当前分配给未完成工作项的用户。 这是必填字段。

   ![](assets/bulk-assignments-workload-balancer-replace-selected-350x345.png)

1. 在&#x200B;**要分配的用户**&#x200B;字段中，单击下拉箭头从建议的用户列表中进行选择或键入其他用户名。 默认情况下，列表中列出的用户与“智能分配”的条件相匹配。 有关详细信息，请参阅[智能分配概述](../../manage-work/tasks/assign-tasks/smart-assignments.md)。

   Workfront会显示一个注释，说明当前分配的用户将替换第二个用户的项目数以及这些用户将替换哪些角色。

   ![](assets/bulk-replace-user-confirmation-before-replacing-nwe-350x49.png)

1. 单击&#x200B;**替换**。

   所选项目的全部工作项中的第一个用户被第二个用户替换。

   您将收到一个确认函，确认有多少工作项将原始用户分配替换为所选的第二个用户。

### 取消分配用户 {#unassign-user}

您可以在选定项目中为用户分配的所有工作项中取消分配用户。

在使用工作负载均衡器中的批量分配从用户的所有分配中取消分配用户时，出现以下情况：

* 指定的用户将从其分配到的所有工作项中删除。
* 如果未分配的用户与工作角色相关联，则移除用户后，工作角色仍会分配给工作项。

* 如果将指定的用户分配给已完成的工作项，则该用户仍会分配给这些工作项。

有关用户和工作角色分配的更多信息，请参阅在工作负载均衡器](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)中分配工作的概述[。

要从选定项目中的工作项取消分配用户，或为其分配的选定任务或问题取消分配用户，请执行以下操作：

1. 开始在工作负载均衡器中分配工作项（如上所述），然后选择&#x200B;**取消分配**。

1. 在&#x200B;**要取消分配的用户**&#x200B;字段中，单击下拉箭头从用户列表中进行选择。 只有当前分配给指定项目中未完成工作项的用户才会显示。 这是必填字段。

   ![](assets/bulk-assignments-workload-balancer-unassign-selected-350x318.png)

   Workfront显示有关当前已分配用户将被取消分配的项目数的注释。

   ![](assets/bulk-unassign-user-confirmation-before-assigning-nwe-350x45.png)

1. 单击&#x200B;**取消分配**。\
   您会收到有关已删除指定用户的工作项数的确认。


