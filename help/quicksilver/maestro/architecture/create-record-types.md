---
title: 创建记录类型
description: 记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以创建自定义记录类型，以说明在组织的生命周期中所需的工作项。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--this is linked to the UI in an empty workspace screen-->

# 创建记录类型

{{planning-important-intro}}

记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以创建自定义记录类型，这些记录类型说明在组织的生命周期中所需的工作相关项。

有关记录类型的详细信息，请参阅 [记录类型概览](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <td> Adobe Workfront
   </td>
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
   <p>当前：计划</p>
   或
   <p>新增：标准 </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Workfront Planning没有访问级别控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区的权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 有关创建记录类型的注意事项

* 您可以通过以下方式在工作区中创建记录类型：

   * 自动：
      * 使用模板创建工作区时。

        有关信息，请参阅 [创建工作区](../architecture/create-workspaces.md).

      * 当您使用Excel或CSV文件导入它们时。

        >[!IMPORTANT]
        >
        >此功能自2024年3月21日起已暂时禁用。 之后将启用该功能。

     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront Planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/maestro/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/maestro/records/connect-records.md). -->
   * 手动：

      * 从头开始。

        本文介绍了如何从头开始创建记录类型。

* 您可以在分区内移动记录类型，也可以在工作区的一个分区之间移动记录类型。 不能将记录类型从一个工作区移动到另一个工作区。

## 使用工作区模板创建记录类型

在使用Workfront Planning模板创建工作区时，您可以自动创建记录类型。 每个模板都包含示例记录类型。

从模板创建工作区时，记录类型将分组到以下部分：

* 操作记录类型
* 分类标准

您可以在“操作记录类型”和“分类”部分中手动添加记录类型。

有关创建工作区的信息，请参见 [创建工作区](../architecture/create-workspaces.md).

有关每个模板中包含的记录类型的信息，请参阅 [工作区模板列表](../architecture/workspace-templates.md).

## 从头开始创建记录类型

{{step1-to-maestro}}

默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要为其创建记录类型的工作区。
1. （可选）单击 **添加分区** 以向工作区中添加新分区。
1. 单击 **添加记录类型**.
1. （视情况而定）启用通过导入Excel或CSV文件创建记录类型时，单击 **从头开始**. 否则， **添加记录类型** 框打开。

   ![](assets/add-record-type-box-with-appearance-options.png)

1. 更新以下信息：

   * 将“无标题记录类型”替换为您未来记录类型的名称。 <!--did they bring back the field label here and did they rename it to "Name"-->
   * **描述**：添加有关记录类型的更多信息。
   * 为与记录类型关联的图标选择颜色和形状。 执行以下操作：
      * 选择用于标识新记录类型的颜色。 这是记录类型图标的颜色。 默认情况下选中“灰色”。
      * 从列表中选择一个图标，或开始键入图标的名称以描述其表示的内容，然后在显示时选择它。 这是记录类型的图标。 默认情况下，会选择一个文件图标。

1. 单击 **创建**.

   记录类型信息卡会添加到部分和您选择的工作区。
记录类型的描述将显示在信息卡上。

   ![](assets/record-type-card-with-description.png)

1. （可选）将鼠标悬停在记录类型卡片上，单击 **更多** 图标 ![](assets/more-menu.png) 图标，然后单击 **编辑** 修改有关记录类型的信息。
1. （可选）单击记录类型卡以打开记录类型页面。

   ![](assets/operational-record-type-blank.png)

   默认情况下，记录类型页面显示在表视图中。 表的列是与新记录类型关联的字段。 每一行都是您必须添加的唯一记录。

   >[!TIP]
   >
   >    如果从Excel或CSV文件导入记录类型，则也会导入记录。

   默认情况下，以下字段显示在操作记录类型的表视图列中：

   * 名称
   * 描述
   * 开始日期
   * 结束日期
   * 状态

1. （可选）在页面的标题中更新记录类型名称

   或

   单击 **更多** 图标 ![](assets/more-menu.png) 记录类型名称的右侧，然后单击 **编辑** 以重命名它或更改有关它的信息。 有关更多信息，请参阅 [编辑记录类型](/help/quicksilver/maestro/architecture/edit-record-types.md).

1. （可选）单击 **+新记录** 以添加所选记录类型的记录。 有关更多信息，请参阅 [创建记录](../records/create-records.md).
1. （可选）单击 **+** 图标来添加更多字段到记录类型。

   有关创建字段的详细信息，请参阅 [创建字段](../fields/create-fields.md).

1. （可选）单击标题中记录类型名称左侧的左箭头，以返回选定的工作区。

1. （可选）在工作区中，单击并按住记录类型卡片，以将记录类型拖放到所需位置，或将其移动到其他部分。

   更改将自动保存。

   有关在记录类型页面中添加记录、删除或编辑记录类型或更新视图的其他信息，请参阅以下文章：

   * [创建记录](../records/create-records.md)
   * [删除记录类型](../architecture/delete-record-types.md)
   * [编辑记录类型](../architecture/edit-record-types.md)
   * [管理记录视图](../views/manage-record-views.md)

## 通过导入Excel或CSV文件创建记录类型

>[!IMPORTANT]
>
>此功能自2024年3月21日起已暂时禁用。 之后将启用该功能。

使用Excel或CSV文件导入记录类型时，请考虑以下事项：

* Excel文件的每一页都变为记录类型。
* 每个工作表的列将成为与每个记录类型关联的字段。
* 字段对于其各自的记录类型是唯一的。
* 每个工作表中的每一行都成为与其各自记录类型相关联的唯一记录。
* Excel文件的每一页不应超过以下内容：
   * 50,000行
   * 500列
* Excel文件不应大于5MB。
* 不支持空工作表。

要使用Excel文件导入记录类型，请执行以下操作：

{{step1-to-maestro}}

默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要为其创建记录类型的工作区。
1. 单击 **添加记录类型**.
1. 单击 **Excel/CSV**.
1. 拖放以前保存在计算机上的Excel或CSV文件，或单击 **选择CSV或Excel文件** 以浏览其中一个。
1. 单击 **查看您的数据**.

   预览和编辑框显示以下信息：

   * 工作表或未来记录类型的名称显示在左侧面板中。 默认情况下，Workfront Planning会为每个新记录类型选择一个图标和一种颜色。
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

   以下信息导入到Workfront Planning中：

   * 新记录类型
   * 与每个记录类型关联的新字段
   * 与每个记录类型关联的新记录

   您可以开始管理记录类型页面上的字段和记录。

   有权访问Workfront Planning的每个人现在可以查看和编辑导入的记录类型及其信息。 <!--this will change with permissions-->

<!--## Connect record types with object types from another application

You can connect a record type and an object type from another application. This creates a read-only record type in Workfront Planning that corresponds to the object type in the other application. 

For example, you can create record types by connecting Workfront Planning record types with Workfront projects. As a result, the Workfront project object type is imported into Workfront Planning as a read-only record type. By default, the record type is named "Workfront Project." (********************)has this name changed? Lusine wanted to change it at some point***********)
    
You can import the following objects from the following applications: 

* From Workfront:

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

For more information, see [Connect record types](../architecture/connect-record-types.md). 
-->