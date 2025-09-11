---
title: 创建记录类型
description: 记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以创建自定义记录类型，以说明在组织的生命周期中所需的工作项。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: ff5bc262a5ed2a22099c058ebdb61bc32485b201
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 2%

---


<!--this is linked to the UI in an empty workspace screen-->

# 创建记录类型

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以创建自定义记录类型，这些记录类型说明在组织的生命周期中所需的工作相关项。

有关记录类型的详细信息，请参阅[记录类型概述](/help/quicksilver/planning/architecture/overview-of-record-types.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

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
<p>贵组织的Workfront实例必须载入Adobe Unified Experience才能访问Workfront Planning。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
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
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

## 有关创建记录类型的注意事项

* 您可以通过以下方式在工作区中创建记录类型：

   * 自动：
      * 使用模板创建工作区时。

        有关信息，请参阅[创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)。

      * 当您使用CSV或Excel文件导入这些文件时。

        有关详细信息，请参阅[通过从CSV或Excel文件导入信息来创建记录类型](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md)。

     >[!TIP]
     >
     >从CSV或Excel文件导入记录类型时，还可以导入记录和字段。

   * 手动：

      * 从头开始。

        本文介绍了如何从头开始创建记录类型。

     <!--
        * <span class="preview">By importing them from another workspace or adding cross-workspace record types</span>
            <span class="preview">For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md). </span>-->


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
1. 单击&#x200B;**添加记录类型**，然后单击&#x200B;**手动添加**。

   将打开“添加记录类型”框。
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![添加具有外观选项的记录类型框](assets/add-record-type-box-with-appearance-options.png)

1. 在&#x200B;**外观**&#x200B;选项卡上更新以下信息：

   * 将“无标题记录类型”替换为您未来记录类型的名称。<!--did they bring back the field label here and did they rename it to "Name"-->
   * **描述**：添加有关记录类型的详细信息。
   * 为与记录类型关联的图标选择颜色和形状。 执行以下操作：
      * 选择用于标识新记录类型的颜色。 这是记录类型图标的颜色。 默认情况下选中“灰色”。
      * 从列表中选择一个图标，或开始键入图标的名称以描述其表示的内容，然后在显示时选择它。 这是记录类型的图标。 默认情况下，会选择一个文件图标。


   <!--old setting:
    1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Connectivity scope** section: 
        * Enable the **Connect from other workspace** setting. When enabled, the record type is accessible and can be connected from other workspaces. 
        * Choose from which workspaces the record type can be accessed. Choose from the following options:
            * **System wide**: Users can connect to this record type from all workspaces where they have manage permissions. 
            * **Specific workspaces**: Add the names of the workspaces where workspace managers can connect to this record type. 
    -->

1. （可选且有条件）如果您是系统管理员，请单击&#x200B;**高级设置**&#x200B;并在&#x200B;**跨工作区功能**&#x200B;部分中更新以下信息： <!--the info here is duplicated in the Edit record types article-->
   * 启用&#x200B;**允许在其他工作区中连接到此记录类型**&#x200B;设置：这允许工作区管理员从其他工作区连接到此记录类型。\
     您可以指定此记录类型可以连接的工作区。 可使其可用于所有工作区，或指定可在其中导入它的特定工作区。
有关详细信息，请参阅[为记录类型配置跨工作区功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。


   ![在“高级设置”选项卡上创建“记录类型”框](assets/create-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release dynamic record types; the preview tags might need to be edited, too:
        <div class="preview">
        1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Cross-workspace capability** section: **** the info here is duplicated in the Edit record types article ***
            * Enable the **Allow adding this record type to other workspaces** setting: This allows workspace managers to add this record type to other workspaces. 
                You can designate specific users who can add this record type to other workspaces. 
            * Enable the **Allow connecting to this record type in other workspaces** setting: This allows workspace managers to connect to this record type from other workspaces.  
                You can designate which workspaces this record type can be connected from. You can make it available for all workspaces or designate specific ones where you can import it.
            For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).  </div>
            ******** replace screen shot below **********
            ![Create record type box on advanced settings tab](assets/create-record-type-box-advanced-settings-tab.png) 
        -->

1. 单击&#x200B;**保存**。

   记录类型信息卡会添加到部分和您选择的工作区。
记录类型的描述将显示在信息卡上。

   ![带有说明的记录类型信息卡](assets/record-type-card-with-description.png)

   如果选择从其他工作区连接此记录，则记录卡上会显示&#x200B;**从其他工作区连接**&#x200B;图标![从其他工作区连接图标](assets/connect-from-other-workspaces-icon.png)。

   <!--<span class="preview">If you configured the cross-workspace capabilities for the record, the **connect from other spaces** icon ![Connect record type from other spaces icon](assets/connect-from-other-workspaces-icon.png) and the **add to other workspaces** icon ![Add record type to other workspaces](assets/global-icon.png) also display on the card. </span>-->

1. （可选）将鼠标悬停在记录类型卡片上，单击右上角的&#x200B;**更多**&#x200B;图标![更多菜单](assets/more-menu.png)，然后单击&#x200B;**编辑**&#x200B;以修改有关记录类型的信息。
1. （可选）单击记录类型卡以打开记录类型页面。

   ![操作记录类型为空](assets/operational-record-type-blank.png)

   默认情况下，记录类型页面显示在表视图中。 表的列是与新记录类型关联的字段。 每一行都是您必须添加的唯一记录。

   默认情况下，以下字段显示在操作记录类型的表视图列中：

   * 名称
   * 描述
   * 开始日期
   * 结束日期
   * 状态

1. （可选）在页面的标题中更新记录类型名称

   或

   单击记录类型名称右侧的&#x200B;**更多**&#x200B;图标![更多菜单](assets/more-menu.png)，然后单击&#x200B;**编辑**&#x200B;以重命名它或更改有关它的信息。 有关详细信息，请参阅[编辑记录类型](/help/quicksilver/planning/architecture/edit-record-types.md)。

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

## 通过从CSV或Excel文件导入信息创建记录类型

从CSV或Excel文件导入信息时，可以导入以下内容：

* 记录类型
* 记录
* 记录字段

有关详细信息，请参阅[通过从CSV或Excel文件导入信息来创建记录类型](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md)。

<!--

<div class="preview">

## Create record types by importing them from another workspace 

You can add record types to a workspace by importing them from another workspace. You can only add record types that have been configured as centralized record types. 

For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

</div>

-->