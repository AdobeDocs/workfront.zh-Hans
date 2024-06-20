---
title: 管理记录页面布局
description: 您可以在Adobe Workfront Planning中编辑记录预览和页面的布局。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 869a1f9e4fd7e3b65591050530b96d6dae9e230c
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# 管理记录页面布局

{{planning-important-intro}}

您可以在Adobe Workfront Planning中编辑记录预览和页面的布局。

记录预览是记录类型视图中显示的记录页面的较小视图。

当您更改记录预览和页面的布局时，更改会影响相同类型的所有记录的预览框和详细信息页面。

本文介绍了如何更改记录预览框或记录页面的布局和外观。 有关编辑记录的信息，请参见 [编辑记录](/help/quicksilver/planning/records/edit-records.md).

必须先创建记录类型和记录，然后才能开始编辑记录页。

有关信息，请参阅以下文章：

* [创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)

* [创建记录](/help/quicksilver/planning/records/create-records.md)

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
   <p>新增：浅色或更高</p>
   或
   <p>当前：工作或更高</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Adobe Workfront Planning没有访问控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区的或更高权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅 <a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*有关详细信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 有关编辑记录页面的注意事项

* 默认情况下，记录的详细信息和预览页面显示与该记录关联的所有字段。

* 您不能在预览或详细信息页面中为记录添加新字段。 您必须在表格视图中添加新字段，才能在预览和详细信息页面中显示它们。

* 您可以将部分添加到记录预览或详细信息页面，以按通用标准组织信息并使其更易于查找。

* 以下更改将影响同一类型的所有记录，并且访问这些记录的所有用户都可以看到这些更改：

   * 重新排列字段
   * 添加或删除部分

* 显示在记录预览中所做的更改会立即显示在记录详细信息页面中。 在记录页面中所做的更改也会显示在记录预览框中。

* 向记录添加封面图像或缩略图不是记录预览或页面整体布局的一部分。 您可以为每个记录添加唯一的封面图像或缩略图。 有关信息，请参阅 [将封面图像添加到记录](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) 和 [向记录添加缩略图](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## 向记录预览或页面添加分区

向记录页添加节时，请考虑以下事项：

* 一个页面上可以具有的节数没有限制。
* 分区不能为空。 在一个部分中，必须至少有一个字段。
* 可以将字段从一个区域拖放到另一个区域。 有关更多信息，请参阅部分 [重新排列记录预览或详细信息页面中的字段](#rearrange-fields-in-the-record-preview-or-details-page) 本文章中。
* 从分区中删除所有字段时，该分区将自动删除且无法恢复。

要将节添加到记录预览或页面，请执行以下操作：

{{step1-to-planning}}

1. 单击工作区的卡片。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。

1. 从任何类型的视图中，单击记录的名称

   或

   从表格视图中，单击 **打开详细信息** 图标 ![](assets/open-details-icon-in-table-name-field.png) 在第一列中。

   记录的预览将在视图中打开。

   ![](assets/details-box.png)

1. （可选）单击 **在新选项卡中打开** 图标 ![](assets/open-details-in-a-new-tab-icon.png) 在记录预览的右上角，在新选项卡中打开记录页面。

   此时将打开记录页面。

   ![](assets/details-page.png)

1. 在记录预览或页面中，将鼠标悬停在字段左侧的空格上，然后单击 **添加分区** 图标 ![](assets/add-section-icon.png) 以添加分区。
1. 在部分的名称内单击并替换 **无标题部分** 名称，然后单击Enter。 在部分下显示的字段自动成为新部分的一部分。
1. 开始将字段拖放到新部分，如部分所述 [重新排列记录预览或详细信息页面中的字段](#rearrange-fields-in-the-record-preview-or-details-page) 本文章中。

1. （可选）将鼠标悬停在区域名称上，然后单击 **更多** 菜单 ![](assets/more-menu.png).

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. （可选）执行以下操作之一以编辑部分：

   * 单击 **重命名** 重命名分区

     >[!TIP]
     >
     > 通过单击名称，可以内联重命名截面。

   * 单击 **上移** 将节向上移动一个位置

     或

     单击 **下移** 将节向下移动一个位置。
部分中的所有字段都会随部分一起移动。

   * 单击 **删除** 以删除部分。 该部分已被删除，无法恢复。 访问此类型记录的所有用户将不再查看已删除的分区。

1. 单击区域名称左侧的向下箭头可将其折叠，单击向右箭头可将其展开。
默认情况下，所有部分都处于扩展状态。

1. （可选）单击 **抓取** 图标 ![](assets/grab-icon.png) 区域名称的左侧，然后将其拖放到所需位置。

   对于查看记录的所有用户，相同类型的所有记录的预览和页面中的区段新位置都会更新。

   对部分和字段顺序的所有更改都将自动保存。

## 重新排列记录预览或详细信息页面中的字段

{{step1-to-planning}}

1. 单击工作区的卡片。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。

1. 从任何类型的视图中，单击记录的名称

   或

   从表格视图中，单击 **打开详细信息** 图标 ![](assets/open-details-icon-in-table-name-field.png) 在第一列中。

   记录的预览将在视图中打开。

   ![](assets/details-box.png)

1. （可选）单击 **在新选项卡中打开** 图标 ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> 在记录预览的右上角，在新选项卡中打开记录页面。

   此时将打开记录页面。

   ![](assets/details-page.png)

1. 在记录预览或页面中，单击 **抓取** 图标 ![](assets/grab-icon.png) 字段名称的左侧，然后将其拖放到所需位置。 <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   对于查看记录的所有用户，字段的新位置会在相同类型的所有记录的预览和页面中更新。

   自动对记录预览或页面保存布局所做的所有更改。

