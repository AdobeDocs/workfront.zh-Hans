---
title: 创建记录
description: 使用Adobe Workfront Planning时，记录是记录类型的实例。 您可以在Workfront Planning中为每个记录类型创建唯一记录，方法是：将记录手动添加到表视图中，从列表中导入记录，复制记录，或在将其连接到其他记录时创建记录。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: b27b01e1efacc3fc459cec0a53b2c11cbe5e132b
workflow-type: tm+mt
source-wordcount: '2388'
ht-degree: 0%

---


# 创建记录

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

在Adobe Workfront Planning中，记录是记录类型的实例。

您可以通过执行以下操作之一来创建记录：

* [通过从记录类型表视图内联添加记录来创建记录](#create-records-by-adding-them-inline-from-the-record-type-table-view)
* [使用任何记录类型视图中的“新建记录”或“请求记录”按钮创建记录](#create-records-using-the-new-record-or-request-record-button-from-any-record-type-view)
* [从外部列表中复制并粘贴记录列表](#create-records-by-copying-and-pasting-them-from-an-external-list)
* [从表视图复制记录](#create-records-by-duplicating-them)
* [在连接其他记录时创建记录](#create-records-as-you-connect-them)
* [通过向记录类型提交请求表单来创建记录](#create-records-by-submitting-a-request-form-to-a-record-type)
* [通过从CSV或Excel文件导入信息创建记录](#create-records-by-importing-records-from-a-csv-or-excel-file)
* [使用自动化创建记录](#create-records-by-using-automations)

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



