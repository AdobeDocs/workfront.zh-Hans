---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作负载平衡器中筛选信息
description: 为了高效查找工作项并重点关注您管理的用户或项目，我们强烈建议您在工作负载平衡器中使用过滤器。
author: Alina
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
source-git-commit: 10b905c8a66f2507cbfac7c15a01f38d40ab3e00
workflow-type: tm+mt
source-wordcount: '2466'
ht-degree: 0%

---

# 在工作负载平衡器中筛选信息

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

作为资源管理器，您可以使用负载平衡器来查看和管理用户的工作负载。 有关工作负载平衡器的更多常规信息，请参阅以下文章：

* [工作负载平衡器概述](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
* [导航工作负载平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>为了高效查找工作项并重点关注您管理的用户或项目，我们强烈建议您在工作负载平衡器中使用过滤器。 这样，在开始管理资源的分配之前，您便可以显示正确的信息。
>
>当您保存并应用新过滤器，然后从工作负载平衡器中导航离开时，即使在注销并重新登录之后，该过滤器仍会保留。


本文包含有关负载平衡器中过滤器的信息。 有关Workfront中过滤器的信息，请参阅 [过滤器Adobe Workfront概述](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

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
   <td> <p>任意计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>在为团队或在“资源”区域使用工作负载平衡器时进行计划 </p>
   <p>使用项目的负载平衡器时工作 </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>查看或更高权限访问以下内容：</p> 
    <ul> 
     <li> <p>资源管理</p> </li> 
     <li> <p>项目</p> </li> 
     <li> <p>任务</p> </li> 
     <li> <p>问题</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>过滤器、视图和分组</p> </li> 
    </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>在生成或编辑过滤器时，编辑对过滤器、视图和分组的访问权限</span> </p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目、任务、问题的权限或更高权限</p>
   <p>管理要编辑或删除的过滤器的权限</p>
     </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 工作负载平衡器中的过滤器概述

在工作负载平衡器中使用过滤器时，请考虑以下事项：

* 根据您从何处访问工作负载平衡器，Workfront可能已经在为您过滤信息。 有关预应用过滤器的信息，请参阅部分 [工作负载平衡器中预应用的过滤器](#pre-applied-filters-in-the-workload-balancer) 在本文中。
* 您可以创建并应用过滤器，而无需保存它，也可以保存过滤器以备以后重复使用。
* 在不保存的情况下应用过滤器时，可以通过刷新页面还原到原始列表。
* 您可以查看您创建的过滤器，或其他用户创建并与您共享的过滤器。
* 在删除或编辑共享过滤器时，该过滤器也会被删除或编辑，以供与之共享该过滤器的所有人使用。
* 在某个区域的负载平衡器中创建过滤器时，这些过滤器在其他区域中不可用。

   例如，在“资源配置”区域中创建的过滤器在项目或团队的负载平衡器中不可用。

   有关在何处查找工作负载平衡器的信息，请参阅 [找到工作负载平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* 您只能查看与所选过滤器匹配的项目，这些过滤器也与工作负载平衡器屏幕上显示的时间轴内的日期匹配。

## 工作负载平衡器中预应用的过滤器 {#pre-applied-filters-in-the-workload-balancer}

工作负载平衡器在两个不同的区域中显示信息：

* **未分配的工作区**:尚未分配给用户的工作项。
* **分配的工作区**:分配给用户的工作项。

   有关每个区域中显示内容的信息，请参阅 [导航工作负载平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

>[!IMPORTANT]
>
>负载平衡器的每个区域都有其自己的一组过滤器，它们彼此独立工作。 您必须配置两个过滤器，以指示您希望在每个区域中看到哪些信息。

工作负载平衡器显示用户及其工作项。
仅当分配给用户的工作项目的日期与屏幕上显示的时间范围匹配时，才会显示分配给用户的工作项目。

根据您从何处访问工作负载平衡器，“未分配”和“已分配”区域已按特定条件进行过滤，如下表所述：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Workfront区域，用于访问工作负载平衡器</strong></td> 
   <td><b>默认情况下显示在“未分配工作”区域中的项目</b> </td> 
   <td><b>默认情况下，在“已分配的工作”区域中显示的项目</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">资源区</td> 
   <td>默认情况下，此处不显示任何项目。 您必须自定义过滤器才能查看此区域中的工作项目。</td> 
   <td>属于您任何团队的成员的用户及其工作项目。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">团队</td> 
   <td>分配给团队或团队的工作项目以及工作角色。 </td> 
   <td> <p>属于选定团队成员的用户及其工作项目。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目</td> 
   <td> <p>此区域中将显示未分配的工作项或分配给选定项目中的团队或职务角色的项目。</p> </td> 
   <td> <p>在系统默认筛选器时，分配给选定项目上至少一个工作项的用户及其项目上的工作项 <b>此项目的工作项目</b> 中。 </p>

<p>系统默认筛选器时 <b>此项目的工作项目</b> ，则项目的“已分配的工作”区域会显示分配给选定项目上至少一个项目的用户的所有工作项。  </p> 默认情况下，此过滤器处于取消选中状态。

<b>注释</b>
<p>您可以在项目的工作负载平衡器中启用显示所有用户选项，以显示系统中的所有用户。 有关更多信息，请参阅 <a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">导航工作负载平衡器</a></p>

</td> 
  </tr> 
 </tbody> 
</table>

## 创建工作负载平衡器过滤器

无论您从何处访问工作负载平衡器，为工作负载平衡器中的“未分配的工作”和“已分配的工作”区域创建过滤器的过程都是相同的。 有关查找工作负载平衡器的信息，请参阅 [找到工作负载平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

您可以从头开始创建过滤器，或编辑其中一个预定义过滤器。 有关可编辑的现有过滤器的信息，请参阅 [在工作负载平衡器中编辑现有过滤器](#edit-an-existing-filter-in-the-workload-balancer) 章节。

1. 转到工作负载平衡器。

   有关访问工作负载平衡器的信息，请参阅 [导航工作负载平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. 单击 **过滤器** 图标 ![](assets/filter-icon.png) 的右上角 **未分配的工作** 或 **分配的工作** 区域。

   过滤器生成器框显示在右侧。 为其创建过滤器的区域的名称将显示在框标题中。

   ![](assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png)

1. （可选和视情况而定）如果您在“资源配置”区域访问“工作负载平衡器”，则预定义的默认过滤器可能已应用于“已分配的工作”区域。 您可以编辑并保存默认过滤器的副本。

   >[!TIP]
   >
   >默认过滤器显示属于您的任何团队的用户及其工作项目。 您可以编辑此过滤器的副本。

   如果您访问 [!UICONTROL 工作负载平衡器] 在项目中，[!UICONTROL 此项目的工作项目]“筛选器”。 这仅显示分配给此项目中用户的工作项。 您可以复制并保存此过滤器的副本。

   默认情况下， [!UICONTROL 工作负载平衡器] 显示分配给项目上所有用户的所有工作项。


1. 单击 **新建过滤器。**

   ![](assets/new-filters-empty-panel-workload-balancer-350x460.png)

1. 要创建过滤器，请执行以下操作：

   1. 在第一个下拉菜单中选择字段名称，或单击 **浏览字段** 开始键入默认不显示的字段名称。

      >[!IMPORTANT]
      >
      >引用自定义字段时，必须键入字段名称，而不是字段标签。 字段标签显示在附加到对象的自定义表单上。 有关标签和自定义字段名称之间差异的信息，请参阅 [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. （视情况而定）如果您单击 **浏览字段**，在 **搜索** 字段，并在其显示在列表中时将其选中。

      ![](assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png)

      >[!TIP]
      >
      >您可以从以下部分选择字段：
      >
      >* **最近选择**:您最近过滤的字段。
      >* **建议的字段**:最常用的字段。



   1. 从第二个下拉菜单中选择一个修饰符。 有关Workfront过滤器修饰符的信息，请参阅 [过滤器和条件修饰符](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).
   1. 为要筛选的字段选择或键入一个值。

      >[!NOTE]
      >
      > 当您想要显示特定组合中的工作对象时，可以应用以下过滤器：&quot;Portfolio名称包含营销。&quot; 这会显示属于名称中包含“营销”的任何组合的工作项。
      >
      >![](assets/portfolio-name-filter-statement-wb-350x262.png)

   1. （可选）单击 **删除** 图标 ![](assets/delete.png) ，以删除筛选条件。

1. （可选）单击 **添加过滤器** 要添加其他筛选条件，请重复步骤4中的操作。

   <!--(NOTE: ensure this stays correct)-->

1. 单击 **应用** 将筛选器的结果应用到所选的负载平衡器区域而不保存它。

   左侧的工作项列表会更新。

   >[!IMPORTANT]
   >
   >当您添加的所有筛选器语句同时为true时，结果将显示在工作负载平衡器中。

   过滤器会一直保留，直到您刷新页面为止。

   的 **应用** 按钮替换为 **另存为新** 按钮。

1. 单击 **另存为新** 以保存过滤器以供将来使用。

   ![](assets/new-filters-save-as-box-unassigned-area-wb-350x467.png)

   >[!TIP]
   >
   >单击 **取消** 随时将您带回过滤器构建区域。

1. 选择 **无标题过滤器** 并输入新过滤器的名称。
1. 从 **图标** 下拉菜单。

   ![](assets/new-filters-select-icon-expanded-drop-down-wb.png)

1. （可选）为过滤器添加描述，以指示其唯一性。 描述显示在过滤器列表的过滤器名称下。
1. 单击&#x200B;**保存**。

   保存的过滤器显示在过滤器框的“我的过滤器”区域中。

   有关应用保存的过滤器的信息，请参阅部分 [删除工作负载平衡器中保存的过滤器](#delete-a-saved-filter-in-the-workload-balancer) 在本文中。

1. （视情况而定）将鼠标悬停在 **“过滤器”图标** ![](assets/filter-icon.png) 的右上角 **未分配的工作** 或 **分配的工作** 显示工具提示的区域，其中包含当前应用的过滤器名称或数量。

   ![](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## 复制过滤器

您可以复制和编辑过滤器以创建新过滤器。

1. 转到工作负载平衡器。

   有关访问工作负载平衡器的信息，请参阅 [导航工作负载平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. 单击 **过滤器** 图标 ![](assets/filter-icon.png) 的右上角 **未分配的工作** 或 **分配的工作** 区域。

   过滤器生成器框显示在右侧。 为其创建过滤器的区域的名称将显示在框标题中。

1. 将鼠标悬停在现有过滤器上，单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **复制**.

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > 在编辑过滤器时，您可以单击 **更多** 菜单，然后单击 **复制**.

1. 编辑复制过滤器的以下信息：

   * 名称

      默认情况下，新过滤器名称为“（原始过滤器名称）复制”。

   * 图标
   * 描述
   * 任何字段、修饰符或值。

1. （可选）单击 **添加过滤器** 向复制的过滤器中添加更多语句。
1. 单击 **保存** 以在 **我的过滤器** 的上界。

   原始过滤器保持不变，复制的过滤器将另存为新过滤器。

## 在工作负载平衡器中编辑现有过滤器 {#edit-an-existing-filter-in-the-workload-balancer}

您可以编辑工作负载平衡器中保存的过滤器。

>[!TIP]
>
>在您编辑与他人共享的过滤器时，他们还会看到您所做的更改。

1. 转到工作负载平衡器。

   有关访问工作负载平衡器的信息，请参阅 [导航工作负载平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. 单击 **“过滤器”图标** ![](assets/filter-icon.png) 的右上角 **未分配** 或 **分配的工作** 区域。\
   过滤器生成器显示在右侧。

1. 将鼠标悬停在要编辑的过滤器上，然后单击 **编辑** ![](assets/wb-edit-filter-icon.png).

   ![](assets/filter-more-menu-options-wb.png)

1. 执行下列操作之一：

   * 修改任何filter语句
   * 单击 **添加过滤器** 添加新筛选器语句
   * 单击 **删除** 图标 ![](assets/delete.png) 删除现有filter语句。

1. （可选）单击 **应用**.

   结果将在左侧的负载平衡器中更新，以说明您对过滤器所做的更改。

1. 单击 **保存。**

   结果将在左侧的工作负载平衡器中更新，并且过滤器将更新为您选择的新信息。

## 删除工作负载平衡器中保存的过滤器 {#delete-a-saved-filter-in-the-workload-balancer}

在删除过滤器之前，请考虑以下事项：

* 无法恢复已删除的过滤器。
* 您无法删除预定义过滤器。
* 无法删除未保存的过滤器。 在注销并重新登录到Workfront后，系统会自动删除这些配置文件。
* 删除共享过滤器时，也会为与其共享的所有用户删除该过滤器。
* 删除所有保存的过滤器后，将根据原始默认值显示工作负载平衡器。

>[!NOTE]
>
>删除与他人共享的过滤器时，也会为其删除该过滤器。

1. 转到工作负载平衡器
1. 单击 **“过滤器”图标** ![](assets/filter-icon.png) 的右上角 **未分配的工作** 或 **分配的工作** 区域。\
   过滤器生成器框显示在右侧。

1. 将鼠标悬停在过滤器上，然后单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **删除**.
   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   >在编辑过滤器时，您可以单击 **更多** 菜单，然后单击 **删除**.

1. （可选）单击 **取消** 以避免删除并返回过滤器列表。
1. 单击 **删除** 以确认删除。

   此过滤器将为您和所有拥有该过滤器权限的用户而删除。

## 在负载平衡器中共享过滤器

您可以共享您创建的过滤器，或其他用户与您共享的过滤器。

在工作负载平衡器中共享过滤器时，请考虑以下事项：

* 您可以与活动用户、团队、角色和公司共享过滤器，也可以让过滤器对Workfront实例中的每个人都可见。
* 在项目或团队的负载平衡器中，不显示在“资源”区域中共享的过滤器。
* 您与其他人共享的负载平衡器过滤器在Workfront的其他区域中不可见。

要共享过滤器，请执行以下操作：

1. 转到工作负载平衡器
1. 单击 **“过滤器”图标** ![](assets/filter-icon.png) 的右上角 **未分配的工作** 或 **分配的工作** 区域。\
   过滤器生成器框显示在右侧。

1. 将鼠标悬停在过滤器上，然后单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **共享。**

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > 在编辑过滤器时，您可以单击 **更多** 菜单，然后单击 **共享**.

   此时会显示过滤器共享框。

1. 启用 **查看系统范围** 设置。 这会为Workfront中的任何人授予查看过滤器的权限。

   或

   开始在中键入要与其共享过滤器的用户、团队、角色、组或公司的名称 **授予** 字段。

   ![](assets/new-filters-sharing-ui-wb-350x422.png)

1. （可选）单击实体名称旁边的向右箭头以编辑其对过滤器的权限，然后启用 **查看** 或 **管理** 选项。

   ![](assets/new-filters-granular-permissions-for-manage-wb-350x107.png)

1. （可选）通过执行以下操作之一，启用或禁用实体的附加权限：

   1. 单击 **查看** 并禁用 **共享** 选项。 默认情况下处于启用状态。

   1. 单击 **管理** 和禁用 **共享** 或 **删除** 选项。 默认情况下，会启用这些设置。
   >[!TIP]
   >
   >用户无法获得比其访问级别更高的权限。 如果他们在访问级别无权访问“编辑”过滤器，则无法接收管理过滤器的权限。 Workfront会为这些用户禁用“管理”选项，并且该选项会变暗。

1. 单击 **共享**. 过滤器将与您指定的实体共享。

   您共享的过滤器显示在 **与我共享** 框的下方。

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
