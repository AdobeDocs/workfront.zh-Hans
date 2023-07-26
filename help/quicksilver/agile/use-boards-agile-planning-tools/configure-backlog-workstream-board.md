---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: 在工作流展示板上配置积压
description: 您可以选择在工作流中的展示板上显示积压列，并为从工作流卡列表中拉入展示板积压的卡定义查询。
author: Lisa
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# 在工作流展示板上配置积压

您可以选择在工作流中的展示板上显示积压列，并为从工作流卡列表中拉入展示板积压的卡定义查询。

>[!NOTE]
>
>如果您在积压工作列中添加的新信息卡与查询条件不匹配，则当展示板刷新时，信息卡将从积压工作中消失，并且仅在信息卡列表中可用。 您可以随时更改查询以调整哪些卡片显示在积压工作列中。

积压事项列和查询在独立展示板上不可用。 有关将引入列添加到独立展示板的信息，请参见 [将引入列添加到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

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

## 在工作流展示板上配置积压

{{step1-to-boards}}

1. 打开要在其中工作的工作流。 要打开工作流，请单击 [!UICONTROL **查看工作流**].
1. 单击工作流中的任意板以将其打开。
1. 单击 [!UICONTROL **配置**] ，打开“配置”面板。
1. 打开 [!UICONTROL **在此讨论区中包含积压事项列**].

   积压事项列将添加到展示板的左侧。 在将查询应用于它之前，它保持空白。

1. 展开 [!UICONTROL **积压查询**].

   >[!NOTE]
   >
   >默认查询可能已应用于积压，显示卡列表中所有具有状态且状态为“未完成”的工作项。

1. 单击 [!UICONTROL **添加条件**] 然后单击“空”字段。
1. 选择要作为查询依据的字段。

   您可以选择的字段是信息卡上的默认字段。

1. 选择查询修改量。

   修饰符选项取决于它们可以应用的字段。 例如，“name”字段不包含“大于”或“小于”作为修饰符选项，因为这些修饰符仅适用于数字。

1. 选择值。

   当您使用“exists”或“not exists”作为修饰符时，该值不可用。

   例如，如果选择“到期日”和“存在”，则积压将显示已分配到期日的卡片。 任何没有到期日期的信息卡都不会被拉入积压。

1. （可选）单击 [!UICONTROL **添加条件**] 以向查询中添加其他条件。

   ![积压查询](assets/backlog-query-wrkstrm-board.png)

1. （可选）单击 [!UICONTROL **创建组**] 添加一组使用OR运算符连接到第一个条件的条件。
1. 单击 [!UICONTROL **保存查询**].

   这将应用查询，并且符合条件的卡片将显示在积压列中。
