---
title: 编辑记录
description: 您可以在Adobe Workfront Planning中编辑记录信息。 必须先创建记录类型，然后才能开始创建和编辑记录。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '2731'
ht-degree: 0%

---


# 编辑记录

<!--keep the choice values information in yellow till Jan 2026-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

您可以通过编辑与记录关联的字段值，在Adobe Workfront Planning中编辑记录信息。

必须先创建记录类型，然后才能开始创建和编辑记录。

有关信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

有关创建记录的信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。

&lt;！ — 在此提及，详细信息视图中的字段与表格视图中的字段相同 — 本文从“管理记录”视图链接，其中一个引用此信息 — >

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
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>任何Workfront和任何Planning包</p> <p>任何工作流和任何计划包</p>
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>向工作区和记录类型提供或更高权限  </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p> </td> 
  </tr>   
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>Standard</p> 
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> -->

## 有关编辑记录的注意事项

* 如果您获得了工作区的权限，则可以编辑您创建的记录或由其他人创建的记录。
* 您可以从以下区域编辑记录字段：

   * 记录视图中的记录预览
   * 记录的详细信息页面
   * 内联，在表格视图中。
   * 日历和时间轴视图，在调整记录大小或拖放记录时。 这将更新记录的日期。

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

     您无法从外部源复制信息并将其粘贴到任何其他字段类型中，包括Workfront或其他应用程序的连接字段。

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

1. 将鼠标悬停在记录栏的末尾上，单击，将其边距拖放到另一个日期。 这会自动更新记录的开始日期或结束日期。

   时间轴视图上的![左端栏可调整大小](assets/left-end-bar-handle-to-resize-timeline-view.png)

1. 单击并保留一个记录栏，然后将它拖放到另一个位置以更新其时间轴和日期。 记录的开始日期和结束日期会自动更新。

1. 单击记录栏以打开其详细信息区域并编辑所有字段。

   有关信息，请参阅本文中[在视图](#edit-a-record-from-the-records-preview-in-a-view)中编辑记录预览中的记录。

### 在记录类型的日历视图中编辑记录

<!--add another step about drag and drop here when that is available-->

1. 在日历视图中打开记录类型页面。 有关信息，请参阅[管理日历视图](/help/quicksilver/planning/views/manage-the-calendar-view.md)。
1. （视情况而定）将鼠标悬停在日历视图中记录栏的末尾上，然后单击，将其边距拖放到其他日期。 这会自动更新记录的开始日期或结束日期。

   ![日历视图上的左侧栏以调整大小](assets/left-end-bar-handle-to-resize-calendar-monthly-view.png)

1. 单击并保留一个记录栏，然后将它拖放到另一个位置以更新其时间轴和日期。 记录的开始日期和结束日期会自动更新。

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

## 在更新字段设置值时编辑单选或多选字段设置

<!--some of this information is also available in Edit fields article - update both when necessary-->

当更新单选或多选字段中的信息时，可以向该字段添加新选项，而无需编辑该字段。

>[!IMPORTANT]
>
>本节中介绍的功能仅在表视图中可用。 它不适用于显示单选或多选字段的任何其他区域。

**示例**

您可能有一个名为Status的单选字段，该字段具有选项New和Closed，并且您要为In progress状态添加选项。 您可以通过执行以下操作之一来添加选择：

* 编辑字段。 有关信息，请参阅[编辑字段](/help/quicksilver/planning/fields/edit-fields.md)
* 在表格视图中编辑记录时添加新选项，如下所述。

要在编辑记录时向现有选择字段添加新选择，请执行以下操作：

1. 转到记录类型页面并打开表格视图。
1. 在表格视图中添加要向其添加选择的单选或多选字段作为新列。 有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。
1. 通过双击字段的单元格，开始内联编辑字段。
1. 键入要添加选择的名称，然后单击&#x200B;**添加选择**。

   ![在表视图的单选字段中添加选项](assets/add-choice-in-table-view-for-single-select-field.png)

   新选项会立即添加到单选字段中。

   <span class="preview">每个选择中还新增了一个选择值。 您可以在API调用或其他集成中使用选择值。 有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。</span>

