---
title: 管理记录页面
description: 您可以在Adobe Workfront Planning中编辑记录框和页面的布局。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# 管理记录页面

{{maestro-important-intro}}

您可以在Adobe Workfront Planning中编辑记录框和页面的布局。 您可以在记录视图中显示记录框。

记录框是记录类型视图中显示的记录页的较小视图。

当您更改记录框和页面的布局时，该框和页面会针对同一类型的所有记录进行更改。

必须先创建记录类型和记录，然后才能开始编辑记录页。

有关信息，请参阅以下文章：

* [创建记录类型](../architecture/create-record-types.md)

* [创建记录](/help/quicksilver/maestro/records/create-records.md)

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
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*有关详细信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 有关编辑记录页面的注意事项

* 重新排列记录框或页面中的字段会重新排列该类型的所有记录以及访问这些记录的所有用户的字段。
* 向记录添加封面图像不是记录框或页面的总体布局的一部分。 您可以为每个记录添加唯一的封面图像。 有关信息，请参阅 [将封面图像添加到记录](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

## 重新排列记录框或页面中的字段

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

1. 在记录框或页面中，单击抓取图标 ![](assets/grab-icon.png) 字段名称的左侧，然后将其拖放到所需位置。

   对于查看记录的所有用户，该字段的新位置将在所有相同类型的记录所在的框和页面中更新。

   自动保存对记录框或页面布局所做的所有更改。

