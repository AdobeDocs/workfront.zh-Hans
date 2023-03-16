---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 使用工作负载平衡器批量分配工作
description: 您可以使用Adobe Workfront工作负载平衡器手动为用户分配工作项。
author: Alina
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '1543'
ht-degree: 2%

---

# 使用工作负载平衡器批量分配工作

<!--drafted
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 
-->

您可以使用Adobe Workfront工作负载平衡器手动为用户分配工作项。

有关使用工作负载平衡器将工作分配给用户的一般信息，请参阅 [工作负载平衡器中分配工作的概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>在资源区中使用负载平衡器时进行计划</p>
   <p>使用团队或项目的负载平衡器时工作</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对以下项的访问权限：</p> 
    <ul> 
     <li> <p>资源管理</p> </li> 
     <li> <p>项目</p> </li> 
     <li> <p>任务</p> </li> 
     <li> <p>问题</p> </li> 
    </ul> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>对包含“进行分配”的项目、任务和问题具有或更高的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在负载平衡器中进行批量分配的注意事项

* 您可以快速管理一个或多个项目中多个任务和问题的用户分配。 工作负载平衡器中会立即显示分配中的更改。
* 您不能将资源分配给已完成的工作项或已完成项目中的项。
* 批量分配用户时，您可以执行以下操作：

   * 将用户分配给当前分配给作业角色的所有工作项。
   * 替换用户之间的用户分配。
   * 从用户的所有工作项目中取消分配用户。

**示例**

* 您负责对多个新项目进行用户分配。 最初是通过模板创建的项目，并且已将作业角色分配给项目中的各种任务。 您希望将特定用户Jackie Simms分配给当前分配给工作角色的所有任务。 您可以使用“分配”功能将这些任务分配给Jackie Simms。
* Jackie Simms分配了3个不同项目的45项任务。 杰基离开了组织，现在你需要将她的任务重新分配给其他用户。 您可以使用“替换”功能将这些任务分配给新人员。
* 跨2个不同项目的10个任务会分配给另一个用户Rick Kuvec。 您意识到Rick错误地被分配给了这些任务，但您不确定此时需要将这些任务分配给谁。 您需要同时将Rick取消分配给所有任务。 您可以使用“取消分配”函数从这些任务中删除Rick。

## 在工作负载平衡器中批量分配工作

1. 转到要分配工作的工作负载平衡器。

   您可以在“资源”区域、项目或团队级别使用负载平衡器将工作分配给用户。 有关工作负载平衡器在Workfront中的位置的详细信息，请参阅 [找到工作负载平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).


1. 单击 **批量分配** ![](assets/bulk-assignments-wb.png) 工作负载平衡器顶部。

   将在工作负载平衡器右侧打开“批量分配”面板。

1. （视情况而定）如果您从“资源”区域或团队访问工作负载平衡器，请展开 **项目：名称** 下拉菜单，然后使用过滤器修改工具选择要为其分配的项目或项目。 您可以按名称（这是默认选项）或状态选择项目。

有关Workfront过滤器修饰符的信息，请参阅 [过滤器和条件修饰符](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

>[!NOTE]
>
>默认情况下，当您访问项目的工作负载平衡器时，将选择项目名称。

![](assets/project-name-status-dropdown-bulk-assignments-wb-nwe-350x133.png)

1. （可选）单击 **选择项目任务** 选择要为其分配的任务或任务，然后在 **任务：名称** 下拉菜单中，按名称（这是默认选项）或状态选择任务，然后使用过滤器修饰符搜索特定任务。

有关Workfront过滤器修饰符的信息，请参阅 [过滤器和条件修饰符](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

>[!NOTE]
>
>您无法选择处于“完成”状态的任务。

![](assets/task-name-status-dropdown-bulk-assignments-wb-nwe-350x102.png)

>[!TIP]
>
>如果要对问题和任务进行批量分配，请将此选择留空。

1. （可选）单击 **删除** 图标 ![](assets/delete.png) 选定标准旁边的

   或

   单击 **全部清除** “批量分配”(Bulk Assignments)面板右上角的，用于删除所有选择。

1. 选择以下选项之一，然后继续执行下述步骤：

   * [分配用户](#assign-user)
   * [替换用户](#replace-user)
   * [取消分配用户](#unassign-user)

   >[!TIP]
   >
   >如果没有与所选过滤器匹配的项目，则这些选项将变暗。

### 分配用户 {#assign-user}

在工作负载平衡器中使用批量分配来分配用户时，会发生以下情况：

* 将用户分配到选定项目中当前分配给指定角色的所有工作项。
* 未将用户分配到以下类型的工作项：

   * 已分配给用户的项目。
   * 已完成的项目。

* 如果您选择的用户与指定的角色没有关联，则该角色将被用户的主角色中的用户替换。

要将用户分配到以前分配给作业角色的工作项，请执行以下操作：

1. 按照上述说明，在工作负载平衡器中使用批量分配开始分配工作项，然后选择 **分配**.

1. 在 **角色分配** 字段中，单击下拉箭头可从角色列表中进行选择。 只显示当前在指定项目内分配的角色。 这是必填字段。

   ![](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. 在 **要分配的用户** 字段中，单击下拉箭头可从建议用户列表中进行选择，或键入其他用户的名称。

   从以下区域选择用户：

   * **建议的分配**:符合所选角色且符合智能分配标准的用户。 有关更多信息，请参阅 [智能分配概述](../../manage-work/tasks/assign-tasks/smart-assignments.md).
   * **其他分配**:系统中能够完成所选角色的所有用户。

      >[!TIP]
      >
      >“其他分配”区域中仅列出前50个用户。
   选择用户后，Workfront会显示一个注释，说明将分配您指定用户的项目数量以及将替换哪些作业角色。

   >[!TIP]
   >
   >用户的所有角色都会显示在列表中，位于用户名下。


1. 单击 **分配**.

   指定的角色将替换为您选择的用户。

   您将收到有关有多少工作项已将所选角色替换为选定用户的确认信息。

   ![](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

### 替换用户 {#replace-user}

您可以将已分配到工作项的用户替换为选定项目中的其他用户。

在工作负载平衡器中使用批量分配将用户替换为其他用户时，会发生以下情况：

* 替换用户被分配给选定项目中当前分配给原始用户的所有工作项。

* 未将新用户分配到任何已标记为“完成”的工作项。
* 如果与第一用户关联的角色与第二用户的任何角色不匹配，则将为其主角色分配第二用户。

要将用户替换为其他用户，请执行以下操作：

1. 按如上所述，开始在工作负载平衡器中分配工作项，然后选择 **替换**.
1. 在 **当前分配的用户** 字段中，单击下拉箭头可从用户列表中进行选择。 仅显示当前分配给指定项目中未完成工作项的用户。 这是必填字段。

   ![](assets/bulk-assignments-workload-balancer-replace-selected-350x345.png)

1. 在 **要分配的用户** 字段中，单击下拉箭头可从建议用户列表中进行选择，或键入其他用户名。 默认情况下，列表中列出的用户与智能分配的条件相匹配。 有关更多信息，请参阅 [智能分配概述](../../manage-work/tasks/assign-tasks/smart-assignments.md).

   Workfront显示有关当前分配的用户将替换第二个用户的项目数量以及将替换哪些角色的注释。

   ![](assets/bulk-replace-user-confirmation-before-replacing-nwe-350x49.png)

1. 单击 **替换**.

   选定的第一个用户将被选定项目的所有工作项中的第二个用户替换。

   您将收到有关有多少工作项已将原始用户分配替换为选定第二个用户的确认。

### 取消分配用户 {#unassign-user}

您可以从选定项目中分配给用户的所有工作项中取消分配用户。

在工作负载平衡器中使用批量分配从用户的所有分配中取消分配用户时，会发生以下情况：

* 将从分配给指定用户的所有工作项中删除指定用户。
* 如果未分配的用户与作业角色关联，则在删除该用户时，作业角色仍会分配给工作项。

* 如果将指定用户分配到已完成的工作项，则用户仍会被分配到这些工作项。

有关用户和作业角色分配的详细信息，请参阅 [工作负载平衡器中分配工作的概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

要从选定项目中的工作项或为选定任务或分配任务或问题的工作项中取消分配用户：

1. 按如上所述，开始在工作负载平衡器中分配工作项，然后选择 **取消分配**.

1. 在 **要取消分配的用户** 字段中，单击下拉箭头可从用户列表中进行选择。 只有当前分配给指定项目中未完成工作项的用户才会显示。 这是必填字段。

   ![](assets/bulk-assignments-workload-balancer-unassign-selected-350x318.png)

   Workfront显示有关当前分配的用户将被取消分配的项目数的说明。

   ![](assets/bulk-unassign-user-confirmation-before-assigning-nwe-350x45.png)

1. 单击 **取消分配**.\
   您将收到有关删除指定用户的工作项数量的确认。

 
