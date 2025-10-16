---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 导航工作负载均衡器
description: 使用工作负载均衡器了解资源的可用性并将工作分配给用户。 本文将引导您使用可用于更新工作负载均衡器的视图和导航工作负载均衡器的图标和设置。
author: Lisa
feature: Resource Management
exl-id: 60dabfc5-6a2e-4368-9dac-db48d0307895
source-git-commit: e1580f7b9065fce7bb31ab0c7edb00fd2856e1df
workflow-type: tm+mt
source-wordcount: '4334'
ht-degree: 0%

---

# 导航工作负载均衡器

<!--Audited: 12/2024-->

使用Adobe Workfront中的工作负载均衡器，根据用户的可用性将工作分配给用户。 本文介绍了如何使用设置和选项来导航工作负载均衡器并显示与您相关的信息。 此处列出的其他文章介绍如何使用工作负载均衡器管理您的资源及其工作分配。

工作负载均衡器在Adobe Workfront的多个区域中可用。 在所有区域导航都类似。

有关工作负载均衡器位置的更多信息，请参阅[找到工作负载均衡器](https://experienceleague.adobe.com/zh-hans/docs/workfront/using/manage-resources/the-workload-balancer/locate-workload-balancer)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td>
  </tr>
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>在资源区域使用工作负载均衡器时进行规划；在使用团队或项目的工作负载均衡器时进行工作</p></td>
  </tr>
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>查看以下内容或更高访问权限：</p> 
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
   <td>查看或更高权限的项目、任务和问题</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查看工作负载均衡器中的项目的注意事项

查看工作负载均衡器时，请考虑以下事项：

* 工作负载均衡器根据工作分配在两个单独的区域显示工作项。 工作项和用户显示在以下区域中：

   * **未分配的工作**：没有分配或仅分配给工作角色或团队的项。
   * **已分配的工作**：至少分配给一个用户的项目。 分配的项显示在分配的用户的名称下。

  >[!NOTE]
  >
  >* 分配给工作角色或团队的工作项以及分配给用户的工作项既显示在“未分配的工作”区域中，也显示在“已分配的工作”区域中的已分配用户名下。
  >* 分配给用户的工作项和工作角色（其中工作角色被选为该项的主要被分配人）显示在“未分配的工作”区域中。
  >* 分配给多个用户的工作项显示在“已分配的工作”区域的所有已分配用户名下。
  >* 启用“显示角色分配”设置后，角色分配会显示在“未分配工作”区域的工作项下。 有关信息，请参阅本文中的[自定义视图](#customize-the-view)部分。

  有关详细信息，请参阅[在工作负载均衡器](/help/quicksilver/resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md#assignment-areas-in-the-workload-balancer)中分配工作的概述[工作负载平衡器](/help/quicksilver/resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)中的分配区域。

* 当项目在某个时间段内没有任务时，该项目级别的栏在该时间段为空白。

  ![在某个时间段内没有任务的项目](assets/wb-no-tasks-in-time-period.png)

* 当您没有查看某些项的权限时，它们显示为&#x200B;**无法访问的工作项**&#x200B;或&#x200B;**无法访问的项目**。

  ![不可访问的工作项](assets/wb-inaccessible-work-items.png)

* 工作项的名称显示在左侧，其时间轴显示在右侧。
* 每个工作项的总计划小时数显示在工作项名称的右侧，以及代表工作项时间线的栏的左侧。
* 每个项目的总计划小时数显示在项目名称的右侧，以及表示项目时间线的栏的左侧。

  项目的计划小时数信息是工作负载平衡器中列出的所有项目的计划小时数总计，而不是项目的计划小时数总计。

有关在工作负载均衡器中查看信息的更多信息，另请参阅以下文章：

* [找到工作负载均衡器](../workload-balancer/locate-workload-balancer.md)
* [工作负载均衡器中的过滤器信息](../workload-balancer/filter-information-workload-balancer.md)
* [使用链接共享工作负载均衡器](../workload-balancer/share-link-for-workload-balancer.md)
* [使用摘要更新工作负载均衡器中的工作项](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md)

有关使用工作负载均衡器管理资源的信息，另请参阅以下文章：

* [在工作负载均衡器中分配工作的概述](https://experienceleague.adobe.com/zh-hans/docs/workfront/using/manage-resources/the-workload-balancer/assign-work-in-workload-balancer)
* [在工作负载均衡器中管理用户分配](https://experienceleague.adobe.com/zh-hans/docs/workfront/using/manage-resources/the-workload-balancer/manage-user-allocations-workload-balancer)

## 在资源区域为多个项目导航工作负载均衡器

工作负载均衡器在您从中访问的所有区域中导航都类似。

以下子部分介绍了如何在工作负载均衡器中查看多个项目的信息。

您可以调整工作负载均衡器中的许多设置和选项，以在对您最有意义的时间范围内显示您需要关注的信息。

选择要应用于视图的设置后，工作负载均衡器会在您每次从任何浏览器或设备访问它时记住这些设置。

### 在资源区访问多个项目的工作负载均衡器

要在多个项目的工作负载均衡器中导航，请执行以下操作：

{{step1-to-resourcing}}

1. 单击左侧面板中的&#x200B;**工作负载均衡器**。

   ![工作负载平衡器](assets/nwe-balancer-global.png)

   工作负载均衡器在以下两个区域显示从本周开始的工作分配信息：

   * **未分配的工作**&#x200B;区域显示以下工作项：

      * 应用过滤器后，会显示分配给角色、团队或未分配的工作项（任务和问题）。
默认情况下，“未分配工作”区域不显示任何工作项。 我们建议使用过滤器来显示本区域为您提供的相关信息。

        有关使用过滤器的信息，请参阅工作负载均衡器[中的](../workload-balancer/filter-information-workload-balancer.md)过滤器信息。

      * 仅在启用“显示角色分配”设置时，才会显示工作项下的角色分配。 有关信息，请参阅本文中的[自定义视图](#customize-the-view)部分。

      * 仅当您启用“按项目分组”设置时，才会显示项目。 有关信息，请参阅本文中的[自定义视图](#customize-the-view)部分。

   * **已分配的工作**&#x200B;区域显示以下工作项：

      * 默认情况下，系统中的所有活动用户都将显示在此区域中。 我们建议使用过滤器来限制此区域中的信息量。 如果将用户分配给项目，则工作项目也会显示在用户的名称下。

      * 分配给至少一个用户的任务和问题显示在用户名下。

        在“已分配的工作”区域中，用户名下的工作项按下列标准排序，顺序如下：

         1. 计划开始日期（最早的在前）
         1. 计划完成日期（最早的在前）
         1. 按项目字母顺序（仅当前两个标准对于多个工作项相同时）

            >[!TIP]
            >
            >* 您可以通过从“项目排序依据”设置中选择选项来自定义项目排序。
            >
            >* 仅当您启用“按项目分组”设置时，才会显示项目。
            > 
            >有关自定义设置的信息，请参阅本文中的[自定义视图](#customize-the-view)部分。

1. （可选）单击&#x200B;**已分配工作**&#x200B;区域中的![筛选器](assets/filter-icon.png)图标&#x200B;**筛选器图标**，然后在筛选器框的&#x200B;**建议**&#x200B;区域中选择&#x200B;**默认筛选器**。

   应用默认筛选器时，属于任何团队及其工作项的用户会显示。 您可以编辑此筛选器的副本。

   >[!TIP]
   >
   >默认过滤器仅在资源区域的工作负载均衡器中可用。

1. 继续执行以下步骤以导航工作负载均衡器：

   * [在工作负载均衡器中选择时间范围](#select-a-time-frame-in-the-workload-balancer)
   * [自定义视图](#customize-the-view)
   * [分配工作项并调整用户分配](#assign-work-items-and-adjust-user-allocations)
   * [在图表中查看分配](#view-allocations-in-a-chart)

### 在工作负载均衡器中选择时间范围

1. 访问&#x200B;**资源**&#x200B;区域的工作负载均衡器，如本文中[访问资源区域中的多个项目的工作负载均衡器](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)部分所述。

   工作负载均衡器显示从本周开始的工作分配信息。

1. 使用水平滚动查看超出屏幕限制的工作项的时间线。
1. 单击左上角的&#x200B;**后退或前进**&#x200B;图标![后退和前进图标](assets/back-and-forward-icons.png)以导航时间轴，然后单击&#x200B;**今天**&#x200B;以返回当前周。
1. 单击工具栏上的&#x200B;**时间范围下拉菜单**，然后单击要显示的时段的开始日期。 默认情况下，在日历中选择的第一周是您导航到的周。

   ![日历选择](assets/calendar-date-picker-wb.png)

1. 从以下选项中选择要在工作负载均衡器中一次显示的周数：
   * 1 周
   * 2 周
   * 4周。 这是默认设置。
   * 6 周
   * 3 个月

   ![选择周](assets/3-months-12-weeks-drop-down-wb.png)

1. 单击工具栏中的以下选项之一可按不同的时间范围显示信息：
   * **天**：默认情况下，显示从今天日期开始的4周内按天显示信息。
   * **周**：按周显示四周的信息。
   * **月**：按月显示三个月的信息。

1. 继续导航工作负载均衡器，如以下部分所述。

### 自定义视图

1. 访问&#x200B;**资源**&#x200B;区域的工作负载均衡器，如本文中[访问资源区域中的多个项目的工作负载均衡器](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)部分所述。

   工作项的名称在左侧列出，由工作负载均衡器右侧的栏表示。 栏的长度表示工作项的时间线。

1. （可选且推荐）使用“未分配”和“已分配的工作”区域中的筛选器以仅显示与您相关的工作项或用户。

   有关详细信息，请参阅工作负载均衡器[中的](../workload-balancer/filter-information-workload-balancer.md)过滤器信息。

   默认情况下，蓝色条表示项目和任务的时间线，栗色条表示问题。

   当选择颜色主题与项目匹配时，可以更改项目和任务栏的颜色。 有关详细信息，请继续阅读此过程。

   已分配工作区域中的工作项按以下标准按项目排序：
   1. 计划开始日期（最早的在前）
   1. 计划完成日期（最早的在前）
   1. 按项目字母顺序（仅当前两个标准对于多个工作项相同时）

1. 单击“未分配”或“已分配”区域左侧的&#x200B;**向右箭头**&#x200B;可展开项目名称（在“未分配”区域）和用户名（在“已分配”区域）下的所有项。

   >[!TIP]
   >
   >仅在启用“按项目分组”设置时，工作项才会列在“未分配”区域的项目名称下。

1. 单击“未指定”或“已指定”区域左侧的&#x200B;**向下箭头**&#x200B;以折叠项目名称（在“未指定”区域）和用户名（在“已指定”区域）下的所有项。

1. 将鼠标悬停在上方，然后将&#x200B;**分隔线**&#x200B;拖放到左侧面板和时间轴区域之间以调整左侧面板的大小。

   ![分隔线](assets/wb-adjust-panel-size.png)

1. 单击&#x200B;**设置**&#x200B;图标![设置图标](assets/settings-gear-icon.png)。

   右侧将显示设置面板。

   ![工作负载均衡器设置面板](assets/workload-balancer-settings.png)

   从下面列出的选项中进行选择，以更新在工作负载均衡器中查看的信息，然后单击“设置”框右上角的&#x200B;**X图标**&#x200B;以将其关闭。

   * **按项目分组**：选择该选项后，将按项目对“未分配”和“已分配”工作区域中的项进行分组。 默认情况下，该选项处于选中状态。

   * **包括来自问题的小时数**：选择此项后，分配给用户的问题会显示在“已分配工作”区域中的用户名下，而未分配给用户的问题会显示在“未分配工作”区域中。 从问题开始的已计划小时数计入项目和已分配工作区域中的用户的已计划小时数。
   * **显示预计日期**：选择此选项时，除计划时间线外，还会显示工作项的预计时间线。 请注意以下事项：
      * 项目、任务和问题的预计时间线在任务、问题和项目栏上方显示为深蓝线。
      * 在计划时间线之外的预计时间线以浅蓝色显示，即使您更新颜色主题也是如此，如下所述。
      * 您无权查看的项目的投影时间线以浅灰色显示，下面有一行。
      * 当任务或问题在到期计划完成日期之前完成时，剩余天数的分配数将被截止，并且不计入用户的分配。 仅当同时启用显示预计日期设置和显示分配图标时，才会显示此字段。

     >[!TIP]
     >
     >请注意，当工作项的计划或预计时间线（不一定同时发生）在所选时间范围内时，工作项会在工作负载均衡器中显示。

   * **显示已完成的工作**：启用此项后，已完成的任务和问题将显示在“已分配的工作”区域中。 默认情况下启用此功能。

     任务或问题栏完成时，其右上角会显示一个绿色复选标记图标。 在项目的选定时间范围内的任务或问题完成时，为项目显示相同的图标。
   * **显示剩余时间**：启用此功能后，Workfront会根据用户计划显示其每天可以工作的时间与在分配给用户的“已分配的工作”区域中为其分配的小时数之间的差值。 默认情况下禁用此项，默认情况下显示分配时间。
   * **显示角色分配**：启用此项后，角色分配会显示在“未分配工作”区域中，位于其分配的工作项下。 默认情况下启用此功能。

   * 在&#x200B;**选择颜色主题**&#x200B;部分中，为项目和任务栏选择所需的颜色。

     >[!TIP]
     >
     >选择颜色主题的设置不会影响问题栏的颜色。 问题始终显示在褐色栏中。

     从以下项中选择：
      * **默认**：所有项目及其工作项的栏都以蓝色显示。
      * **项目**：与每个项目及其任务关联的栏会根据项目的名称而更改。 属于项目的所有任务都以与项目颜色匹配的条状显示。 项目栏以较浅的阴影显示，以将其与任务区分开。 当选择不显示分配时，项目栏还包括项目图标。
      * **项目状态**：与每个项目及其工作项关联的栏将更改为项目状态的颜色。

        项目状态是与项目组关联的状态。 如果组没有特定于组的状态，则工作项栏的颜色为系统级别项目状态的颜色。 显示系统和自定义状态。 有关组状态的信息，请参阅[创建或编辑组状态](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。

   * 在&#x200B;**在**&#x200B;中显示用户分配部分中，从以下内容中选择：
      * **小时**：将分配的时间显示为小时。 这是默认设置。
      * **百分比**：显示已分配时间占总可用时间的百分比
   * 在&#x200B;**排序首选项**&#x200B;部分中，选择您希望在工作负载均衡器中对项排序的方式。 从以下选项中选择：
      * **按主要角色对用户排序**：用户按其主要角色的字母顺序显示在分配的工作区域中。
      * **按字母顺序对用户排序**：用户在“已分配的工作”区域中按其名字的字母顺序显示。
      * **项目排序依据**：从下拉菜单中选择一个项目字段，以按该字段在“未分配”或“已分配”工作区域中按字母顺序对项目排序。

   >[!TIP]
   >
   >只有在启用了按项目分组设置时，您才能按项目排序。 否则，此设置将灰显。

1. （可选且视情况而定）将颜色主题更改为项目状态时，将鼠标悬停在左侧项目的名称上可查看项目的状态。

   ![项目状态工具提示](assets/hover-over-project-status-tooltip-350x115.png)

### 分配工作项并调整用户分配

1. 访问资源区域中的工作负载均衡器，如本文中[访问资源区域中的多个项目的工作负载均衡器](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)部分所述。
1. 单击&#x200B;**显示分派图标** ![显示分派图标](assets/show-allocations-icon-small.png)以查看工作项的每日或每周计划小时数。

   这将用未分配和已分配工作区域中的每日或每周计划小时数替换工作项栏中的名称。 默认情况下禁用此设置。

   显示过度分配的天数以红色显示。

   >[!TIP]
   >
   >* 显示分派选项仅影响为项目、任务、问题和不可访问项显示的内容。 默认情况下，会显示用户的每日已计划小时数，该小时数不能隐藏。
   >* 您必须启用按项目分组设置以显示项目的每日计划小时数。
   >* 当您按周查看工作负载均衡器时，显示的小时数是每周计划小时数。

1. （可选）将鼠标悬停在用户行中的已分配时间上以了解用户的容量和分配。 容量是用户根据其计划提供的可用性。

   ![分配的时间详细信息](assets/overallocation-vs-capacity-tooltip-wb-nwe.png)

1. （可选）单击&#x200B;**隐藏分派图标** ![显示分派图标](assets/show-allocations-icon-small.png)以在工作项的栏中显示任务和问题的名称。
1. 单击任务、问题或角色名称右侧的&#x200B;**更多菜单**&#x200B;图标![更多图标](assets/more-icon.png)，然后单击以下选项之一。

   ![更多菜单](assets/more-menu-right-of-task-350x104.png)

   * **将此工作项分配给**，然后在&#x200B;**搜索人员、角色或团队**&#x200B;字段中开始键入要将此工作项分配到的用户、角色或团队的名称。

     单击&#x200B;**高级**&#x200B;访问工作项的高级工作分配屏幕。 有关详细信息，请参阅[创建高级工作](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md)。

     您还可以使用以下快捷方式分配任务或问题：

      * 在Windows中：按住CTRL并单击任务栏或问题栏。
      * 在Mac中：按住CMD单击任务栏或问题栏。

     有关在工作负载均衡器中将工作项分配给用户的更多信息，请参阅[在工作负载均衡器中分配工作的概述](../workload-balancer/assign-work-in-workload-balancer.md)。

     >[!NOTE]
     >
     >启用“显示角色分配”设置后，角色分配仅显示在“未分配工作”区域的工作项下。 有关信息，请参阅本文中的[自定义视图](#customize-the-view)部分。 在&#x200B;**更多**&#x200B;菜单中，角色分配仅具有&#x200B;**将此项分配给**&#x200B;选项。

     >[!TIP]
     >
     >如果您的Workfront或组管理员在环境中启用了委托，请使用“工作总揽”选项卡将用户分配给任务或问题。 有关委派工作的信息，请参阅[委派任务和问题](../../manage-work/delegate-work/how-to-delegate-work.md)。

   * **编辑分配**，然后编辑用户的每日或每周分配。 有关管理用户分配的信息，请参阅[在工作负载均衡器](../workload-balancer/manage-user-allocations-workload-balancer.md)中管理用户分配。

   * **打开摘要**。 “摘要”面板将在右侧打开，然后单击“工作总揽”字段，并开始在&#x200B;**搜索人员、角色或团队**&#x200B;字段中键入用户、角色或团队的名称以分配该项目。 有关详细信息，请参阅本文中的[显示有关任务和问题的更多信息](#display-more-information-about-tasks-and-issues)部分。

1. （可选）双击工作项栏中用户的每日或每周分配以编辑分配的小时数，然后单击&#x200B;**保存**&#x200B;图标![保存图标](assets/save-allocations-wb.png)以保存分配，或单击&#x200B;**取消**&#x200B;图标![取消图标](assets/cancel-allocations-wb.png)以删除您调整的分配。

   >[!TIP]
   >
   >保存和取消图标会在任务或问题的时间线栏的末尾显示。
   >
   >![保存或取消手动分配](assets/cancel-and-save-icon-on-adjust-allocation-bar-wb-highlighted.png)

   有关管理用户分配的信息，请参阅[在工作负载均衡器](../workload-balancer/manage-user-allocations-workload-balancer.md)中管理用户分配。

1. 单击&#x200B;**批量分配**&#x200B;以批量分配工作项。

   有关详细信息，请参阅[使用工作负载均衡器批量分配工作](../workload-balancer/assign-work-in-workload-balancer-in-bulk.md)。
1. 从&#x200B;**未分配的工作**&#x200B;区域或用户拖动项目，并将它们拖放到其他用户上以进行分配。

   有关详细信息，请参阅[通过拖放在工作负载均衡器中分配工作](../workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)。

### 在图表中查看分配

您可以在图表中查看分配，而不是按每日或每周数字查看分配。

1. 访问资源区域中的工作负载均衡器，如本文中[访问资源区域中的多个项目的工作负载均衡器](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)部分所述。
1. 单击&#x200B;**图表图标** ![图表图标](assets/user-allocation-chart-icon.png)以图表格式显示用户分配。

   用户过度分配的天数显示为红色块，而用户分配不足或容量不足的天数显示为蓝色块。

   块的大小表示分配的数量：框越大，用户分配到当天或本周工作项的时间就越多。

   ![用户分配为图表](assets/wb-allocation-as-chart.png)

### 显示有关任务和问题的更多信息

您可以在工作负载均衡器中查看有关任务和问题的更多信息。

1. 访问资源区域中的工作负载均衡器，如本文中[访问资源区域中的多个项目的工作负载均衡器](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)部分所述。
1. 要在“摘要”面板中查看更多信息，请执行下列操作之一：

   * 单击任务或问题栏以打开右侧的“摘要”面板。
   * 单击&#x200B;**打开摘要**&#x200B;图标![打开摘要图标](assets/summary-panel-icon.png)，然后单击任务或问题栏以打开摘要面板。
   * 单击任务或问题右侧的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**打开摘要**。

   有关在工作负载均衡器的摘要中更新任务信息的信息，请参阅[使用摘要更新工作负载均衡器中的工作项](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md)。

1. 将鼠标悬停在任务或问题的名称上可查看有关该任务或问题的更多信息。 任务或问题上方会显示一个框，其中包含下列信息：

   * 任务或问题的名称。
   * 项目的名称。
   * 计划的开始日期和完成日期。
   * 计划的小时数。
   * 对于任务，为前置任务编号。
   * 对于任务，此框上角的指示器指示任务是否准备好处理。

   ![任务详细信息](assets/task-bar-hover-over-detail-wb.png)

1. 单击左侧工作项的名称以访问该工作项。 工作项将在新的浏览器选项卡中打开。

### 全屏显示工作负载均衡器

1. 访问资源区域中的工作负载均衡器，如本文中[访问资源区域中的多个项目的工作负载均衡器](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)部分所述。

1. 单击&#x200B;**全屏**&#x200B;图标![全屏图标](assets/full-screen.png)以全屏显示工作负载均衡器。

   工作负载均衡器占据整个屏幕。 浏览器窗口和选项卡将从视图中排除。

1. 单击&#x200B;**退出全屏**&#x200B;图标![退出全屏图标](assets/exit-full-screen.png)以返回默认屏幕并在浏览器选项卡中查看工作负载均衡器。

## 导航团队的工作负载均衡器

在团队的工作负载均衡器中导航类似于在多个项目的工作负载均衡器中导航。 有关信息，请参阅本文中的[为多个项目导航工作负载均衡器](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)部分。

{{step1-to-team}}

默认情况下，将显示主团队的页面。

1. 单击左侧面板中的&#x200B;**工作负载均衡器**。

   ![团队的工作负载均衡器](assets/nwe-balancer-team-350x172.png)

   默认情况下，团队的工作负载均衡器显示以下信息：

   * 在&#x200B;**未分配的工作**&#x200B;区域：分配给团队或团队和工作角色且未分配给用户的工作项。 启用“显示角色分配”设置后，角色分配会显示在“未分配工作”区域的工作项下。
   * 在&#x200B;**已分配工作**&#x200B;区域：分配给用户的工作项显示在用户名下。

1. 继续导航团队的工作负载均衡器，如本文的资源区域[部分中的](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)导航多个项目的工作负载均衡器中所述。

## 在单个项目的工作负载均衡器中导航

{{step1-to-projects}}

1. 单击项目名称以打开项目页面。
1. 单击左侧面板中的&#x200B;**工作负载均衡器**。

   ![项目的工作负载均衡器](assets/nwe-balancer-project-350x152.png)

   默认情况下，项目的工作负载均衡器显示以下信息：

   * 在&#x200B;**未分配的工作**&#x200B;区域：项目上已分配给角色或团队但未分配给用户的工作项。 启用“显示角色分配”设置后，角色分配会显示在“未分配工作”区域的工作项下。
   * 在&#x200B;**已分配工作**&#x200B;区域：项目中至少分配给一个用户的工作项。

   我们建议使用过滤器来仅显示对您重要的用户。

   例如，您可以考虑仅显示属于您的团队或组的用户。 有关详细信息，请参阅工作负载均衡器[中的](../workload-balancer/filter-information-workload-balancer.md)过滤器信息。

1. （可选）在分配的工作区域中单击&#x200B;**筛选器**&#x200B;图标![筛选器图标](assets/filter-icon.png)，然后从筛选器面板的&#x200B;**建议**&#x200B;区域中选择&#x200B;**此项目的工作项**&#x200B;选项。 默认情况下，此筛选器处于取消选中状态。

   选择此选项时，将仅显示分配给选定项目上用户的项。

   如果未选择该选项，则会显示项目上分配给用户的所有项，无论这些项属于哪个项目。

1. （可选且推荐）在已分配的工作区域中应用筛选器以显示对您很重要但可能未分配到项目中的项的用户，然后单击&#x200B;**显示所有用户**&#x200B;图标![显示所有用户图标](assets/show-all-users-icon-project-workload-balancer.png)。

   通过显示所有用户，您可以显示Workfront中尚未分配给项目工作或其他角色的所有用户。

   您可以先应用过滤器，以减少显示的用户数。

   例如，您可能希望首先筛选属于您的团队或组的用户，然后显示所有这些用户。

   有关如何构建过滤器的信息，请参阅工作负载均衡器中的[过滤器信息](../workload-balancer/filter-information-workload-balancer.md)。

   >[!NOTE]
   >
   > 显示所有用户选项仅适用于项目的工作负载均衡器。

1. （可选）单击&#x200B;**显示角色分配**&#x200B;图标![显示角色分配图标](assets/show-role-allocation-icon.png)。

   此时将显示“角色分配”面板。

   您可以查看与项目中的工作角色以及从“方案规划者”链接到项目的计划相关联的工作角色的相关计划小时数信息。

   有关详细信息，请参阅[在项目和计划之间协调资源分配概述](../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md)。

   >[!NOTE]
   >
   >如果您的组织尚未购买Workfront Scenario Planner的许可证，则无法查看计划工作角色信息。 在这种情况下，您只能查看与项目中的工作角色关联的已计划小时数。 有关详细信息，请参阅[使用Scenario Planner](../../scenario-planner/access-needed-to-use-sp.md)所需的访问权限。

1. 继续导航项目的工作负载均衡器，如本文的[导航多个项目的工作负载均衡器](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)部分中所述。

### 导航用户的工作负载均衡器

您可以在自己的用户配置文件上访问工作负载均衡器。

{{step1-click-profile-pic}}

1. 单击左侧面板中的&#x200B;**工作负载均衡器**。

   此时将显示用户的工作负载均衡器。

   ![用户的工作负载均衡器](assets/workload-balancer-user.png)

   默认情况下，用户的工作负载均衡器按信息显示以下内容：

   * **已分配的工作**：已分配给特定用户的任务和问题。

   >[!NOTE]
   >
   >用户配置文件上的工作负载均衡器是只读的，无法更改分配和分配。

1. 继续导航用户的工作负载均衡器，如本文的[导航多个项目的工作负载均衡器](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)部分中所述。


<!--old content below - this used to be a one-large-procedure article - outdated, and rewrote it above with several smaller procedures: 

# Navigate the Workload Balancer

<!-drafted note for 22.4 release: remove all production/ preview references at Prod release>

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

Use the Workload Balancer to understand the availability of your resources as well as to assign work to your users. This article walks you through using the icons and settings available to update the view for and navigate the Workload Balancer.

>[!NOTE]
>
>The Workload Balancer is a resource scheduling tool that will eventually replace the current resource scheduling tools which are currently deprecated. 
>
>For more information about removing the resource scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).
>
>We recommend that you use the Workload Balancer for scheduling your resources.

The Workload Balancer is available in multiple areas of Adobe Workfront. Navigating it is similar in all areas. This article describes how to navigate the Workload Balancer for multiple projects in the Resourcing area. For more information about where the Workload Balancer is located, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

For information about managing resources using the Workload Balancer, also consider reading the following articles:

* [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
* [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, when using the Workload Balancer in all areas in the Production environment</p>
   <p><span class="preview">Work, when using the Workload Balancer of a project, in the Preview environment</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, and issues </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations for viewing items in the Workload Balancer

Consider the following when viewing the Workload Balancer:

* Projects display in the Workload Balancer only when the Group by Project setting is enabled. This setting is enabled by default.
* Mousing over a task or an issue displays the following additional information about the task or issue:

  * Project name

  * Task or issue name

  * Parent task

  * Planned Start and Completion Dates

  * Number of Planned Hours

  * Ready to start or Not ready status

  ![task-pop-up-with-additional-info-in-workload-balancer](assets/task-pop-up-with-additional-info-in-global-wb.png)

* When a project has no tasks during a period of time, the bar at the project level becomes a dimmed color.

  ![Break in project timeline](assets/wb-break-in-project-timeline-with-no-tasks-highlight-350x80.png)

* When you don't have permissions to see certain items, they display as **Inaccessible work items** or **Inaccessible projects**.

  ![Inaccessible items](assets/balancer-inaccessible-items-and-projects-highlighted-350x108.png)

* The names of the work items display on the left and within the timeline selected on the right. 
* The total of Planned Hours for each work item displays to the right of the name of the work items on the left. 
* The total of the Planned Hours for each project displays to the right of the name of the project on the left.

  The Planned Hours information for the project is a total of Planned Hours from all items listed in the Workload Balancer, and not a total of Planned Hours on the project.

## Overview of the Unassigned Work and Assigned Work areas

The Workload Balancer displays work items in two separate areas, depending on their assignments.

The two areas of the Workload Balancer display the following information:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Unassigned Work</td> 
   <td> <p>This area displays tasks <span class="preview">and issues</span> unassigned to users. </p> <p>Projects display when the Group by Project setting is enabled.</p> <p>This area does not display any work items by default. We recommend using filters to display relevant information for you in this area.</p> <p>After you apply a filter, this area displays the following work items:</p> 
    <ul> 
     <li>unassigned</li> 
     <li>assigned to a team </li> 
     <li>assigned to a job role</li> 
     <li> <p>assigned to a team and a role at the same time</p> </li> 
    </ul> <p>Tip: Items assigned to a user as the primary assignee do not display in the Unassigned Work area. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assigned Work</td> 
   <td> <p> All active users in the system display in this area by default. We recommend using filters to limit the amount of information in this area.  </p> <p>Both tasks and issues display in the Assigned Work area. </p> <p>Projects display when the Group by Project setting is enabled.</p> <p>The work items that the users are assigned to display under their names. </p> <p>If a work item is assigned to multiple users, the item displays under each assigned user. </p> </td> 
  </tr> 
 </tbody> 
</table>

For information about applying a filter in the Workload Balancer, see [Filter information in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

![Empty unassigned area](assets/balancer-empty-unassiged-area-350x179.png)

## Navigate the Workload Balancer

You can update the view in the Workload Balancer to display exactly the information you need to focus on in the time frame that makes the most sense to you.

After selecting the settings you want to apply to your view, the Workload Balancer remembers these settings every time you access it from any browser or device.

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Resourcing**.
1. Click **Workload Balancer** in the left panel.

   The Workload Balancer displays work assignment information starting with the current week. The names of work items are listed on the left side as well as represented by bars on the right side of the of the Workload Balancer within their respective timelines. By default, blue bars represent the timelines of projects and tasks and maroon bars represent issues.

   >[!TIP]
   >
   >You can change the color of the bars for projects and tasks when you select your color scheme to match the project. For more information, continue reading this procedure.

   The work items that display under the name of users in the Workload Balancer are sorted by the following criteria, in this order:

   1. Planned Start Date (oldest first)
   1. Planned Completion Date (oldest first)
   1. Alphabetical by project (only when the first two criteria are identical for multiple work items)

1. Click the right-pointing arrow to the left of the Unassigned or Assigned areas to expand all items under the project names (in the Unassigned area) and under the user names (in the Assigned area).
1. Click the down-pointing arrow to the left of the Unassigned or Assigned areas to collapse all items under the project names (in the Unassigned area) and under the user names (in the Assigned area).
1. Use the horizontal scroll to navigate the timelines of work items that extends beyond the limits of the screen. 
1. Use the vertical scroll to display additional users and work items. 
1. Drag and drop the separation line between the left panel and the timeline areas to adjust the size of the left panel.

   ![Separation between left panel and timeline](assets/separation-line-between-left-panel-and-timeline-highlighted-nwe-350x174.png)

1. Click the **Filter icon** ![Filter icon](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or the **Assigned Work** areas to select the type of information to display in the Workload Balancer.

   For information about filtering information in the Workload Balancer, see [Manage filters in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md). 

1. Click the right-pointing arrow next to **Unassigned Work** to expand this area or the down-pointing arrow to collapse it.

   >[!TIP]
   >
   >No items display in this area by default. You must apply a filter to view unassigned work items.

1. Drag and drop the separation line between the **Unassigned Work** and **Assigned Work** areas to adjust their size.

   ![Separation line between areas](assets/modern-scheduler-separation-line-between-areas-350x278.png)

1. Click the back or forward icons ![Back and forward icons](assets/back-and-forward-icons.png) to navigate the timeline, then click **Today** to return to the current week. 

1. Click the **time frame drop-down menu** on the toolbar, then click the beginning date of the period you want to display. By default, the first week selected on the calendar is the week you navigated to.

   ![Calander date picker](assets/calendar-date-picker-wb.png)


1. Click one of the following options in the toolbar to display information by different time frames:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Day</td> 
      <td>Displays information by day for four weeks starting with today's date, by default. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Week</td> 
      <td>Displays information by week for four weeks. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Month</td> 
      <td> <p><span>Displays information by month for three months.</span> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Select the number of weeks you want to display at one time in the Workload Balancer from the following options:

   * 1 week
   * 2 weeks
   * 4 weeks. This is the default setting.
   * 6 weeks
   * 3 months
   ![3 months dropdown](assets/3-months-12-weeks-drop-down-wb.png)     

1. Click the **Settings** icon ![Settings icon](assets/settings-gear-icon.png).

   The Settings panel displays.

   ![Settings box](assets/settings-box-options-global-with-color-theme-and-percentage-wb-nwe.png)

   Select from the options listed below to update the information you view in the Workload Balancer, then click the **X icon** in the upper-right of the Settings box to close it.

   * **Group by Project**: When this is selected, the items in the Unassigned and Assigned Work areas are grouped by project. This is selected by default.

     ![Group by project](assets/group-by-project-350x530.png)

   * **Include hours from issues**: When this is selected, issues assigned to users display under the user's name in the Assigned Work area <span class="preview">and issues that are not assigned to users display in the Unassigned Work area</span>. The Planned Hours from the issues count towards the Planned Hours for the project and for the user in the Assigned Work area. 

        ![Issue on Workload Balancer](assets/issue-on-workload-balancer-350x20.png)

   
      * **Show Projected Dates**: When this is selected, the projected timeline of work items displays in addition to the planned timeline. Notice the following:

         * The projected timeline of project, tasks, and issues displays as a dark blue line above the task, issue, and project bars.
         * The projected timeline that is outside of the planned timeline displays in light blue, even when you update the color theme, as described below.
         * The projected timeline for the items that you have no access to view displays in light gray with a line underneath.
         * When a task or issue completes before the due Planned Completion Date the allocation numbers for the remaining days are struck through and do not count towards the user's allocation. This displays only when both the Show Projected Dates setting and the Show allocation icon are enabled.

         ![Task issue projected timelines](assets/task-issue-projected-timelines-350x91.png)

         >[!TIP]
         >
         >Notice that work items display in the Workload Balancer when either their planned or the projected timelines (not necessarily both at the same time) occur during the timeframe selected.

   * **Show completed work**: When this is enabled, tasks and issues that are completed display in the Assigned Work area. This is enabled by default.

     A green checkmark icon ![Checkmark icon](assets/green-checkmark-icon.png) displays to the upper-right corner of a task or issue bar when they are completed. The same icon displays for a project when the tasks or issues for the selected time frame of the project are completed. 
   
   * **Show remaining time**: When this is enabled, Workfront displays the difference between the daily time for which the user is available to work based on their schedules and the hours for which they are allocated in the Assigned Work area for the users. This is disabled by default and allocated time displays by default.

   * In the **Select color theme** section, select the color that you want for the project and task bars.  

      >[!NOTE]
      >
      >The setting for selecting the color theme  does not affect the color of the issue bars. Issues always display in a maroon-color bar. 


      Select from the following:

      * **Default**: The bars for all projects and their work items display in blue.  
      * **Project**: The bars associated with each project and its tasks change according to the name of the project. All tasks that belong to the project display in bars that match the color of the project. The project bars display in a lighter shade to distinguish them from the tasks. The project bars also include a project icon when choosing not to display allocations.
      * **Project Status**: The bars associated with each project and its work items change to the color of the status of the project.

        >[!TIP]
        >
        >* The project status is that associated with the Group of the project. If the Group does not have group-specific statuses, the color of the work item bars is that of the system-level project status. Both system as well as custom statuses display. For information about group statuses, see [Create or edit a group status](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
        
   * In the **Display user allocation in** section, select from the following:

      * **Hours**: Displays allocated time as hours. This is the default. 
      * **Percentage**: Displays allocated time as a percentage of the total available time

   * In the **Sorting preferences** section, select how you want the items to be sorted in the Workload Balancer. Select from the following options: 

      * **Sort users by Primary Role**: Users display in the alphabetical order of their Primary Roles in the Assigned Work area.

      * **Sort users alphabetically**: Users display in the alphabetical order of their first names in the Assigned Work area.

      * **Sort projects by**: Select a project field from the drop-down menu to sort projects alphabetically by that field in the Unassigned or Assigned Work areas. 

      >[!TIP]
      >
      >You can sort by projects only when the Group by Project setting is enabled. Otherwise, this setting is dimmed.


1. (Optional and conditional) If you changed the color theme to Project Status, hover over the name of a project on the left to view the status of the project.

   ![Project status tooltip](assets/hover-over-project-status-tooltip-350x115.png)

1. <span class="preview">(Conditional and recommended) In the Workload Balancer of a project, apply a filter in the Assigned Work area to display users that are important to you but might not be assigned to items on the project, then click the **Show all users** icon ![Show all users   ](assets/show-all-users-icon-project-workload-balancer.png). This displays other users in the system that are not yet assigned on the project. For information about how to build a filter, see [Manage filters in the Workload Balancer](../workload-balancer/filter-information-workload-balancer.md).</span>

 
   >[!TIP]
   >
   ><span class="preview">The Show all users icon is available only for the Workload Balancer of a project.</span> 

1. Click the **Chart icon** ![Chart icon](assets/user-allocation-chart-icon.png) to display the user allocation in a chart format. Days where the user is overallocated display as red blocks, and days where the user is underallocated or at capacity display as blue blocks. The size of the blocks indicates the amount of the allocation: the larger the box, the more time the user is allocated to work items for that day or week.

   ![User allocation chart](assets/user-allocation-chart-350x237.png)

1. Click the **Show allocations icon** ![Show allocations icon](assets/show-allocations-icon-small.png) to view the daily or weekly Planned Hours for work items.

   This replaces the name in the bars of the work items with the amount of daily or weekly Planned Hours in the Unassigned and Assigned Work areas. This setting is disabled by default.

   >[!TIP]
   >
   >* The Show allocations setting only affects what displays for projects, tasks, issues and inaccessible items. Daily Planned Hours for users display by default and cannot be hidden.
   >* You must enable the Group by Project setting to display daily Planned Hours for projects. 
   >* When you view the Workload Balancer by week, the hours displayed are the weekly Planned Hours. 

   Days that show overallocations display in red. 

1. (Optional) Hover over the allocated time in the user line to understand what the capacity and allocation of the user. The capacity is the availability of the user according to their schedule.

   ![Overallocation vs capacity](assets/overallocation-vs-capacity-tooltip-wb-nwe.png)

1. (Optional) Click the **Hide allocations icon** ![Show allocations icon](assets/show-allocations-icon-small.png) to display the name of the tasks in the bars of the work items. 
1. Click the **More menu** icon ![More icon](assets/more-icon.png) to the right of a task or issue name, then click one of options below. 

   ![More menu](assets/more-menu-right-of-task-350x104.png)

      * **Assign this to**, then start typing the name of a user, role, or team you want to assign the work item to in the **Search people, role, or teams** field.
    
      >[!TIP]
      >
      >You can also use the following shortcuts to assign tasks or issues:
      >
      >* In Windows: CTRL+click the task or issue bar.
      >* In Mac: CMD+click the task or issue bar.

      For more information about assigning work items to users in the Workload Balancer, see [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md). 

      >[!TIP]
      >
      >If your Workfront or group administrator enabled delegations in your environment, use the Assignments tab to assign users to the task or issue. For information about delegating work, see [Manage task and issue delegation](../../manage-work/delegate-work/how-to-delegate-work.md).

   * **Edit allocations**, then edit the daily or weekly allocations for the user. For information about managing user allocations, see [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

1. Click the bar of a task or issue to open the Summary panel on the right

   Or

   Click **Open Summary** icon ![Open Summary icon](assets/summary-panel-icon.png), then click the bar of a task or issue to open the Summary panel

   Or

   Click the **More** menu ![More icon](assets/more-icon.png) to the right of a task or issue, then click **Open Summary**.

   For information about updating task information in the Summary in the Workload Balancer, see [Update work items in the Workload Balancer using the Summary](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

    The Summary panel opens on the right. 

1. Click **Bulk Assignments** to assign work items in bulk.

   For more information, see [Assign work in bulk using the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md). 

1. Click the **Full screen** icon ![Full screen icon](assets/full-screen.png) to display the Workload Balancer in full screen, then click the **Exit full screen** icon ![Exit full screen](assets/exit-full-screen.png) to return to the default screen. 
1. (Optional) Double-click a daily or weekly allocation for a user inside the bar of a work item to edit the number of allocated hours, then click the **Save** icon ![Save icon](assets/save-allocations-wb.png) to save the allocations or the **Cancel** icon ![Cancel icon](assets/cancel-allocations-wb.png) to remove the allocations you adjusted.

   >[!TIP]
   >
   >The Save and Cancel icons display towards the end of a task or an issue's timeline bar.

   For information about managing user allocations, see [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md). 

1. Click the name of a work item on the left to access it. 
1. Click the **Shareable link icon** ![](assets/wb-shearable-link-icon-small.png) to copy the direct URL for the Workload Balancer to your clipboard. 
1. (Optional) Share the link with any user who does not have direct access to the Workload Balancer.

   For information about sharing the Workload Balancer with a link, see [Share the Workload Balancer with a link](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md). 

1. (Conditional) From the Workload Balancer of a project, click the **Show role allocations** icon ![Show role allocations](assets/show-role-allocation-icon.png).

   The Role Allocation panel displays. You can view information about Planned Hours associated with job roles on the project and job roles associated with initiatives from the Scenario Planner. For more information, see [Overview of reconciling resource allocations between projects and initiatives](../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

   >[!TIP]
   >
   >You cannot view initiative job role information if your organization has not purchased a license for the Workfront Scenario Planner. In this case, you can only view the planned hours associated with job roles on the project. For more information, see [Access needed to use the Scenario Planner](../../scenario-planner/access-needed-to-use-sp.md).

-->
