---
title: 将封面图像添加到记录
description: 编辑记录时，您可以在Adobe Workfront Planning中将封面图像添加到记录页来个性化记录。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 8bfada77ac7b1b2a8d8fb2feec8a8167a1397cdc
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 0%

---


<!--update the metadata with real information-->

# 将封面图像添加到记录

{{planning-important-intro}}

编辑记录时，您可以在Adobe Workfront Planning中将封面图像添加到记录页来个性化记录。

有关编辑记录的信息，请参见 [编辑记录](/help/quicksilver/planning/records/edit-records.md).

必须先创建记录类型，然后才能开始创建和编辑记录。

有关信息，请参阅 [创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md).

## 访问要求

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding cover images-->

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
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <p>当前：工作或更高</p>
   <p>新增：标准</p>  
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Workfront Planning没有访问控制 </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td>  <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> <p>有关信息，请参阅 <a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*有关详细信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 有关记录页封面图像的注意事项

您可以通过向记录页添加封面图像对其进行个性化设置。

请考虑以下事项：

* 封面图像对于一个记录是唯一的，并且不适用于同一类型的所有记录。
* 只能添加图像文件作为封面图像。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 您可以从任何视图的记录预览或记录页面将封面图像添加到单个记录。
* 无法从记录视图添加封面图像。
* 每次创建记录时，Workfront都会自动上传封面图像。 您可以稍后修改此图像。

## 将封面图像添加到记录

通过在记录预览或页面顶部添加封面图像，可以个性化记录。

{{step1-to-planning}}

1. 单击要对其记录进行个性化的工作区，

   或

   从工作区中，展开现有工作区名称右侧的向下箭头，然后选择要对其记录进行个性化的工作区。

   此时会打开工作区，并显示记录类型。

1. 单击记录类型卡片。

   此时将打开记录类型页面。

1. 从任何类型的视图中，单击记录

   或

   从表格视图中，单击 **打开详细信息** 图标 ![](assets/open-details-icon-in-table-name-field.png) 在第一列中。

   记录的预览将在视图中打开。

   ![](assets/details-box.png)

1. （可选）单击 **在新选项卡中打开** 图标 ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> 在记录预览的右上角，在新选项卡中打开记录页面。

   此时将打开记录页面。

   ![](assets/details-page.png)

1. 在记录预览或页面中，单击 **添加封面**


   或

   将鼠标悬停在现有封面图像上，单击 **更多** 菜单 ![](assets/more-menu.png) ，然后单击 **上传**. <!--check the casing here; I logged a bug for this-->
此 **记录封面** 框在 **上传** 选项卡。

   ![](assets/record-cover-box-for-upload.png)

1. 单击 **浏览图像** 并浏览计算机上的图片，以将其选中并添加。

1. （可选）要在保存图像之前删除图像，请单击 **上传新图像** 图标 ![](assets/upload-new-image-icon.png) ，并上传新图像。

1. （可选）单击 **图库** 选项卡，然后单击图像库中的图像。 无法修改图像库。

   ![](assets/record-cover-box-for-gallery.png)

1. 单击 **使用图像**.

   图像会上载到记录预览或页面顶部，并且更改会自动保存。

   ![](assets/record-page-with-cover-image.png)

1. （可选）将鼠标悬停在图像上，然后单击 **更多** 菜单 ![](assets/more-menu.png) 在封面图像的右下角，执行以下操作之一：

   * 单击 **上传** 如果要替换封面图像并重复步骤6以上传和保存新图像，请执行以下操作：
   * 单击 **重新定位**，并使用 **重新定位** 工具 ![](assets/reposition-tool-icon.png) 将封面图像置中，然后单击 **保存** 完成时。
   * 单击 **移除** 以卸下封面图像。

   Workfront会自动保存您所做的更改。
