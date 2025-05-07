---
title: 管理记录视图
description: 使用Adobe Workfront Planning时，您可以在表、时间轴或日历视图中显示记录。 本文介绍了如何创建视图以及编辑或删除现有视图。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 3dfac5ada17248f5c67380b56b9a0969b10b73e6
workflow-type: tm+mt
source-wordcount: '1537'
ht-degree: 1%

---


# 管理记录视图

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

在Adobe Workfront Planning区域中选择记录类型后，您可以在以下视图中显示该类型的所有记录：

* 表

  有关详细信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

* 时间线

  有关详细信息，请参阅[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

* 日程表

  有关详细信息，请参阅[管理日历视图](/help/quicksilver/planning/views/manage-the-calendar-view.md)。

本文介绍了有关记录视图的以下信息：

* [创建和编辑视图](#create-or-edit-record-views)
* [删除视图](#delete-views)
* [复制视图](#duplicate-views)
* [在视图中启用实时状态指示器](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


## 访问要求

+++ 展开以查看访问要求。

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront规划<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
<p>以下任意Workfront计划：</p> 
<ul><li>选择</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning不适用于旧版Workfront计划</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入Adobe Unified Experience，才能访问Workfront Planning的所有功能。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准 </p>
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理视图的权限</p>  
   <p>查看对视图的权限以临时更改视图设置或复制它</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面模板</p></td> 
   <td> <p>在生产环境中，必须将所有用户（包括系统管理员）分配到包含Planning的布局模板。</p>
<p><span class="preview">在“预览”环境中，标准用户和系统管理员默认启用Planning。</span></p></td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用记录视图时的注意事项

* Workfront Planning中的视图特定于记录类型。 不能将同一视图应用于两种不同的记录类型。
* 您创建的视图仅对您以及与您共享这些视图的用户可见。
* 当您修改或删除视图时，将会修改该视图，并删除具有该视图权限的所有用户。
* 每个用户最多可创建100个视图。 您可以为记录类型显示100多个视图，但一个用户只能创建100个视图。
* 您可以与其他人共享您创建的视图。 有关信息，请参阅[共享视图](/help/quicksilver/planning/access/share-views.md)。
* 以下元素对于每个记录视图都是唯一的：

   * 筛选条件
   * 分组
   * 排序
   * 条形图外观（用于时间轴视图）

  <!-- some of these are not available in all of the views - edit above-->

  例如，在表格视图中创建筛选器时，筛选器结果仅在选定视图中可见，而不在与记录类型关联的所有视图中可见。

  >[!NOTE]
  >
  > 某些视图元素可能并非对所有视图都可用。


## 记录视图之间的异同

下表显示了表、时间轴和日历视图之间的异同：

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 功能 | 表格视图 | 时间线视图 | 日历视图 |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| 在列表或表中显示记录 | ✓ |              | |
| 默认情况下，将所有字段显示为表中的列 | ✓ |              |    |
| 隐藏或显示字段（或列） | ✓ |               |    |
| 编辑每个记录的字段值 | ✓ |               |             |
| 将记录添加为视图中的新行 | ✓ |               |        |
| 在视图中添加字段作为新列 | ✓ |               |         |
| 从外部列表中复制行并将其粘贴到表中 | ✓ |               |          |
| 在时间轴中显示记录 |            | ✓ |             |
| 筛选记录 | ✓ | ✓ | ✓ |
| 显示日历中的记录 |           |              | ✓ |
| 组记录 | ✓ | ✓ |
| 排序记录 | ✓ |              |
| 颜色代码记录 |           | ✓ | ✓ |
| 颜色代码分组 |           | ✓ |
| 搜索特定记录 | ✓ | ✓ |
| 与他人共享视图 | ✓ | ✓ | ✓ |
| 从视图打开记录的页面 | ✓ | ✓ |    |
| 按年份和季度显示记录 |           | ✓ |    |
| 按月显示记录 |           | ✓ | ✓ |
| 按周显示记录 |           |               | ✓ |


## 创建或编辑视图 {#create-or-edit-views}

{{step1-to-planning}}


1. 单击工作区的卡片。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。

   默认情况下，所选类型的所有记录都会显示在表格视图中。

1. 单击&#x200B;**+视图**&#x200B;以添加新视图。
1. 从以下视图类型中选择：

   * 表
   * 时间线
   * 日程表

   将使用选定的视图创建新选项卡。

   根据屏幕的宽度，**更多**&#x200B;菜单![更多](assets/more-menu.png)中可能会显示其他视图。


>[!TIP]
>
>创建记录类型时，缺省情况下还会创建表格视图。
>
>要创建时间轴或日历视图，您为其构建视图的记录类型必须至少有两个日期字段。
>
>否则，“时间轴”和“日历”选项将灰显。
>

![记录类型列表中的查看类型下拉列表](assets/view-types-drop-down-from-record-type-list.png)

1. （视情况而定）创建时间线或日历视图时，单击&#x200B;**下一步**。

   默认情况下，Workfront会为视图提供以下名称之一：

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   该数字是自动生成的增量。

1. （视情况而定）为将在时间轴或日历视图中显示的记录选择&#x200B;**开始**&#x200B;和&#x200B;**结束日期**。

   >[!TIP]
   >
   >    您可以从记录日期字段中选择，或从连接的记录或对象类型中选择查找日期字段。 当您选择查找字段作为时间轴和日历视图的开始和结束日期时，必须为日期字段(MAX或MIN)使用聚合器。 有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

1. 单击&#x200B;**创建**。

   该视图将显示为新选项卡。 视图会按照其创建或与您共享时的时间顺序显示。
1. （可选）单击最后一个视图旁边的&#x200B;**更多**&#x200B;菜单![更多向下插入符号图标视图](assets/more-caret-down-icon-views.png)以显示所选记录类型的所有视图。

   其他视图显示在最后一个视图选项卡之后的&#x200B;**更多**&#x200B;菜单下。 **更多**&#x200B;菜单旁边的数字显示其他视图的数量。
1. （可选）要在创建视图后重命名视图，请单击“视图”下拉菜单，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png) > **重命名**&#x200B;以更新视图名称

   或

   双击视图名称并开始键入新名称。 <!--ensure there is not another saving step here?!-->

1. （可选）要管理特定类型的视图，请参阅以下文章：

   * [管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [管理日历视图](/help/quicksilver/planning/views/manage-the-calendar-view.md)


## 删除视图

{{step1-to-planning}}

1. 单击工作区的卡片。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。

   默认情况下，所选类型的所有记录都会显示在表格视图中。

1. 将鼠标悬停在视图选项卡中的某个视图名称上，然后单击视图名称左侧的&#x200B;**更多** ![更多菜单](assets/more-menu.png)，然后单击&#x200B;**删除**。
首先，您可能需要单击最后一个选项卡左侧的&#x200B;**更多**&#x200B;以查找要删除的视图。

1. 单击&#x200B;**删除**&#x200B;以确认。<!--ensure there is not another saving step here?!-->

   所有有权访问记录区域的用户都将删除该视图，并且无法恢复它。

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## 复制视图

如果要保留视图的多个版本，并在这些版本之间进行细微更改，则可以复制视图。

复制视图会创建现有视图的相同副本。

原始视图的共享权限不会转移到复制的视图。

{{step1-to-planning}}

1. 单击工作区的卡片。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。
默认情况下，所选类型的所有记录都会显示在表格视图中。

1. 将鼠标悬停在要复制的视图的选项卡上，单击视图名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**复制**。

   ![查看包含重复选项的更多菜单](assets/view-more-menu-with-duplicate-option.png)


   视图重复，新视图的名称遵循以下模式： `Original view's name (Copy)`。 新的视图选项卡将显示在所有视图选项卡的末尾。

## 在视图中启用实时显示状态指示器

默认情况下，与编辑记录信息的其他用户头像将显示在所有记录视图的右上角。

显示表格视图时，还可以查看查看查看记录时其他用户正在编辑的字段。

1. 转到记录类型页面并打开任意视图。
1. （视情况而定）如果同时有其他用户编辑所选类型的记录，则其头像将显示在视图的右上角。
1. 单击头像旁边的下拉菜单，然后选择&#x200B;**显示协作者**&#x200B;切换开关。 默认情况下，该切换处于选中状态。

   ![显示协作者切换选定项](assets/show-collaborators-toggle-selected.png)

1. （视情况而定）打开表格视图，另一个人正在主动编辑的字段会以对应于表格视图中其头像轮廓的颜色突出显示。

   如果头像的高亮颜色为灰色，则用户在30秒前停止了主动编辑记录。

   ![实时指示器表字段和头像连接](assets/real-time-indicator-table-field-and-avatar-connection.png)

   >[!TIP]
   >
   >您可以从任何视图中选择&#x200B;**显示协作者**&#x200B;切换开关。 他人当前编辑的字段仅在表格视图中列出。
