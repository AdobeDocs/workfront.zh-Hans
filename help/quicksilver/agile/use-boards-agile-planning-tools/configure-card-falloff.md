---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: 配置卡衰减
description: 您可以配置讨论区，以便卡片可以按计划存档，或从讨论区中退出。
author: Courtney
feature: Agile
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 7%

---

# 配置卡衰减

您可以配置一个讨论区，以便按照计划对讨论区进行归档或“流失”。 您可以在特定列中设置卡片，使其在特定天数或周内从讨论区中消失。

卡从主板上掉落时，就会被存档。 您可以使用筛选器显示存档的卡片。 有关详细信息，请参阅[在讨论区中筛选和搜索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>投稿人或更高版本</p> 
   <p>请求或更高版本</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关此表中的信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置卡衰减

{{step1-to-boards}}

1. 访问讨论区。 有关信息，请参阅[创建或编辑讨论区](../../agile/get-started-with-boards/create-edit-board.md)。
1. 单击讨论区右侧的&#x200B;**[!UICONTROL “配置”]**&#x200B;以打开“配置”面板。
1. 展开&#x200B;**[!UICONTROL 卡]**。
1. 打开&#x200B;**[!UICONTROL 自动从讨论区存档卡片]**。

   ![卡片衰减设置](assets/card-falloff-switch.png)

1. 选择何时从主板存档卡。 您最多可以选择8周或60天。

   日期由卡的上次修改时间确定。

1. 选择要从哪一列中删除卡。
1. 单击确认消息上的&#x200B;**[!UICONTROL “保存”]**。
1. 单击&#x200B;**[!UICONTROL 隐藏配置]**&#x200B;以关闭[!UICONTROL 配置]面板。 当您刷新主板时，配置设置会自动应用。
