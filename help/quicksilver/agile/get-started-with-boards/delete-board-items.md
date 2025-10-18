---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 从展示板中删除或存档信息卡
description: 从展示板中删除信息卡时，该信息卡会被永久删除，并且无法恢复。 存档信息卡会将其发送到存档，您可以稍后将其还原到展示板。
author: Jenny
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# 从展示板中删除或存档信息卡

从展示板中删除临时信息卡时，该信息卡会被永久删除，并且无法恢复。 删除已连接的卡后，可以手动将其重新添加到展示板中。

如果从动态展示板中删除已连接的信息卡，则在刷新展示板时，该信息卡会重新显示，因为该展示板类型从特定项目拉入所有任务和问题。 要删除卡，必须从Workfront项目中删除连接的任务或问题。

从任何具有引入列的其他展示板类型中删除已连接信息卡时，如果尚未将已连接任务或问题标记为完成，则在刷新展示板时，该信息卡将重新出现在引入列中。 有关引入列的详细信息，请参阅[将引入列添加到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)。

存档信息卡会将其发送到存档，您可以稍后将其还原到展示板。

已存档的信息卡不会同步到Workfront任务和问题。 如果您还原一张卡，它将再次同步。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>参与者或更高版本</p> 
   <p>请求或更高版本</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 从展示板中删除信息卡

{{step1-to-boards}}

1. 访问展示板。 有关信息，请参阅[创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md)。
1. 单击卡片上的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单![更多菜单](assets/more-icon-spectrum.png)，然后选择&#x200B;**[!UICONTROL 删除]**。
1. 单击确认消息上的&#x200B;**[!UICONTROL 删除]**。

## 存档展示板中的信息卡

1. 访问展示板。
1. 单击卡片上的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单![更多菜单](assets/more-icon-spectrum.png)，然后选择&#x200B;**[!UICONTROL 存档]**。

   除非应用过滤器来显示已存档的信息卡，否则信息卡会从展示板中隐藏。 有关详细信息，请参阅本文中的[筛选展示板以显示已存档的卡片](#filter-a-board-to-show-archived-cards)。

   已存档的卡片上出现[!UICONTROL 存档]图标![存档](assets/archive-icon-spectrum-25x20.png)。 您无法编辑已存档的信息卡，但可以将其删除或将其移动到另一列。

1. 若要还原已存档的卡，请单击卡上的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单![更多](assets/more-icon-spectrum.png)，然后选择&#x200B;**[!UICONTROL 还原]**。

## 筛选展示板以显示已存档的展示卡

默认情况下，展示板上仅显示活动信息卡。 您可以筛选展示板以显示任何已存档的信息卡。

1. 访问展示板。
1. 单击展示板右侧的&#x200B;[!UICONTROL **配置**]&#x200B;以打开“配置”面板。
1. 展开&#x200B;[!UICONTROL **卡片**]。
1. 打开&#x200B;[!UICONTROL **在展示板上显示已存档的卡片**]。
1. 单击&#x200B;[!UICONTROL **筛选器**]，展开[!UICONTROL 已存档信息卡]部分，然后选择&#x200B;**[!UICONTROL 已存档信息卡]**&#x200B;以显示任何已存档的信息卡。

   该过滤器显示已存档信息卡的数量。

   ![筛选已存档的卡片](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >如果未打开配置设置以显示已存档的信息卡，则筛选器中无法使用[!UICONTROL 已存档的信息卡]部分。 有关详细信息，请参阅[自定义卡片上显示的字段](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md)。

1. 再次选择&#x200B;**[!UICONTROL 已存档信息卡]**&#x200B;以清除该选项并仅显示活动信息卡。
