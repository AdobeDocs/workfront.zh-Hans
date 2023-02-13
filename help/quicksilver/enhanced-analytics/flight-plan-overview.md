---
title: 在Enhanced Analytics中查看飞行计划可视化
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: “飞行计划”可视化图表显示有多少个项目（在应用的过滤标准内）在飞行中，这些项目在整个生命周期中发生了哪些条件变化，这些项目在多大程度上遵守了计划的完成期限。
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 2%

---

# 在Enhanced Analytics中查看飞行计划可视化

“飞行计划”可视化图表显示有多少个项目（在应用的过滤标准内）在飞行中，这些项目在整个生命周期中发生了哪些条件变化，这些项目在多大程度上遵守了计划的完成期限。

![](assets/flight-plan-350x132.png)

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
   <td> <p>查看对项目的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

有关使用Enhanced Analytics的先决条件，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 了解飞行计划可视化图表

在项目的实际持续时间内，您只能看到以下项目条件：

* 准时
* 处于风险中
* 存在问题

要了解项目条件，请参阅 [项目条件和条件类型概述](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

“飞行计划”可视化图表显示了以下项目详细信息：

* **计划持续时间**:水平蓝线表示项目的计划长度，其中任一行末尾的三角形表示开始日期和结束日期。

   ![](assets/planned-duration-line-350x37.png)

* **实际持续时间**:计划持续时间下方的粗色线条表示项目的实际长度。 线条的颜色会根据项目生命周期中该特定时间项目的条件而发生更改。

   ![](assets/actual-duration-line.png)

* **实际条件**:厚的彩色线条还会显示项目在不同时间的条件。 线条的颜色会根据项目的条件而发生更改：

   * **绿色**:On Target
   * **橙色**:面临风险
   * **红色**:遇到麻烦

   ![](assets/actual-condition-color.png)

通过将鼠标悬停在“飞行计划”可视化中的项目行上，可以查看有关项目计划时间范围、当前项目条件以及自定义条件（如果适用）的信息。 要更深入地查看可能影响持续时间或条件的内容，您可以在“增强的分析”区域中查看其他可视化图表。

查看此信息可帮助您确定：

* 什么事件会将项目延长到超出原始计划完成日期的时间。
* 当项目开始出现问题时。
* 同一时间段内打开的项目数量。
* 活动项目的数量。
* 哪些项目需要特别关注或支持。

有关如何为此可视化图表获取最佳数据的信息，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 查看飞行计划可视化

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **Analytics**.
1. （可选）要使用其他日期范围，请从日期范围筛选器中选择新的开始日期和结束日期。

   ![](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （视情况而定）如果您需要限制项目数据集，请选择并应用您要使用的过滤器。

   有关在Enhanced Analytics中添加过滤器的更多信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   添加过滤器后，最多会显示50个项目的数据，并且即使您离开页面或注销Workfront后，这些过滤器仍保持活动状态。

1. （可选）要放大日期范围，请在可视化中选择一个点以表示日期范围的开始日期，然后拖到日期范围的结束日期。

   所有其他可视化图表将更新至同一日期范围，并创建时间范围过滤器。

   ![](assets/timeframe-filter-350x220.png)

1. （可选）要更改项目的排序方式，请单击 **排序依据** 菜单，然后选择新的排序选项：

   * **A - Z**
   * **Z - A**
   * **计划的完成日期**
   * **计划的开始日期**

   页面上的所有其他可视化图表将进行更新，以匹配您的排序选择。

1. （视情况而定）如果数据集中有50个以上的项目，请使用可视化左下角的箭头从一组50个项目导航到下一个项目。

   页面上的所有其他可视化图表都会进行更新，以匹配您选择的页面。

   ![](assets/pagination-350x118.png)

1. 将鼠标悬停在项目条形图上可查看蓝色日期线以及以下详细信息：

   * 计划时间表
   * 当前条件
   * 自定义条件（如果适用）

   ![](assets/project-bar-graph-350x143.png)

1. （可选）要导出可视化数据，请单击 **导出** 图标 ![](assets/export.png) 在可视化的右上角，选择导出格式：

   * **图表 (PNG)**
   * **数据表(XSLX)**

1. 要查看更多项目信息，请单击可视化上的项目，以打开飞行可视化中的燃尽和任务。

   这些可视化图表可帮助您更深入地了解导致项目偏离轨道的原因。 它们还使签入正在进行的项目变得容易。\
   有关“燃耗”可视化图表的详细信息，请参阅 [在Enhanced Analytics中查看燃耗可视化](../enhanced-analytics/burndown-overview.md). 有关“飞行可视化中的任务”的详细信息，请参阅 [在增强分析中查看“飞行”可视化中的任务](../enhanced-analytics/tasks-in-flight-overview.md).

