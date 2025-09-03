---
title: 编辑记录
description: 您可以在Adobe Workfront Planning中编辑记录信息。 必须先创建记录类型，然后才能开始创建和编辑记录。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 4e295b4fdbbde7439567ef2a4f4383ad8dea738c
workflow-type: tm+mt
source-wordcount: '2332'
ht-degree: 0%

---


# 编辑记录

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

您可以通过编辑与记录关联的字段值，在Adobe Workfront Planning中编辑记录信息。

必须先创建记录类型，然后才能开始创建和编辑记录。

有关信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

有关创建记录的信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。

&lt;！ — 在此提及，详细信息视图中的字段与表格视图中的字段相同 — 本文从“管理记录”视图链接，其中一个引用此信息 — >

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
   <td> <p>标准</p> 
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
   <td>  <p>为工作区和记录类型</a>贡献或更高权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr>

</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   


## 有关编辑记录的注意事项

* 如果您获得了工作区的权限，则可以编辑您创建的记录或由其他人创建的记录。
* 您可以从以下区域编辑记录字段：

   * 记录视图中的记录预览
   * 记录的详细信息页面
   * 内联，在表格视图中。
<!--* You can edit a record's dates from the following areas:
        * All areas listed above
        * <span class="preview">In a timeline view, by resizing the record bars</span>
         * <span class="preview">In a calendar monthly view, by resizing the record bars</span>
        For information, see [Create records](/help/quicksilver/planning/records/create-records.md). -->

<!-- when drag and drop is available replace the last 2 points with this:

* <span class="preview">In a timeline view, by resizing the record bars or dragging and dropping the record bars in a new position</span>
* <span class="preview">In a calendar view, by resizing the record bars when viewing it by month, or by dragging and dropping the record bars in a new position</span>
    For information, see [Create records](/help/quicksilver/planning/records/create-records.md).
-->

* 当用户编辑视图中的记录时，更改会立即在所有视图中可见，并且记录页面对所有其他用户可见。

* 以下类型的字段会自动更新，您无法手动编辑其值：
   * 来自其他记录的链接字段
   * 公式类型字段
   * 系统字段（“创建者”、“创建日期”、“上次修改者”、“上次修改日期”）
* 如果显示的记录链接到其他记录，则您正在编辑的记录的新信息将反映在链接的记录上。
* 不能批量编辑记录。<!--this will probably change-->
* 只有当URL以以下内容开头时，才会被识别为单行文本字段类型中的链接： http://、https://、ftp://或www。.
* 您可以向每张记录添加封面图像。 每个记录的图像都是唯一的，并且不适用于同一时间的所有记录。
* 您可以编辑记录页中的字段顺序并为记录添加封面图像。 有关详细信息，请参阅[管理记录页布局](/help/quicksilver/planning/records/manage-the-record-page.md)。

## 编辑记录

您可以从以下区域编辑记录：

* [表格视图](#edit-a-record-inline-in-the-table-view-of-a-record-type)
* [时间线视图](#edit-a-record-in-the-timeline-view-of-a-record-type)
* [日历视图](#edit-a-record-in-the-calendar-view-of-a-record-type)
* [在视图中预览记录](#edit-a-record-from-the-records-preview-in-a-view)
* [记录的页面](#edit-a-record-from-the-records-page)
* [“规划”部分中的Workfront对象](#edit-a-record-from-a-workfront-object-in-the-planning-section)

要编辑记录的日期，请执行以下操作：

* [调整时间轴和日历视图中记录栏的大小]

### 在记录类型的表视图中编辑内联记录

从表视图编辑记录时，会指示查看记录时其他用户正在编辑哪个字段。

有关详细信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

当您在分组或子分组中的最后一个记录之后添加新记录时，Workfront会自动更新新记录的分组中包含的字段。 如果需要，您可以手动编辑这些字段，并且可能会从分组中删除记录。

有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。

{{step1-to-planning}}

1. 单击要编辑其记录的工作区

   工作区将打开，记录类型显示为卡片。
1. 单击记录类型卡片。

   此时将打开记录类型页面。
1. （视情况而定）单击表视图的选项卡或单击&#x200B;**+视图**&#x200B;以创建表视图。 表格视图应为默认视图，除非您在上次访问记录类型时已在其他类型的视图中查看了该记录类型。

   与所选记录类型关联的记录将显示在表格视图中。
1. 单击记录行内部以开始编辑有关内联记录的信息。

   ![使用格式化表格视图编辑记录段落字段](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!TIP]
   >
   >  您无法编辑以下字段的信息，因为它们是只读的，Workfront会自动更新它们：
   >  
   >  * 通过连接记录类型创建的链接字段。 有关详细信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。
   >  * 以下类型的字段：“创建者”、“创建日期”、“上次修改者”、“上次修改日期”和“公式”字段。

1. （可选且有条件）编辑段落类型字段时，请使用以下&#x200B;**富文本**&#x200B;格式选项：

   * 粗体
   * 斜体
   * 下划线
   * 添加链接
   * 添加项目符号列表
   * 添加编号列表

   ![段落字段上的富文本工具栏](assets/rich-text-toolbar-on-paragraph-field.png)

1. （可选）双击连接的记录字段以将连接的记录或对象添加到另一记录。 有关详细信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。
1. 按键盘上的&#x200B;**Enter**&#x200B;键或单击行外以保存更改。 更改将自动保存。 **已保存**&#x200B;指示器短暂显示在表格视图的右上角，表示已保存更改。


1. （可选）要将信息从一个字段复制并粘贴到另一个字段，请执行下列操作之一：

   * 复制一个字段的一个或多个现有值，然后将它们粘贴到另一记录上相同类型的字段中
   * 单击某列的列标题以将其选中并复制，然后单击另一列的列标题并粘贴所复制列的内容。 列必须包含类似的字段类型。
   * 按住Shift键，单击在表中选取几行，复制选定行中的信息，然后单击另一行，然后将选定信息粘贴到新行中，并在新行之后粘贴以下几行。
   * 复制一个单元格中的信息，然后选择多个单元格并将相同的信息粘贴到多个单元格中。 您可以选择多个单元格，并将相同的信息粘贴到相邻行和列的多个单元格中。
   * 选择包含要复制信息的现有单元格的右下角，然后将其拖放到要粘贴相同信息的相邻单元格中。 所有单元格都必须包含相同类型的信息。

     ![在表视图中用于复制粘贴的可拖动右下角](assets/dragable-lower-right-corner-for-copy-paste-in-table-view.png)


   * 从外部源复制一个或多个单元格（例如，Excel文件），然后将它们粘贴到以下字段类型之一：

      * Workfront Planning连接字段。
      * 人员字段。 仅支持具有一个值的字段。

     您无法从外部源复制信息并将其粘贴到任何其他字段类型中，包括Workfront或AEM Assets连接字段。

   >[!NOTE]
   >
   >请考虑以下事项：
   >
   >* 使用以下键盘快捷键来复制和粘贴信息：
   >   * 复制：CTRL + C (对于Mac，为⌘ + C)
   >   * 粘贴：CTRL + V (⌘ + V for Mac)
   >
   >* 您不能在记录页面中复制和粘贴字段值。 仅记录类型的表视图支持此功能。
   >* 不能复制和粘贴以下字段类型的字段值：
   >
   >    * 连接记录类型时创建的查找字段。 您可以复制和粘贴链接的记录字段。 有关详细信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。
   >    * 以下类型的字段：“创建者”、“创建日期”、“上次修改者”、“上次修改日期”

1. （可选）使用以下键盘快捷键可撤消或重做编辑或复制和粘贴记录信息：

   * 按CTRL + Z (⌘ + Z表示Mac)可撤消更改
   * 按CTRL + Shift + Z (⌘ + Shift + Z用于Mac)以重做更改

   >[!TIP]
   >
   >    您可以在一行中多次使用键盘快捷键来撤消多项更改。

1. （可选）向记录中添加缩略图。 有关信息，请参阅[将缩略图添加到记录](/help/quicksilver/planning/records/add-thumbnails-to-records.md)。


### 在记录类型的时间线视图中编辑记录

<!--add another step about drag and drop here when that is available-->

1. 在时间线视图中打开记录类型页面。 有关信息，请参阅[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。
<!--
1. <span class="preview">Hover over the ends of a record's bar, click, drag and drop its margin to another date. This automatically updates either the start or end date of the record.</span>  

    <span class="preview">![Left-end bar on timeline view to resize](assets/left-end-bar-handle-to-resize-timeline-view.png)</span>

-->

1. 单击记录栏以打开其详细信息区域并编辑所有字段。

   有关信息，请参阅本文中[在视图](#edit-a-record-from-the-records-preview-in-a-view)中编辑记录预览中的记录。

### 在记录类型的日历视图中编辑记录

<!--add another step about drag and drop here when that is available-->

1. 在日历视图中打开记录类型页面。 有关信息，请参阅[管理日历视图](/help/quicksilver/planning/views/manage-the-calendar-view.md)。
<!--
1. (Conditional) Select **Month** in the upper-right dropdown menu.
1. <span class="preview">Hover over the ends of a record's bar, click, drag and drop its margin to another date. This automatically updates either the start or end date of the record.</span>  

    <span class="preview">![Left-end bar on calendar view to resize](assets/left-end-bar-handle-to-resize-calendar-monthly-view.png)</span>
-->

1. 单击记录栏以打开其详细信息区域并编辑所有字段。

   有关信息，请参阅本文中[在视图](#edit-a-record-from-the-records-preview-in-a-view)中编辑记录预览中的记录。

### 在视图中编辑记录预览中的记录

{{step1-to-planning}}

1. 单击要编辑其记录的工作区

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。

1. 从任何类型的视图中，单击记录

   或

   从表格视图中，单击第一列中的&#x200B;**打开详细信息**&#x200B;图标![在表格名称字段](assets/open-details-icon-in-table-name-field.png)中打开详细信息图标。 记录的预览将在视图中打开。

   ![详细信息框](assets/details-box.png)

1. （可选）单击记录标题右侧的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**重命名**。 这将更新显示为记录标题的字段。

   记录的标题是在表格视图中查看记录时显示的主要字段。 有关信息，请参阅[主字段概述](/help/quicksilver/planning/fields/primary-field-overview.md)。

1. 开始编辑记录预览中的字段信息。

   >[!TIP]
   >
   >  您无法编辑以下字段的信息，因为它们是只读的，Workfront会自动更新它们：
   >  
   >  * 通过连接记录类型创建的其他记录的查找字段。 有关详细信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。
   >  * 以下类型的字段：“创建者”、“创建日期”、“上次修改者”、“上次修改日期”和“公式”字段。

1. （可选）单击&#x200B;**添加封面**&#x200B;以将封面图像添加到记录。 有关详细信息，请参阅[将封面图像添加到记录](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)。

1. （可选）将鼠标悬停在缩略图图标上，然后单击&#x200B;**更多** ![更多菜单](assets/more-menu.png) > **编辑缩略图**&#x200B;以添加缩略图图像。 有关信息，请参阅[将缩略图添加到记录](/help/quicksilver/planning/records/add-thumbnails-to-records.md)。

   Workfront会自动保存您所做的更改。

1. （可选）单击记录预览框右上角的&#x200B;**实时指示器** ![实时指示器图标](assets/real-time-indicator-icon.png)，然后启用&#x200B;**显示协作者**&#x200B;设置以实时突出显示其他人正在编辑的字段。

   此区域显示同时访问记录的所有用户的名称和头像。

   禁用该设置时，头像和名称将列在实时指示器区域中，并且正在编辑的字段不会突出显示。

   ![实时指示器扩展记录预览框](assets/real-time-indicator-expanded-record-preview-box.png)

1. （可选）单击记录详细信息页面&#x200B;**中的**&#x200B;导出![菜单](assets/export-icon-in-record-details-page.png)导出图标以导出记录详细信息。 有关信息，请参阅[导出记录的详细信息](/help/quicksilver/planning/records/export-the-record-page.md)。

1. （可选）单击记录预览右上角的&#x200B;**在新标签中打开**&#x200B;图标![在新标签中打开详细信息](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it-->以在新标签中打开记录页面。 继续编辑记录，如本文中[从记录的页面](#edit-a-record-from-the-records-page)部分编辑记录中所述。

### 从记录的页面编辑记录

{{step1-to-planning}}

1. 单击要编辑其记录的工作区

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。

1. 执行下列操作之一：

   * 从任何视图中，访问记录的预览，如本文中[从记录的预览中编辑记录](#edit-a-record-from-the-records-preview-in-a-view)部分中所述，然后单击记录预览右上角的&#x200B;**在新标签中打开**&#x200B;图标![在新标签中打开详细信息](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it-->以在新标签中打开记录的页面。

   * 在&#x200B;**表**&#x200B;视图中，将鼠标悬停在记录名称上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**查看**

     ![记录行的上下文菜单](assets/contextual-menu-for-record-row.png)

     此时将打开记录页面。

     ![详细信息页面](assets/details-page.png)

1. （可选）单击记录标题右侧的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**重命名**。 这将更新显示为记录标题的字段。

   记录的标题是在表格视图中查看记录时显示的主要字段。 有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

1. 单击记录页面上的任何可编辑字段以编辑它。

   >[!TIP]
   >
   >  您无法编辑以下字段的信息，因为它们是只读的，Workfront会自动更新它们：
   >  
   >  * 通过连接记录类型创建的链接字段。 有关详细信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。
   >  * 以下类型的字段：“创建者”、“创建日期”、“上次修改者”、“上次修改日期”和“公式”字段。

1. （可选）单击显示任何字段右侧的信息图标以查看字段的说明。
1. （可选）单击&#x200B;**添加封面**&#x200B;以将封面图像添加到记录

   或

   将鼠标悬停在现有封面图像上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png) > **上传**&#x200B;以添加新的封面图像来记录。

   有关详细信息，请参阅[将封面图像添加到记录](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)。

1. （可选）将鼠标悬停在现有缩略图上，或悬停在详细信息页面上的&#x200B;**缩略图图标** ![记录缩略图图标](assets/record-thumbnail-icon-on-details-page.png)上，然后单击&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png) > **编辑缩略图**&#x200B;以添加记录的缩略图。

   有关详细信息，请参阅[将缩略图添加到记录](/help/quicksilver/planning/records/add-thumbnails-to-records.md)。

   Workfront会自动保存您所做的更改。

1. （可选）单击记录页面右上角的&#x200B;**实时指示器** ![实时指示器图标](assets/real-time-indicator-icon.png)，然后启用&#x200B;**显示协作者**&#x200B;设置以实时突出显示其他人正在编辑的字段。

   此区域显示同时访问记录的所有用户的名称和头像。

   禁用该设置时，头像和名称将列在实时指示器区域中，并且正在编辑的字段不会突出显示。

   ![实时指示器扩展记录预览框](assets/real-time-indicator-expanded-record-preview-box.png)

1. （可选）单击记录详细信息页面&#x200B;**中的**&#x200B;导出![菜单](assets/export-icon-in-record-details-page.png)导出图标以导出记录详细信息。 有关信息，请参阅[导出记录的详细信息](/help/quicksilver/planning/records/export-the-record-page.md)。


## 在Planning部分中编辑来自Workfront对象的记录

将记录与Workfront对象连接后，您可以在Workfront中编辑该对象的Planning部分的Workfront Planning记录。

有关详细信息，请参阅[管理来自Workfront对象的记录连接](/help/quicksilver/planning/records/manage-records-in-planning-section.md)。


<!--

<div class="preview">

## Add new choices to an existing select field when editing records in the table view

You can add new choices to an existing single- or multi-select field when editing records in the table view. 

>[!IMPORTANT]
>
>The functionality described in this section is available only in the table view. It is not available in any other areas where single- or multi-select fields display.


**EXAMPLE**

You might have a single-select field called Status that has the choices New and Closed, and you want to add a choice for an In progress status. You can add the choice by doing one of the following things:

* Editing the field. For information, see [Edit fields](/help/quicksilver/planning/fields/edit-fields.md)
* Adding a new option while editing the record in the table view, as described below. 


To add a new choice to an existing select field when editing a record: 

1. Go to a record type page and open the table view. 
1. Add the single- or multi-select field that you would like to add a choice to in the table view as a new column. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md). 
1. Start editing the field inline by double-clicking the cell for the field. 
1. Type the name of the choice you want to add, then click **Add choice**.

    ![Add choice in single-select field in table view](assets/add-choice-in-table-view-for-single-select-field.png)

    The new choice is added immediately to the single-select field. 

</div>

-->