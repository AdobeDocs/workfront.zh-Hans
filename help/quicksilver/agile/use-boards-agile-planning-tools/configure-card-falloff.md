---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: 配置卡片衰减
description: 您可以配置展示板，以便按计划存档信息卡或从展示板上删除信息卡。
author: Lisa
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
source-git-commit: 2dfa3e7b215a8234453b2d688031c993978e02ae
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# 配置卡片衰减

您可以配置展示板，以便按计划存档信息卡或“从展示板上流失”。 您可以设置特定列中的信息卡，以便在特定天数或周内从展示板中流失。

当信息卡从展示板上掉下来时，信息卡会被存档。 您可以使用过滤器显示已存档的信息卡。 有关更多信息，请参阅 [在展示板中筛选和搜索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

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
   <td> <p>[!UICONTROL请求]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 配置卡片衰减

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 展示板]**.
1. 访问展示板。 有关信息，请参阅 [创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 单击 **[!UICONTROL 配置]** 打开“配置”面板。
1. 展开 **[!UICONTROL 卡片]**.
1. 打开 **[!UICONTROL 自动将信息卡从展示板存档]**.

   ![卡片衰减设置](assets/card-falloff-switch.png)

1. 选择何时从展示板存档信息卡。 您最多可以选择4周或30天。

   日期由上次修改卡的时间确定。

1. 选择要从中删除卡的列。
1. 单击 **[!UICONTROL 保存]** 确认消息。
1. 单击 **[!UICONTROL 隐藏配置]** 关闭 [!UICONTROL 配置] 的上界。 当您刷新展示板时，将自动应用配置设置。
