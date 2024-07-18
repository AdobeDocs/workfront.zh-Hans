---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: 项目关键路径概述
description: 确定项目的关键路径是Adobe Workfront的一种自动方式，它可标记项目中可能会影响项目时间线的任务序列。 可能会影响项目时间线的任务将标记为关键路径任务。
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# 项目关键路径概述

确定项目的关键路径是Adobe Workfront的一种自动方式，它可标记项目中可能会影响项目时间线的任务序列。 可能会影响项目时间线的任务将标记为关键路径任务。

以下功能可能会影响项目的关键路径：

* 项目的工作分解结构。

  有关工作分解结构的详细信息，请参阅[确定项目中的工作分解结构](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* 完成每项任务所需的时间（持续时间）。
* 任务之间的依赖关系。

  请考虑以下事项：

   * 当关键路径上的任务具有前置任务关系时，如果前置任务或后置任务的日期更改直接影响其依赖项，则其前置任务或后置任务也处于关键路径上。

     >[!TIP]
     >
     >当任务的后续任务的日期不直接影响其依赖任务的日期并且不影响项目的日期时，后续任务不在“关键路径”上。
     >
     >
     >![](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * 当子任务被标识为“关键路径”任务时，如果父任务的预计起始日期和时间与子任务的预计起始日期和时间相同，则父任务也被标识为“关键路径”任务。

考虑到这些特征，系统将使用最早任务与决定项目结束的任务之间的最长路径来计算关键路径。 关键路径计算会考虑在不延长项目时间的情况下，每个任务可以开始和完成的最早和最晚时间。 此过程可确定哪些任务是“关键”任务（属于最长路径），以及哪些任务具有“总浮动时间”（可以延迟，但不会延长项目时间）。

关键路径上任务活动的任何延迟都会直接影响项目的预计完成日期（关键路径上没有浮点）。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看任务或更高访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看任务的权限或更高的权限 </p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 查看关键路径

您可以在Workfront应用程序的以下区域中查看属于关键路径的任务：

* [在甘特图中查看关键路径](#view-the-critical-path-in-the-gantt-chart)
* [在任务列表或报告中查看关键路径](#view-the-critical-path-in-a-task-list-or-report)

### 在甘特图中查看关键路径 {#view-the-critical-path-in-the-gantt-chart}

要在甘特图中查看关键路径上的任务，请执行以下操作：

1. 转到要查看其关键路径的项目。
1. 单击左侧面板中的&#x200B;**任务**。
1. 单击任务列表右上角的&#x200B;**甘特图**&#x200B;图标。

   ![甘特图图标__1_.png](assets/gantt-chart-icon--1-.png)

1. 展开&#x200B;**选项**&#x200B;菜单，然后启用&#x200B;**关键路径**&#x200B;选项。

   在甘特图中，关键路径上的任务在时间线上方有一条红线。

   ![crtical_path_on_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### 在任务列表或报告中查看关键路径 {#view-the-critical-path-in-a-task-list-or-report}

要查看哪些任务位于任务列表中的关键路径上：

1. 转到要查看其关键路径的项目。
1. 单击左侧面板中的&#x200B;**任务**。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**状态**。

   关键路径上的任务在列表的&#x200B;**标志**&#x200B;列中具有&#x200B;**关键路径**&#x200B;标志。

   您可以将同一视图应用于任务报告。

   有关创建报告的详细信息，请参阅文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

   或

   从&#x200B;**筛选器**&#x200B;下拉菜单中，选择&#x200B;**新建筛选器**。

1. 单击&#x200B;**添加筛选器规则**，然后在&#x200B;**仅显示包含……**&#x200B;字段的“任务”中开始键入&#x200B;**Is Critical**。

1. 当它出现在列表中时将其选中。
1. 单击&#x200B;**保存筛选器**。

   该列表应仅显示关键路径上的任务。
