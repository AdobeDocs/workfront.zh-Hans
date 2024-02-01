---
title: 将缩略图添加到记录
description: 您可以在Adobe管理器中编辑记录信息，并将每个记录与单个缩略图相关联，以使它们易于识别。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

<!--update the metadata with real information-->

# 将缩略图添加到记录

{{maestro-important-intro}}

您可以在AdobeMaestro中将记录与唯一的缩略图相关联，以便轻松识别它们。

必须先创建记录类型，然后才能开始创建和编辑记录。
有关信息，请参阅 [创建记录类型](../architecture/create-record-types.md).

## 访问要求

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Maestro没有访问控制 </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>为工作区提供或更高权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td>  <p>必须为包括Workfront管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的Maestro区域。 </p> <p>有关信息，请参阅 <a href="/help/quicksilver/maestro/access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## 有关记录缩略图的注意事项

为了从视觉上区分表格视图中的记录，您可以将唯一的缩略图图像与每个记录相关联。

请考虑以下事项：

* 您只能添加图像文件作为缩略图。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 可以将缩略图图像添加到表格视图中的各个记录。
* 缩略图属于记录信息，它们显示在显示记录的视图中。 例如，缩略图与记录信息一起显示在以下区域中：

   * 表视图中记录的主要字段
   * 时间线视图中的记录栏。
* 您无法从记录的“详细信息”页面或时间线视图中添加记录缩略图。
* 缩略图不显示在记录的详细信息页面中。

## 向记录添加缩略图

{{step1-to-maestro}}

1. 选择要为其添加缩略图的记录的工作区，然后单击记录类型卡片。

   这将打开记录类型页面。
1. 从中选择表格视图 **视图** 下拉菜单。 所选类型的所有记录都会显示在表格中。
1. 将鼠标悬停在主字段信息上，单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **缩略图**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   主字段是显示在表视图第一列中的字段。 主字段始终冻结，不能隐藏或重新定位。

   此 **录制缩略图** 框打开。

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. 在 **上传** 选项卡，拖放要作为缩略图添加的文件，或单击 **选择以上传**，然后浏览以添加图像文件。 文件必须保存在计算机上。
1. （可选）使用调整大小工具裁切图像并调整其大小。
1. 单击 **使用图像** 将图像添加为缩略图。
这将关闭 **录制缩略图** 盒子。
1. （视情况而定）如果您至少具有表视图的Contribute权限，请单击 **字段** 表视图的右上角。
1. 选择 **缩略图** 切换可显示缩略图。 默认情况下，该选项处于取消选中状态。

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   主字段值的左侧将显示缩略图。
1. （可选且视情况而定）如果您没有Contribute或更高版本的视图权限，请从 **视图** 下拉菜单，或创建视图。
1. （可选）要删除缩略图，请将鼠标悬停在主字段上，然后单击 **更多** 菜单 ![](assets/more-menu.png)> **缩略图** > **移除** 图标 ![](assets/remove-image-icon.png)，然后单击 **保存更改**.
