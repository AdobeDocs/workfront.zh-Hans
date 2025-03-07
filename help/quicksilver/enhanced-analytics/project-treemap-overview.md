---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: 在增强型分析中查看项目树状图可视化图表
description: 项目树状图可视化图表是在特定时间范围内工作的小时数或天数视图，与其他工作量的大小相比较。 这有助于您了解人员投入到项目中的时间。
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 59e021aa3ae66e4fc8d9ce9eb57616f948e6cd90
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 2%

---

# 在增强型分析中查看项目树状图可视化图表

>[!IMPORTANT]
>
>增强型分析将于5月26日这一周从Workfront中删除。 Workfront Data Connect是一种新的替代解决方案，可用于复制您当前使用的任何Enhanced Analytics可视化图表。 <br>有关详细信息，请参阅[Enhanced Analytics弃用](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)指南。


<!-- Audited: 12/2023 -->

项目树状图可视化图表是在特定时间范围内工作的小时数或天数视图，与其他工作量的大小相比较。 这有助于您了解人员投入到项目中的时间。

![项目树状图](assets/project-treemap-350x126.png){width="700"}

## 访问要求

+++ 展开以查看访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront计划</a></td> 
   <td> <p>业务或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a></td> 
   <td>   <p>新增：</p> 
   <ul><li>浅色或更高</li></ul>
   <p>当前：</p>
   <ul><li>审阅或更高</li></ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看对项目的访问权限</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

有关使用增强型分析的先决条件，请参阅[增强型分析概述](../enhanced-analytics/enhanced-analytics-overview.md)中的“先决条件”部分。

## 了解项目树形图可视化图表

项目树形图可视化图表中的框表示项目，框的大小表示在不同项目上所花费时间的比较。 包装盒越大，花在项目上的时间就越多。

项目树形图可视化图表包括：

* **较小的浅蓝色框**：具有较少小时或天数的项目显示为浅蓝色的小框。

  ![较小的框](assets/project-treemap-smaller-box.png)

* **更大、深蓝色的框**：具有更多小时或天数的项目显示为具有深蓝色的大框。

  ![较大的框](assets/project-treemap-larger-box-350x205.png)

* **Medium大小的蓝色框**：介于两个类别之间的项目显示为中等大小的框，深蓝色和浅蓝色之间带有蓝色阴影。 中型盒子有3种可能的蓝色色调。

右侧的图例显示每种蓝色阴影的完成小时数划分信息。 此图例是动态的，可根据数据更新。

![树状图小时已完成](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>如果您按持续时间而不是计划小时数查看项目树状图可视化图表，此图例显示每种蓝色阴影的已工作天数细分。\
>![树状图工作天数](assets/project-treemap-days-worked.png)>

查看此信息可以帮助您确定：

* 在选定的日期范围内所处理的事项的优先级。
* 哪些团队在花费时间。
* 如果团队关注正确的事。
* 单击某个特定项目时，该项目范围在该时间段内发生了什么变化。

要了解如何为此可视化获取最佳数据，请参阅[增强分析概述](../enhanced-analytics/enhanced-analytics-overview.md)。

## 查看项目树状图可视化图表

1. 单击主菜单图标![主菜单图标](assets/main-menu-icon-16x12.png)，然后选择&#x200B;**Analytics**。
1. （可选）要使用不同的日期范围，请从日期范围过滤器中选择新的开始日期和结束日期。

   ![选择日期范围](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅[在增强型分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

1. （视情况而定）如果您需要限制项目数据集，请选择并应用要使用的过滤器。

   有关在增强分析中添加筛选器的详细信息，请参阅[在增强分析中应用筛选器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

   添加过滤器后，会显示最多50个项目的数据，即使您离开页面或退出Workfront，过滤器也会保持活动状态。

1. （可选）要更改项目的排序方式，请单击项目树状图可视化右上角的&#x200B;**排序方式**&#x200B;菜单，然后选择新的排序选项：

   * **A - Z**
   * **Z - A**
   * **计划完成日期**
   * **计划开始日期**

   页面上的所有其他可视化图表将更新以匹配您的排序选择。

1. （视情况而定）如果数据集中有超过50个项目，请使用可视化图表左下角的箭头，从包含50个项目的组导航到下一个项目。

   页面上的所有其他可视化图表将更新以匹配您选择的页面。

   ![分页](assets/pagination-350x118.png)

1. （可选）将视图从&#x200B;**计划小时数**&#x200B;更改为&#x200B;**持续时间**。

   默认情况下选择已计划小时数。

1. 将鼠标悬停在项目上可查看项目完成情况、计划总小时数、已完成总小时数以及每天在项目上花费的平均小时数。

   ![树状图项目详细信息](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >如果您选择了&#x200B;**持续时间**&#x200B;视图，您将看到以下持续时间详细信息：
   >
   >* **计划时间范围**：计划完成项目的天数。
   >* **已工作天数**：在顶部选定的日期范围内完成的每项任务的计划持续时间除以一天中的小时数。
   >   
   >![树状图持续时间](assets/duration-treemap-350x159.png)
   >
   >有关持续时间的更多信息，请参阅[增强型分析概述](../enhanced-analytics/enhanced-analytics-overview.md)中的“持续时间视图”部分。

1. （可选）要导出可视化数据，请单击可视化右上角的&#x200B;**导出图标** ![导出图标](assets/export.png)，然后选择导出格式：

   * **图表(PNG)**
   * **数据表(XSLX)**

1. 单击某个项目可打开“燃尽”和“外部测试版中的任务”可视化图表，以更深入地了解任务和小时（或天数）对项目大小有何影响。

有关燃尽可视化图表的详细信息，请参阅[在增强型分析中查看燃尽可视化图表](../enhanced-analytics/burndown-overview.md)。 有关外部测试版中任务的更多信息，请参阅[在增强型分析中查看外部测试版中的任务](../enhanced-analytics/tasks-in-flight-overview.md)。

