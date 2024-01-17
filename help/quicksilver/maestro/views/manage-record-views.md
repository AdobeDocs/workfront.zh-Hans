---
title: 管理记录视图
description: 使用Adobe管理器时，可以在表格或时间线视图中显示记录。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: daa195b0273a232692fe47691a2926579b87ba6b
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 管理记录视图

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>本文中的信息是指AdobeMaestro，它是Adobe Workfront提供的新产品。
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。 您必须是Workfront客户才能使用Maestro功能。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

在Adobe管理器中选择记录类型后，您可以在以下视图中显示该类型的所有记录：

* 表

  有关更多信息，请参阅 [管理表视图](../views/manage-the-table-view.md).
* 时间线

  有关更多信息，请参阅 [管理时间线视图](../views/manage-the-timeline-view.md).

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
<p>贵公司必须注册AdobeMaestro封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
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
   <td> <p>Maestro没有访问级别控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理视图的权限</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">布局模板</td>
   <td> <p>系统管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## 使用Maestro视图时的注意事项

* Maestro中的视图是特定于记录类型的。 不能将同一视图应用于两种不同的记录类型。
* 您创建的视图仅对您以及与您共享这些视图的用户可见。
* 为操作记录类型构建视图与为分类记录类型构建视图相同。
* 当您修改或删除视图时，将会修改该视图，并删除具有该视图权限的所有用户。
* 以下元素对于Maestro中的每个视图都是唯一的：

   * 筛选
   * 分组
   * 排序

  <!-- some of these are not available in all of the views - edit above-->

  例如，在表格视图中创建筛选器时，筛选器结果仅在选定视图中可见，而不在“视图”下拉菜单中列出的所有视图中可见。

  >[!NOTE]
  >
  > 由于Maestro当前处于Beta状态，因此某些视图元素可能不可用于这两个视图。

本文介绍了有关Maestro视图的以下信息：

* [创建和编辑视图](#create-or-edit-record-views)
* [删除视图](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
* [共享视图](#share-a-view)

## 表格视图和时间线视图之间的异同

下表显示了Maestro中的表和时间线视图之间的异同：

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 功能 | 表格视图 | 时间线视图 |
|-----------------------------------------------------------------------|------------|---------------|
| 在列表或表中显示记录 | ✓ {\f13 } |              |
| 默认情况下，将所有字段显示为表中的列 | ✓ {\f13 } |              |
| 隐藏或显示字段（或列） | ✓ {\f13 } |               |
| 编辑每个记录的字段值 | ✓ {\f13 } |               |
| 将记录添加为视图中的新行 | ✓ {\f13 } |               |
| 在视图中添加字段作为新列 | ✓ {\f13 } |               |
| 从外部列表中复制行并将其粘贴到表中 | ✓ {\f13 } |               |
| 在时间轴中显示记录 |            | ✓ {\f13 } |
| 筛选记录 | ✓ {\f13 } | ✓ {\f13 } |
| 组记录 | ✓ {\f13 } | ✓ {\f13 } |
| 排序记录 | ✓ {\f13 } |              |
| 颜色代码记录 |           | ✓ {\f13 } |
| 颜色代码分组 |           | ✓ {\f13 } |
| 搜索特定记录 | ✓ {\f13 } | ✓ {\f13 } |
| 共享视图 | ✓ {\f13 } | ✓ {\f13 } |
| 从视图中打开记录的“详细信息”页面 | ✓ {\f13 } | ✓ {\f13 } |

## 创建或编辑视图 {#create-or-edit-views}

{{step1-to-maestro}}


默认情况下，将打开您上次访问的工作区。 有关创建工作区的信息，请参见 [创建工作区](../architecture/create-workspaces.md).
1. 单击记录类型卡片。 有关创建记录类型的信息，请参阅 [创建记录类型](../architecture/create-record-types.md).

   默认情况下，所选类型的所有记录都会显示在表格视图中。

1. 单击 **视图** 下拉菜单，然后选择现有的 **表格视图** ![](assets/table-view-icon.png) 或单击 **“创建视图”>“表”** 创建表视图

   或

   选择现有 **时间线视图** ![](assets/timeline-view-icon.png) 查看或单击 **“创建视图”>“时间线”** 创建时间线视图。

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    要创建时间线视图，您为其构建视图的记录类型必须至少有两个日期字段。 否则，“时间轴”选项将灰显。

1. （可选）更新视图的名称，然后单击 **创建** 以保存它。

   默认情况下，Maestro将视图命名为“Table &lt; number >”或“Timeline &lt; number >”。 该数字是自动生成的增量。

1. （可选）要在创建视图后重命名视图，请单击视图下拉菜单，然后单击 **更多** 菜单 ![](assets/more-menu.png) > **重命名** 更新视图名称。 <!--ensure there is not another saving step here?!-->
1. （可选）要管理特定类型的视图，请参阅以下文章：

   * [管理表视图](../views/manage-the-table-view.md)
   * [管理时间线视图](../views/manage-the-timeline-view.md)


## 删除视图

{{step1-to-maestro}}

默认情况下，将打开您上次访问的工作区。 有关创建工作区的信息，请参见 [创建工作区](../architecture/create-workspaces.md).

1. 单击记录类型卡片。

   有关创建记录类型的信息，请参阅 [创建记录类型](../architecture/create-record-types.md).

   默认情况下，所选类型的所有记录都会显示在表格视图中。

1. 单击视图下拉菜单，将鼠标悬停在列表中的某个视图上，然后单击 **更多** 菜单 ![](assets/more-menu.png) > **删除**.
1. 单击 **删除** 以确认。 <!--ensure there is not another saving step here?!-->

   该视图将为所有能够访问Maestro区域的用户删除，并且无法恢复。

## 共享视图

有关共享视图的信息，请参阅 [共享视图](/help/quicksilver/maestro/access/share-views.md).

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->
