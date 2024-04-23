---
title: 将封面图像添加到记录
description: 您可以在Adobe Workfront Planning中编辑记录信息，并将每个记录与封面图像相关联，以个性化记录的页面。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

<!--update the metadata with real information-->

# 将封面图像添加到记录

{{maestro-important-intro}}

您可以在Adobe Workfront Planning中编辑记录信息，并将每个记录与封面图像相关联，以个性化记录的页面。

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
<p>贵组织必须注册Adobe Workfront Planning测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
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

## 有关记录页封面图像的注意事项

您可以通过向记录页添加封面图像对其进行个性化设置。 该图像对于每个记录都是唯一的，并且不适用于相同类型的所有记录。

请考虑以下事项：

* 只能添加图像文件作为封面图像。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 您可以从任何视图的记录框或记录页面将封面图像添加到单个记录。
* 不能从表格视图内联添加封面图像。

## 将封面图像添加到记录

您可以在记录框或页面顶部添加封面图像，以个性化记录。

{{step1-to-maestro}}

您上次访问的工作区将打开。

1. （可选）单击工作区名称右侧的向下箭头，选择要更新其记录的工作区。

1. 单击记录类型卡片。

   此时将打开记录类型页面。

1. 从任何类型的视图中，单击记录的名称

   或

   从表格视图中，单击 **打开详细信息** 图标 ![](assets/open-details-icon-in-table-name-field.png) 记录名称的左侧。

   记录的框在视图中打开。

   ![](assets/details-box.png)

   >[!TIP]
   >
   >您可以查看 **打开详细信息** 图标仅当“名称”字段是主字段时，才显示表格视图中记录的“名称”字段左侧的图标。

1. （可选）单击 **在新选项卡中打开** 图标 ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> 在记录框的右上角，在新选项卡中打开记录页面。

   此时将打开记录页面。

   ![](assets/details-page.png)

1. 在记录框或页面中，单击 **添加封面**. <!--check the casing here; I logged a bug for this-->
此 **记录封面** 框打开。

1. 单击 **选择以上传** 并浏览计算机上的图片，以选择、添加图片，然后单击 **使用图像**.

   图像将上传到记录框或页面的顶部，并且更改会自动保存。

   ![](assets/record-page-with-cover-image.png)

1. （可选）将鼠标悬停在图像上，然后单击 **更多** 菜单 ![](assets/more-menu.png) 在封面图像的右下角，执行以下操作之一：

   * 单击 **上传** 如果要替换封面图像并重复步骤6以上传和保存新图像，请执行以下操作：
   * 单击 **重新定位**，并使用 **重新定位** 工具 ![](assets/reposition-tool-icon.png) 将封面图像置中，然后单击 **保存** 完成时。
   * 单击 **移除** 以卸下封面图像。

   Workfront会自动保存您所做的更改。