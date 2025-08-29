---
title: 创建记录
description: 使用Adobe Workfront Planning时，记录是记录类型的实例。 您可以在Workfront Planning中为每个记录类型创建唯一记录，方法是：将记录手动添加到表视图中，从列表中导入记录，复制记录，或在将其连接到其他记录时创建记录。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: b291525db0105081b5ff3dd65d9d2b3267a2f60c
workflow-type: tm+mt
source-wordcount: '2814'
ht-degree: 0%

---


# 创建记录

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

在Adobe Workfront Planning中，记录是记录类型的实例。

您可以通过执行以下操作之一来创建记录：

* [使用任何记录类型视图中的“新建记录”或“请求记录”按钮](#create-records-using-the-new-record-or-request-record-button-from-any-record-type-view)
* [从记录类型表格视图内联添加它们](#create-records-by-adding-them-inline-from-the-record-type-table-view)

<div class="preview">

* [在记录类型时间线视图中添加它们](#create-records-by-adding-them-in-the-record-type-timeline-view)

</div>

<!--
<div class="preview">

* [Add them in the record type calendar view](#create-records-by-adding-them-in-the-record-type-calendar-view)

</div>
-->

* [从外部列表中复制并粘贴记录列表](#create-records-by-copying-and-pasting-them-from-an-external-list)
* [从表视图复制记录](#create-records-by-duplicating-them)
* [从其他记录连接它们](#create-records-as-you-connect-them)
* [提交请求表单到记录类型](#create-records-by-submitting-a-request-form-to-a-record-type)
* [从CSV或Excel文件导入信息](#create-records-by-importing-records-from-a-csv-or-excel-file)
* [使用自动化](#create-records-by-using-automations)

有关管理表或时间线视图中的记录的信息，请参阅以下文章：

* [管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)
* [管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)

## 访问要求

+++ 展开以查看访问要求。  

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
   <td> 标准
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p> 
   <p>在将记录连接到要创建的对象类型（项目、项目和项目组合）时，在Workfront中编辑对这些对象的访问权限。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p>为要添加记录的工作区和记录类型分配或更高权限。 </p>
   <p>查看或更高权限的工作区和记录类型，以使用记录页面上的“请求记录”按钮创建记录</p>
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
   <p>管理Workfront对象（项目组合）的权限以添加子对象（项目）。</p>
   </td> 
  </tr>

</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用任何记录类型视图中的“新建记录”或“请求记录”按钮创建记录

对工作区以及记录类型具有查看权限的用户只能使用记录类型页面上的“请求记录”按钮来创建记录。

对工作区和记录类型具有Contribute和“管理”权限的用户可以使用记录类型页面上的“新建记录”按钮创建记录。


>[!IMPORTANT]
>
>工作区管理员必须为记录类型创建请求表单，以便具有查看权限的用户使用请求表单添加记录。 否则，查看权限用户无法创建记录。

{{step1-to-planning}}

1. 单击要在其中添加记录的工作区。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。 有关创建记录类型的信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

   记录类型页面将在您上次访问的视图中打开。 默认情况下，将在表格视图中打开记录类型页面。
所选类型的所有记录都将显示在视图中。

1. （视情况而定）在任意视图中，根据工作区和记录类型权限，单击屏幕右上角的以下内容：

   * 如果您对工作区和记录类型具有Contribute或更高权限，请单击&#x200B;**新建记录**

     或

   * 如果您对工作区和记录类型具有查看权限，请单击&#x200B;**请求记录**。

1. （视情况而定）如果您单击&#x200B;**新记录**，请执行以下操作：

   1. 单击以下方法之一创建记录，然后单击&#x200B;**继续**：

      * **手动添加**。 记录的预览框打开。\
        添加有关记录的信息，如从第6步开始，通过从本文中的记录类型表视图[节内联添加记录来创建记录](#create-records-by-adding-them-inline-from-the-record-type-table-view)中所述。<!--insure this stays accurate-->
      * **从文件上载**
添加记录，如文章[中所述。通过从CSV或Excel文件导入信息创建记录](/help/quicksilver/planning/records/import-file-to-create-records.md)，从步骤6开始。<!--ensure this stays accurate-->
      * **提交请求**
此时将打开记录类型的请求表单。

        工作区管理员必须创建请求表单，以便能够使用请求表单添加记录。

        >[!TIP]
        >
        >某些记录类型可能具有多个表单。 单击一个以将其打开。

        按照文章[提交Adobe Workfront Planning请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)中的说明添加记录，从步骤6开始。<!--ensure this stays accurate-->

      ![创建记录选择模式的三种方法](assets/three-ways-to-create-records-choice-modal.png)

1. （视情况而定）如果您单击&#x200B;**请求记录**，请执行以下操作：

   1. （视情况而定）如果记录类型有多个请求表单，请单击其中一个以选择它。
   2. 从第6步开始，按照文章[提交Adobe Workfront Planning请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)中所述，继续在表单中添加信息以创建记录。<!--ensure this stays accurate-->

1. （视情况而定）审查新记录。

   根据您选择添加记录的方式，可能会出现以下情况：

   * 新记录将添加到记录类型，除非您选择使用具有审批流程的请求表单添加记录。 在创建记录之前，必须由所有批准者进行批准。
   * 如果您使用CSV或Excel电子表格添加记录，则向记录类型添加多个记录。
   * 如果您通过提交请求表单来添加请求，则新请求会添加到Workfront请求区域的Planning选项卡中。

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    The following items are created in Workfront Planning:

    * A read-only record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Planning record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Planning records you're linking from. 
   
-->

## 通过从记录类型表视图内联添加记录来创建记录

您可以在记录类型页面的表格视图中创建记录，因为您是内联添加记录的。

有关编辑记录信息的信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

{{step1-to-planning}}

1. 单击要在其中添加记录的工作区。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。 有关创建记录类型的信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

   记录类型页面将在您上次访问的视图中打开。 默认情况下，将在表格视图中打开记录类型页面。
所选类型的记录将显示在视图中。

1. （视情况而定）从表格视图中，执行以下操作之一：

   * 在表的最后一行中或在分组中的最后一个记录之后单击&#x200B;**新建记录**

     >[!TIP]
     >
     >当您在分组或子分组中的最后一个记录之后添加新记录时，Workfront会自动填充分组中包含的字段。 如果需要，您可以手动编辑这些字段，并且可能会从分组中删除记录。

   * 在键盘上从表格的任意列或行单击&#x200B;**Shift + Enter**。 这会在您开始的记录下添加一个空行。
   * 将鼠标悬停在记录的主字段上，单击该字段右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**在上方插入记录**&#x200B;或&#x200B;**在下方插入记录**。

   ![在表行中添加新的营销活动](assets/adding-a-new-campaign-in-table-row.png)

   Workfront会自动将缩略图上传到每条新记录。 您可以稍后修改这些图像。 有关信息，请参阅[将封面图像添加到记录](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)。

   新记录将添加到表中。

1. 单击新记录的主要字段

   或

   单击记录名称左侧的&#x200B;**打开详细信息**&#x200B;图标![表名称字段中的打开详细信息图标](assets/open-details-icon-in-table-name-field.png)。

   预览框在表中打开。

1. 开始在您在预览框中看到的字段中键入有关新记录的信息。

   >[!NOTE]
   >
   >  * 记录没有必填字段。 但是，我们建议您为记录的主要字段添加信息，因为在将记录相互链接时，识别记录会很有帮助。 有关主字段的详细信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)和[主字段概述](/help/quicksilver/planning/fields/primary-field-overview.md)。
   >
   >  * 引用其他记录类型或计算字段的字段为只读字段。

1. （视情况而定）在表中添加记录时，在打开记录的预览框之前，继续添加每行的信息，然后在键盘上单击&#x200B;**Enter**&#x200B;以保存更改。

   或

   单击新记录名称或记录名称左侧的&#x200B;**打开详细信息**&#x200B;图标![在表名称字段中打开详细信息图标](assets/open-details-icon-in-table-name-field.png)以打开预览框并在详细信息区域编辑记录信息。

   >[!TIP]
   >
   >当名称字段是主字段时，您只能从记录的名称字段访问&#x200B;**打开详细信息**&#x200B;图标。

1. （可选）在记录的预览框中，单击&#x200B;**在新标签中打开**&#x200B;图标![在右上角的新标签中打开详细信息](assets/open-details-in-a-new-tab-icon.png)以新标签中打开记录的页面。 继续编辑记录页面上的记录。 有关信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

   Workfront会自动保存您所做的更改。

1. （可选）关闭预览框或单击记录名称左侧的返回箭头（如果打开了记录的页面）。

1. （可选）在表视图中添加新记录或其信息时，请使用以下键盘快捷键撤消或重做添加新记录或其信息：

   * 按CTRL + Z (⌘ + Z表示Mac)可撤消更改
   * 按CTRL + Shift + Z (⌘ + Shift + Z用于Mac)以重做更改


<div class="preview">

## 通过在记录类型时间线视图中添加记录来创建记录

您可以在记录类型页面的时间线视图中双击来创建记录。

有关创建时间表视图的信息，请参阅[管理时间表视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

{{step1-to-planning}}

1. 单击要在其中添加记录的工作区。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   记录类型页面将在您上次访问的视图中打开。

1. 首先单击以打开时间线视图，或创建时间线视图。

   >[!NOTE]
   >
   >仅当至少有两个日期字段与记录类型关联时，才能创建时间线视图。
1. 双击时间轴中的任意位置。

   将打开一个新记录框。<!--might need a new screen shot for Production - might add a title etc-->

   ![时间轴上的新记录框（具有未命名的记录栏）](assets/new-record-small-box-on-timeline.png)
1. 更新以下信息：

   * **名称**：输入记录名称。 如果将其留空，Workfront会默认将其命名为&#x200B;**无标题**。

     >[!TIP]
     >
     >如果根据时间线设置在记录栏中显示记录的“名称”，则如果保留为空，该名称在记录栏中不可见。

   * **记录日期字段**：更新记录日期。

     创建时间线视图时，根据为开始日期和结束日期选择的字段自定义日期字段的名称。

     默认情况下，日期值会根据时间线视图的显示方式预先选择。 存在以下情况：

      * 按&#x200B;**年**：记录的开始和结束日期跨越一个月。
      * 按&#x200B;**季度**：记录的开始和结束日期跨一周。
      * 按&#x200B;**月**：记录的开始和结束日期跨三天。

1. （可选）单击以下图标之一：

   * **展开** ![展开图标](assets/expand-icon.png)以在预览窗口中打开记录详细信息。
   * **删除** ![删除图标](assets/delete-icon.png)以删除记录。
   * **关闭** ![关闭图标](assets/close-icon.png)以关闭新记录框。

   除非您单击&#x200B;**删除**&#x200B;图标，否则该记录将立即添加到时间轴以及表和日历视图。
   <!--1. (Optional) Hover over the record's bar in the timeline and drag and drop the ends of the bar to a different date. This automatically changes the start and end date of the record.-->
1. （可选）单击时间轴中的记录栏以打开记录的详细信息窗口，并更新其信息、将其删除或添加注释。

   >[!TIP]
   >
   >默认情况下，Workfront会将记录与缩略图和封面图像相关联。
   >
   >仅当在视图的“设置”中启用缩略图时，缩略图才会显示在时间轴视图中。

</div>

<!--

<div class="preview">

## Create records by adding them in the record type calendar view

You can create records in the calendar view of a record type page, by double-clicking anywhere on the calendar. 

For information about creating a calendar view, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md).

{{step1-to-planning}}
  
1. Click the workspace where you want to add records.

    The workspace opens and the record types display as cards.

1. Click a record type card. 

    The record type page opens in the view that you last accessed. 

1. Click to open a calendar view, or create a calendar view.

    >[!NOTE]
    >
    >You can create a calendar view only if there are at least two date fields associated with the record type.
1. Double-click anywhere on the calendar. 

    A new record box opens. (********might need a new screen shot for Production - might add a title etc*********)

    ![New record box on calendar with unnamed record bar](assets/new-record-small-box-on-calendar.png)

1. Update the following information:

    * **Name**: Enter the name of the record. If you leave it empty, Workfront names it **Untitled** by default. 
    
        >[!TIP]
        >
        >If you display the Name of the record in the record bars according to the calendar settings, the name is not visible in the record bar if left empty. 

    * **Record date fields**: Update the dates of the record. 
        
        The names of the date fields are customized according to the fields selected for the Start and End dates when the calendar view was created.

        By default, date values are preselected depending on how you display the calendar view. The following scenarios exist:

        * By **Month**: The record start and end dates span one day.
        * By **Week**: The record start and end dates span two days.

1. (Optional) Click one of the following icons: 

    * **Expand** ![Expand icon](assets/expand-icon.png) to open the record details in the preview window. 
    * **Delete** ![Delete icon](assets/delete-icon.png) to delete the record.
    * **Close**  ![Close icon](assets/close-icon.png) to close the new record box. 

    The record is added to the calendar as well as to the table and timeline views immediately, unless you clicked the **Delete** icon. 

1. (Optional) Click the record bar in the calendar to open the record's details window and update its information, delete it, or add comments. 

    >[!TIP]
    >
    >By default, Workfront associates the record with a thumbnail and a cover image.
    >
    >The thumbnail displays in the calendar view only when it is enabled in the Settings of the view. 

</div>

-->

## 通过从外部列表中复制和粘贴记录来创建记录

1. 开始在“表”视图中创建记录，如[通过手动将记录添加到本文中的记录类型](#create-records-by-manually-adding-them-to-a-record-type)来创建记录一节中所述。

   确保表视图具有要使用新记录信息填充的列（或字段）。

1. 在表的最后一行中单击&#x200B;**新建&lt;记录类型名称>**，以向表中添加您想要的新记录数量的新行。

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

   将在Workfront Planning区域中导入以下信息：

   * 行包含新记录
   * 列填充记录字段的信息。

## 通过复制记录创建记录

有关复制记录的信息，请参阅[复制记录](/help/quicksilver/planning/records/copy-or-duplicate-records.md)。

## 连接记录时创建记录

从其它记录连接时，可以创建以下对象类型：

* Workfront Planning记录
* Workfront对象

本节介绍在将记录与其他记录连接时如何创建Workfront Planning记录。

>[!NOTE]
>
>在将Workfront项目和项目组合连接到Workfront Planning记录时创建Planning项目和项目组合，与在从其他记录连接它们时创建Planning记录类似。
>
>有关从Workfront Planning创建Workfront对象的信息，请参阅将Workfront对象连接到记录时[从Workfront Planning创建这些对象](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)。

您必须具备以下条件，才能通过从现有记录连接来添加新记录：

* 连接的记录类型。 有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。
* 记录。
* Workfront Planning和Workfront中的正确访问和权限，如本文的[访问要求](#access-requirements)部分所述。

要在从其他记录连接记录时创建记录，请执行以下操作：

1. 开始连接Workfront Planning记录，如文章[连接记录](/help/quicksilver/planning/records/connect-records.md)中所述。 您可以从以下区域连接记录：

   * Workfront Planning的以下区域中的连接字段：

      * 表格视图
      * 记录的详细信息页面或预览框

   * Workfront中项目、项目组合或项目群的“规划”部分中的连接字段。

     有关信息，请参阅[管理来自Workfront对象的记录连接](/help/quicksilver/planning/records/manage-records-in-planning-section.md)。

1. （视情况而定）如果在尝试连接时找不到记录，请单击&#x200B;**+添加**

   或
开始键入名称，然后单击&#x200B;**+添加**。 **+ Add**&#x200B;按钮后跟您连接到的记录类型的名称。 例如，将品牌添加到现有营销活动时，“添加品牌”。 您键入的名称还遵循“添加”按钮。

   ![添加按钮以在突出显示的上下文中创建记录](assets/add-button-to-create-records-in-context-highlighted.png)

   将创建记录并将其添加到连接的记录字段。

   >[!IMPORTANT]
   >
   >* 从记录中连接项目、项目组合和项目群时，只能在Workfront中创建它们。
   >
   >* 从Workfront Planning中的记录连接组或公司时，无法创建组或公司。
   > 

1. （可选）转到您创建其记录的记录类型的表格视图。 新记录将显示在视图的最后一行。
1. （可选）开始在表视图中添加新记录的信息
或
单击其名称可打开详细信息页面并在其中添加信息。

## 通过向记录类型提交请求表单来创建记录

当有人为记录类型创建请求表单并与您共享指向该记录类型的链接后，您可以提交一个请求，为记录类型创建记录。

有关信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。

Workfront用户和组织外部的用户均可向Planning记录类型提交请求并创建记录（如果它们具有指向请求表单的链接）。

有关信息，请参阅[提交Adobe Workfront计划请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)。

## 从CSV或Excel文件导入记录类型时创建记录

在使用CSV或Excel文件导入记录类型时，可以导入记录。

有关信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

## 通过从CSV或Excel文件导入记录来创建记录

从CSV或Excel文件导入信息时，您可以导入现有记录类型的记录。

有关信息，请参阅[通过从CSV或Excel文件导入信息创建记录](/help/quicksilver/planning/records/import-file-to-create-records.md)。

## 使用自动化创建记录

您可以在Workfront Planning中配置自动处理，激活自动处理后，创建从Planning记录触发的记录。 创建的记录会自动连接到从中触发自动化的记录。

您可以在Workfront Planning的记录页面中配置和激活自动化。 创建的连接记录将放置到运行自动化的记录类型的连接字段中。

有关信息，请参阅[使用Adobe Workfront Planning记录自动化创建对象](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)。



