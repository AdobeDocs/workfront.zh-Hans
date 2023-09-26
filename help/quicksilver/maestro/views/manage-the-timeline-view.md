---
title: 管理时间线视图
description: 访问AdobeMaestro中的记录类型页面时，可以在时间轴视图中显示记录。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 1%

---


# 管理时间线视图

<!--
title: Manage the timeline view in Adobe Maestro
description: You can display records in a timeline view, when accessing the record type page in Adobe Maestro. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

访问AdobeMaestro中的记录类型页面时，可以在时间轴视图中显示记录。

有关主视图的信息，请参见 [在Adobe大师中管理记录视图](../views/manage-record-views.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe产品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵公司必须注册AdobeMaestro封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
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
   <td role="rowheader">访问级别</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">布局模板</td>
   <td> <p>系统管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/grant-access.md">授予对Adobe大师的访问权限</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 管理时间线视图 {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

创建时间线视图时，所选记录类型的所有记录都按时间顺序显示在时间线中。

请考虑以下事项：

* 仅当至少有两个日期字段与记录类型关联时，才能创建时间轴视图。 当有一个或没有与记录类型关联的日期字段时，“时间轴”视图选项将灰显。
* 根据与记录关联的日期，在以下场景中，某些记录可能不会显示在时间轴视图中：

   * 当开始日期和结束日期没有值时
   * 当“开始”或“结束”日期没有值时
   * 当开始日期在结束日期之后时

<!--these are NOT available now because there won't be a table for the timeline view for the near future, per Andy: 
* The records displayed in the timeline view also display in a view-only table to the left of the timeline. 
* Each row in the table and each bar on the timeline represent the same record. 
* Each column in the table is a record field. The columns of this table are preconfigured and cannot be customized. 
* Only a limited number of fields (or columns) display in the timeline view table. 
* You cannot do the following in a timeline view:
     * Add rows or records
     * Add columns or fields
     * Edit record information
-->

创建时间线视图时，所选记录类型的所有记录在时间线中默认显示为条形。

要管理时间线视图，请执行以下操作：

1. 转到要查看其时间线的记录类型页面。
1. 创建时间线视图，如文章所述 [管理记录视图](../views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   与您选择的记录类型关联的记录以时间轴的形式显示为条形。

1. 执行以下操作之一可在时间轴中导航：

   * 单击左右图标或使用水平滚动条在时间轴中前后移动。
   * 单击 **今天** 将时间线居中到今天的日期。
   * 从时间范围下拉菜单中选择以下选项之一以更新时间增量：

      * 年
      * 季度
      * 月
1. 单击 **切换到标准** 以单独行显示记录的视图 <!--check to see if they updated the name of the setting here-->

   或

   单击 **切换到紧凑视图** 在同一行中显示其日期不相交的记录。 <!--check to see if they updated the name of the setting here-->

   默认情况下，记录显示在“压缩”视图中。

1. 更新以下视图元素，如以下子部分所述：
   * [筛选条件](#add-filters)
   * [分组](#add-grouping)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->
   * [设置](#edit-the-timeline-view-settings)

### 添加过滤器

过滤器可帮助您减少屏幕上显示的信息量。

在时间线视图中使用过滤器时，请考虑以下事项：

<!-- this list is almost identical to the one for the table view - update both-->

* 为时间轴视图创建的筛选器在应用于同一记录类型时独立于表格视图中的筛选器。

* 这些过滤器对于您选择的视图是唯一的。 同一记录类型的两个时间轴视图可以应用不同的筛选器。 查看同一时间轴视图的两个用户会看到当前应用的同一过滤器。

* 不能为您构建并应用于时间线视图的过滤器命名。

* 删除筛选器会将其从访问与您相同记录类型的任何人中移除，并使用与您使用的相同视图。

在时间轴视图中添加筛选器与在表视图中添加筛选器相同。

有关更多信息，请参阅文章中的“添加过滤器”部分 [管理表视图](../views/manage-the-table-view.md).

### 添加分组

<!-- if groupings are identical between the table and the timeline, consider replacing this section with this: 

Adding groupings in the timeline view is identical to adding filters in the table view. 

For more information, see the "Add filters" section in the article [Manage the table view](../views/manage-the-table-view.md). -->


将分组应用于视图时，您可以按类似的信息对记录进行分组。

在时间线视图中使用分组时，请考虑以下事项：

* 可以在表格视图和时间线视图中应用分组。 表格视图的分组独立于相同记录类型的时间线视图中的分组。
* 您可以在Maestro视图中应用3个级别的分组。 这些记录按您选择的分组顺序分组。
* 在使用API时，您最多可以应用4个级别的分组。

要添加分组，请执行以下操作：

1. 创建时间线视图，如文章所述 [管理记录视图](../views/manage-record-views.md).
1. 单击 **分组**.

   ![](assets/grouping-ui-timeline-view.png)

1. 单击其中一个建议字段，或单击 **选择其他字段** 并搜索其他字段，然后在列表中显示该字段时单击该字段。

   >[!TIP]
   >
   >您无法选择链接的字段。

   分组将自动应用于时间轴，并且记录显示在分组框中。 分组中的项目数显示在分组行上。

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. （可选）重复上述步骤以添加最多3个分组。

   应用的分组数将显示在工具栏右上角的分组图标的左侧。

   ![](assets/grouping-applied-in-timeline-view.png)

1. （可选）单击 **x** 图标删除分组

   或

   单击 **全部清除** 以删除所有分组。

1. 在 **记录分组条件** 方框关闭它。

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### 编辑时间线视图设置 {#edit-the-timeline-view-settings}

更新时间线视图设置以指示在视图的时间线部分中显示的信息。

1. 创建时间线视图，如文章所述 [管理记录视图](../views/manage-record-views.md).
1. 单击 **设置**.
1. 单击 **日期和时间** 在左侧面板中，然后选择 **开始日期** 和 **结束日期** 以在时间轴上显示。 您可以选择默认的“开始”和“结束”日期，也可以选择任何可用的日期字段。 表示记录的条形图从您为开始日期指定的日期开始，结束日期对应于结束日期。

   >[!NOTE]
   >
   >    对于开始日期或结束日期没有值或者开始日期晚于结束日期的记录，不会显示在时间轴视图中。


1. 单击 **记录详细信息** 以指明要在记录栏上显示的字段。

   默认情况下，“名称”字段处于选中状态。

1. 单击 **添加字段** 最多向记录栏添加4个字段。
1. 在 **搜索字段** 框中，然后单击要添加字段。

   >[!TIP]
   >
   >   * 必须先创建这些字段，然后才能将其添加到记录栏。
   > 
   >   * 您必须至少选择一个字段。 **名称** 默认情况下处于选中状态。

   右侧将显示时间轴上栏的外观。

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. 单击&#x200B;**保存**。

   这些记录将按照您选择的规范显示在时间轴视图中。


