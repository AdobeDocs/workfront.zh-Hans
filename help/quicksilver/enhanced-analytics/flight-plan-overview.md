---
title: 在增强型分析中查看外部测试版计划可视化图表
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 外部测试计划可视化显示有多少项目（在应用的筛选标准内）正在外部测试，这些项目在整个生命周期中发生了什么条件更改，以及这些项目与其计划的完成截止日期的符合程度。
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 4%

---

# 在增强型分析中查看外部测试版计划可视化图表

外部测试计划可视化显示有多少项目（在应用的筛选标准内）正在外部测试，这些项目在整个生命周期中发生了什么条件更改，以及这些项目与其计划的完成截止日期的符合程度。

![](assets/flight-plan-350x132.png)

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront计划</a>*</td> 
   <td> <p>业务或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>*</td> 
   <td> <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。<br>有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看对项目的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 先决条件

有关使用增强型分析的先决条件，请参阅[增强型分析概述](../enhanced-analytics/enhanced-analytics-overview.md)中的“先决条件”部分。

## 了解外部测试版计划可视化图表

在项目的实际持续时间中，您只能看到以下项目完成情况：

* 准时
* 处于风险中
* 存在问题

要了解项目条件，请参阅[项目条件和条件类型概述](../manage-work/projects/manage-projects/project-condition-and-condition-type.md)。

外部测试版计划可视化显示以下项目详细信息：

* **计划持续时间**：蓝色水平线表示项目的计划长度，线末端的三角形表示开始日期和结束日期。

  ![](assets/planned-duration-line-350x37.png)

* **实际持续时间**：计划持续时间下方的彩色粗线表示项目的实际长度。 线条的颜色根据项目在项目生命周期中的该特定时间的状态而变化。

  ![](assets/actual-duration-line.png)

* **实际完成情况**：粗的彩色线条还显示不同时刻项目的完成情况。 线的颜色根据项目的条件而变化：

   * **绿色**：目标
   * **橙色**：有风险
   * **红色**：存在问题

  ![](assets/actual-condition-color.png)

通过将鼠标悬停在外部测试计划可视化图表中的项目行上，您可以查看有关项目的计划时间范围、当前项目条件以及（如果适用）自定义条件的信息。 要更深入地了解可能影响持续时间或条件的因素，您可以查看增强分析区域中的其他可视化图表。

查看此信息可以帮助您确定：

* 哪些事件使项目延长超过原始计划完成日期。
* 项目何时开始遇到问题。
* 同一时段内有多少个项目处于开放状态。
* 有多少项目处于活动状态。
* 哪些项目需要额外的关注或支持。

有关如何获得此可视化图表的最佳数据的信息，请参阅[增强型分析概述](../enhanced-analytics/enhanced-analytics-overview.md)。

## 查看外部测试版计划可视化图表

1. 单击&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon-16x12.png)，然后选择&#x200B;**分析**。
1. （可选）要使用不同的日期范围，请从日期范围过滤器中选择新的开始日期和结束日期。

   ![](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅[在增强型分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

1. （视情况而定）如果您需要限制项目数据集，请选择并应用要使用的过滤器。

   有关在增强分析中添加筛选器的详细信息，请参阅[在增强分析中应用筛选器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

   添加过滤器后，会显示最多50个项目的数据，即使您离开页面或退出Workfront，过滤器也会保持活动状态。

1. （可选）要放大日期范围，请在可视化图表上选择一个点作为日期范围的起点，然后拖动到日期范围的终点。

   所有其他可视化都会更新到相同的日期范围，并创建一个时间范围过滤器。

   ![](assets/timeframe-filter-350x220.png)

1. （可选）要更改项目的排序方式，请单击外部测试版计划可视化右上角的&#x200B;**排序方式**&#x200B;菜单，然后选择新的排序选项：

   * **A - Z**
   * **Z - A**
   * **计划完成日期**
   * **计划开始日期**

   页面上的所有其他可视化图表将更新以匹配您的排序选择。

1. （视情况而定）如果数据集中有超过50个项目，请使用可视化图表左下角的箭头，从包含50个项目的组导航到下一个项目。

   页面上的所有其他可视化图表将更新以匹配您选择的页面。

   ![](assets/pagination-350x118.png)

1. 将鼠标悬停在项目条形图上可查看蓝色日期线以及以下详细信息：

   * 计划时间线
   * 当前条件
   * 自定义条件（如果适用）

   ![](assets/project-bar-graph-350x143.png)

1. （可选）要导出可视化数据，请单击可视化右上角的&#x200B;**导出**&#x200B;图标![](assets/export.png)，然后选择导出格式：

   * **图表(PNG)**
   * **数据表(XSLX)**

1. 要查看更多项目信息，请单击可视化图表上的项目以打开Flight中的燃尽和任务可视化图表。

   这些可视化图表可以帮助您更深入地了解导致项目偏离正轨的原因。 它们还可以让您轻松签入正在进行的项目。\
   有关燃尽可视化图表的详细信息，请参阅[在增强型分析中查看燃尽可视化图表](../enhanced-analytics/burndown-overview.md)。 有关外部测试版中任务的更多信息，请参阅[在增强型分析中查看外部测试版中的任务](../enhanced-analytics/tasks-in-flight-overview.md)。

