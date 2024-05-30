---
title: 向记录添加缩略图
description: 您可以在Adobe Workfront Planning中编辑记录信息，并将每个记录与单个缩略图相关联，以便轻松识别。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

<!--update the metadata with real information-->

# 向记录添加缩略图

{{planning-important-intro}}

您可以在Adobe Workfront Planning中将记录与唯一缩略图相关联，以便轻松识别。

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
<p>您的组织必须注册到Workfront Planning的早期访问阶段 </p>
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
   <td> <p>Workfront Planning没有访问控制 </p>  
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
   <td>  <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> <p>有关信息，请参阅 <a href="/help/quicksilver/maestro/access/access-overview.md">访问概述</a>. </p>  
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
* 不能从记录的页面或其他类型的视图添加记录缩略图。
* 缩略图不显示在记录的页面上。

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

<!--
Replace the section above with the following when we release generate thumbnails:

## Add a thumbnail to a record

You can add a thumbnail to a record in the following ways:

* Upload a file from your computer
* Generate an image with a prompt

### Upload a thumbnail to a record

{{step1-to-maestro}}

1. Select the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Upload** tab, and drag and drop a file to add as a thumbnail
   Or
   Click **Select to upload**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) Use the sizing tool to crop and resize the image.
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
1. (Conditional) If you have at least Contribute permissions to the table view, click **Fields** in the upper-right corner of the table view. 
1. Select the **Thumbnail** toggle to display the thumbnail. This is deselected by default. 

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   The thumbnail displays to the left of the primary field value. 
1. (Optional and conditional) If you do not have Contribute or higher permissions to the view, select a new view from the **View** drop-down menu, or create a view. 
1. (Optional) To remove the thumbnail, hover over the primary field and click the **More** menu ![](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![](assets/remove-image-icon.png), then click **Save changes**.

### Generate a thumbnail for a record

{{step1-to-maestro}}

1. Select the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->