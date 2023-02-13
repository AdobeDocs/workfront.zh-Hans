---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 运行报表
description: 您可以运行任何有权查看的报表。
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---


# 运行报表

您可以运行任何有权查看的报表。

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对报表、功能板、日历的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 运行报表

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **报表**.

1. 从以下选项中进行选择：

   * **我的报告：** 已创建的报表。
   * **与我共享：** 其他用户与您共享的报表。
   * **所有报表：** 系统中您有权访问的所有报表。

1. 单击要运行的报表的名称。\
   或\
   如果报表是使用提示创建的，请从下拉菜单中选择相应的信息，然后单击 **运行报表**.\
   有关提示的更多信息，请参阅 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   报表内容会在报表的右上角显示一个时间戳，其中包含从运行报表的用户的上下文运行报表的日期、时间和时区。

1. （可选）单击 **“重新加载”图标** ![](assets/qs-report-refresh-icon.png) 在浏览器中显示报表一段时间后，刷新报表结果。

1. （视情况而定）如果报表使用过滤器或提示，请单击 **显示过滤器和提示** 显示您正在查看的报表中使用的过滤器和提示列表。 如果报表仅包含过滤器或仅包含提示， **显示过滤器** 或 **显示提示** 中。

   ![显示过滤器和提示](assets/qs-reports-showfiltersandprompts-2022-350x136.png)

   信息显示在页面左侧报表名称的下方。 对于提示，此信息介绍了在运行报告时所做的提示选择，如步骤4中所述。

1. 如果您使用的是“自定义提示”，则不会显示这些提示。 只显示系统提示。 自定义过滤器始终显示。

## 查看缓存的报表

如果报表在浏览器中显示了一段时间，则可能会缓存该报表。 执行以下任一操作时，您可以强制重新加载缓存的报表：

* 编辑报表设置并保存报表。
* 更改“视图”、“组”或“过滤器”。
* 单击 **“重新加载”图标**
此选项位于消息框内页面右上角，用于指示保存报表的时间，或位于报表所在功能板右上角。 有关重新加载功能板的更多信息，请参阅文章中的“显示功能板”部分 [功能板入门](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* 通过导航到“摘要”、“矩阵”或“图表”选项卡，访问报表中第一页以外的任何页面。
