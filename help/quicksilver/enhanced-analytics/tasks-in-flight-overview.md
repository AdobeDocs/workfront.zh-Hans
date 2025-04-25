---
title: 在Enhanced Analytics中查看外部测试版中的任务可视化图表
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 外部测试版中的任务可视化图表显示某个项目正在执行的任务数（在应用的筛选标准内）、每个任务完成的百分比以及任务的进度如何。
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 4%

---

# 在Enhanced Analytics中查看外部测试版中的任务可视化图表

>[!IMPORTANT]
>
>增强型分析将于5月26日这一周从Workfront中删除。 Workfront Data Connect是一种新的替代解决方案，可用于复制您当前使用的任何Enhanced Analytics可视化图表。 <br>有关详细信息，请参阅[Enhanced Analytics弃用](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)指南。


外部测试版中的任务可视化图表显示某个项目正在执行的任务数（在应用的筛选标准内）、每个任务完成的百分比以及任务的进度如何。

外部测试版中的![任务](assets/tasks-in-flight-possible-replacement-350x104.png)

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">Adobe Workfront计划</a>*</td> 
   <td> <p>业务或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>*</td> 
   <td> <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对项目的访问权限</p> <p>查看任务访问权限（要更新任务，您需要对任务的编辑访问权限。）</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。<br>有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看对项目和任务对象的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 先决条件

有关使用增强型分析的先决条件，请参阅[增强型分析概述](../enhanced-analytics/enhanced-analytics-overview.md)中的“先决条件”部分。

## 了解外部测试版中的任务可视化图表

外部测试版计划中的任务可视化显示以下任务详细信息：

* **计划任务持续时间**：任务栏的长度表示计划持续时间，该持续时间基于任务的开始日期和完成日期。

  ![外部测试版中的任务持续时间](assets/tasks-in-flight-duration-350x80.png)

* **已完成的工作量**：任务栏中的深蓝色表示任务已完成的工作量。 此完成百分比显示在任务栏的右侧。

  ![外部测试版中的任务深蓝色](assets/tasks-in-flight-dark-blue-350x35.png)

* **剩余工作量**：任务栏中的浅蓝色表示任务需要完成的工作量。

  外部测试版中的![任务浅蓝色](assets/tasks-in-flight-light-blue-350x35.png)

此信息可以帮助您确定：

* 集中工作努力的地方。
* 哪些任务可能会使项目面临风险。
* 任务距离完成有多远。
* 您需要与谁讨论特定任务。

要了解如何为此可视化获取最佳数据，请参阅[增强分析概述](../enhanced-analytics/enhanced-analytics-overview.md)。

## 查看外部测试版中的任务可视化图表

1. 单击主菜单图标![主菜单图标](assets/main-menu-icon-16x12.png)，然后选择&#x200B;**Analytics**。
1. （可选）要使用不同的日期范围，请从日期范围过滤器中选择新的开始日期和结束日期。

   ![选择日期范围](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅[在增强型分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

1. （视情况而定）如果您需要限制项目数据集，请选择并应用要使用的过滤器。

   有关在增强分析中添加筛选器的详细信息，请参阅[在增强分析中应用筛选器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

   添加过滤器后，会显示最多50个项目的数据，即使您离开页面或退出Workfront，过滤器也会保持活动状态。

1. 在外部测试版计划或项目树状图可视化图表上，单击项目以查看更多信息。

   此时将显示“燃尽”和“飞行中的任务”可视化图表。

   >[!NOTE]
   >
   >要了解有关这些其他可视化图表的更多信息，请参阅：
   >
   >   
   >   
   >   * [在增强型分析中查看外部测试版计划可视化图表](../enhanced-analytics/flight-plan-overview.md)
   >   * [在增强型分析中查看项目树状图可视化图表](../enhanced-analytics/project-treemap-overview.md)
   >   * [在增强型分析中查看燃尽可视化图表](../enhanced-analytics/burndown-overview.md)
   >   
   >

1. （可选）要放大日期范围，请在可视化图表上选择一个点作为日期范围的起点，然后拖动到日期范围的终点。

   所有其他可视化都会更新到相同的日期范围，并创建一个时间范围过滤器。

   ![时间范围筛选器](assets/timeframe-filter-350x220.png)

1. （可选）要更改任务的排序方式，请单击&#x200B;**排序依据**&#x200B;菜单，然后选择新的排序选项：

   * **完成日期**
   * **按字母顺序A-Z**
   * **工作细分结构** （此选项与任务在项目中的显示顺序匹配。）

   页面上的所有其他可视化图表将更新以匹配您的排序选择。

1. 查看选定项目中任务的进度，然后将鼠标悬停在特定任务上可查看计划小时数、计划到期日和完成百分比。

   ![外部测试版中的任务详细信息](assets/tasks-in-flight-task-details-350x242.png)

1. 单击某个任务可打开屏幕右侧的任务详细信息，您可以在其中查看有关该任务的详细信息、查看或输入更新或者对该任务进行更改。

   ![任务详细信息](assets/task-details-qs-350x675.png)

1. （可选）要导出可视化数据，请单击可视化右上角的&#x200B;**导出图标** ![导出图标](assets/export.png)，然后选择导出格式：

   * **图表(PNG)**
   * **数据表(XSLX)**

