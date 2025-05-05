---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 查看实际小时数
description: 您在Adobe Workfront中登录工作项的小时数被视为实际小时数。
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# 查看实际小时数

您在Adobe Workfront中登录工作项的小时数被视为实际小时数。

实际小时数表示完成任务、问题或项目所用的实际时间。

我们建议在工作项（即任务和问题）上记录小时数。

但是，作为Workfront管理员，您可以允许用户在项目上记录时间，具体取决于您组织内的工作流程。

有关如何设置系统以允许用户登录项目的时间的详细信息，请参阅[配置时间表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

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
   <td> <p>查看或更高权限的任务、项目或问题</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看任务、项目或问题的权限或更高</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 任务和问题的实际小时数与项目的实际小时数

任务和问题的实际小时数表示直接在任务和问题上记录的小时数。

>[!NOTE]
>
>子任务的实际小时数将累计到父任务的实际小时数。 以下公式适用于父任务的实际小时数：

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

项目的实际小时数表示项目中所有任务（包括直接记录到父任务中的小时数）、项目中所有问题以及项目本身的实际小时数的总和。

以下公式适用于项目中的实际小时数：

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## 查找实际小时数

对于任务、项目和问题，查找项目的实际小时数值是相同的。

您可以在下列位置找到有关任务的“实际小时数”信息：

* 详细信息部分中的[实际小时数](#actual-hours-in-the-details-section)
* [小时部分中的实际小时数](#actual-hours-in-the-hours-section)
* 报表中的[实际小时数](#actual-hours-in-reports)
* [资源管理工具中的实际小时数](#actual-hours-in-resource-management-tools)

### 详细信息部分中的实际小时数 {#actual-hours-in-the-details-section}

对于项目、任务和问题，在“详细信息”部分中查找实际小时数是相同的。

要在任务详细信息中查找实际小时数，请执行以下操作：

1. 转到要查看其实际小时数的任务。
1. 单击左侧面板中的&#x200B;**任务详细信息**。
1. 单击&#x200B;**概述**&#x200B;并注意&#x200B;**实际小时数**&#x200B;值。

   这是在该任务上记录的小时总数。

### 小时部分中的实际小时 {#actual-hours-in-the-hours-section}

对于项目、任务和问题，在小时部分中查找实际小时数是相同的。

要查找以小时数表示的实际小时数部分，请执行以下操作：

1. 转到要查看其实际小时数的任务。
1. 单击左侧面板中的&#x200B;**小时**。

   根据您的配置，“小时”部分可能会列在&#x200B;**显示更多**&#x200B;下。

   这会显示任务记录的小时条目列表。

1. 确保&#x200B;**标准**&#x200B;视图和&#x200B;**项目**&#x200B;分组已应用于此列表。

   **小时**&#x200B;列的分组行中显示的数字是任务的实际小时总数。

### 报表中的实际小时数 {#actual-hours-in-reports}

在构建任务、问题或项目报告时，您可以在报告中显示每个任务、问题或项目的实际小时数值。

将“实际小时数”列添加到任务视图与在报告中构建视图类似。

要在任务报告中显示实际小时数，请执行以下操作：

1. 单击Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**报表**。
1. 单击&#x200B;**新建报告**，然后选择&#x200B;**任务**&#x200B;作为对象。

1. 单击&#x200B;**添加列**，并在显示&#x200B;**显示在此列**&#x200B;下拉字段时开始键入&#x200B;**实际小时数**。 当字段显示在列表中时，选择该字段。

1. 单击&#x200B;**保存+关闭**&#x200B;以保存报告。

   实际小时数列显示每个任务记录的小时数。

### 资源管理工具中的实际小时数 {#actual-hours-in-resource-management-tools}

如果要查看用户对其分配的任务和问题所做工作的进度，可以在以下资源管理工具中查看这些进度：

* 利用率报表。\
  有关利用率报告的信息，请参阅[资源利用率报告概览](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

* 资源规划者。

  有关在资源规划程序中查看实际小时数的信息，请参阅在使用用户视图[&#128279;](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)时查看资源规划程序中的可用小时、计划小时和实际小时数或FTE 。

## 记录时间

您可以通过多种方式记录任务、问题和项目的时间。

有关在Workfront中记录时间的详细信息，请参阅[记录时间](../../../timesheets/create-and-manage-timesheets/log-time.md)。
