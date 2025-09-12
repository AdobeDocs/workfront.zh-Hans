---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 管理讨论区管理员视图
description: 讨论区管理员视图包含您的帐户中每个讨论区的列表，系统管理员可以使用它们快速了解讨论区的总体详细信息。
author: Jenny
feature: Agile
source-git-commit: 56263c3f868e7abdaf973c5c03411a2e63ba645d
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 1%

---

# 管理讨论区管理员视图

“展示板管理视图”包含您的帐户中每个展示板的列表，系统管理员可以使用它们快速获取整个展示板详细信息的快照，包括上次更新时间、每个展示板有多少张展示板等等。

在此区域中，您可以执行以下操作：

* 筛选展示板列表
* 配置展示板列表列
* 将讨论区列表分组

## 访问要求

+++ 展开以查看访问要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p>
        <p> 规划 </p></td> 
  </tr> 
    <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>系统管理员 </p>
        </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

您必须先创建一个展示板，然后才能从“管理员视图”中查看该展示板。

有关详细信息，请参阅[创建或编辑展示板](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md)。

## 筛选展示板列表

{{step1-to-boards}}

1. 在&#x200B;**讨论区**&#x200B;页面上，选择&#x200B;**管理员视图**&#x200B;选项卡。

1. 选择&#x200B;**筛选器**。 将打开&#x200B;**筛选器**&#x200B;面板。

1. 请按照以下步骤配置过滤器：

   1. （可选）单击&#x200B;**日历**&#x200B;图标![日历图标](assets/calendar-icon.png)，然后选择一个日期范围，以按该时间范围内最后修改的展示板进行筛选。

   1. （可选）在&#x200B;**模板**部分中，选择列表将按其筛选的展示板模板类型。 您可以选择多个模板类型。
有关展示板模板类型的详细信息，请参阅[创建或编辑展示板](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md)。

   1. （可选）在&#x200B;**Is Archived**&#x200B;部分中，选择是显示已存档还是未存档展示板。 您可以选择多个选项。

      ![是已存档的部分](assets/is-archived-section.png)

1. 单击&#x200B;**筛选器**&#x200B;面板外部以将其关闭。 您的筛选器选择将保留应用于展示板列表，直到它更改回默认视图。

   >[!NOTE]
   >
   >要删除筛选器，请打开&#x200B;**筛选器**&#x200B;面板，然后单击右上角的&#x200B;**返回默认值**。

## 配置展示板列表列

{{step1-to-boards}}

1. 在&#x200B;**讨论区**&#x200B;页面上，选择&#x200B;**管理员视图**&#x200B;选项卡。

1. 选择&#x200B;**列**。 将打开&#x200B;**字段可见性和顺序**&#x200B;面板。

1. 通过选择或取消选择与每列内联的切换开关，配置哪些列显示在“展示板”列表中：

   * **所有者**
   * **上次更新时间**
   * **成员**
   * **已存档**
   * **模板**
   * **卡计数**

1. （可选）要调整字段的显示顺序，请单击并按住字段左侧的&#x200B;**拖动**&#x200B;图标，然后将其拖动到新位置。

   ![单击并拖动](assets/click-and-drag.png)

1. 单击&#x200B;**字段可见性和顺序**&#x200B;面板外部以将其关闭。 您的列配置将保留应用于展示板列表，直到对其进行修改为止。

   >[!NOTE]
   >
   > 修改展示板列表列显示时，**列**&#x200B;图标上方会显示一个蓝色圆点，表示当前视图已从默认视图修改过。

## 按特定字段对讨论区列表进行分组

{{step1-to-boards}}

1. 在&#x200B;**讨论区**&#x200B;页面上，选择&#x200B;**管理员视图**&#x200B;选项卡。

1. 选择&#x200B;**组**。 **Group by**&#x200B;面板打开。

1. 选择您要按下列条件对“展示板”列表进行分组的字段：

   * **已存档**
   * **所有者**
   * **模板**

1. （可选）要展开或折叠&#x200B;**分组依据**&#x200B;面板中的分组，请单击&#x200B;**全部折叠**&#x200B;或&#x200B;**全部展开**。

   ![全部折叠](assets/collapse-all.png)

1. （可选）要将分组的显示顺序从A-Z更改为Z-A，请选择列表当前分组依据的字段，然后从下拉列表中选择&#x200B;**Z-A**。

   ![按顺序显示](assets/display-by-order.png)

1. 单击&#x200B;**分组依据**&#x200B;面板外部以将其关闭。 在此处，通过选择分组标题旁边的箭头，可以折叠或展开列表中应用的分组。

   ![折叠或展开](assets/collapse-or-expand.png)

   >[!NOTE]
   >   
   >修改展示板列表分组显示时，**组**&#x200B;图标上方会显示一个蓝色圆点，表示当前视图不同于默认视图。<br>
   >如果要删除分组，请打开&#x200B;**分组依据**&#x200B;面板，然后选择右上角的&#x200B;**全部清除**。
