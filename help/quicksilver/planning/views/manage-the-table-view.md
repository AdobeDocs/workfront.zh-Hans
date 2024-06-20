---
title: 管理表视图
description: 访问Adobe Workfront Planning中的记录类型页面时，您可以在表格视图中显示记录及其字段。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 0dd723b5-d674-4626-8fc2-7da41f3b7f35
source-git-commit: 7882b67578cd5b8792ce582ebab118c8993c9214
workflow-type: tm+mt
source-wordcount: '2543'
ht-degree: 3%

---

# 管理表视图

<!--
title: Manage the table view
description: You can display records in a table view when using Adobe Workfront Planning. 
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

访问Adobe Workfront Planning中的记录类型页面时，您可以在表格视图中显示记录及其字段。

有关记录视图以及如何管理它们的信息，请参阅 [管理记录视图](/help/quicksilver/planning/views/manage-record-views.md).

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
   <td role="rowheader"><p>Adobe Workfront许可证</p></td>
   <td>
   <p>任何</p> 
   <p>系统管理员只能访问他们创建的视图或与他们共享的视图。 </p>
  </td>
  </tr>

<tr>
   <td role="rowheader">访问级别配置</td>
   <td> <p>AdobeWorkfort计划没有访问级别控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理视图的权限</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">布局模板</td>
   <td> <p>系统管理员必须在布局模板中添加Planning区域。 有关信息，请参阅 <a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## 管理表视图 {#manage-a-table-view}

<!--insert screen shot of table view-->

创建表视图时，选定类型的所有记录都会显示在表中。 每一行是一个唯一记录，每一列是一个记录字段。 默认情况下，显示所有字段和所有记录。

要管理表视图，请执行以下操作：

1. 创建表格视图，如文章中所述 [管理记录视图](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/table-view-example.png)

1. （可选）单击 **行高**，然后从以下选项中进行选择以修改表行的高度：
   * 短
   * 中
   * 高

1. 更新以下视图元素，如以下子部分所述：
   * [列（或字段）](#add-columns-or-fields)
   * [行（或记录）](#add-rows-or-records)
   * [过滤器](#add-filters)
   * [分组](#add-groupings)
   * [排序](#add-a-sort)


### 添加列（或字段） {#add-columns}

表格视图的列标题显示与视图中记录关联的字段。 表格视图中显示的相同字段也会显示在记录的详细信息部分中。 有关更多信息，请参阅 [编辑记录](/help/quicksilver/planning/records/edit-records.md).

<!--this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default.-->

向视图添加列与向记录类型添加字段相同。

在一个表格视图中最多可添加500个字段（或列）。

1. 转到记录类型页面并选择 **表** 从“视图”下拉菜单中查看。

   <!-- replace above with this when view redesign: Go to a record type page and click a table view tab, or click **+ View **to add a new view, then choose **Table**. -->
1. 开始添加字段（或列），如文章中所述 [创建字段](/help/quicksilver/planning/fields/create-fields.md).

   您添加的列对访问记录类型的所有用户都可见，并且作为新字段添加到记录的页面上。

1. 执行以下操作之一以重新排序表中的列：

   * 抓住列标题并将其拖放到所需位置。 在您对表格进行其他调整之前，您移动的列会以蓝色背景短暂显示。

   * 单击 **字段** 在表工具栏中，按所需顺序拖放字段，然后单击 **字段可见性和顺序** 方框关闭它。

     ![](assets/fields-setting-table-view-toolbar-expanded.png)


     >[!TIP]
     >
     >* 默认情况下，“名称”字段始终是表视图中的第一个字段。 将此字段视为主字段。
     >
     >* 不能将“名称”字段移动到另一个位置，除非指定另一个字段作为主字段。 有关详细信息，请继续执行步骤4。 <!--accurate?-->
     >
     >

   * 通过更改主字段将第一列中的字段替换为其他字段。 有关详细信息，请继续执行步骤4。 <!--accurate?-->

1. （可选）将鼠标悬停在表首列中任何未显示的字段的列标题中的字段名称上，单击字段名称右侧的向下箭头，然后单击 **设置为主字段**.

   ![](assets/set-as-primary-field-option-table-view.png)

1. 单击 **设置字段** 以确认。

   该字段将成为主字段，这意味着它将显示为表视图的第一列。 前一个主字段移至第二列。

   主要字段成为记录的标题，显示在记录页面的标题区域中，以及记录显示的任何位置。 例如，记录标题显示在连接的字段和所有视图中。 有关主字段的更多信息，请参阅 [主字段概述](/help/quicksilver/planning/fields/primary-field-overview.md).

1. 单击并拖动列分隔线，然后将它们拖放到所需位置以增加列的宽度。

   >[!TIP]
   >
   >您对列宽和顺序所做的更改是永久性的，并且所有访问记录类型的用户都可以看到这些更改。

1. 将鼠标悬停在列标题上，单击向下箭头，然后单击 **隐藏字段**

   或

   单击 **字段** 并禁用与要隐藏的字段（或列）关联的切换。 此 **字段可见性和顺序** 框显示。

   >[!TIP]
   >
   >隐藏字段的数量显示在工具栏中的字段图标的左侧。


1. 单击 **字段** 图标，并启用与要在表格列中显示字段关联的切换。 默认显示所有字段。

1. 执行以下操作可快速查找与关键字匹配的记录：

   1. 单击 **Search** 图标 ![](assets/search-icon.png) 并开始键入与屏幕上所显示记录的任何字段关联的关键字。 正确匹配的数量显示在搜索项目旁边，具有正确匹配的字段会高亮显示。

      ![](assets/search-box-with-results-blue-outline-table-view.png)

      您可以使用屏幕上可见的任何单词或特殊字符。

      不能使用与表格视图中隐藏的字段关联的关键字。

   1. 按 **输入** 在键盘上转到下一个找到的字段。

   1. （可选）如果有多个匹配项，请单击搜索关键字右侧的向上箭头和向下箭头以查找表中的所有匹配项。

   1. 单击 **x** 图标，以清除搜索关键词。


### 添加行（或记录） {#add-rows}

表格视图的行显示所选记录类型的单个记录。

对于记录类型，最多可以有50,000条记录（或行）。

1. 转到记录类型页面并选择 **表** 从“视图”下拉菜单中查看。

<!-- replace above with this when view redesign: Go to a record type page and click a table view tab, or click **+ View **to add a new view, then choose **Table**. -->
1. 开始添加记录（或行），如文章中所述 [创建记录](/help/quicksilver/planning/records/create-records.md).

   您在表视图中添加的记录会立即保存，并且所有对工作区具有“查看”或更高权限的用户都可以看到这些记录。

1. （可选）向每条记录添加缩略图，然后单击 **字段** 选择表格右上角的切换开关， **缩略图** 字段以将其显示在主字段的左侧。 默认情况下，该复选框处于取消选中状态。

   有关信息，请参阅 [向记录添加缩略图](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. （可选）选择一行中的一个或多个记录，然后拖放 **句柄** 图标 ![](assets/handle-icon.png) 以重新排列行。

   >[!NOTE]
   >
   >如果对表视图至少应用一种排序，则无法对行重新排序。

   <!-- this is not possible right now:

    1. To reorder the rows, click the row header, drag and drop it in the desired location. 

        The changes you make to the row order are permanent and visible to all users who access the record type
    -->

<!-- this section below links from the timeline view; consider splitting them if they become different-->

### 添加过滤器 {#add-filters}

过滤器可帮助您减少屏幕上显示的信息量。

在表格视图中使用过滤器时，请考虑以下事项：
<!-- this list is almost identical to the one for the table view - update both-->

* 为表格视图创建的筛选器在应用于同一记录类型时独立于时间轴视图中的筛选器。

* 这些过滤器对于您选择的视图是唯一的。 同一记录类型的两个表视图可以应用不同的筛选器。 查看同一表格视图的两个用户会看到当前应用的同一筛选器。

* 您不能将您构建和应用的过滤器命名为表视图。

* 删除筛选器会将其从与您访问相同记录类型的任何人中移除，并使用与您使用的相同视图。

* 向表格视图添加筛选器与向时间轴视图添加筛选器相同。

* 您可以按连接的记录字段或查找字段进行筛选，但不能对允许链接到多个记录的字段进行筛选。

* 您可以引用与当前记录类型相距最多4级的字段。 例如，如果您正在为“活动”记录类型创建过滤器，并且活动连接到产品记录类型，而产品记录类型连接到营销活动记录类型，而营销活动记录类型又连接到Workfront项目，则您可以在为活动记录类型创建的过滤器中引用项目的预算。

要将过滤器添加到表格视图，请执行以下操作：

1. 为记录类型页面创建表视图，如文章中所述 [管理记录视图](/help/quicksilver/planning/views/manage-record-views.md).
1. 选择表格视图，然后单击 **过滤器** 在表格的右上角。
1. 单击 **添加条件** 并添加以下信息：

   * **选择字段** 要过滤的对象 <!-- the tip below might change-->

   * **选择一个选项** （或过滤器修饰符）以定义字段必须满足哪种条件

     下表显示了每种字段类型的可用修饰符。

     <table>
        <thead>
        <tr>
            <th><b>字段类型</b></th>
            <th><b>修饰符</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>单行、段落、公式 </td>
            <td><p>包含</p>
            <p>不包含</p>
            <p>是</p>
            <p>不是</p>
            <p>为空</p>
            <p>不为空</p></td>
        </tr>
        <tr><td>单选</td>
            <td><p>是</p>
            <p>不是</p>
            <p>是任何</p>
            <p>不是任何</p>
            <p>为空</p>
            <p>不为空</p></td>
        </tr>
        <tr>
            <td>多选，人员</td>
            <td><p>具有任何</p>
            <p>包含所有</p>
            <p>完全匹配</p>
            <p>没有</p>
            <p>为空</p>
            <p>不为空</p></td>
        </tr>
        <tr>
            <td>数字、百分比、货币</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>为空</p>
            <p>不为空</p></td>
        </tr>
        <tr>
            <td>日期</td>
            <td><p>是</p>
            <p>不是</p>
            <p>晚于</p>
            <p>早于</p>
            <p>介于</p><p>非介于</p>
            <p>为空</p><p>不为空</p></td>
        </tr>

     <tr>
            <td>复选框</td>
            <td><p>是</p>
        </tr>
        </tbody>
        </table>

   * 为所选字段选择值。

   ![](assets/filter-ui-table-view.png)

   您可以添加的筛选条件数量没有限制。

1. （可选）单击 **添加条件** 添加另一个筛选选项并重复上述步骤。 应用的过滤器数显示在过滤器图标的左侧。
1. 单击以下运算符以指示连接筛选条件的方式以及应如何应用：

   * **和**：必须满足所有指定的条件。
   * **或**：必须满足任何指定的条件。 这是默认选项。

   系统会自动过滤记录列表。  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. （可选）单击 **过滤器**，然后单击 **x** 图标以移除过滤器。 <!--right now you cannot "clear all" for filters, but this might come later-->

### 添加分组 {#add-groupings}

<!--this section exists in the timeline view too, but the display is slightly different, so I kept both steps; consider updating both sections if any updates to groupings are introduced-->

将分组应用于视图时，您可以按类似的信息对记录进行分组。

在表格视图中添加分组与向时间轴视图添加分组类似。

请考虑以下事项：

* 可以在表格视图和时间线视图中应用分组。 表格视图的分组独立于相同记录类型的时间线视图中的分组。
* 您可以在视图中应用3个级别的分组。 这些记录按您选择的分组顺序分组。
&lt;!—*在使用API时，您最多可以应用4个级别的分组。  — 现在查看此项 — >
* 这些分组对于您选择的视图是唯一的。 同一记录类型的两个表视图可以应用不同的分组。 查看同一表格视图的两个用户会看到当前应用的相同分组。
* 不能为表视图命名您构建的分组。
* 删除分组会将其从与您访问相同记录类型以及显示与您相同视图的任何人中删除。
* 您可以编辑分组下列出的记录。
* 您可以按连接的记录字段或查找字段进行分组，但不能对允许链接到多个记录的字段进行分组。
* 您可以引用与当前记录类型相距最多4级的字段。 例如，如果要为活动记录类型创建分组，并且活动连接到产品记录类型，而产品记录类型连接到营销活动记录类型，而营销活动记录类型又连接到Workfront项目，则可以在为活动记录类型创建的分组中引用项目的状态。
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

要添加分组，请执行以下操作：

1. 为记录类型创建时间线视图，如文章中所述 [管理记录视图](/help/quicksilver/planning/views/manage-record-views.md).
1. 单击 **分组** 表视图的右上角。

   ![](assets/grouping-ui-table-view-with-linked-fields.png)

1. 单击其中一个建议字段，或单击 **选择其他字段**，搜索其他字段，然后在列表中显示该字段时单击它。

   该分组将自动应用于表，并且记录显示在分组分离行下。

1. （可选）单击 **添加条件** 并重复上述步骤以添加最多3个分组。

   为分组选择的字段数将显示在分组图标旁边。

   ![](assets/grouping-applied-in-table-view.png)

1. （可选）内部 **记录分组条件** 框中，单击 **x** 图标为分组选择的字段的右侧，以删除分组

   或

   单击 **全部清除** 以删除所有字段。

1. 在 **记录分组条件** 方框关闭它。
1. （可选）单击 **+新记录** 在任何分组结束时添加新记录，然后刷新页面以将新记录添加到相应的分组。 <!--this might need to be changed when they add the Refresh button on the toolbar of the table view-->

### 添加排序 {#sort-information}

通过应用排序，您可以按指定顺序组织信息。

您可以对以下信息进行排序：

* 表格视图中的所有记录。 <!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

在表视图中排序记录时，请考虑以下事项：

<!-- if this is available for the timeline view, update both when you update one-->

* 排序对于您选择的视图是唯一的。 同一记录类型的两个表视图可以应用不同的排序标准。 查看同一表格视图的两个用户会看到当前应用的相同排序。

* 不能对您生成的排序进行命名并应用于表视图。

* 当您导航离开时，您创建的排序将保留。

* 您可以按记录类型的表视图中显示的字段数进行排序。

* 仅当链接的字段允许单个值，或者允许选择了汇总选项（总和、平均、最大值、最小值）的多选值时，它们才可排序。

* 删除分类标准会将其从与您访问相同记录类型的任何人中移除，并使用与您使用的相同视图。

* 您可以按连接的记录字段或查找字段进行排序，但不能对允许链接到多个记录的字段进行排序。

* 您可以引用与当前记录类型相距最多4级的字段。 例如，如果您正在为“活动”记录类型创建排序，并且活动连接到产品记录类型，而产品记录类型连接到营销活动记录类型，而营销活动记录类型又连接到Workfront项目，则您可以在为活动记录类型创建的排序中引用项目的“状态”。

排序 <!--ungrouped (add this when sorting for groupings will be available--> 记录，请执行以下操作：

1. 创建表格视图，如文章中所述 [管理记录视图](/help/quicksilver/planning/views/manage-record-views.md).
1. 单击 **排序** 图标 ![](assets/sort-icon.png) 在表格的右上角

   或

   将鼠标悬停在表视图中的列名上，单击列标题名右侧的向下箭头，然后单击 **按此字段排序**. 该字段将作为排序选择添加到表格视图右上角的排序图标中。

1. （视情况而定）在 **记录排序方式** 框中，单击其中一个建议的字段，或单击 **选择其他字段** 并搜索其他字段，然后在列表中显示该字段时单击该字段。

   排序将自动应用于表格视图，并且记录显示按您选择的标准排序。

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. （可选）单击 **添加条件**，并重复上述步骤以按其他字段排序。

   要排序的字段数显示在工具栏右上角排序图标的左侧。 您只能选择显示在表格视图列中的字段。

1. （可选）在 **记录排序方式** 框中，单击 **x** 图标来移除排序

   或

   单击 **全部清除** 以删除排序中的所有字段。

1. 在 **记录排序方式** 方框关闭它。

   ![](assets/sorting-in-table-view.png)

   表格中显示的信息根据您选择的标准排序。

   为排序选择的字段显示一个排序图标，后跟一个数字，指示应用排序的顺序。

<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->
