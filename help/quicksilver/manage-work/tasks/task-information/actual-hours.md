---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 查看实际小时数
description: 您在Adobe Workfront中登录工作项的小时数被视为实际小时数。
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---

# 查看实际小时数

<!-- Audited: 5/2025 -->

您在Adobe Workfront中登录工作项的小时数被视为实际小时数。

实际小时数表示完成任务、问题或项目所用的实际时间。

我们建议在工作项（即任务和问题）上记录小时数。 但是，作为Workfront管理员，您还可以允许用户根据组织的工作流记录项目时间。

有关如何设置系统以允许用户登录项目的时间的详细信息，请参阅[配置时间表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> 
   <p>新增：标准<p>
   <p>或</p>
   <p>当前：工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看或更高权限的任务、项目或问题</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看任务、项目或问题的权限或更高</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 任务和问题的实际小时数与项目的实际小时数

任务和问题的实际小时数表示直接在任务和问题上记录的小时数。

子任务的实际小时数将累计到父任务的实际小时数。 以下公式适用于父任务的实际小时数：

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

项目的实际小时数表示所有项目任务（包括直接在父任务中记录的小时数）、所有项目问题以及项目本身中记录的实际小时数的总数。

以下公式适用于项目中的实际小时数：

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## 查找实际小时数

对于任务、项目和问题，查找项目的实际小时数值是相同的。

### 详细信息部分中的实际小时数 {#actual-hours-in-the-details-section}

对于项目、任务和问题，在“详细信息”部分中查找实际小时数是相同的。

要在任务详细信息中查找实际小时数，请执行以下操作：

1. 转至要查看其实际小时数的任务。
1. 在左侧面板中，单击&#x200B;**任务详细信息**。 将显示&#x200B;**概述**&#x200B;部分。
1. 在&#x200B;**工作时间**&#x200B;部分中找到&#x200B;**实际小时数**&#x200B;值。 这是在该任务上记录的小时总数。

### 小时部分中的实际小时 {#actual-hours-in-the-hours-section}

对于项目、任务和问题，在小时部分中查找实际小时数是相同的。

要查找以小时数表示的实际小时数部分，请执行以下操作：

1. 转至要查看其实际小时数的任务。

1. 在左侧面板中，单击&#x200B;**小时**。 此时将显示任务上记录的小时条目列表，**小时**&#x200B;列显示任务的实际小时总数。

1. 确保&#x200B;**标准**&#x200B;视图和&#x200B;**项目**&#x200B;分组已应用于此列表。

### 报表中的实际小时数 {#actual-hours-in-reports}

在构建任务、问题或项目报告时，您可以在报告中显示每个任务、问题或项目的实际小时数值。

要在任务报告中显示实际小时数，请执行以下操作：

{{step1-to-reports}}

1. 在&#x200B;**报表**&#x200B;页面上，单击&#x200B;**新建报表**，然后选择&#x200B;**任务**&#x200B;作为对象。
1. 在页面的右下角，单击&#x200B;**添加列**。
1. 在出现的&#x200B;**显示在此列**&#x200B;下拉字段中，开始键入&#x200B;**实际小时数**，然后在该字段出现在列表中时选择该字段。

1. 在页面的左下角，单击&#x200B;**保存+关闭**&#x200B;以保存报告。

1. 在&#x200B;**命名此报告以保存它**&#x200B;对话框中，输入新的报告名称，然后单击&#x200B;**应用**。

### 资源管理工具中的实际小时数 {#actual-hours-in-resource-management-tools}

如果要查看用户对其分配的任务和问题所做工作的进度，可以在以下资源管理工具中查看这些进度：

* 利用率报表。\
  有关信息，请参阅[资源利用率报告概览](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

* 资源规划者。

  有关信息，在使用用户视图](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)时，请参阅资源规划者中的[查看可用、计划和实际小时数或FTE。


### Workfront <!--database and the--> API <!--, and custom data-->中的实际小时数

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

存储小时数的大多数Workfront字段都会在几分钟内保存在Workfront数据库中。 例如，任务的“计划小时数”字段的名称在Workfront数据库中为`workRequired`，以分钟为单位存储。

在API调用或计算的自定义字段或列中访问这些字段时，您必须考虑从分钟到小时的转换。

根据您访问实际小时数的方式，可以将它们存储在数据库中的以下字段和单位中：

* 在API中：鉴于以下版本的Workfront API计划于2025年晚些时候发布，实际小时数的`valuefield`为`actualWorkRequiredDouble`，以小时数存储。 当前版本将实际小时数存储为`actualWorkRequired`，以分钟为单位。
* 在Workfront界面（计算的自定义字段和列）中：实际小时数的`valuefield`是`actualWorkRequired`，以分钟为单位存储。

<!--Change the above with this when we fix this for the Workfront UI: 

You must use the following valuefield name for Actual Hours in API calls or calculated custom fields or columns in Workfront: `actualWorkRequiredDouble`. -->

有关在计算列或字段中使用实际小时数的信息，请参阅[报告常见问题解答](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md)。

## 记录时间

您可以通过多种方式记录任务、问题和项目的时间。

有关详细信息，请参阅[记录时间](../../../timesheets/create-and-manage-timesheets/log-time.md)。
