---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 查看实际小时数
description: 您在Adobe Workfront中登录工作项的小时数被视为实际小时数。 实际小时数表示完成任务、问题或项目所用的实际时间。
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: 055228fd15d670a214039575dc076ab36f6e99eb
workflow-type: tm+mt
source-wordcount: '1220'
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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>标准<p>
   <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看或更高权限的任务、项目或问题</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看任务、项目或问题的权限或更高</p></td> 
  </tr> 
 </tbody> 
</table>

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Tasks,&nbsp;Projects, or Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a task, a project, or an issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 实际小时数与旧版实际小时数

根据您从中访问实际小时数的Workfront区域，这些小时数可能是以下记录的小时数之一：

* 在项目、任务和问题报告和列表中：

   * **实际小时数**： 2021年5月之后为项目、任务或问题记录的小时数。 它们以小时为单位存储在Workfront数据库中，其valuefield为`actualWorkRequiredDouble`。
   * **传统实际小时数**：随时为项目、任务或问题记录的小时数，包括2021年5月之前的小时数。 它们在Workfront数据库中以分钟为单位存储，其valuefield为`actualWorkRequired`。

     >[!IMPORTANT]
     >
     >项目的实际成本使用旧版实际小时数进行计算。

* 在项目、任务或问题详细信息区域中，实际小时数可显示在以下字段中：

   * **实际小时数**：在“详细信息”选项卡中，这些是2021年5月之后为项目、任务或问题记录的小时数。 它们以小时为单位存储在Workfront数据库中，其valuefield为`actualWorkRequiredDouble`。
   * **实际小时数**：在项目、任务或问题自定义表单中，当使用引用实际小时数本机字段的本机字段引用自定义字段访问时。 这些是2021年5月之后为项目、任务或问题记录的小时数。 它们以小时为单位存储在Workfront数据库中，其valuefield为`actualWorkRequiredDouble`。

>[!NOTE]
>
>建议尽可能使用实际小时数字段，因为旧版实际小时数字段可能会由于递增方式而显示不准确的小时数。

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
1. （可选且视情况而定）如果将实际小时数本机字段引用添加到项目、任务或问题自定义表单，请转到自定义表单，并在自定义字段中找到实际小时数。 这是为该对象记录的小时数总计。

### 小时部分中的实际小时 {#actual-hours-in-the-hours-section}

对于项目、任务和问题，在小时部分中查找实际小时数是相同的。

要在任务的小时数部分中查找实际小时数，请执行以下操作：

1. 转至要查看其实际小时数的任务。

1. 在左侧面板中，单击&#x200B;**小时**。 此时将显示任务上记录的小时条目列表，**小时**&#x200B;列显示任务的实际小时总数。

1. 确保&#x200B;**标准**&#x200B;视图和&#x200B;**项目**&#x200B;分组已应用于此列表。
1. 任务的实际小时数显示在&#x200B;**实际小时数**&#x200B;列的分组行中。

### 报表中的实际小时数和旧版实际小时数

在构建任务、问题或项目报告时，您可以显示报告中每个任务、问题或项目的实际小时数和旧版实际小时数值。

有关实际小时数和旧版实际小时数之间差异的信息，请参阅本文中的[实际小时数和旧版实际小时数](#actual-hours-vs-legacy-actual-hours)部分。

要在任务报表中显示实际小时数和传统实际小时数，请执行以下操作：

{{step1-to-reports}}

1. 在&#x200B;**报表**&#x200B;页面上，单击&#x200B;**新建报表**，然后选择&#x200B;**任务**&#x200B;作为对象。
1. 在页面的右下角，单击&#x200B;**添加列**。
1. 在&#x200B;**在此列**&#x200B;中显示下拉字段中，开始键入&#x200B;**实际小时数**，然后在该字段出现在列表中时选择该字段。
1. 重复上述步骤以将&#x200B;**传统实际小时数**&#x200B;字段添加到报表中。

1. 在页面的左下角，单击&#x200B;**保存+关闭**&#x200B;以保存报告。

1. 在&#x200B;**命名此报告以保存它**&#x200B;对话框中，输入新的报告名称，然后单击&#x200B;**应用**。
1. 对项目或问题报告重复相同的步骤。

### 资源管理工具中的实际小时数 {#actual-hours-in-resource-management-tools}

如果要查看用户对其分配的任务和问题所做工作的进度，可以在以下资源管理工具中查看这些进度：

* 利用率报表。\
  有关信息，请参阅[资源利用率报告概览](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

* 资源规划者。

  有关信息，在使用用户视图[时，请参阅资源规划者中的](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)查看可用、计划和实际小时数或FTE。


### Workfront API中的实际小时数

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

存储小时数的大多数Workfront字段都会在几分钟内保存在Workfront数据库中。 例如，任务的“计划小时数”字段的名称在Workfront数据库中为`workRequired`，以分钟为单位存储。

在API调用或计算的自定义字段或列中访问这些字段时，您必须考虑从分钟到小时的转换。

项目、任务或问题记录的实际小时数当前以分钟的形式存储在Workfront数据库中，其valuefield为`actualWorkRequired`。

鉴于以下版本的Workfront API计划于2025年晚些时候发布，实际小时数存储在数据库中的以下字段和单位中：

* **实际小时数**： 2021年5月之后为项目、任务或问题记录的小时数。 它们以小时为单位存储在Workfront数据库中，其valuefield为`actualWorkRequiredDouble`。
* **传统实际小时数**：随时为项目、任务或问题记录的小时数，包括2021年5月之前的小时数。 它们在Workfront数据库中以分钟为单位存储，其valuefield为`actualWorkRequired`。

  >[!IMPORTANT]
  >
  >项目的实际成本使用旧版实际小时数进行计算。

  有关在计算列或字段中使用实际小时数的信息，请参阅[报告常见问题解答](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md)。

## 记录时间

您可以通过多种方式记录任务、问题和项目的时间。

有关详细信息，请参阅[记录时间](../../../timesheets/create-and-manage-timesheets/log-time.md)。
