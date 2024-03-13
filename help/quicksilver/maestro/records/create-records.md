---
title: 创建记录
description: 使用Adobe Workfront规划功能时，记录是记录类型的实例。 在创建单个记录之前，必须先创建记录类型。 创建分类记录与创建操作记录相同。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 创建记录

{{maestro-important-intro}}

在Adobe Workfront规划功能中，记录是记录类型的实例。

您可以具有以下类型的记录：

* **操作记录**：它们表示与工作相关的对象。 例如，对于名为“Campaign”的运营记录，您可以拥有名为“Monthly Newsletter”或“Summer Sale”的记录。
* **分类记录**：它们表示可与操作记录关联的属性。 例如，对于名为“渠道”的分类记录类型，您可以命名分类，如“电子邮件”、“社交媒体”或“广告”。

创建操作记录与创建分类记录相同。

您可以通过执行以下操作之一来创建记录：

* 为记录类型手动创建它们
  <!-- not possible anymore: * Connect them to records from other applications-->
* 通过复制和粘贴外部列表中的信息创建记录。

本文介绍了如何创建记录。 有关管理表或时间线视图中的记录的信息，请参阅以下文章：

* [管理表视图](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [管理时间线视图](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

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
<p>贵组织必须注册Adobe Workfront规划功能封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
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
   <td> <p>Adobe Workfront规划功能没有访问控制 </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>为工作区提供或更高权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 通过手动将记录添加到记录类型来创建记录 <!--in a record type table (I don't think you can create them elsewhere right now)-->

您可以在记录类型页面的表格视图中创建记录。

有关编辑记录信息的信息，请参阅 [编辑记录](/help/quicksilver/maestro/records/edit-records.md).

{#step1-to-maestro}

默认情况下，将打开您上次访问的工作区。 有关创建工作区的信息，请参见 [创建工作区](../architecture/create-workspaces.md).
1. 单击记录类型卡片。 有关创建记录类型的信息，请参阅 [创建记录类型](../architecture/create-record-types.md).

   记录类型页面将在您上次访问的视图中打开。 默认情况下，将在表格视图中打开记录类型页面。
所选类型的所有记录都显示在表格视图中。

1. （视情况而定）如果记录类型页面未在表视图中打开，请单击 **视图** 下拉菜单，然后选择现有的 **表格视图** ![](assets/table-view-icon.png) 或单击 **“创建视图”>“表”** 创建表格视图。

<!--Replace the above with this when we release the tabbed views: 
1. (Conditional) If the record type page does not open in the table view, click the tab of a table view, or click **+ View** to create a table view. -->

1. 要添加新记录，请单击 **新记录** 在表的最后一行

   或

   单击 **Shift + Enter** 从表格的任意列或行访问键盘。 这会添加一个空行。

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. 开始在新行中输入有关新记录的信息。

   >[!NOTE]
   >
   >  * 记录没有必填字段。 但是，我们建议您为记录添加名称，因为在将记录相互链接时，识别记录会很有帮助。
   >
   >  * 引用其他记录类型或计算字段的字段为只读字段。

1. 继续添加每行的信息，然后单击 **输入** 以保存更改。

<!--Or 
    
    Click the new record's name or the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to the left of the record name. The **Details** box opens in the table. 

      >[!TIP]
      >
      >    You can access the Details box only from the name field of the record when the Name field is a primary field. 

  1. Start editing the record's information in the Details box. Workfront automatically saves your changes. 
  1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the Details box to open the record's **Details** page in a new tab. Continue editing the record on the Details page.
    -->

1. （可选）使用以下键盘快捷键可撤消或重做添加新记录：

   * CTRL + Z(Mac为⌘ + Z)可撤消更改
   * 按CTRL + Shift + Z(对于Mac，按⌘ + Shift + Z)可重做更改

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](../architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](../architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](../records/connect-records.md). 

    The following items are created in Maestro:

    * A read-only Maestro record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Maestro record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Maestro records you're linking from. 
   
-->

## 通过复制和粘贴外部列表中的信息创建记录

1. 开始在“表”视图中创建记录，如一节中所述 [通过手动将记录添加到记录类型来创建记录](#create-records-by-manually-adding-them-to-a-record-type) 本文章中。

   确保表视图具有要使用新记录信息填充的列（或字段）。

1. 单击 **新建&lt;记录类型名称>** 在表的最后一行中，向表中添加所需数量的新行。

   例如，如果要粘贴来自其他应用程序的10条新记录的信息，请向表格视图添加10行。

1. 在另一个应用程序中，创建要导入的记录列表。

   例如，您可以使用Excel电子表格来创建列表。

   该列表应包含表格格式的信息。

   >[!TIP]
   >
   > 列表的列应包含有关您在Workfront中拥有的现有字段的信息。
   >
   > 确保您已在Workfront中创建了所需的字段，并且工作表中的信息以与Workfront中每个字段信息匹配的正确格式显示。

1. 从另一个应用程序中，选择多个行和列，然后将信息粘贴到记录类型表格视图中，从第一个新记录开始。

   将在Workfront规划功能区域中导入以下信息：

   * 行包含新记录
   * 列填充记录字段的信息。
