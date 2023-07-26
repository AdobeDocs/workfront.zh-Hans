---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: 配置信息卡减少
description: 您可以配置展示板，以便按计划存档信息卡或使其从展示板上脱落。
author: Lisa
feature: Agile
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# 配置信息卡减少

您可以配置展示板，以便按计划存档信息卡，或使信息卡“从展示板中流失”。 您可以在特定列中设置卡片，以使其在特定天数或几周内从展示板中流失。

当卡从板上掉落时，将其存档。 您可以显示带有过滤器的存档信息卡。 有关更多信息，请参阅 [在展示板中过滤和搜索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

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
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 配置信息卡减少

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 讨论区]**.
1. 访问展示板。 有关信息，请参阅 [创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 单击 **[!UICONTROL 配置]** ，打开“配置”面板。
1. 展开 **[!UICONTROL 卡片]**.
1. 打开 **[!UICONTROL 自动从展示板中存档卡片]**.

   ![卡片回退设置](assets/card-falloff-switch.png)

1. 选择何时从展示板中存档卡片。 您最多可以选择8周或60天。

   日期由上次修改信息卡的时间确定。

1. 选择要从中删除卡片的列。
1. 单击 **[!UICONTROL 保存]** 确认消息上。
1. 单击 **[!UICONTROL 隐藏配置]** 关闭 [!UICONTROL 配置] 面板。 当您刷新主板时，配置设置会自动应用。
