---
title: 在增强分析中查看“飞行”可视化中的任务
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: “飞行中的任务”可视化图表显示项目正在进行的任务数（在应用的筛选条件内）、每个任务已完成的工作百分比以及任务的进度。
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# 在增强分析中查看“飞行”可视化中的任务

“飞行中的任务”可视化图表显示项目正在进行的任务数（在应用的筛选条件内）、每个任务已完成的工作百分比以及任务的进度。

![](assets/tasks-in-flight-possible-replacement-350x104.png)

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront计划</a>*</td> 
   <td> <p>业务或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>*</td> 
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看项目访问权限</p> <p>查看对任务的访问权限（要更新任务，您需要对任务的编辑访问权限。）</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。<br>有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目和任务对象的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

有关使用Enhanced Analytics的先决条件，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 了解飞行可视化图表中的任务

“飞行计划”可视化中的任务显示了以下任务详细信息：

* **计划任务持续时间**:任务栏的长度表示计划的持续时间，该持续时间基于任务的开始日期和完成日期。

   ![](assets/tasks-in-flight-duration-350x80.png)

* **工作完成**:任务栏中的深蓝色表示任务已完成的工作量。 此完成百分比显示在任务栏的右侧。

   ![](assets/tasks-in-flight-dark-blue-350x35.png)

* **剩余的工作**:任务栏中的浅蓝色表示任务需要完成的工作量。

   ![](assets/tasks-in-flight-light-blue-350x35.png)

此信息可帮助您确定：

* 集中工作的地方。
* 哪些任务可能会让项目面临风险。
* 任务完成的距离。
* 你需要跟谁谈谈具体的任务。

要了解如何获取此可视化图表的最佳数据，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 在“飞行”可视化中查看任务

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **Analytics**.
1. （可选）要使用其他日期范围，请从日期范围筛选器中选择新的开始日期和结束日期。

   ![](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （视情况而定）如果您需要限制项目数据集，请选择并应用您要使用的过滤器。

   有关在Enhanced Analytics中添加过滤器的更多信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   添加过滤器后，最多会显示50个项目的数据，并且即使您离开页面或注销Workfront后，这些过滤器仍保持活动状态。

1. 在飞行计划或项目树状图可视化中，单击某个项目可查看更多信息。

   “燃耗”和“飞行任务”可视化图表显示。

   >[!NOTE]
   >
   >要进一步了解这些其他可视化图表，请参阅：
   >
   >   
   >   
   >   * [在Enhanced Analytics中查看飞行计划可视化](../enhanced-analytics/flight-plan-overview.md)
   >   * [在增强型分析中查看项目树状图可视化](../enhanced-analytics/project-treemap-overview.md)
   >   * [在Enhanced Analytics中查看燃耗可视化](../enhanced-analytics/burndown-overview.md)


1. （可选）要放大日期范围，请在可视化中选择一个点以表示日期范围的开始日期，然后拖动到日期范围的结束日期。

   所有其他可视化图表将更新至同一日期范围，并创建时间范围过滤器。

   ![](assets/timeframe-filter-350x220.png)

1. （可选）要更改任务的排序方式，请单击 **排序依据** ，然后选择新的排序选项：

   * **完成日期**
   * **按字母顺序 A 到 Z**
   * **工作分解结构** （此选项与任务在项目中的显示顺序匹配。）

   页面上的所有其他可视化图表将进行更新，以匹配您的排序选择。

1. 查看选定项目中任务的进度，然后将鼠标悬停在特定任务上，以查看计划小时数、计划到期日期和完成百分比。

   ![](assets/tasks-in-flight-task-details-350x242.png)

1. 单击任务以打开屏幕右侧的任务详细信息，您可以在屏幕中查看有关任务、查看或输入更新的详细信息，或对任务进行更改。

   ![](assets/task-details-qs-350x675.png)

1. （可选）要导出可视化数据，请单击 **导出图标** ![](assets/export.png) 在可视化的右上角，选择导出格式：

   * **图表 (PNG)**
   * **数据表(XSLX)**

