---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: 向展示板添加进气柱
description: 您可以选择在展示板中添加一个摄取列，根据您定义的过滤器，在将任务和问题添加到Workfront中时，将其自动作为连接的卡片提取。
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: 81d68656c5dc4811884cde53193139856f290f4d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 向展示板添加进气柱

您可以选择在展示板中添加一个摄取列，在将任务和问题作为连接的信息卡添加到时，将其自动提取 [!DNL Workfront]，基于您定义的过滤器。 进纸列可用作看板团队的积压工作列、支持团队在问题添加到请求队列时查看问题的进纸位置，或您需要的任何其他目的。

一个展示板上只允许有一列进纸，它始终显示为最左侧的栏。

进纸柱在动态板上不可用。

摄入量限制为300项任务和300项问题。 它们按项目上定义的优先级排序。 有关优先级的信息，请参阅 [更新任务优先级](/help/quicksilver/manage-work/tasks/task-information/task-priority.md) 和 [更新问题优先级](/help/quicksilver/manage-work/issues/issue-information/update-issue-priority.md).

有关列的更多信息，请参阅 [管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). 有关已连接卡的信息，请参阅 [在主板上使用连接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!DNL Request] 或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 创建进气列

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **[!UICONTROL 展示板]**.
1. 访问展示板。 有关信息，请参阅 [创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 单击 **[!UICONTROL 配置]** 打开“配置”面板。
1. 展开 **[!UICONTROL 展示板]**.
1. 打开 **[!UICONTROL 动态摄取要登入的项目]**.

   ![创建进气列](assets/create-intake-column2.png)

   进纸柱在板的左侧添加。 在对其应用过滤器之前，它将一直留空。

1. 单击 **[!UICONTROL 筛选源]** 选择 **[!UICONTROL 任务]** 或 **[!UICONTROL 问题]**.

   >[!NOTE]
   >
   >您可以过滤进气列以包含任务和问题，但必须为每个对象类型分别设置过滤器。
   >
   >此外，保存的过滤器和系统默认过滤器也可供您选择。

1. 在过滤器面板上，单击 **[!UICONTROL 新建过滤器]** 以开始使用。

   ![单击新建过滤器](assets/intake-filter-dialog5.png)

1. 构建过滤器并单击 **[!UICONTROL 另存为新]**.

   ![过滤器生成器](assets/intake-filter-dialog6.png)

   此示例显示了对特定项目中状态为 [!UICONTROL 新建] 或 [!UICONTROL 正在进行]，并且已分配给我。

   有关构建过滤器的详细信息，请参阅文章中的“在标准生成器中创建或编辑过滤器”部分 [在中创建或编辑过滤器 [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. 命名过滤器并单击 **[!UICONTROL 保存]**.

   ![键入过滤器的名称](assets/intake-filter-dialog7.png)

   为过滤器指定唯一名称后，您便可以搜索该名称。

1. 该过滤器会显示在已保存过滤器的列表中，并自动应用于进气列。 单击过滤器面板顶部的X以将其关闭。

   ![保存的过滤器](assets/intake-filter-dialog8.png)

1. （可选）要与他人共享该过滤器，请将鼠标悬停在保存的过滤器上，单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单图标](assets/more-icon-spectrum.png)，然后选择 **[!UICONTROL 共享]**. 在过滤器共享框中选择要与之共享的用户或团队。 有关更多信息，请参阅 [共享过滤器、查看或分组](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. （可选）要在摄入列中同时包含任务和问题，请单击 **[!UICONTROL 筛选源]** 并选择另一个对象以创建另一个过滤器。
1. 添加完过滤器后，请查看进入列以验证是否显示了正确的任务和问题。

   ![引入列](assets/intake-column-added3.png)

   在将信息卡移入其他展示板列之前，信息卡进入列中不可编辑。 您可以单击卡片以在只读视图中将其打开，也可以单击 ![打开任务或问题](assets/boards-launch-icon.png) 在新的浏览器选项卡中打开任务或问题。

   您可以手动对进气列上的项目重新排序。

   摄取列右上方的图标显示当前该列中的卡片数量以及应用的过滤器数量。

   >[!NOTE]
   >
   >您可以随时更新过滤器，方法是打开“配置”面板，单击 **[!UICONTROL 筛选源]**，然后选择 **[!UICONTROL 任务]** 或 **[!UICONTROL 问题]**.

1. （可选）要在进气列中搜索项目，请单击 ![“搜索”图标](assets/search-icon.png) 列中。
1. （可选）要将信息卡从进入列移动到另一列，请将信息卡拖放到您希望显示的位置。

   或

   单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单图标](assets/more-icon-spectrum.png) ，然后选择 **[!UICONTROL 移动]**. 然后，在 **[!UICONTROL 移动项目]** 框中，选择另一列并选择 **[!UICONTROL 移动]**.

1. （可选）要删除摄取列，请单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单图标](assets/more-icon-spectrum.png) 选择 **[!UICONTROL 删除]**.
