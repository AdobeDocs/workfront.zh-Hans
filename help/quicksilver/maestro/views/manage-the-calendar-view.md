---
title: 管理日历视图
description: 您可以在日历视图中显示记录及其字段。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: ff52e43fc5ed5a7939b9e28b2bda195e94e81724
workflow-type: tm+mt
source-wordcount: '338'
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

{{maestro-important-intro}}

您可以从记录类型页在日历视图中显示记录及其字段。

有关Maestro视图以及如何管理这些视图的信息，请参阅 [管理记录视图](../views/manage-record-views.md).

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
   <td role="rowheader">访问级别配置</td>
   <td> <p>Maestro没有访问级别控制 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理视图的权限</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">布局模板</td>
   <td> <p>系统管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


## 管理日历视图 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

请考虑以下事项：

* 仅当至少有两个日期字段与记录类型关联时，才能创建日历视图。 如果有一个或没有与记录类型关联的日期字段，则“日历”视图选项将灰显。
* 以下方案：

   * 当开始日期和结束日期没有值时，记录不会显示在日历上
   * 当“开始”或“结束”日期没有值时，记录显示为一天事件
   * 当开始日期晚于结束日期时，记录不会显示在日历上。

要管理日历视图，请执行以下操作：

1. 转到要查看其日历的记录类型页面。
1. 创建日历视图，如文章所述 [管理记录视图](../views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   与您选择的记录类型关联的记录在日历中显示为条形。

1. 执行以下操作之一以浏览日历：

   * 单击左右图标或使用水平滚动条在日历中前后移动。
   * 单击 **今天** 将日历居中到今天的日期。
   * 从时间范围下拉菜单中选择以下选项之一以更新时间增量：

      * 月