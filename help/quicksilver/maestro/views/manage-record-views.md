---
title: 管理记录视图
description: 使用Adobe Workfront规划时，您可以在表、时间轴或日历视图中显示记录。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 1%

---

# 管理记录视图

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

在Adobe Workfront规划区域中选择记录类型后，您可以在以下视图中显示该类型的所有记录：

* 表

  有关更多信息，请参阅 [管理表视图](../views/manage-the-table-view.md).

* 时间线

  有关更多信息，请参阅 [管理时间线视图](../views/manage-the-timeline-view.md).

* 日历

  有关更多信息，请参阅 [管理日历视图](/help/quicksilver/maestro/views/manage-the-calendar-view.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 产品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵组织必须注册Adobe Workfront计划封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront计划</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">访问级别配置</td>
   <td> <p>Workfront规划没有访问级别控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理视图的权限</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">布局模板</td>
   <td> <p>系统管理员必须在布局模板中添加Planning区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## 使用记录视图时的注意事项

* Workfront Planning中的视图特定于记录类型。 不能将同一视图应用于两种不同的记录类型。
* 您创建的视图仅对您以及与您共享这些视图的用户可见。
* 当您修改或删除视图时，将会修改该视图，并删除具有该视图权限的所有用户。
* 以下元素对于每个记录视图都是唯一的：

   * 筛选
   * 分组
   * 排序

  <!-- some of these are not available in all of the views - edit above-->

  例如，在表格视图中创建筛选器时，筛选器结果仅在选定视图中可见，而不在与记录类型关联的所有视图中可见。

  >[!NOTE]
  >
  > 由于Adobe Workfront规划当前处于测试版状态，因此某些视图元素可能并非对所有视图都可用。

本文介绍了有关记录视图的以下信息：

* [创建和编辑视图](#create-or-edit-record-views)
* [删除视图](#delete-views)
* [复制视图](#duplicate-views)
* [共享视图](#share-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

## 记录视图之间的异同

下表显示了表、时间轴和日历视图之间的异同：

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 功能 | 表格视图 | 时间线视图 | 日历视图 |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| 在列表或表中显示记录 | ✓ {\f13 } |              | |
| 默认情况下，将所有字段显示为表中的列 | ✓ {\f13 } |              |    |
| 隐藏或显示字段（或列） | ✓ {\f13 } |               |    |
| 编辑每个记录的字段值 | ✓ {\f13 } |               |             |
| 将记录添加为视图中的新行 | ✓ {\f13 } |               |        |
| 在视图中添加字段作为新列 | ✓ {\f13 } |               |         |
| 从外部列表中复制行并将其粘贴到表中 | ✓ {\f13 } |               |          |
| 在时间轴中显示记录 |            | ✓ {\f13 } |             |
| 筛选记录 | ✓ {\f13 } | ✓ {\f13 } | ✓ {\f13 } |
| 显示日历中的记录 |           |              | ✓ {\f13 } |
| 组记录 | ✓ {\f13 } | ✓ {\f13 } |
| 排序记录 | ✓ {\f13 } |              |
| 颜色代码记录 |           | ✓ {\f13 } | ✓ {\f13 } |
| 颜色代码分组 |           | ✓ {\f13 } |
| 搜索特定记录 | ✓ {\f13 } | ✓ {\f13 } |
| 共享视图 | ✓ {\f13 } | ✓ {\f13 } | ✓ {\f13 } |
| 从视图中打开记录的“详细信息”页面 | ✓ {\f13 } | ✓ {\f13 } |    |


## 创建或编辑视图 {#create-or-edit-views}

{{step1-to-maestro}}


默认情况下，将打开您上次访问的工作区。 有关创建工作区的信息，请参见 [创建工作区](../architecture/create-workspaces.md).

1. 单击记录类型卡片。 有关创建记录类型的信息，请参阅 [创建记录类型](../architecture/create-record-types.md).

   默认情况下，所选类型的所有记录都会显示在表格视图中。

1. 单击 **+视图** 以添加新视图。
1. 从以下视图类型中选择：

   * 表
   * 时间线
   * 日历

   将使用选定的视图创建新选项卡。

   根据屏幕的宽度，其他视图可能会显示在 **更多** 菜单 ![](assets/more-menu.png).


>[!TIP]
>
>创建记录类型时，缺省情况下还会创建表格视图。
>
>要创建时间轴或日历视图，您为其构建视图的记录类型必须至少有两个日期字段。 否则，“时间轴”和“日历”选项将灰显。
>

![](assets/view-types-drop-down-from-record-type-list.png)

>[!NOTE]
>
>    要创建时间轴或日历视图，您为其构建视图的记录类型必须至少有两个日期字段。 否则，“时间轴”或“日历”选项将灰显。

1. （视情况而定）单击 **下一个**，在创建时间轴或日历视图时。

   默认情况下，Workfront会为视图提供以下名称之一：

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   该数字是自动生成的增量。

1. （视情况而定）选择 **开始** 和 **结束日期** 时间轴或日历视图中显示的记录。
1. 单击 **创建**.

   该视图将显示为新选项卡。 视图会按照其创建或与您共享时的时间顺序显示。
1. （可选）单击 **更多** 菜单 ![](assets/more-caret-down-icon-views.png) 在最后一个视图旁边显示选定记录类型的所有视图。

   其他视图显示在 **更多** “上一视图”选项卡后面的菜单。 旁边的数字 **更多** 菜单显示其他视图的数量。
1. （可选）要在创建视图后重命名视图，请单击视图下拉菜单，然后单击 **更多** 菜单 ![](assets/more-menu.png) > **重命名** 更新视图名称

   或

   双击视图名称并开始键入新名称。  <!--ensure there is not another saving step here?!-->

1. （可选）要管理特定类型的视图，请参阅以下文章：

   * [管理表视图](../views/manage-the-table-view.md)
   * [管理时间线视图](../views/manage-the-timeline-view.md)
   * [管理日历视图](/help/quicksilver/maestro/views/manage-the-calendar-view.md)


## 删除视图

{{step1-to-maestro}}

默认情况下，将打开您上次访问的工作区。 有关创建工作区的信息，请参见 [创建工作区](../architecture/create-workspaces.md).

1. 单击记录类型卡片。

   有关创建记录类型的信息，请参阅 [创建记录类型](../architecture/create-record-types.md).

   默认情况下，所选类型的所有记录都会显示在表格视图中。

1. 将鼠标悬停在视图选项卡中的视图名称上，然后单击 **更多** ![](assets/more-menu.png) 视图名称的左侧，然后单击 **删除**.
首先，您可能需要单击 **更多** ，以查找要删除的视图。

1. 单击 **删除** 以确认。 <!--ensure there is not another saving step here?!-->

   所有有权访问记录区域的用户都将删除该视图，并且无法恢复它。

## 共享视图

有关共享视图的信息，请参阅 [共享视图](/help/quicksilver/maestro/access/share-views.md).

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## 复制视图

如果要保留视图的多个版本，并在这些版本之间进行细微更改，则可以复制视图。

复制视图会创建现有视图的相同副本。

原始视图的共享权限不会转移到复制的视图。

{{step1-to-maestro}}

默认情况下，将打开您上次访问的工作区。

有关创建工作区的信息，请参见 [创建工作区](../architecture/create-workspaces.md).

1. 单击记录类型卡片。 有关创建记录类型的信息，请参阅 [创建记录类型](../architecture/create-record-types.md).

   默认情况下，所选类型的所有记录都会显示在表格视图中。

1. 将鼠标悬停在要复制的视图的选项卡上，然后单击 **更多** 菜单 ![](assets/more-menu.png) 视图名称的右侧，然后单击 **复制**.

   ![](assets/view-more-menu-with-duplicate-option.png)


   视图重复，新视图的名称遵循以下模式： `Original view's name (Copy)`. 新的视图选项卡将显示在所有视图选项卡的末尾。

