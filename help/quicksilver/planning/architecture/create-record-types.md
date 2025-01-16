---
title: 创建记录类型
description: 记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以创建自定义记录类型，以说明在组织的生命周期中所需的工作项。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '1394'
ht-degree: 1%

---


<!--this is linked to the UI in an empty workspace screen-->

# 创建记录类型

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以创建自定义记录类型，这些记录类型说明在组织的生命周期中所需的工作相关项。

有关记录类型的详细信息，请参阅[记录类型概述](/help/quicksilver/planning/architecture/overview-of-record-types.md)。

## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront规划<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
<p>以下任意Workfront计划：</p> 
<ul><li>选择</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning不适用于旧版Workfront计划</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入AdobeUnified Experience，才能访问Workfront Planning的所有功能。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准</p>
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理工作区</a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>布局模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 有关创建记录类型的注意事项

* 您可以通过以下方式在工作区中创建记录类型：

   * 自动：
      * 使用模板创建工作区时。

        有关信息，请参阅[创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)。

      * 当您使用Excel或CSV文件导入它们时。

     >[!TIP]
     >
     >从Excel或CSV文件导入记录类型时，还可以导入记录和字段。

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

有关创建工作区的信息，请参阅[创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)。

有关每个模板包含哪些记录类型的信息，请参阅[工作区模板列表](/help/quicksilver/planning/architecture/workspace-templates.md)。

## 从头开始创建记录类型

{{step1-to-planning}}

1. 单击要在其中创建记录类型的工作区，

   或

   从工作区中，展开现有工作区名称右侧的向下箭头，搜索工作区，然后在工作区显示在列表中时将其选定。
1. （可选）单击&#x200B;**添加节**&#x200B;以向工作区添加新节。
1. 单击&#x200B;**添加记录类型**，然后单击&#x200B;**新建**。

   将打开“添加记录类型”框。
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![](assets/add-record-type-box-with-appearance-options.png)

1. 更新以下信息：

   * 将“无标题记录类型”替换为您未来记录类型的名称。<!--did they bring back the field label here and did they rename it to "Name"-->
   * **描述**：添加有关记录类型的详细信息。
   * 为与记录类型关联的图标选择颜色和形状。 执行以下操作：
      * 选择用于标识新记录类型的颜色。 这是记录类型图标的颜色。 默认情况下选中“灰色”。
      * 从列表中选择一个图标，或开始键入图标的名称以描述其表示的内容，然后在显示时选择它。 这是记录类型的图标。 默认情况下，会选择一个文件图标。

1. 单击&#x200B;**创建**。

   记录类型信息卡会添加到部分和您选择的工作区。
记录类型的描述将显示在信息卡上。

   ![](assets/record-type-card-with-description.png)

1. （可选）将鼠标悬停在记录类型卡片上，单击右上角的&#x200B;**更多**&#x200B;图标![](assets/more-menu.png)，然后单击&#x200B;**编辑**&#x200B;以修改有关记录类型的信息。
1. （可选）单击记录类型卡以打开记录类型页面。

   ![](assets/operational-record-type-blank.png)

   默认情况下，记录类型页面显示在表视图中。 表的列是与新记录类型关联的字段。 每一行都是您必须添加的唯一记录。

   默认情况下，以下字段显示在操作记录类型的表视图列中：

   * 名称
   * 描述
   * 开始日期
   * 结束日期
   * 状态

1. （可选）在页面的标题中更新记录类型名称

   或

   单击记录类型名称右侧的&#x200B;**更多**&#x200B;图标![](assets/more-menu.png)，然后单击&#x200B;**编辑**&#x200B;以重命名它或更改有关它的信息。 有关详细信息，请参阅[编辑记录类型](/help/quicksilver/planning/architecture/edit-record-types.md)。

1. （可选）单击&#x200B;**+新记录**&#x200B;以添加所选记录类型的记录。 有关详细信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
1. （可选）单击表右上角的&#x200B;**+**&#x200B;图标以向记录类型添加更多字段。

   有关创建字段的详细信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

1. （可选）单击标题中记录类型名称左侧的左箭头，以返回选定的工作区。

1. （可选）在工作区中，单击并按住记录类型卡片，以将记录类型拖放到所需位置，或将其移动到其他部分。

   更改将自动保存。

   有关在记录类型页面中添加记录、删除或编辑记录类型或更新视图的其他信息，请参阅以下文章：

   * [创建记录](/help/quicksilver/planning/records/create-records.md)
   * [删除记录类型](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [编辑记录类型](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)

## 通过导入Excel或CSV文件创建记录类型

使用Excel或CSV文件导入记录类型时，请考虑以下事项：

* Excel文件的每一页都变为记录类型。 工作表的名称将成为记录类型的名称。
* 如果只有一个工作表，或者导入CSV文件，则文件的名称将成为记录类型的名称。
* 每个工作表的列标题将成为与每个记录类型关联的字段。
* 字段对于其各自的记录类型是唯一的。
* 每个工作表中的每一行都成为与其各自记录类型相关联的唯一记录。
* Excel文件的每一页不应超过以下内容：
   * 10,000行
   * 500列
* Excel文件不应大于5MB。
* 不支持空工作表。

要使用Excel或CSV文件导入记录类型，请执行以下操作：

{{step1-to-planning}}

1. 单击要在其中创建记录类型的工作区，

   或

   从工作区中，展开现有工作区名称右侧的向下箭头，搜索工作区，然后在工作区显示在列表中时将其选定。
1. 单击&#x200B;**添加记录类型**。
1. 单击&#x200B;**来自文件**。
1. 拖放以前保存在您计算机上的Excel或CSV文件，或单击&#x200B;**选择CSV或Excel文件**&#x200B;以浏览一个。
1. 单击&#x200B;**预览和编辑**。

   显示&#x200B;**预览和编辑**&#x200B;框并显示以下信息：

   * 工作表或未来记录类型的名称显示在左侧面板中。 默认情况下，Workfront Planning会为每个新记录类型选择一个图标和一种颜色。
   * 选择第一个工作表或记录类型，并且与其关联的字段的名称显示为列标题。 默认情况下，会选择每个字段的类型。
   * 每一行表示一个新记录。 只有前10条记录会显示在“预览和编辑”框中。

   ![](assets/preview-and-edit-box.png)

1. （可选）单击左侧面板中每个页面的名称以查看其中包含的信息。

   >[!NOTE]
   >
   >不支持空的页面，这些页面将呈灰显状态。

1. （可选）从左侧面板中取消选择不想导入的工作表。

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   取消选择的工作表显示有灰色背景。

1. （可选）单击列标题右侧的向下箭头，以执行以下操作之一：

   * 重命名其中一个字段
   * 更改&#x200B;**字段类型**
   * 更新字段&#x200B;**描述**

1. （视情况而定）更新字段相关信息后，单击&#x200B;**保存**。

1. 准备导入文件时，请单击&#x200B;**导入**。

   以下信息导入到Workfront Planning中：

   * 新记录类型
   * 与每个记录类型关联的新字段
   * 与每个记录类型关联的新记录

   您可以开始管理记录类型页面上的字段和记录。

   有权访问Workfront Planning的每个人现在可以查看和编辑导入的记录类型及其信息。
