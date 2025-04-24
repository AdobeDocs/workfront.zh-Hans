---
title: 管理日历视图
description: 您可以在日历视图中显示记录及其字段。 本文介绍了如何创建日历视图，以及如何编辑或删除现有视图。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: f171db8474df703fddbf63a673f9bfbd2ab2db27
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 1%

---

# 管理日历视图

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>   -->

{{planning-important-intro}}

您可以从记录类型页在日历视图中显示记录及其字段。

有关Adobe Workfront Planning视图以及如何管理这些视图的信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

## 访问要求

+++ 展开以查看访问要求。

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
<p>贵组织的Workfront实例必须载入Adobe Unified Experience，才能访问Workfront Planning的所有功能。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准 </p>
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
   <td>   <p>管理视图的权限</p>  
   <p>查看对视图的权限以临时更改视图设置</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## 管理日历视图 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

请考虑以下事项：

* 仅当至少有两个日期字段与记录类型关联时，才能创建日历视图。 如果有一个或没有与记录类型关联的日期字段，则“日历”视图选项将灰显。

  您可以从记录日期字段中选择，或从连接的记录或对象类型中选择查找日期字段。
* 存在以下情况：

   * 当“起始日期”和“终止日期”均没有值时，这些记录不会显示在日历中
   * 当“开始”或“结束”日期没有值时，记录显示为一天事件
   * 当开始日期在结束日期之后时，该记录不会显示在日历上。

要管理日历视图，请执行以下操作：

1. 转到要查看其日历的记录类型页面。
1. 创建日历视图，如[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)一文中所述。

   ![日历视图示例](assets/calendar-view-example.png)

   与您选择的记录类型关联的记录在日历中显示为条形。 栏的颜色与记录图标的颜色匹配。

1. 执行以下操作之一以浏览日历：

   * 单击左右图标或使用水平滚动条在日历中前后移动。
   * 单击&#x200B;**今天**&#x200B;可将日历居中到今天的日期。
   * 从时间范围下拉菜单中选择以下选项之一以更新时间增量：

      * **月**：记录显示在每月日历中。


      * **周**：记录显示在以下区域中：

         * 跨越多天的记录将显示在日历顶部。
         * 持续一天或更短的记录，显示在日历视图的下半部分。 如果选择显示开始日期和结束日期的小时，则记录会在发生日期的相应时间显示。


1. 更新以下视图元素，如以下子部分所述：
   * [过滤器](#add-filters)
   * [设置](#edit-the-calendar-view-settings)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### 添加过滤器

您可以使用过滤器减少屏幕上显示的信息量。

在日历视图中使用过滤器时，请考虑以下事项：

<!-- this list is almost identical to the one for the table view - update both-->

* 您为日历视图创建的筛选器与应用于同一记录类型的任何其他视图中的筛选器是相互独立的。

* 这些过滤器对于您选择的视图是唯一的。 同一记录类型的两个日历视图可以应用不同的筛选器。

* 查看同一日历视图的两个用户会看到当前应用的同一筛选器。

* 无法为日历视图命名您构建的过滤器。

* 删除筛选器会将其从与您访问相同记录类型以及显示与您相同的视图的任何人中删除。

* 在日历视图中添加筛选器与在表视图中添加筛选器相同。

  有关详细信息，请参阅文章[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)中的“添加筛选器”部分。

* 您可以按连接的记录字段或查找字段进行筛选。

* 您可以按显示多个值的查找字段进行筛选。

### 编辑日历视图设置

编辑日历视图设置与编辑时间轴视图的设置类似。

有关详细信息，请参阅文章[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)中的“编辑时间线视图设置”部分。
