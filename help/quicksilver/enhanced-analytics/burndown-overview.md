---
title: 在增强型分析中查看燃尽可视化图表
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 燃尽可视化图表显示特定项目在一段时间内的燃尽，并帮助您了解项目完成情况、速度和剩余小时数或天数之间的关系。
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# 在增强型分析中查看燃尽可视化图表

<!-- Audited: 12/2023 -->

燃尽可视化图表显示特定项目在一段时间内的燃尽，并帮助您了解项目完成情况、速度和剩余小时数或天数之间的关系。

![增强分析燃尽示例](assets/burndown120623.png)

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>
      <p>新建：任何</p>
      <p>或</p>
      <p>当前：业务或更高</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
      <p>新增：浅色或更高</p>
      <p>或</p>
      <p>当前：审阅或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看对项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看</p> </td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 先决条件

有关使用增强型分析的先决条件，请参阅[增强型分析概述](../enhanced-analytics/enhanced-analytics-overview.md)中的“先决条件”部分。

## 了解燃尽可视化图表

实心蓝线显示从开始日期到计划完成日期的计划速率。 当工作被添加、移除或更新时，这条线会随之发生调整，当项目达到计划的完成日期时，它就会变成虚线。

![计划的周转率](assets/burndown-planned-line.png)

实际行显示一段时间内在项目上花费的小时数或天数。 此行的颜色表示每天的项目完成情况：

* **绿色**：项目符合目标。

  ![目标](assets/burndown-green.png)

* **橙色**：项目有风险。

  ![处于风险中](assets/burndown-orange.png)

* **红色**：项目存在问题。

  ![存在问题](assets/burndown-red.png)

有关这些项目条件的详细信息，请参阅[项目条件和条件类型的概述](../manage-work/projects/manage-projects/project-condition-and-condition-type.md)。

当实际线条垂直向上移动时，工作已添加到项目中。 当线条垂直向下移动时，项目的工作已移除或完成。

在可视化图表的x轴下方，您可以看到有关任务和小时数（或天数）在给定日期如何变化的更多信息（添加数量、完成数量以及两者的差异）。

在“燃尽”可视化图表中查看所有这些信息有助于您确定：

* 单个项目在一段时间内的运行状况
* 进入（或计划外工作）的问题如何影响计划工作
* 哪些事件使您的项目超过了原始完成日期

要了解如何为此可视化获取最佳数据，请参阅[增强分析概述](../enhanced-analytics/enhanced-analytics-overview.md)。

## 查看燃尽可视化图表

{{step1-to-analytics}}

1. （可选）要使用不同的日期范围，请从日期范围过滤器中选择新的开始日期和结束日期。

   ![选择日期](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅[在增强型分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

1. （视情况而定）如果您需要限制项目数据集，请选择并应用要使用的过滤器。

   有关在增强分析中添加筛选器的详细信息，请参阅[在增强分析中应用筛选器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

   添加过滤器后，会显示最多50个项目的数据，即使您离开页面或退出Workfront，过滤器也会保持活动状态。

1. （可选）要放大日期范围，请在可视化图表上选择一个点作为日期范围的起点，然后将其拖动到日期范围的终点。

   所有其他可视化都会更新到同一日期范围，并自动创建时间范围过滤器。

   ![时间范围筛选器](assets/timeframe-filter-350x220.png)

1. 在外部测试版计划或项目树状图可视化图表上，单击项目以查看更多信息。

   此时将显示“燃尽”和“飞行中的任务”可视化图表。

   >[!NOTE]
   >
   >要了解有关这些其他可视化图表的更多信息，请参阅：
   >
   >   * [在增强型分析中查看外部测试版计划可视化图表](../enhanced-analytics/flight-plan-overview.md)
   >   * [在增强型分析中查看项目树状图可视化图表](../enhanced-analytics/project-treemap-overview.md)
   >   * [在Enhanced Analytics中查看外部测试版中的任务可视化图表](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. （可选）将视图从计划小时数更改为&#x200B;**持续时间**。

   默认情况下选择已计划小时数。

   >[!NOTE]
   >
   >选择&#x200B;**持续时间**&#x200B;会将所有小时信息更改为天。\
   >![持续时间燃尽](assets/duration-burndown-350x112.png)\
   >有关增强分析区域中持续时间的详细信息，请参阅[增强分析概述](../enhanced-analytics/enhanced-analytics-overview.md#duration-view)中的“持续时间视图”部分。

1. 单击折线图上的任意点。

   确切日期会显示，而且图形下方会显示有关选定日期的任务和小时数（或天数）的更多信息。

   ![燃尽详细信息](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >如果实际速度是沿可视化图表的x轴运行的平面线（内联0小时或0天），则意味着没有向项目添加计划的小时数或天数。\
   >如果实际速度是x轴上方的平直线（与小时数或天数内联）且永远不会降低，则意味着在过滤的时间段内未完成任何任务。

1. （可选）要导出可视化数据，请单击可视化右上角的&#x200B;**导出**&#x200B;图标![导出图标](assets/export.png)，然后选择导出格式：

   * 图表 (PNG)
   * 数据表(XSLX)

1. （可选）要查看有关所选项目中任务进度的详细信息，请查看外部测试版中的任务可视化图表，该可视化图表显示在燃尽可视化图表下方。 有关详细信息，请参阅[在增强型分析中查看外部测试版中的任务可视化图表](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md)。
