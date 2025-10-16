---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 运行报表
description: 您可以运行有权查看的任何报表。
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---


# 运行报表

您可以运行有权查看的任何报表。

<!-- Audited: 11/2024 -->

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
      <p>标准</p>
      <p>规划</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看对报告、功能板和日历的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
     <td> <p>查看报表的权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 运行报表

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 报表]**。

1. 从以下选项中选择：

   * **我的报告：**&#x200B;您已创建的报告。
   * **与我共享：**&#x200B;其他用户与您共享的报告。
   * **所有报告：**&#x200B;系统中您有权访问的所有报告。

1. 单击要运行的报表的名称。\
   或\
   如果报告是使用提示创建的，请从下拉菜单中选择相应的信息，然后单击&#x200B;**运行报告**。\
   有关提示的详细信息，请参阅[向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。\
   报告的内容会在报告的右上角显示一个时间戳，该时间戳包括从运行报告的用户的上下文中运行报告的日期、时间和时区。

1. （可选）如果报表在浏览器中显示了一段时间，请单击&#x200B;**重新加载图标** ![重新加载图标](assets/unshimmed-report-refresh-icon.png)以刷新报表中的结果。

1. （视情况而定）如果报告使用筛选器或提示，请单击&#x200B;**显示筛选器和提示**&#x200B;以显示您正在查看的报告上使用的筛选器和提示列表。 如果报告仅包含筛选器或仅包含提示，则改为显示&#x200B;**显示筛选器**&#x200B;或&#x200B;**显示提示**。

   ![显示筛选器和提示](assets/unshimmed-show-filters-and-prompts.png)

   信息显示在页面左侧的报表名称下方。 对于提示，这是有关在运行报告时所做的提示选择的信息，如步骤3中所述。

1. 如果正在使用自定义提示，则不会显示它们。 仅显示系统提示。 始终显示自定义筛选条件。

## 查看缓存的报告

如果报表在浏览器中显示了一段时间，则可能会缓存该报表。 执行以下任何操作时，都可以强制重新加载缓存的报表：

* 编辑报告设置并保存报告。
* 更改视图、组或筛选器。
* 单击&#x200B;**重新加载图标** ![重新加载图标](assets/unshimmed-report-refresh-icon.png)
此选项在页面的右上角消息框中可用，表示保存报告的时间，或者它位于报告所在的仪表板的右上角。 有关重新加载功能板的更多信息，请参阅[功能板入门](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md)一文中的“显示功能板”部分。

* 通过导航到“摘要”、“矩阵”或“图表”选项卡，访问第一页以外的任何报告页面。
