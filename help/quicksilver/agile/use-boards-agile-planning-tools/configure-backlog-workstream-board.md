---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: 在工作流板上配置积压
description: 您可以选择在工作流中的展示板上显示积压工作列，并为从工作流卡片列表中提取到展示板积压工作的卡片定义查询。
author: Lisa
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 75bb5af9564947a39e1cb46f9d6be2c03eb07acc
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 在工作流板上配置积压

您可以选择在工作流中的展示板上显示积压工作列，并为从工作流卡片列表中提取到展示板积压工作的卡片定义查询。 这些选项在独立主板上不可用。 有关向独立展示板添加进气列的信息，请参阅 [向展示板添加进气柱](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

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

## 在工作流板上配置积压

{{step1-to-boards}}

1. 打开要在其中工作的工作流。 要打开工作流，请单击 [!UICONTROL **查看工作流**].
1. 单击工作流中的任意展示板以将其打开。
1. 单击 [!UICONTROL **配置**] 打开“配置”面板。
1. 打开 [!UICONTROL **在此展示板上包含积压工作列**].

   积压工作列将添加在展示板左侧。 在您对查询应用查询之前，该查询将保留为空。

1. 展开 [!UICONTROL **积压查询**].

   >[!NOTE]
   >
   >默认查询可能已应用于积压工作，显示卡列表中不属于小版本且处于“完成”状态的所有工作项。

1. 单击 [!UICONTROL **添加条件**] ，然后单击“empty”字段。
1. 选择要查询的字段。

   您可以从中选择的字段是信息卡上的默认字段。

1. 选择查询修饰符。

   修饰符选项取决于可应用到的字段。 例如，“name”字段没有“大于”或“小于”作为修饰符选项，因为这些修饰符仅适用于数字。

1. 选择值。

   当您使用“存在”或“不存在”作为修饰符时，该值不可用。

   例如，如果选择“到期日期”和“存在”，积压工作将显示已分配到期日期的卡片。 任何没有到期日期的卡都不会被提取到积压工作中。

1. （可选）单击 [!UICONTROL **添加条件**] 以向查询添加其他条件。

   ![积压查询](assets/backlog-query-wrkstrm-board.png)

1. （可选）单击 [!UICONTROL **创建组**] 添加一组条件，这些条件用OR运算符连接到第一个条件。
1. 单击 [!UICONTROL **保存查询**].

   将应用查询，并且符合标准的卡会显示在积压工作列中。
