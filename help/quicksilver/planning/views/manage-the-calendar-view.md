---
title: 管理日历视图
description: 您可以在日历视图中显示记录及其字段。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 278d740303b0fa2f1d1b10801634ce76ce0f5739
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# 管理日历视图

<!--
title: Manage the calendar view
description: You can display records in a calendar view.
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

您可以从记录类型页在日历视图中显示记录及其字段。

有关Adobe Workfront Planning功能视图以及如何管理这些视图的信息，请参阅 [管理记录视图](/help/quicksilver/planning/views/manage-record-views.md).

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
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>  
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


## 管理日历视图 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

请考虑以下事项：

* 仅当至少有两个日期字段与记录类型关联时，才能创建日历视图。 如果有一个或没有与记录类型关联的日期字段，则“日历”视图选项将灰显。
* 存在以下情况：

   * 当“起始日期”和“终止日期”均没有值时，这些记录不会显示在日历中
   * 当“开始”或“结束”日期没有值时，记录显示为一天事件
   * 当开始日期在结束日期之后时，该记录不会显示在日历上。

要管理日历视图，请执行以下操作：

1. 转到要查看其日历的记录类型页面。
1. 创建日历视图，如文章所述 [管理记录视图](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   与您选择的记录类型关联的记录在日历中显示为条形。 栏的颜色与记录图标的颜色匹配。

1. 执行以下操作之一以浏览日历：

   * 单击左右图标或使用水平滚动条在日历中前后移动。
   * 单击 **今天** 将日历居中到今天的日期。
   * 从时间范围下拉菜单中选择以下选项之一以更新时间增量：

      * 月
1. 更新以下视图元素，如以下子部分所述：
   * [过滤器](#add-filters)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Settings](#edit-the-calendar-view-settings)-->
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

  有关更多信息，请参阅文章中的“添加过滤器”部分 [管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md).

* 您可以按连接的记录字段或查找字段进行筛选，但不能对允许链接到多个记录的字段进行筛选。
