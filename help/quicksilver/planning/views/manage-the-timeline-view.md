---
title: 管理时间线视图
description: 在Adobe Workfront Planning记录类型页面的时间轴视图中访问和编辑记录。 使用筛选器、分组和设置自定义时间轴。 使用“划分”功能显示连接的记录。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '1941'
ht-degree: 0%

---

# 管理时间线视图

<!--
title: Manage the timeline view 
description: You can display records in a timeline view, when accessing the record type page in Adobe Workfront Planning. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

访问Adobe Workfront Planning中的记录类型页面时，可在时间轴视图中显示记录。

有关记录视图的信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

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
   <p>新增：标准</p>
   或
   <p>当前：计划 </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> Adobe Workfront Planning没有访问控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理视图的权限</p>  
   <p>查看对视图的权限以临时更改视图设置</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> <p>有关信息，请参阅<a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>。 </p> 
</td>
  </tr>
 </tbody>
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


<!--EDIT PERMISSIONS AND ACCESS AND REPLACE THE table above with the following table at Planning GA release: 
## Access requirements

You must have the following to be able to access Workfront Planning: 

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
<p>Any of the following new Workfront plans:</p>
<ul><li>Select</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is not available for legacy Workfront plans</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning plan*</p></td>
   <td>
<p>Any of the following Workfront Planning plans:</p>
<ul><li>Planning</li>
<li>Planning Plus</li>
</ul>
<p>For more information about what is included in each Workfront Planning plan, see <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront pricing and packaging</a>. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <ul><li><p>Any, to view Workfront Planning information</p></li>
   <li><p>Standard, to create workspaces</p></li></ul>
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
   <td>
   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">Customize the Main Menu using a layout template</a> and and <a href="../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md">Assign users to a layout template</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  

*********ensure that the link ^^^^^^^^above^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************

-->


## 管理时间线视图 {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

创建时间线视图时，所选记录类型的所有记录都按时间顺序显示在时间线中。

请考虑以下事项：

* 仅当至少有两个日期字段与记录类型关联时，才能创建时间轴视图。 当有一个或没有与记录类型关联的日期字段时，“时间轴”视图选项将灰显。

  构建时间线视图时，您可以从以下日期字段中选择：

   * 记录日期
   * 记录系统生成的字段：创建日期、上次修改日期
   * 来自连接的记录或对象类型的查找日期。
* 根据与记录关联的日期，在以下场景中，某些记录可能不会显示在时间轴视图中：

   * 当开始日期和结束日期没有值时
   * 当“开始”或“结束”日期没有值时
   * 当开始日期在结束日期之后时

要管理时间线视图，请执行以下操作：

1. 转到要查看其时间线的记录类型页面。
1. 创建时间线视图，如[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)一文中所述。

   ![](assets/timeline-view-example.png)

   与所选记录类型关联的记录在时间轴中显示为条形，默认情况下，这些记录按其开始日期的时间顺序排序。

   >[!TIP]
   >
   >    时间轴中记录的排序在压缩视图中不可见。

1. （可选且有条件）记录名称被截断时，将鼠标悬停在记录栏上会显示记录的全名和其他信息。

1. 执行以下操作之一可在时间轴中导航：

   * 单击左右图标或使用水平滚动条在时间轴中前后移动。 刷新页面将保留所选的时间范围。
   * 单击&#x200B;**今天**&#x200B;可将时间线居中到今天的日期。
   * 从时间范围下拉菜单中选择以下选项之一以更新时间增量：

      * 年
      * 季度
      * 月
1. 单击&#x200B;**切换到标准**&#x200B;视图以单独行<!--check to see if they updated the name of the setting here-->显示记录

   或

   单击&#x200B;**切换到紧凑视图**&#x200B;可显示日期不相交的记录。<!--check to see if they updated the name of the setting here-->

   默认情况下，记录显示在“压缩”视图中。

1. 执行以下操作可快速查找与关键字匹配的记录：

   1. 单击&#x200B;**搜索**&#x200B;图标![](assets/search-icon.png)并开始键入与屏幕上显示的记录的任何字段相关联的关键字。 正确匹配的数量显示在搜索项目旁边，具有正确匹配的记录会高亮显示。

      ![](assets/search-box-and-results-timeline-view.png)

      您可以使用屏幕上可见的任何单词或特殊字符。

      不能使用与不在时间轴视图中显示的字段关联的关键字。

   1. 在键盘上按Enter键以转到下一个找到的字段。
   1. （可选）如果有多个匹配项，请单击搜索关键字右侧的向上箭头和向下箭头以查找表中的所有匹配项。
   1. 单击搜索框中的&#x200B;**x**&#x200B;图标以清除搜索关键字。

1. 更新以下视图元素，如以下子部分所述：
   * [过滤器](#add-filters)
   * [分组](#add-grouping)
   * [设置](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->

### 添加过滤器

您可以使用过滤器减少屏幕上显示的信息量。

在时间线视图中使用过滤器时，请考虑以下事项：

<!-- this list is almost identical to the one for the table view - update both-->

* 您为时间轴视图创建的筛选器与应用于同一记录类型的任何其他视图中的筛选器独立工作。

* 这些过滤器对于您选择的视图是唯一的。 同一记录类型的两个时间轴视图可以应用不同的筛选器。

* 查看同一时间轴视图的两个用户会看到当前应用的同一过滤器。

* 您无法为时间线视图命名您构建的过滤器。

* 删除筛选器会将其从与您访问相同记录类型以及显示与您相同的视图的任何人中删除。

* 在时间轴视图中添加筛选器与在表视图中添加筛选器相同。

  有关详细信息，请参阅文章[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)中的“添加筛选器”部分。

* 您可以按连接的记录字段或查找字段进行筛选。
* 您可以按显示多个值的查找字段进行筛选。


### 添加分组

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

将分组应用于视图时，您可以按类似的信息对记录进行分组。

在时间轴视图中添加分组与将分组添加到表格视图类似。

在时间线视图中使用分组时，请考虑以下事项：

* 可以在表格视图和时间线视图中应用分组。 表格视图的分组独立于相同记录类型的时间线视图中的分组。
* 您可以在视图中应用3个级别的分组。 这些记录按您选择的分组顺序分组。
&lt;！—*在使用API时，您最多可以应用4个级别的分组。  — 现在查看此项 — >
* 这些分组对于您选择的视图是唯一的。 同一记录类型的两个表视图可以应用不同的分组。 查看同一表格视图的两个用户会看到当前应用的相同分组。
* 不能为表视图命名您构建的分组。
* 删除分组会将其从与您访问相同记录类型以及显示与您相同视图的任何人中删除。
* 您可以编辑分组下列出的记录。
* 您可以按连接的记录字段或查找字段分组。
* 当按查找字段对具有多个值（尚未由聚合器汇总）的字段进行分组时，记录将按字段值的每个唯一组合进行分组。
* 您可以引用与当前记录类型相距最多4级的字段。 例如，如果要为活动记录类型创建分组，并且活动连接到产品记录类型，而产品记录类型连接到营销活动记录类型，而营销活动记录类型又连接到Workfront项目，则可以在为活动记录类型创建的分组中引用项目的状态。
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

要在时间轴视图中添加分组，请执行以下操作：

1. 为记录类型创建时间线视图，如[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)一文中所述。
1. 单击时间轴视图右上角的&#x200B;**分组**。

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. 单击其中一个建议的字段，或单击&#x200B;**选择其他字段**，搜索其他字段，然后在列表显示该字段时单击它。

   分组将自动应用于时间轴，并且记录显示在分组框中。

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. （可选）重复上述步骤以添加最多3个分组。

   为分组选择的字段数将显示在分组图标旁边。

   <!-- update screen shot with view redesign-->

   ![](assets/grouping-applied-in-timeline-view.png)

1. （可选）在&#x200B;**按**&#x200B;对记录进行分组框中，单击为分组选择的字段右侧的&#x200B;**x**&#x200B;图标以删除该分组

   或

   单击&#x200B;**全部清除**&#x200B;可删除所有字段。

1. 单击&#x200B;**按**&#x200B;分组记录框外部以将其关闭。
1. （可选）单击&#x200B;**Settings**，然后单击&#x200B;**Color**&#x200B;进行颜色代码分组。 有关详细信息，请参阅本文中的[编辑时间线视图设置](#edit-the-timeline-view-settings)部分。
   <!--1. (Optional) Click **Breakdown** to display connected records on the timeline. For information, see the section [Use the Breakdown feature to display connected records in the timeline view](#break-down-connected-records-in-the-timeline-view)-->

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### 编辑时间线视图设置 {#edit-the-timeline-view-settings}

更新时间线视图设置，以指示信息在视图的时间线部分中显示什么及如何显示。

1. 为记录类型创建时间线视图，如[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)一文中所述。
1. 单击&#x200B;**设置**。
1. 单击左侧面板中的&#x200B;**日期和时间**，然后选择要显示在时间轴上的&#x200B;**开始日期**&#x200B;和&#x200B;**结束日期**。 您可以选择默认的“开始”和“结束”日期，也可以选择任何可用的日期字段。 表示记录的条形图从您为开始日期指定的日期开始，结束日期对应于结束日期。

   >[!NOTE]
   >
   >对于开始日期或结束日期没有值或者开始日期晚于结束日期的记录，不会显示在时间轴视图中。

1. 单击左侧面板中的&#x200B;**栏样式**&#x200B;以指示要在记录栏上显示的字段。

   默认情况下会选择记录的主字段（或标题），如在记录的表格视图中定义的那样。<!--adjust this when the primary field is released??-->

1. （可选且视情况而定）如果您将缩略图添加到记录，请选择“缩略图”选项以在记录栏中显示与记录关联的图像。

   >[!NOTE]
   >
   >    必须先在表格视图中添加缩略图，然后才能在时间轴视图中显示它们。 有关详细信息，请参阅[将缩略图添加到记录](/help/quicksilver/planning/records/add-thumbnails-to-records.md)。

1. 单击&#x200B;**添加字段**&#x200B;可向记录栏添加最多4个字段。
1. 在&#x200B;**搜索字段**&#x200B;框中单击，然后单击要添加字段。

   >[!TIP]
   >
   >   * 必须先创建这些字段，然后才能将其添加到记录栏。
   > 
   >   * 您必须至少选择一个字段。 默认情况下已选择&#x200B;**名称**。

   右侧将显示时间轴上栏的外观。

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. 单击左侧面板中的&#x200B;**颜色**，以自定义时间轴中记录和分组的颜色。

   ![](assets/color-tab-timeline-view.png)

1. （视情况而定，可选）如果向时间轴视图添加了分组，请从以下选项中进行选择，以在&#x200B;**设置分组颜色**&#x200B;部分中设置分组的颜色：

   * **默认（灰色）**：分组的颜色设置为灰色。 这是默认设置。
   * **字段值**：分组的颜色与您分组依据的字段的颜色匹配。

     >[!NOTE]
     >
     >    * 您只能将颜色与具有颜色编码选项的字段匹配。 例如，可以将颜色与“状态”字段匹配，或可与颜色关联的选项进行匹配。
     >    
     >    * 不能将颜色与链接记录或对象类型中的查找字段匹配。


   例如，多选或单选字段可以具有颜色编码选项。

   如果按没有颜色编码选项的字段分组，则分组颜色保持灰色。

   >[!TIP]
   >
   >如果未将分组添加到时间轴视图，则不会显示此部分。

1. 在&#x200B;**设置记录颜色**&#x200B;部分中，从以下选项中进行选择以设置记录的颜色：

   * **记录类型**：记录的颜色与您选择的记录类型的颜色相匹配。 这是默认选项。
   * **字段值**：记录的颜色与您指定的字段的颜色匹配。 继续执行步骤10。<!--ensure this stays accurate-->
   * **分组**：记录的颜色与您为分组指定的颜色相匹配。 当未将分组应用于时间轴视图时，此选项将灰显。
   * **无**：记录显示在白色栏中。

1. （视情况而定）如果您为记录颜色选择了&#x200B;**字段值**，请从&#x200B;**将记录颜色与**&#x200B;下拉菜单中选择一个字段。

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   下拉菜单中仅显示具有颜色编码选项的字段。

   例如，多选或单选字段可以具有颜色编码选项。

   如果对于所选的记录类型没有带颜色编码选项的字段，则此选项将灰显。

1. 单击&#x200B;**保存**。

   这些记录将按照您选择的规范显示在时间轴视图中。

<!--
### Use the Breakdown feature to display connected records in the timeline view

You can display connected records in a record's timeline view by using the Breakdown feature. Breaking down records by their connections allows you to view the timelines of other connected records and understand how they might affect the performance and deadlines of your records. 

#### Considerations when using the Breakdown feature

* You can display connected records or objects under the records of the selected record type in the timeline view. 
* You can display the following in the timeline view, using the Breakdown feature:
    * Workfront Planning records connected to the selected record type. 
    * Workfront (*************or AEM Assets*************)  object types connected to the selected record type.
    * Workfront Planning records or objects from other application that are connected to records connected to the selected record type. 
    
        For example, you might connect campaigns to portfolios. In addition, you might connect  another record type, products, with projects, as well as with campaigns. When you build the campaign timeline view, you can break down the campaigns by portfolios, products, and projects. 

* You cannot display object types that are connected only to Workfront objects in Workfront, but are not connected to a Workfront Planning record type. You can only display object or record types that are connected in Workfront Planning. 

    For example, tasks, are connected to projects in Workfront. Using the Breakdown feature, you can display projects that are connected to campaigns in Planning, but not tasks connected to projects in Workfront. 

    If you want to display both portfolios and projects in the timeline view of a Workfront Planning record type, both the portfolios and the projects must be connected to the Planning record or to a record connected to the Planning record whose timeline view you are managing.
* You can only display record types that are associated with at least two date fields. 
* The date fields for the record types you want to display in the timeline view must be visible in the table view of the selected record type, as lookup fields. 
* The Start and End dates of the record types you want to display in the timeline view must by in chronological order. For example, if a record has a Start date of January 31 and an End date of January 1, it does not display in the timeline view. For more information, see the section [Manage a timeline view](#manage-a-timeline-view) in this article. 
* There is a limit of 5 record types that you can include in a record's breakdown. 


#### Break down connected records in the timeline view

1. Create a timeline view for a record type, as described in the article [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 
1. Click **Breakdown**.
1. Expand the **Select a linked record type** box and select a connected record type. (**************add new screen shot***************)

    ![](assets/breakdown-picker-and-button-on-timeline.png)

    >[!TIP]
    >
    >    If you do not have any connected records, or if the connected records do not have at least two date fields, the **Select a linked record type** box is not available.

1. Choose a **Start date** and an **End date field**.

    >[!TIP]
    >
    >    The Start and End dates must be sequential. If the End date is before the Start date, no records will display in the timeline. 

    A right-pointing arrow displays on the selected record's bar in the timeline, if they they are connected with other records. 

    ![](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)    


1. (Optional) Repeat the steps above to add more connected records. 

    >[!TIP]
    >
    >    You can add up to 5 connected records in a timeline using the Breakdown feature. 


-->