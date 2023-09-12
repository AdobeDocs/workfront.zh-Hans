---
title: 创建记录类型
description: 记录类型是AdobeMaestro的对象类型。 在Maestro中，您可以创建自定义记录类型，以说明在组织的生命周期中所需的工作项。
hidefromtoc: true
hide: true
source-git-commit: 6e219089f68db651f5eb8369e3c6df83b6cd823b
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# 创建记录类型

>[!IMPORTANT]
>
>目前，AdobeMaestro是封闭测试版计划的一部分，该计划对有限数量的客户开放。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

记录类型是AdobeMaestro的对象类型。 在Maestro中，您可以创建自定义记录类型，以说明在组织的生命周期中所需的工作相关项目。

记录类型可以是以下任一类型：

* **操作记录类型**
* **分类标准**

有关Maestro记录类型的详细信息，请参阅 [记录类型和分类概述](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

创建操作记录类型与创建分类记录类型类似。 本文介绍了如何创建操作记录类型。

有关创建分类的信息，请参阅 [创建分类记录类型](../architecture-and-fields/create-a-taxonomy.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 <tbody>
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

## 有关创建记录类型的注意事项

* 通过执行以下操作之一，可在工作区中创建记录类型：

   * 自动:
      * 使用模板创建工作区时。

        有关信息，请参阅 [创建工作区](../architecture-and-fields/create-workspaces.md).
      * 当您使用Excel或CSV文件导入它们时。 这不适用于分类记录类型。
      * 从另一个应用程序创建与对象类型的连接时，向记录类型添加字段时。 这会在Maestro中创建只读记录类型，该记录类型连接到原始应用程序中的对象类型。 这不适用于分类记录类型。

     有关连接对象类型与Maestro记录的信息，请参见 [连接记录](../records/connect-records.md).
   * 手动:

      * 从头开始.

## 使用工作区模板创建记录类型

在使用模板创建工作区时，您可以自动创建记录类型。 每个Maestro模板都包含示例操作和分类记录类型。

有关创建工作区的信息，请参见 [创建工作区](../architecture-and-fields/create-workspaces.md).

有关每个模板中包含的记录类型的信息，请参阅 [工作区模板列表](../architecture-and-fields/workspace-templates.md).

## 从头开始创建记录类型

本文介绍了如何从头开始创建操作记录类型。 从头开始创建操作记录类型与创建分类类似。

有关分类的详细信息，请参阅 [创建分类](../architecture-and-fields/create-a-taxonomy.md).

1. 单击 **主菜单** 图标 ![](assets/main-menu-workfront.png) 在Workfront的右上角， <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 然后单击 **大师** ![](assets/maestro-icon.png).

   默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要为其创建记录类型的工作区。
1. 单击 **添加记录类型**.
1. （视情况而定）如果要创建操作记录类型，请单击 **从头开始**. 创建分类时，此选项不可用。

   将打开“添加记录类型”框。

   ![](assets/add-record-type-box-with-appearance-options.png)

1. 选择以下信息：

   * **记录名称**：将“无标题的操作记录类型”替换为您未来记录类型的名称。 <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **外观**：定义与记录类型关联的图标的颜色和形状。 执行以下操作：
      * 选择用于标识新记录类型的颜色。 这是记录类型图标的颜色。 默认情况下选中“灰色”。
      * 从列表中选择一个图标，或开始键入图标的名称以描述其表示的内容，然后在显示时选择它。 这是记录类型的图标。 默认情况下，会选择一个文件图标。

1. 在 **添加记录类型** 框以保存记录。

   记录类型信息卡会添加到您选择的工作区。
记录类型包含的信息卡上显示的字段数。
1. （可选）单击记录类型卡以打开记录类型页面。

   ![](assets/operational-record-type-blank.png)

   默认情况下，记录类型页面显示在“表”视图中。 表的列是与新记录类型关联的字段。 每一行都是您必须添加的唯一记录。

   默认情况下，以下字段显示在操作记录类型的表视图列中：

   * 名称

     “名称”字段是唯一自动为分类创建的字段。
   * 描述
   * 开始日期
   * 结束日期
   * 状态

1. （可选）更新页面标题中的记录类型名称

   或

   单击 **更多** 图标 ![](assets/more-menu.png) 记录类型名称的右侧，然后单击 **重命名** 以对其进行重命名。

1. （可选）单击 **+新建&lt;记录类型名称>** 以添加所选记录类型的记录。 有关更多信息，请参阅 [创建记录](../records/create-records.md).
1. （可选）单击 **+** 图标来添加更多字段到记录类型。 有关更多信息，请参阅 [创建字段](../architecture-and-fields/create-fields.md).
1. （可选）单击记录类型名称左侧的左箭头，以返回选定的工作区。

   记录类型卡显示记录类型包含的字段数和连接数。

   ![](assets/campaign-card-with-fields-and-connections-highlighted.png)

   有关在记录类型页面中添加记录、删除或编辑记录类型或更新视图的其他信息，请参阅以下文章：

   * [创建记录](../records/create-records.md)
   * [删除记录类型](../architecture-and-fields/delete-record-types.md)
   * [编辑记录类型](../architecture-and-fields/edit-record-types.md)
   * [在Adobe大师中管理记录视图](../views/manage-record-views.md) <!--add information here about the sorting and grouping when available-->

## 通过导入Excel或CSV文件创建记录类型

使用Excel或CSV文件导入记录类型时，请考虑以下事项：

* 在Maestro中，Excel文件的每一页都成为记录类型。
* 每个工作表的列将成为与每个记录类型关联的字段。
* 字段对于其各自的记录类型是唯一的。
* 每个工作表中的每一行都成为与其各自记录类型相关联的唯一记录。
* Excel文件的每一页不应超过以下内容：
   * 10,000行
   * 500列
* Excel文件不应大于5MB。
* 不支持空工作表。

要使用Excel文件导入记录类型，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-workfront.png) 在Workfront的右上角， <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 然后单击 **大师** ![](assets/maestro-icon.png).

   默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要为其创建记录类型的工作区。
1. 单击 **添加记录类型**.
1. （视情况而定）如果要创建操作记录类型，请单击 **Excel/CSV**.

   >[!NOTE]
   >
   >    创建分类记录类型时，此选项不可用。

1. 拖放以前保存在计算机上的Excel或CSV文件，或单击 **选择CSV或Excel文件** 以浏览其中一个。
1. 单击 **查看您的数据**.

   预览和编辑框显示以下信息：

   * 工作表或未来记录类型的名称显示在左侧面板中。 默认情况下，Maestro会为每个新记录类型选择一个图标和颜色。
   * 选择第一个工作表或记录类型，并且与其关联的字段的名称显示为列标题。 默认情况下，会选择每个字段的类型。
   * 每一行表示一个新记录。 只有前10条记录会显示在“预览和编辑”框中。

   ![](assets/preview-and-edit-box.png)

1. （可选）单击左侧面板中每个页面的名称以查看其中包含的信息。

   >[!NOTE]
   >
   >    不支持空的页面，这些页面将呈灰显状态。


1. （可选）单击 **选择要导入的工作表** 下拉菜单并取消选择不想导入的工作表。

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   取消选择的工作表显示有灰色背景。

1. 单击 **导入** 准备导入文件时。

   以下信息导入到Maestro中：

   * 新记录类型
   * 与每个记录类型关联的新字段
   * 与每个记录类型关联的新记录

   您可以开始管理记录类型页面上的字段和记录。

   有权访问Maestro的每个人都可以查看和编辑导入的记录类型及其信息。 <!--this will change with permissions-->

## 将记录类型与其他应用程序的对象类型连接

在创建Maestro记录类型与另一个应用程序的对象类型之间的连接时，可以导入记录类型。 这会在Maestro中创建与第三方应用程序中的对象类型对应的只读记录类型。

例如，您可以通过将Maestro记录类型与Workfront项目连接来创建记录类型。 因此，Workfront项目对象类型会作为只读记录类型导入Maestro。 默认情况下，记录类型命名为“Workfront项目”。 <!--has this name changed? Lusine wanted to change it at some point-->

您可以从以下应用程序导入以下对象：

* 从Workfront：

   * 项目
   * 项目组合
   * 项目群

有关更多信息，请参阅 [连接记录类型](../architecture-and-fields/connect-record-types.md).








