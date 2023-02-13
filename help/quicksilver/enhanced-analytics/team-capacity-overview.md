---
title: 在Enhanced Analytics中查看“团队容量”可视化
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: “团队容量”可视化图表显示了主团队的总容量，无论这些容量是被过度分配还是分配不足，以及容量在一段时间内的动态性。
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# 在Enhanced Analytics中查看“团队容量”可视化

“团队容量”可视化图表显示了主团队的总容量，无论这些容量是被过度分配还是分配不足，以及容量在一段时间内的动态性。

![](assets/team-capacity-350x110.png)

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
   <td> <p>查看项目访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。<br>有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
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

## 了解“团队能力”可视化图表

“团队能力”可视化图表显示在给定日期分配给主团队的工作量。

* **倦怠**:当点线上方的蓝色填充颜色较深时，主团队会为他们分配比团队可用工作小时数内完成的工作时间更多。 这表明，该团队的配置过度，可能正在接近倦怠。

   ![](assets/team-capacity-over-capacity.png)

* **无挑战**:当点线下方有较深的蓝色填充颜色时，家庭团队可用的工作时间超过分配给他们的工作量。 这表示该团队分配不足，可能没有受到挑战。

   ![](assets/team-capacity-under-capacity.png)

* **余额**:当浅蓝色或更透明的蓝色填充颜色正上方、正下方或虚线处的位置显示时，主团队会为他们分配一定的工作时间，以便他们能够在可用的工作时间内完成工作。 这表示该团队的工作量更加平衡。

   ![](assets/team-capacity-at-capacity.png)

将鼠标悬停在可视化上的任意点上，可显示给定日期的以下详细信息：

* **计划小时数**:这是团队需要完成的计划工时数。
* **可用小时数**:这是团队可以工作的工时数。
* **容量**:除了能力百分比之外，还会显示“按能力”、“按能力”或“超量”能力的标识。

查看此信息可帮助您确定：

* 主队被过度分配或分配不足时。
* 如果主队每天分配过多或分配不足。
* 家庭团队的工作量是每天如何的一致。
* 如果您的新工作产生了容量问题。

要了解如何获取此可视化图表的最佳数据，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 查看“团队能力”可视化图表

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **Analytics**.
1. 在左侧面板中，选择 **人员**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. （可选）要使用其他日期范围，请从日期范围筛选器中选择新的开始日期和结束日期。

   ![](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （视情况而定）如果您未设置团队过滤器，请添加团队过滤器，然后选择要查看其数据的每个团队。

   有关在Enhanced Analytics中添加过滤器的更多信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   添加过滤器后，最多会显示50个项目的数据，并且即使您离开页面或注销Workfront后，这些过滤器仍保持活动状态。

1. 在“资源能力”可视化图表上，单击团队以查看更多信息。

   此时会显示“团队容量”可视化。

   有关“资源能力”可视化的详细信息，请参阅 [在Enhanced Analytics中查看资源容量可视化](../enhanced-analytics/resource-capacity-overview.md).

1. （可选）要放大日期范围，请在可视化中选择一个点以表示日期范围的开始日期，然后拖动到日期范围的结束日期。

   所有其他可视化图表将更新至同一日期范围，并创建时间范围过滤器。

   ![](assets/timeframe-filter-350x220.png)

1. 将鼠标悬停在图表行上的某个点上，可查看给定日期的计划小时数和计划小时数，以及容量百分比，以及当时主团队是结束、接受还是接受容量。

   ![](assets/team-capacity-capacity-pop-up-350x351.png)

1. （可选）要导出可视化数据，请单击 **导出图标** ![](assets/export.png) 在可视化的右上角，选择导出格式：

   * **图表 (PNG)**
   * **数据表(XSLX)**

