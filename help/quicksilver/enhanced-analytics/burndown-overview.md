---
title: 在Enhanced Analytics中查看燃耗可视化
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: “燃耗”可视化显示特定项目随时间的燃耗，并帮助您了解项目条件、速度与剩余小时数（即天数）之间的关系。
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: d337008d4fca8c41b98b10f9059ec1cc379811e1
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# 在Enhanced Analytics中查看燃耗可视化

“燃耗”可视化显示特定项目随时间的燃耗，并帮助您了解项目条件、速度与剩余小时数（即天数）之间的关系。

![](assets/burndown-350x112.png)

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
   <td> <p>查看项目访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。<br>有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

有关使用Enhanced Analytics的先决条件，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 了解燃耗可视化图表

实蓝线显示从开始日期到计划完成日期的计划速度。 当添加、删除或更新工作时，此行会进行调整，并在项目达到计划完成日期时变为虚线垂直行。

![](assets/burndown-planned-line.png)

实际线条显示项目在一段时间内所花费的小时数（即天数）。 此线条的颜色表示每天项目的状态：

* **绿色**:项目已定位。

   ![](assets/burndown-green.png)

* **橙色**:项目面临风险。

   ![](assets/burndown-orange.png)

* **红色**:项目有问题。

   ![](assets/burndown-red.png)

有关这些项目条件的更多信息，请参阅 [项目条件和条件类型概述](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

当实际行垂直向上移动时，已向项目中添加工作。 当线条垂直向下移动时，已移除或完成项目的工作。

在可视化图表的x轴下方，您可以查看有关任务和小时数（或天数）在给定日期（添加量、完成量以及两者之间的差异）的更多信息。

在“燃耗”可视化中查看所有这些信息可帮助您确定：

* 单个项目一段时间的运行状况
* 出现问题（或计划外工作）对计划工作有何影响。
* 哪些事件会将您的项目延长到原始完成日期之后。

要了解如何获取此可视化图表的最佳数据，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 查看燃耗可视化

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **Analytics**.
1. （可选）要使用其他日期范围，请从日期范围筛选器中选择新的开始日期和结束日期。

   ![](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （视情况而定）如果您需要限制项目数据集，请选择并应用您要使用的过滤器。

   有关在Enhanced Analytics中添加过滤器的更多信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   添加过滤器后，最多会显示50个项目的数据，并且即使您离开页面或注销Workfront后，这些过滤器仍保持活动状态。

1. （可选）要放大日期范围，请在可视化中选择一个点以表示日期范围的开始日期，然后拖到日期范围的结束日期。

   所有其他可视化图表将更新至同一日期范围，并创建时间范围过滤器。

   ![](assets/timeframe-filter-350x220.png)

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
   >   * [在增强分析中查看“飞行”可视化中的任务](../enhanced-analytics/tasks-in-flight-overview.md)


1. （可选）将视图从计划小时数更改为 **持续时间**.

   默认情况下，会选择计划小时数。

   >[!NOTE]
   >
   >选择 **持续时间** 将所有小时信息更改为天。\
   >![](assets/duration-burndown-350x112.png)\
   >有关“增强分析”区域持续时间的更多信息，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

1. 单击折线图上的任意点。

   将显示确切日期，下面显示了选定日期的任务和小时数（或天数）的进一步信息。

   ![](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >如果实际速度是沿可视化图表的x轴（内联0小时或0天）运行的平直线，则表示未向项目添加计划小时数（即天数）。\
   >如果实际速度是一条直线，在x轴上方（内联x轴的小时数或天数），且从不下降，则表示在过滤的时间段内未完成任务。

1. （可选）要导出可视化数据，请单击 **导出** 图标 ![](assets/export.png)在可视化的右上角，选择导出格式：

   * **图表 (PNG)**
   * **数据表(XSLX)**

1. （可选）要查看选定项目中任务进度的详细信息，请查看“燃耗”可视化下方的“飞行中的任务”可视化。
