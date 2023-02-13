---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 查看实际小时数
description: 您在Adobe Workfront中登录工作项目的小时数被视为实际小时数。
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# 查看实际小时数

您在Adobe Workfront中登录工作项目的小时数被视为实际小时数。

实际小时数表示您完成任务、问题或项目所花费的实际时间。

我们建议应记录工作时间，这些项目是任务和问题。

但是，作为Workfront管理员，您还可以允许用户登录项目的时间，具体取决于您组织中的工作流。

有关如何设置系统以允许用户登录项目的时间的更多信息，请参阅 [配置工时单和工时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

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
   <td> <p>查看或更高程度地访问任务、项目或问题</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看任务、项目或问题的更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 任务和问题的实际工时数与项目的实际工时数

任务和问题的实际小时数表示直接记录任务和问题的小时数。

>[!NOTE]
>
>子任务的实际小时数累计到父任务的实际小时数。 以下公式适用于父任务上的实际小时数：

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

项目的实际小时数表示项目上所有任务（包括直接在父任务上记录的小时数）、项目上的所有问题以及项目本身上记录的实际小时数的总和。

以下公式适用于项目的实际小时数：

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## 查找实际小时数

对于任务、项目和问题，查找项目的“实际小时数”值的方式相同。

您可以在以下位置找到有关任务的实际工时信息：

* [“详细信息”部分中的实际小时数](#actual-hours-in-the-details-section)
* [“小时”部分中的实际小时数](#actual-hours-in-the-hours-section)
* [报表中的实际小时数](#actual-hours-in-reports)
* [资源管理工具中的实际工时数](#actual-hours-in-resource-management-tools)

### “详细信息”部分中的实际小时数 {#actual-hours-in-the-details-section}

对于项目、任务和问题，“详细信息”部分中的“查找实际小时数”是相同的。

要在任务详细信息中查找实际工时，请执行以下操作：

1. 转到要查看实际工时的任务。
1. 单击 **任务详细信息** 中。
1. 单击 **概述** 并注意 **实际小时数** 值。

   这是此任务记录的总时数。

### “小时”部分中的实际小时数 {#actual-hours-in-the-hours-section}

对于项目、任务和问题，“小时”部分中的“查找实际小时数”是相同的。

要在“小时数”部分找到实际小时数，请执行以下操作：

1. 转到要查看实际工时的任务。
1. 单击 **小时** 中。

   根据您的配置，“小时”部分可能列在 **显示更多**.

   此时会显示记录任务的小时条目列表。

1. 确保 **标准** 视图和 **项目** 分组将应用于此列表。

   在分组行中显示的 **小时** 列是任务上实际小时数的总数。

### 报表中的实际小时数 {#actual-hours-in-reports}

在生成任务、问题或项目报表时，您可以在报表中显示每个任务、问题或项目的实际小时数值。

向任务视图添加“实际小时数”列与在报表中构建视图类似。

要在任务报表中显示实际小时数，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **报表**.
1. 单击 **新建报表**，然后选择 **任务** 作为对象。

1. 单击 **添加列**，然后开始键入 **实际小时数** 当 **在此列中显示** 将显示下拉字段。 当字段显示在列表中时，选择该字段。

1. 单击 **保存并关闭** 以保存报表。

   “实际小时数”列显示每个任务记录的小时数。

### 资源管理工具中的实际工时数 {#actual-hours-in-resource-management-tools}

如果要查看用户在其分配的任务和问题上的工作进度，可以在以下资源管理工具中查看这些任务和问题：

* 利用率报表。\
   有关利用率报告的信息，请参阅 [资源利用率报告概述](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* 资源规划程序.

   有关在资源计划器中查看实际工时的信息，请参阅 [使用“用户”视图时，在资源计划器中查看可用、计划和实际工时或FTE](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## 日志时间

您可以通过多种方式记录任务、问题和项目的时间。

有关在Workfront中记录时间的更多信息，请参阅 [日志时间](../../../timesheets/create-and-manage-timesheets/log-time.md).
