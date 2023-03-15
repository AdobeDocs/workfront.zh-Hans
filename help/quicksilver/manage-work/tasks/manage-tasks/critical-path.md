---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: 项目关键路径概述
description: 确定项目的关键路径是Adobe Workfront自动标记项目中可能影响项目时间轴的一系列任务的方法。 可能会影响项目时间轴的任务被标记为关键路径任务。
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# 项目关键路径概述

确定项目的关键路径是Adobe Workfront自动标记项目中可能影响项目时间轴的一系列任务的方法。 可能会影响项目时间轴的任务被标记为关键路径任务。

以下功能可能会影响项目的关键路径：

* 项目的工作划分结构。

   有关工作划分结构的详细信息，请参阅 [确定项目中的工作划分结构](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* 完成每项任务所花费的时间（持续时间）。
* 任务之间的依赖关系。

   请考虑以下事项：

   * 当关键路径上的任务具有前置关系时，如果前置路径或后置路径的日期更改直接影响其依赖项，则其前置路径和后置路径也位于关键路径上。

      >[!TIP]
      >
      >当任务的后续日期不直接影响其从属任务的日期，也不影响项目的日期时，后续任务不在关键路径上。
      >
      >
      >![](assets/successor-not-on-critical-path-350x150.png)     >

   * 当子任务被标识为关键路径任务时，如果父任务的预计开始日期和时间与子任务的预计开始日期和时间相同，则父任务也被标识为关键路径任务。

考虑到这些功能，系统会使用最早任务和确定项目结束的任务之间的最长路径来计算关键路径。 关键路径计算考虑了每个任务通过开始和结束而最早和最晚的时间，而无需使项目更长。 此过程确定哪些任务是“关键”（属于最长路径），哪些任务具有“总浮点数”（可以延迟，而不会延长项目）。

关键路径上任务活动的任何延迟都会直接影响项目的预计完成日期（关键路径上没有浮点）。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限访问任务</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看任务的权限或更高权限 </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 查看关键路径

您可以在Workfront应用程序的以下区域中查看属于关键路径的任务：

* [在甘特图中查看关键路径](#view-the-critical-path-in-the-gantt-chart)
* [在任务列表或报表中查看关键路径](#view-the-critical-path-in-a-task-list-or-report)

### 在甘特图中查看关键路径 {#view-the-critical-path-in-the-gantt-chart}

要在甘特图中查看关键路径上的任务，请执行以下操作：

1. 转到要查看其关键路径的项目。
1. 单击 **任务** 中。
1. 单击 **甘特图** 图标。

   ![gantt_chart_icon__1_.png](assets/gantt-chart-icon--1-.png)

1. 展开 **选项** 菜单，然后启用 **关键路径** 选项。

   关键路径上的任务在甘特图中其时间线上方有一条红线。

   ![crtitical_path_on_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### 在任务列表或报表中查看关键路径 {#view-the-critical-path-in-a-task-list-or-report}

要查看任务列表中关键路径上的任务，请执行以下操作：

1. 转到要查看其关键路径的项目。
1. 单击 **任务** 中。
1. 从 **查看** 下拉菜单，选择 **状态**.

   关键路径上的任务具有 **关键路径** 标记 **标记** 列。

   您可以将同一视图应用到任务报表。

   有关创建报告的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   或

   从 **过滤器** 下拉菜单，选择 **新建过滤器**.

1. 单击 **添加过滤器规则** 开始键入 **至关重要** 在 **仅显示任务，其中……** 字段。

1. 当列表中显示时选择它。
1. 单击 **保存过滤器**.

   列表应仅显示关键路径上的任务。
