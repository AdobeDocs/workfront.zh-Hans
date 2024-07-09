---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: 将引入列添加到展示板
description: 您可以选择向展示板添加引入列，以根据您定义的过滤器在Workfront中添加任务和问题时，自动将任务和问题提取为已连接的卡片。
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: d2d96baa060cb3306f1767d179d514b569b0156a
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 3%

---

# 将引入列添加到展示板

您可以选择将引入列添加到展示板，在添加任务和问题时，自动将它们拉入为连接的卡片 [!DNL Workfront]，基于您定义的过滤器。 引入列可以作为Kanban团队的积压列、支持团队查看添加到请求队列中的问题的引入位置或您需要的任何其他目的。

展示板上只允许有一个引入列，并且始终显示为最左侧的列。

摄取列在动态展示板上不可用。 但是，您可以更新用于定义哪些卡片将引入动态展示板上的筛选器。 在动态展示板上更改这些筛选器时，未包含在Workfront任务或问题中的卡片设置（例如标记）将被重置。

>[!NOTE]
>
>出于安全原因，只有展示板所有者才能更改“配置”面板中的展示板过滤器。

引入列限制为300个任务和300个问题。 引入列中项目的默认排序如下：

任务：

* 主要顺序：项目名称
* 次要顺序：工作分解结构

问题：

* 主要顺序：项目名称
* 次要顺序：参考号

>[!IMPORTANT]
>
>如果有多位用户同时使用讨论区，建议经常刷新讨论区。 刷新页面有助于使展示板上的视觉更改保持最新，并防止出现从摄取列将重复卡片移动到展示板的问题。

有关列的详细信息，请参见 [管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). 有关已连接卡的信息，请参阅 [在展示板上使用连接的信息卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!DNL Request] 或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 使用简单过滤器创建引入列

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **[!UICONTROL 讨论区]**.
1. 访问展示板。 有关信息，请参阅 [创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 单击 **[!UICONTROL 配置]** ，打开“配置”面板。
1. 展开 **[!UICONTROL 展示板]**.
1. 打开 **[!UICONTROL 将项目动态摄取到展示板]**.

   ![引入列简单过滤器选项](assets/intake-column-simple-filters.png)

   引入列添加到展示板的左侧。 在将筛选器应用于列表之前，列表会保持空白。

1. （可选）搜索并选择 [!DNL Workfront] [!UICONTROL **项目**].
1. （可选）搜索并选择用户或团队 [!UICONTROL **指定任务**].
1. 选择 [!UICONTROL **包括已完成的工作**] 以在引入列中显示具有“完成”状态的任务和问题。

   >[!NOTE]
   >
   >如果未选中此选项，则当处于其他状态的卡标记为完成时，它们将“从”展示板上“脱落”并且不再显示。

1. 单击 [!UICONTROL **应用**].

   所有对象都以连接的卡片形式显示在展示板摄取列中。

   ![引入列](assets/intake-column-added3.png)

## 使用高级过滤器创建引入列

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **[!UICONTROL 讨论区]**.
1. 访问展示板。 有关信息，请参阅 [创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 单击 **[!UICONTROL 配置]** ，打开“配置”面板。
1. 展开 **[!UICONTROL 展示板]**.
1. 打开 **[!UICONTROL 将项目动态摄取到展示板]**.

   引入列添加到展示板的左侧。 在将筛选器应用于列表之前，列表会保持空白。

1. 单击 [!UICONTROL **使用高级过滤器**].
1. 单击 **[!UICONTROL 添加筛选条件源]** 并选择 **[!UICONTROL 任务]** 或 **[!UICONTROL 问题]**.

   ![引入列高级过滤器选项](assets/intake-column-advanced-filters1.png)

   >[!NOTE]
   >
   >您可以筛选引入列以同时包含任务和问题，但必须为每个对象类型单独设置筛选器。
   >
   >此外，还可选择已保存的筛选器和系统默认筛选器。

1. 在筛选器面板上，单击 **[!UICONTROL 新建过滤器]** 以开始使用。

   ![单击新建过滤器](assets/intake-filter-dialog5.png)

1. 构建过滤器并单击 **[!UICONTROL 另存为新预设]**.

   ![筛选器生成器](assets/intake-filter-dialog6.png)

   此示例显示特定项目中处于以下状态的任务的过滤器： [!UICONTROL 新建] 或 [!UICONTROL 进行中].

   >[!NOTE]
   >
   >建议不要在展示板过滤器上使用“我”（已登录用户）通配符，因为不保证会始终显示已登录用户的任务或问题。 在展示板设置正确的任务和问题后，您可以筛选展示板以显示特定被分配人的项目。 有关更多信息，请参阅 [在展示板中过滤和搜索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   有关构建过滤器的更多详细信息，请参阅文章中的“在标准生成器中创建或编辑过滤器”部分 [在中创建或编辑筛选器 [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. 命名过滤器并单击 **[!UICONTROL 保存]**.

   ![键入筛选器的名称](assets/intake-filter-dialog7.png)

   为过滤器指定唯一名称可让您稍后搜索它。

1. 该过滤器将显示在已保存过滤器的列表中，并自动应用于引入列。 单击过滤器面板顶部的X可将其关闭。

   ![保存的筛选条件](assets/intake-filter-dialog8.png)

1. （可选）要与其他人共享该过滤器，请将鼠标悬停在保存的过滤器上，单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单图标](assets/more-icon-spectrum.png)，并选择 **[!UICONTROL 共享]**. 在筛选器共享框中选择要与之共享的用户或团队。 有关更多信息，请参阅 [共享筛选器、视图或分组](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. （可选）要在引入列中包含任务和问题，请单击 **[!UICONTROL 筛选源]** 并选择另一个对象以创建另一个滤镜。
1. 添加完筛选器后，查看“摄取”列以验证是否显示正确的任务和问题。

   ![引入列](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >您可以随时更新过滤器，方法是打开“配置”面板，单击 **[!UICONTROL 筛选源]**，并选择 **[!UICONTROL 任务]** 或 **[!UICONTROL 问题]**.

## 使用引入列

在将摄取列中的卡片移动到其他展示板列之前，这些卡片不可编辑。 您可以单击卡以以以只读视图将其打开，或单击 ![未结任务或问题](assets/boards-launch-icon.png) 在新的浏览器选项卡中打开任务或问题。

您可以手动重新排序引入列上的项目。

摄取列右上角的图标会显示列中当前有多少卡片，以及应用了多少过滤器。

1. （可选）要搜索引入列中的项目，请单击 ![“搜索”图标](assets/search-icon.png) 在列中。
1. （可选）要将信息卡从摄取列移动到另一列，请将该信息卡拖放到您希望其显示的位置。

   或

   单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单图标](assets/more-icon-spectrum.png) ，然后选择 **[!UICONTROL 移动]**. 然后，在 **[!UICONTROL 移动项目]** 框中，选择另一列，然后选择 **[!UICONTROL 移动]**.

1. （可选）要删除引入列，请单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单图标](assets/more-icon-spectrum.png) 并选择 **[!UICONTROL 删除]**.


