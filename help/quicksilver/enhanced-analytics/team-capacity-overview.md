---
title: 在“增强分析”中查看“团队容量”可视化图表
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 团队容量可视化显示主团队的总容量，无论他们是否分配过多或不足，以及容量在一段时间内的动态变化。
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 4%

---

# 在“增强分析”中查看“团队容量”可视化图表

<!-- Audited: 01/2024 -->

团队容量可视化显示主团队的总容量，无论他们是否分配过多或不足，以及容量在一段时间内的动态变化。

![团队产能](assets/team-capacity.png)

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
   <td role="rowheader">Adobe Workfront许可证概述</td>
   <td>
      <p>新增：浅色或更高</p>
      <p>或</p>
      <p>当前：审阅或更高版本</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>查看对项目的访问权限</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>查看 </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 先决条件

有关使用增强型分析的先决条件，请参阅中的“先决条件”部分 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 了解团队容量可视化

团队容量可视化图表显示给定日期分配给主团队的工作量。

* **燃尽**：当较深的蓝色填充颜色在虚线上方时，为主团队分配的工作时间多于他们能够完成的工作时间（在团队可工作的小时数内）。 这表示团队分配过度，可能接近燃尽。

  ![超出产能](assets/team-capacity-over-capacity.png)

* **不容置疑**：当较深的蓝色填充颜色在虚线下方时，主团队的可用工作时间多于分配给他们的工作量。 这表示团队分配不足，可能无法接受挑战。

  ![低于产能](assets/team-capacity-under-capacity.png)

* **平衡**：当较亮或更透明的蓝色填充颜色位于正上方、正下方或虚线时，主团队会为其分配一定数量的工作时间，他们应能够在其可用工作时间内完成这些工作。 这表示团队的工作量更加均衡。

  ![满负荷](assets/team-capacity-at-capacity.png)

将鼠标悬停在可视化图表上的任何点上会显示给定日期的以下详细信息：

* **计划小时**：这是团队需要完成的计划工作小时数。
* **可用小时数**：这是团队可以工作的时数。
* **容量**：除了能力百分比之外，还会显示指定“处于能力”、“能力不足”或“能力过剩”。

查看此信息可以帮助您确定：

* 主团队分配过多或分配不足时。
* 如果主团队每天分配过多或不足。
* 主团队每天的工作量有多稳定。
* 如果布置新工作，是否会遇到产能问题。

要了解如何为此可视化获取最佳数据，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 查看团队容量可视化图表

{{step1-to-analytics}}

1. 在左侧面板中，选择 **人员**.

   ![选择人员](assets/people-area-cropped-qs-350x276.png)

1. （可选）要使用不同的日期范围，请从日期范围过滤器中选择新的开始日期和结束日期。

   ![日期范围过滤器](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （视情况而定）如果尚未设置团队筛选器，请添加团队筛选器并选择要查看其数据的每个团队。

   有关在增强型分析中添加筛选器的更多信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   添加过滤器后，会显示最多50个项目的数据，即使您离开页面或退出Workfront，过滤器也会保持活动状态。

1. 在资源能力可视化图表上，单击团队以查看更多信息。

   此时将显示团队容量可视化图表。

   有关“资源能力”可视化的详细信息，请参阅 [在Enhanced Analytics中查看资源产能可视化图表](../enhanced-analytics/resource-capacity-overview.md).

1. （可选）要放大日期范围，请在可视化图表上选择一个点作为日期范围的起点，然后拖动到日期范围的终点。

   所有其他可视化都会更新到相同的日期范围，并创建一个时间范围过滤器。

   ![时间范围过滤器](assets/timeframe-filter-350x220.png)

1. 将鼠标悬停在图形生产线上的某个点上，可以查看给定日期的计划小时数和计划小时数、能力百分比以及当时主团队是超出、不足还是处于能力状态。

   ![团队产能弹出窗口](assets/team-capacity-capacity-pop-up-350x351.png)

1. （可选）要导出可视化数据，请单击 **导出** 图标 ![“导出”图标](assets/export.png) 然后选择导出格式：

   * 图表 (PNG)
   * 数据表(XSLX)

