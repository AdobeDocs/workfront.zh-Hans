---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 工作负载均衡器中的过滤器信息
description: 为了高效地查找工作项并专注于您管理的用户或项，我们强烈建议您在工作负载均衡器中使用过滤器。
author: Alina
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '2460'
ht-degree: 0%

---

# 工作负载均衡器中的过滤器信息

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

作为资源管理器，您可以使用工作负载均衡器查看和管理用户的工作负载。 有关工作负载均衡器的更多常规信息，请参阅以下文章：

* [工作负载均衡器概述](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
* [导航工作负载均衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>为了高效地查找工作项并专注于您管理的用户或项，我们强烈建议您在工作负载均衡器中使用过滤器。 这允许您在开始管理资源分配之前显示正确的信息。
>
>当您保存并应用新过滤器，然后导航离开工作负载均衡器时，即使您注销并重新登录，过滤器也会保留。

本文包含有关工作负载均衡器中的过滤器的信息。 有关Workfront中过滤器的信息，请参阅 [过滤器概述](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>在资源区域使用工作负载均衡器时进行规划</p>
   <p>工作，使用团队或项目的工作负载均衡器时</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>查看以下内容或更高访问权限：</p> 
    <ul> 
     <li> <p>资源管理</p> </li> 
     <li> <p>项目</p> </li> 
     <li> <p>任务</p> </li> 
     <li> <p>问题</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>筛选器、视图和分组</p> </li> 
    </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>在构建或编辑筛选器时编辑对筛选器、视图和分组的访问权限</span> </p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看或更高权限的项目、任务、问题</p>
   <p>管理要编辑或删除的筛选器的权限</p>
     </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 工作负载均衡器中的过滤器概述

在工作负载均衡器中使用过滤器时，请考虑以下事项：

* 根据您从何处访问工作负载均衡器，Workfront可能已经在为您过滤信息。 有关预应用过滤器的信息，请参阅部分 [工作负载均衡器中预应用的过滤器](#pre-applied-filters-in-the-workload-balancer) 本文章中。
* 您可以创建和应用筛选器而不保存它，也可以保存筛选器以供以后重复使用。
* 应用筛选器而不保存它时，可以通过刷新页面还原为原始列表。
* 您可以查看您创建的过滤器，或其他用户创建并与您共享的过滤器。
* 在删除或编辑共享过滤器时，也会删除或编辑与其共享该过滤器的每个人的过滤器。
* 在一个区域的工作负载均衡器中创建过滤器时，它们在其他区域不可用。

  例如，在资源区域中创建的过滤器在项目或团队的工作负载均衡器中不可用。

  有关在何处查找工作负载均衡器的信息，请参见 [找到工作负载均衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* 您只能查看与所选过滤器匹配，且与工作负载均衡器屏幕上显示的时间线内的日期匹配的项目。

## 工作负载均衡器中预应用的过滤器 {#pre-applied-filters-in-the-workload-balancer}

工作负载均衡器在两个单独的区域中显示信息：

* **未分配的工作区域**：尚未分配给用户的工作项。
* **已分配的工作区域**：分配给用户的工作项。

  有关每个区域中所显示内容的信息，请参阅 [导航工作负载均衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

>[!IMPORTANT]
>
>工作负载均衡器的每个区域都有其自己的过滤器集，这些过滤器可以相互独立地工作。 您必须配置这两个过滤器，以指示要在每个区域查看哪些信息。

工作负载均衡器显示用户及其工作项。
分配给用户的工作项仅在项日期与屏幕上显示的时间范围匹配时显示。

根据从何处访问工作负载均衡器，已按照特定条件过滤了未分配和已分配区域，如下表所述：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>您访问工作负载均衡器的Workfront区域</strong></td> 
   <td><b>默认显示在“未分配工作”区域中的项目</b> </td> 
   <td><b>默认显示在已分配工作区域中的项目</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">资源区域</td> 
   <td>默认情况下，此处不显示任何项目。 必须自定义筛选器才能查看此区域中的工作项。</td> 
   <td>您任何团队的成员及其工作项目的用户。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">团队</td> 
   <td>分配给团队或团队的工作项以及工作角色。 </td> 
   <td> <p>属于所选团队及其工作项的用户。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目</td> 
   <td> <p>未分配的工作项或分配给选定项目中的团队或工作角色的项将显示在此区域中。</p> </td> 
   <td> <p>当系统默认筛选条件为选定项目上至少分配了一个工作项的用户，及其该项目上的工作项 <b>该项目的工作项</b> 已选中。 </p>

<p>当系统默认筛选器时 <b>该项目的工作项</b> 如果取消选中，则项目的已分配工作区域显示分配给选定项目中的至少一个项目的用户的所有工作项。  </p> 默认情况下，此筛选器处于取消选中状态。

<b>注意</b>
<p>您可以在项目的工作负载均衡器中启用显示所有用户选项以显示系统中的所有用户。 有关更多信息，请参阅 <a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">导航工作负载均衡器</a></p>

</td> 
  </tr> 
 </tbody> 
</table>

## 创建工作负载均衡器过滤器

无论从何处访问工作负载均衡器，为工作负载均衡器中的未分配工作和分配的工作区域创建过滤器的过程都是相同的。 有关定位工作负载均衡器的信息，请参见 [找到工作负载均衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

您可以从头开始创建过滤器，或编辑某个预定义过滤器。 有关可编辑的现有筛选器的信息，请参阅 [在工作负载均衡器中编辑现有过滤器](#edit-an-existing-filter-in-the-workload-balancer) 部分。

1. 转到工作负载均衡器。

   有关访问工作负载均衡器的信息，请参见 [导航工作负载均衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. 单击 **筛选** 图标 ![](assets/filter-icon.png) 在任一个的右上角 **未分配的工作** 或 **已分派工作** 区域。

   右侧将显示过滤器生成器框。 您为其创建过滤器的区域的名称将显示在框的标题中。

   ![](assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png)

1. （可选且视情况而定）如果您在资源区域访问工作负载均衡器，则预定义的默认过滤器可能已应用于已分配的工作区域。 您可以编辑并保存默认筛选器的副本。

   >[!TIP]
   >
   >默认筛选器显示属于您的任何团队的用户及其工作项。 您可以编辑此筛选器的副本。

   如果您访问 [!UICONTROL 工作负载均衡器] 从项目“[!UICONTROL 该项目的工作项]可能已应用“ ”筛选器。 此项仅显示分配给此项目中的用户的工作项。 您可以复制并保存此筛选器的副本。

   默认情况下， [!UICONTROL 工作负载均衡器] 显示分配给项目中所有用户的所有工作项。


1. 单击 **新筛选器。**

   ![](assets/new-filters-empty-panel-workload-balancer-350x460.png)

1. 要创建过滤器，请执行以下操作：

   1. 在第一个下拉菜单中选择字段名称，或单击 **浏览字段** 开始键入默认不显示的字段的名称。

      >[!IMPORTANT]
      >
      >引用自定义字段时，必须键入字段名称而非字段标签。 字段标签显示在附加到对象的自定义表单上。 有关自定义字段的标签和名称之间差异的信息，请参阅 [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. （视情况而定）如果您单击 **浏览字段**，在中键入字段名称 **Search** 字段，并在该字段显示在列表中时将其选定。

      ![](assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png)

      >[!TIP]
      >
      >您可以从以下部分中选择字段：
      >
      >* **最近选择**：您最近过滤过的字段。
      >* **建议的字段**：最常用的字段。


   1. 从第二个下拉菜单中选择一个修饰符。 有关Workfront过滤器修饰符的信息，请参阅 [过滤器和条件修饰符](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).
   1. 为要过滤的字段选择或键入值。

      >[!NOTE]
      >
      > 如果要显示特定项目组合中的工作对象，可以应用以下过滤器：“Portfolio名称包含营销。” 这会显示属于名称中包含“营销”的任意项目组合的工作项。
      >
      >![](assets/portfolio-name-filter-statement-wb-350x262.png)

   1. （可选）单击 **删除** 图标 ![](assets/delete.png) 以删除筛选条件。

1. （可选）单击 **添加筛选器** 要添加其他筛选条件，请重复步骤4中的操作。

   <!--(NOTE: ensure this stays correct)-->

1. 单击 **应用** 将过滤器的结果应用到所选的工作负载均衡器区域而不保存它。

   左侧的工作项列表将更新。

   >[!IMPORTANT]
   >
   >当添加的所有过滤器语句同时为true时，结果将显示在工作负载均衡器中。

   该过滤器会一直保留，直到您刷新页面为止。

   此 **应用** 按钮已替换为 **另存为新预设** 按钮。

1. 单击 **另存为新预设** 以保存过滤器以供将来使用。

   ![](assets/new-filters-save-as-box-unassigned-area-wb-350x467.png)

   >[!TIP]
   >
   >点击 **取消** 可随时将您带回过滤器构建区域。

1. 选择 **无标题的筛选器** 并输入新筛选器的名称。
1. 从中选择新过滤器的图标 **图标** 下拉菜单。

   ![](assets/new-filters-select-icon-expanded-drop-down-wb.png)

1. （可选）添加过滤器描述以指示其独特之处。 描述显示在筛选器列表中的筛选器名称下。
1. 单击&#x200B;**保存**。

   保存的筛选器显示在筛选器框的“我的筛选器”区域中。

   有关应用已保存过滤器的信息，请参阅部分 [删除工作负载均衡器中保存的过滤器](#delete-a-saved-filter-in-the-workload-balancer) 本文章中。

1. （视情况而定）将鼠标悬停在 **过滤器图标** ![](assets/filter-icon.png) 位于的右上角 **未分配的工作** 或 **已分派工作** 区域以显示包含当前应用的过滤器名称或数量的“工具提示”。

   ![](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## 复制筛选器

您可以复制并编辑过滤器以创建新过滤器。

1. 转到工作负载均衡器。

   有关访问工作负载均衡器的信息，请参见 [导航工作负载均衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. 单击 **筛选** 图标 ![](assets/filter-icon.png) 在任一个的右上角 **未分配的工作** 或 **已分派工作** 区域。

   右侧将显示过滤器生成器框。 您为其创建过滤器的区域的名称将显示在框的标题中。

1. 将鼠标悬停在现有筛选器上，单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **复制**.

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > 编辑过滤器时，您可以单击 **更多** 菜单，然后单击 **复制**.

1. 为复制的过滤器编辑以下信息：

   * 名称

     默认情况下，新筛选器名称为“（原始筛选器名称）副本”。

   * 图标
   * 描述
   * 任何字段、修饰符或值。

1. （可选）单击 **添加筛选器** 以将更多语句添加到重复过滤器。
1. 单击 **保存** 将复制的过滤器保存在 **我的筛选器** 区域。

   原始筛选器保持不变，复制的筛选器另存为新筛选器。

## 在工作负载均衡器中编辑现有过滤器 {#edit-an-existing-filter-in-the-workload-balancer}

您可以在工作负载均衡器中编辑已保存的过滤器。

>[!TIP]
>
>在编辑与他人共享的过滤器时，他们也会看到您所做的更改。

1. 转到工作负载均衡器。

   有关访问工作负载均衡器的信息，请参见 [导航工作负载均衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. 单击 **过滤器图标** ![](assets/filter-icon.png) 位于的右上角 **已取消分配** 或 **已分派工作** 区域。\
   筛选器生成器将显示在右侧。

1. 将鼠标悬停在要编辑的筛选器上，然后单击 **编辑** ![](assets/wb-edit-filter-icon.png).

   ![](assets/filter-more-menu-options-wb.png)

1. 执行下列操作之一：

   * 修改任何filter语句
   * 单击 **添加筛选器** 添加新的筛选语句
   * 单击 **删除** 图标 ![](assets/delete.png) 以删除现有的过滤器语句。

1. （可选）单击 **应用**.

   结果将在左侧的工作负载均衡器中更新，以说明您对过滤器所做的更改。

1. 单击 **保存。**

   结果在左侧的工作负载均衡器中更新，过滤器使用您选择的新信息更新。

## 删除工作负载均衡器中保存的过滤器 {#delete-a-saved-filter-in-the-workload-balancer}

删除过滤器前，请考虑以下事项：

* 无法恢复已删除的筛选器。
* 您无法删除预定义过滤器。
* 您无法删除未保存的筛选器。 注销并重新登录到Workfront后，会自动删除它们。
* 删除共享筛选器时，也会删除与其共享该筛选器的所有用户的该筛选器。
* 删除所有保存的过滤器后，工作负载均衡器会根据原始默认值显示。

>[!NOTE]
>
>当您删除与他人共享的过滤器时，该过滤器也会被其他人删除。

1. 转到工作负载均衡器
1. 单击 **过滤器图标** ![](assets/filter-icon.png) 位于的右上角 **未分配的工作** 或 **已分派工作** 区域。\
   右侧将显示过滤器生成器框。

1. 将鼠标悬停在筛选器上，然后单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **删除**.
   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   >编辑过滤器时，您可以单击 **更多** 菜单，然后单击 **删除**.

1. （可选）单击 **取消** 以避免删除并返回过滤器列表。
1. 单击 **删除** 以确认删除。

   该过滤器将为您以及拥有其权限的所有用户删除。

## 在工作负载均衡器中共享过滤器

您可以共享您创建的过滤器或其他用户与您共享的过滤器。

在工作负载均衡器共享过滤器时，请考虑以下事项：

* 您可以与活动用户、团队、角色和公司共享过滤器，也可以让这些过滤器对Workfront实例中的每个人可见。
* 在资源区域共享的过滤器在项目或团队的工作负载均衡器中不可见。
* 您与他人共享的工作负载均衡器过滤器在Workfront的其他区域中不可见。

要共享过滤器，请执行以下操作：

1. 转到工作负载均衡器
1. 单击 **过滤器图标** ![](assets/filter-icon.png) 位于的右上角 **未分配的工作** 或 **已分派工作** 区域。\
   右侧将显示过滤器生成器框。

1. 将鼠标悬停在筛选器上，然后单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **共享。**

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > 编辑过滤器时，您可以单击 **更多** 菜单，然后单击 **共享**.

   此时将显示筛选器共享框。

1. 启用 **查看系统范围** 设置。 这将授予Workfront中的任何人查看筛选器的权限。

   或

   开始键入要在中与其共享该过滤器的用户、团队、角色、组或公司的名称 **将访问权限授予** 字段。

   ![](assets/new-filters-sharing-ui-wb-350x422.png)

1. （可选）单击实体名称旁边的向右箭头以编辑其对筛选器的权限，然后启用 **视图** 或 **管理** 选项。

   ![](assets/new-filters-granular-permissions-for-manage-wb-350x107.png)

1. （可选）通过执行以下操作之一，启用或禁用实体的其他权限：

   1. 单击 **视图** 并禁用 **共享** 选项。 默认情况下处于启用状态。

   1. 单击 **管理** 并禁用 **共享** 或 **删除** 选项。 默认情况下启用它们。

   >[!TIP]
   >
   >用户获得的权限不能高于其访问级别。 如果他们无权在其访问级别编辑“筛选器”，则他们将无权管理筛选器。 Workfront对这些用户禁用了“管理”选项，并且该选项呈灰显状态。

1. 单击&#x200B;**共享**。该筛选器将与您指定的实体共享。

   您共享的过滤器将显示在 **与我共享** 滤镜框的区域。

   ![](assets/new-filters-shared-with-me-area-wb-350x236.png)

<!--   

## Add a filter to your favorites list

You can mark a filter as a favorite for quicker access to it. 

The filters that you mark as a favorite do not count towards your system Favorites list. There is no limit for how many filters you can favorite. 

1. Go to the Workload Balancer
1. Click the **Filter** icon ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or **Assigned Work** areas. The filter builder box displays on the right. 
1. Mouse over a filter, then click the **Favorite** ![](assets/favorites-icon-small.png). 
(NOTE: insert screen shot here with Favorite as part of this menu - same as above ones but with Favorite)
1. The filter is listed in the **Favorited** section inside the filter panel. 
1. (Optional) Click the **Favorite** icon again to remove the filter from the list of favorite filters
(I logged bugs for "Favorited" and "Unfavorite" wordings - make sure these have not updated)
-->
