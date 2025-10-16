---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: 在工作流展示板上配置积压
description: 您可以选择在工作流中的展示板上显示积压列，并为从工作流卡列表中拉入展示板积压的卡定义查询。
author: Lisa
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 在工作流展示板上配置积压

>[!IMPORTANT]
>
>工作流仅适用于特定的客户组。

您可以选择在工作流中的展示板上显示积压列，并为从工作流卡列表中拉入展示板积压的卡定义查询。

>[!NOTE]
>
>如果您在积压工作列中添加的新信息卡与查询条件不匹配，则当展示板刷新时，信息卡将从积压工作中消失，并且仅在信息卡列表中可用。 您可以随时更改查询以调整哪些卡片显示在积压工作列中。

积压事项列和查询在独立展示板上不可用。 有关将引入列添加到独立展示板的信息，请参阅[将引入列添加到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)。

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

## 在工作流展示板上配置积压

{{step1-to-boards}}

1. 打开要在其中工作的工作流。 要打开工作流，请单击&#x200B;[!UICONTROL **查看工作流**]。
1. 单击工作流中的任意板以将其打开。
1. 单击展示板右侧的&#x200B;[!UICONTROL **配置**]&#x200B;以打开“配置”面板。
1. 打开&#x200B;[!UICONTROL **在此展示板上包括积压事项列**]。

   积压事项列将添加到展示板的左侧。 在将查询应用于它之前，它保持空白。

1. 展开&#x200B;[!UICONTROL **积压查询**]。

   >[!NOTE]
   >
   >默认查询可能已应用于积压，显示卡列表中所有具有状态且状态为“未完成”的工作项。

1. 单击&#x200B;[!UICONTROL **添加条件**]，然后单击“空”字段。
1. 选择要作为查询依据的字段。

   您可以选择的字段是信息卡上的默认字段。

1. 选择查询修改量。

   修饰符选项取决于它们可以应用的字段。 例如，“name”字段不包含“大于”或“小于”作为修饰符选项，因为这些修饰符仅适用于数字。

1. 选择值。

   当您使用“exists”或“not exists”作为修饰符时，该值不可用。

   例如，如果选择“到期日”和“存在”，则积压将显示已分配到期日的卡片。 任何没有到期日期的信息卡都不会被拉入积压。

1. （可选）单击&#x200B;[!UICONTROL **添加条件**]&#x200B;以向查询中添加其他条件。

   ![积压查询](assets/backlog-query-wrkstrm-board.png)

1. （可选）单击&#x200B;[!UICONTROL **创建组**]&#x200B;以添加一组使用OR运算符连接到第一个条件的条件。
1. 单击&#x200B;[!UICONTROL **保存查询**]。

   这将应用查询，并且符合条件的卡片将显示在积压列中。
