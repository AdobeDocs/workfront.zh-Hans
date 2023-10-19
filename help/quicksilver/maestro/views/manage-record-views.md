---
title: 管理记录视图
description: 使用Adobe管理器时，可以在表格或时间线视图中显示记录。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 89d590551ffbd23b357f5697163fa56651f294fb
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 1%

---

# 管理记录视图

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>本文中的信息是指AdobeMaestro，它是Adobe公司推出的新产品。
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。
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
   <p> Adobe产品</p> </td>
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
   <td role="rowheader">访问级别</td>
   <td> <p>任何</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">布局模板</td>
   <td> <p>系统管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/grant-access.md">授予对Adobe大师的访问权限</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 使用Maestro视图时的注意事项

* Maestro中的视图是特定于记录类型的。 不能将同一视图应用于两种不同的记录类型。
* 您创建的视图对访问Maestro区域的每个人都可见。 <!-- edit this when we have permissions and the views will be shared only to be visible by others-->
  <!-- this is not yet possible: * You can share views with others if you want them to also apply them to the same record types.-->
* 为操作记录类型构建视图与为分类记录类型构建视图相同。
* 修改或删除视图时，将修改和删除所有可访问Maestro区域的用户。
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
  <!--* [Share a view](#share-views) - not possible yet-->

## 表格视图和时间线视图之间的异同

下表显示了Maestro中的表和时间线视图之间的异同：

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 功能 | 表格视图 | 时间线视图 |
|-----------------------------------------------------------------------|------------|---------------|
| 在列表或表中显示记录 | ✓ {\f13 } |              |
| 默认情况下，将所有字段显示为表中的列 | ✓ |              |
| 隐藏或显示字段（或列） | ✓ |               |
| 编辑每个记录的字段值 | ✓ |               |
| 将记录添加为视图中的新行 | ✓ |               |
| 在视图中添加字段作为新列 | ✓ |               |
| 从外部列表中复制行并将其粘贴到表中 | ✓ |               |
| 在时间轴中显示记录 |            | ✓ |
| 筛选记录 | ✓ | ✓ |
| 组记录 |           | ✓ |
| 排序记录 | ✓ |              |
| 颜色代码记录 |           | ✓ |
| 颜色代码分组 |           | ✓ |

<!--| Sort groupings                                                        | ✓          | ✓             |-->
<!--| Display a limited number of fields as columns, by default                      | ✓          |               |-->

## 创建或编辑视图 {#create-or-edit-views}

1. 单击 **主菜单** 图标 ![](assets/main-menu-workfront.png) 在右上角 <!--or the **Main Menu** icon ![](assets/main-menu-shell.png) in the upper-left corner, if available-->，然后单击 **大师** ![](assets/maestro-icon.png).
默认情况下，将打开您上次访问的工作区。 有关创建工作区的信息，请参见 [创建工作区](../architecture-and-fields/create-workspaces.md).
1. 单击记录类型卡片。 有关创建记录类型的信息，请参阅 [创建记录类型](../architecture-and-fields/create-record-types.md).

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
1. （可选）要管理视图，请参阅以下文章以了解更多信息：

   * [管理表视图](../views/manage-the-table-view.md)
   * [管理时间线视图](../views/manage-the-timeline-view.md)


<!--# Add a view as a favorite - this is not possible yet-->

<!-- ## Share views - not possible yet-->

## 删除视图

1. 从 **主菜单** ![](assets/main-menu-workfront.png) 在屏幕的右上角， <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner of the screen, if available,--> 单击 **大师** ![](assets/maestro-icon.png).

   默认情况下，将打开您上次访问的工作区。 有关创建工作区的信息，请参见 [创建工作区](../architecture-and-fields/create-workspaces.md).
1. 单击记录类型卡片。

   有关创建记录类型的信息，请参阅 [创建记录类型](../architecture-and-fields/create-record-types.md).

   默认情况下，所选类型的所有记录都会显示在表格视图中。

1. 单击视图下拉菜单，将鼠标悬停在列表中的某个视图上，然后单击 **更多** 菜单 ![](assets/more-menu.png) > **删除**.
1. 单击 **删除** 以确认。 <!--ensure there is not another saving step here?!-->

   该视图将为所有能够访问Maestro区域的用户删除，并且无法恢复。

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture-and-fields/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture-and-fields/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->
