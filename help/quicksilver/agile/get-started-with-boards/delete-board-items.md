---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 从展示板中删除或存档信息卡
description: 从展示板中删除信息卡时，该信息卡会被永久删除，并且无法恢复。 存档信息卡会将其发送到存档，您可以稍后将其还原到展示板。
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 46099e6ceba4310453743c023823e8952f5ce553
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# 从展示板中删除或存档信息卡

从展示板中删除临时信息卡时，该信息卡会被永久删除，并且无法恢复。 删除已连接的卡后，可以手动将其重新添加到展示板中。

如果从动态展示板中删除已连接的信息卡，则在刷新展示板时，该信息卡会重新显示，因为该展示板类型从特定项目拉入所有任务和问题。 要删除卡，必须从Workfront项目中删除连接的任务或问题。

从任何具有引入列的其他展示板类型中删除已连接信息卡时，如果尚未将已连接任务或问题标记为完成，则在刷新展示板时，该信息卡将重新出现在引入列中。 有关引入列的详细信息，请参阅 [将引入列添加到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

存档信息卡会将其发送到存档，您可以稍后将其还原到展示板。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 从展示板中删除信息卡

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 讨论区]**.
1. 访问展示板。 有关信息，请参阅 [创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 单击 **[!UICONTROL 更多]** 菜单 ![更多菜单](assets/more-icon-spectrum.png) ，然后选择 **[!UICONTROL 删除]**.
1. 单击 **[!UICONTROL 删除]** 确认消息上。

## 存档展示板中的信息卡

1. 访问展示板。
1. 单击 **[!UICONTROL 更多]** 菜单 ![更多菜单](assets/more-icon-spectrum.png) ，然后选择 **[!UICONTROL 存档]**.

   除非应用过滤器来显示已存档的信息卡，否则信息卡会从展示板中隐藏。 有关更多信息，请参阅 [筛选展示板以显示已存档的展示卡](#filter-a-board-to-show-archived-cards) 本文章中。

   An [!UICONTROL 存档] 图标 ![存档](assets/archive-icon-spectrum-25x20.png) 显示在已存档的信息卡上。 您无法编辑已存档的信息卡，但可以将其删除或将其移动到另一列。

1. 要恢复已存档的卡，请单击 **[!UICONTROL 更多]** 菜单 ![更多菜单](assets/more-icon-spectrum.png) ，然后选择 **[!UICONTROL 恢复]**.

## 筛选展示板以显示已存档的展示卡 {#filter-a-board-to-show-archived-cards}

默认情况下，展示板上仅显示活动信息卡。 您可以筛选展示板以显示任何已存档的信息卡。

1. 访问展示板。
1. 单击 [!UICONTROL **配置**] ，打开“配置”面板。
1. 展开 [!UICONTROL **卡片**].
1. 打开 [!UICONTROL **在展示板上显示已存档的卡片**].
1. 单击 [!UICONTROL **筛选**]，展开 [!UICONTROL 已存档信息卡] 部分，然后选择 **[!UICONTROL 已存档的信息卡]** 以显示任何已存档的信息卡。

   该过滤器显示已存档信息卡的数量。

   ![筛选已存档的卡片](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >此 [!UICONTROL 已存档信息卡] 如果您未打开配置设置显示存档的信息卡，则区域在筛选器中不可用。 有关更多信息，请参阅 [自定义信息卡上显示的字段](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. 选择 **[!UICONTROL 已存档的信息卡]** 再次清除选项并仅显示活动信息卡。
