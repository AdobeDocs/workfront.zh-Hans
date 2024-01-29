---
title: 在Enhanced Analytics中查看资源产能可视化图表
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 在查看Adobe Workfront中的增强型分析资源容量可视化图表时，您可以评估团队是超出、低于还是处于容量状态。
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 1%

---

# 在Enhanced Analytics中查看资源产能可视化图表

<!--Audited: 01/2024-->

在查看Adobe Workfront中的增强型分析资源容量可视化图表时，您可以评估团队是超出、低于还是处于容量状态。

资源可视化图表中说明的团队是指在指定时间段内分配给工作的用户的主团队。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront计划</a>*</td> 
   <td> <p>当前：业务或更高</p>
   或
   <p>新建：任何</p>
    </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证*</td> 
   <td> <p>当前：审阅或更高版本</p>
   或
   <p>新增：标准</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看对项目的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关更多信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 先决条件

有关使用增强型分析的先决条件，请参阅中的“先决条件”部分 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 了解资源产能可视化图表

“资源能力”可视化图表显示团队是超出、不足还是处于能力。 此计算基于：

* **可用产能**：主团队在过滤的时间段内可以工作的总小时数

  >[!NOTE]
  >
  >如果您查看的是未来的时间段，则可用容量是根据团队过去7天的容量来计算的。 因此，不会考虑任何计划的PTO。

* **已计划产能**：在过滤的时间段内，主页团队预计的计划工作小时总数

主页团队的计划小时数和实际计划小时数之间的比较可以帮助您确定您是否没有向主页团队分配足够的工作，或者他们是否可能因大量工作负载而感到倦怠。

![](assets/resource-capacity-350x110.png)

在资源能力可视化图表上，您可以看到以下详细信息：

* **已计划产能**：与主团队名称内联，蓝色圆圈表示分配给主团队的已计划小时数。

  ![](assets/resource-capacity-blue-circle.png)

* **实际产能**：与主团队名称内联，垂直线表示主团队可用的小时数。

  ![](assets/resource-capacity-vertical-line.png)

* **超出产能**：当水平线和蓝色圆显示在垂直线的右侧时，为主团队分配的工作量超过了他们能够完成的可用小时数。 这意味着在过滤的时间段内，团队可能会超出产能。 团队需要完成的剩余小时数显示在蓝色圆圈的右侧。

  ![](assets/resource-capacity-over-capacity.png)

* **低于产能**：当水平线和蓝色圆圈显示在垂直线的左侧时，主团队的可用小时数多于为其分配的计划工作小时数。 这意味着该团队在过滤的时间段内可能没有足够的容量。 主团队完成工作的额外可用小时数显示在蓝色圆圈的左侧。

  ![](assets/resource-capacity-under-capacity.png)

将鼠标悬停在团队的行上会显示计划容量和可用容量的确切小时数，以及主团队超出或低于容量的小时数。

查看此信息可以帮助您确定：

* 如果团队分配过多或不足。
* 主团队关注的最大项目是什么。
* 哪些团队可以工作。

要了解如何为此可视化获取最佳数据，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 查看资源产能可视化图表

{{step1-to-analytics}}

1. 在左侧面板中，选择 **人员**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. （可选）要使用不同的日期范围，请从图表右上角的日期范围过滤器中选择新的开始日期和结束日期。

   ![](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （视情况而定）如果尚未设置团队筛选器，请添加团队筛选器并选择要查看其数据的每个团队。

   有关在增强型分析中添加筛选器的更多信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   添加过滤器后，会显示最多50个项目的数据，即使您离开页面或退出Workfront，过滤器也会保持活动状态。

1. （可选）要放大日期范围，请在可视化图表上选择一个点作为日期范围的起点，然后拖动到日期范围的终点。

   所有其他可视化都会更新到相同的日期范围，并创建一个时间范围过滤器。

   ![](assets/timeframe-filter-350x220.png)

1. 将鼠标悬停在主团队行上可查看以下内容：

   * 还有多少小时可供安排
   * 主团队计划完成的小时数
   * 工作小时总数。 工作总小时数可以具有以下标签：

      * 超过
      * 下
      * 满负荷。

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. （可选）要导出可视化数据，请单击 **“导出”图标** ![](assets/export.png) 然后选择导出格式：

   * **图表(PNG)**
   * **数据表(XSLX)**

1. 单击主团队名称可在团队容量可视化图表中查看更多信息。

   要了解有关团队容量可视化的更多信息，请参阅 [在“增强分析”中查看“团队容量”可视化图表](../enhanced-analytics/team-capacity-overview.md).


