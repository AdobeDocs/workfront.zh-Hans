---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 在展示板中过滤和搜索
description: 您可以筛选展示板以仅显示某些信息卡。
author: Lisa
feature: Agile
exl-id: 26abce82-dcd9-4865-96f4-c710f7f0a0d8
source-git-commit: 55d47665ca53c63142d5b71830fe56a05d991c74
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# 在展示板中过滤和搜索

您可以筛选要显示的展示板：

* 分配给特定人员的卡片
* 带有特定标记的卡片
* 具有特定状态的卡片
* 在特定时间范围内到期的卡片
* 已存档的信息卡
* 连接到特定项目的信息卡

对展示板进行排序，可排列列中的所有卡片。 您不能对单个列进行排序，积压或引入列也不会进行排序。

搜索还可帮助您在展示板上查找特定信息卡。

应用过滤器后，展示板上会显示一个指示器 ![应用于展示板的筛选器](assets/boards-filterapplied-30x30.png). 单击 **[!UICONTROL 全部清除]** 以从展示板中删除所有筛选器，然后单击折叠图标以关闭筛选器面板。

![过滤器面板](assets/boards-all-filters-collapsed-0823.png)

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

## 按被分派人筛选讨论区

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 讨论区]**.
1. 访问展示板。 有关信息，请参阅 [创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 单击 [!UICONTROL **筛选**]，展开 [!UICONTROL 成员] 部分，然后选择要查看其卡片的一个或多个人员。 您还可以显示未分配的卡片。

   ![按成员筛选](assets/boards-filter-by-assignees-0822.png)

## 按标记筛选展示板

1. 访问展示板。
1. 单击 [!UICONTROL **筛选**]，展开 [!UICONTROL 标记] 部分，然后选择要查看的标记。

   ![按标记筛选](assets/boards-filter-by-tags-0822.png)

## 按状态筛选讨论区

1. 访问展示板。
1. 单击 [!UICONTROL **筛选**]，展开 [!UICONTROL 状态] 部分，然后选择要查看的状态类型。

   您还可以隐藏已完成的卡片。

   ![按状态筛选](assets/boards-filter-by-status-0822.png)

## 按到期日期筛选讨论区

1. 访问展示板。
1. 单击 [!UICONTROL **筛选**]，展开 [!UICONTROL 到期日期] 部分，然后选择要查看的日期选项。

   仅显示选定日期范围内的卡片。

   ![按到期日期筛选](assets/boards-filter-by-due-date-0822.png)

## 筛选展示板以显示已存档的展示卡

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
   >此 [!UICONTROL 已存档信息卡] 如果您未打开配置设置显示存档的信息卡，则区域在筛选器中不可用。

1. 选择 **[!UICONTROL 已存档的信息卡]** 再次清除选项并仅显示活动信息卡。

## 按连接过滤展示板

1. 访问展示板。
1. 单击 [!UICONTROL **筛选**]，展开 [!UICONTROL 连接] 部分，然后选择 [!DNL Workfront] 您希望查看的已连接信息卡项目。

   您还可以显示未连接到项目的信息卡。

   ![按连接筛选](assets/boards-filter-by-connection.png)

## 在展示板上排序

当您选择排序依据的选项时，所有列都会被排序。 您不能对单个列进行排序，积压或引入列也不会进行排序。

1. 访问展示板。
1. 单击 [!UICONTROL **排序方式**] 并选择 [!UICONTROL **名称**]， [!UICONTROL **到期日期**]， [!UICONTROL **估计**]， [!UICONTROL **状态**]，或 [!UICONTROL **连接**].

   连接（项目名称）仅适用于连接的卡片，而其他选项将对列中的连接卡片和临时卡片进行排序。

   “用户顺序”选项会将卡片返回到手动设置的顺序，然后再应用任何其他排序选项。 这是列的默认排序。

1. 选择 [!UICONTROL **逆序**] 以按排序选项的反向顺序对列进行排序。

   排序图标上的箭头指示列是按升序还是降序排序。

   应用默认排序以外的排序时，排序图标上会显示指示符 ![应用的排序](assets/sort-applied-boards.png).

   ![按展示板上的列排序](assets/sort-by-columns-in-board.png)

## 在讨论区中搜索

1. 访问展示板。
1. 单击 [!UICONTROL **Search**] 并键入搜索词。 然后，按Enter。

   将显示包含搜索词的所有卡片。

   单击X清除搜索。

   ![在展示板中搜索卡片](assets/boards-searchbox.png)
