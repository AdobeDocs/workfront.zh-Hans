---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 项目、任务和问题的预计完成日期概览
description: 预计完成日期是一个实时的计算指标，用于指明项目、任务或问题何时完成。 当项目、任务或问题标记为已完成时，预计完成日期将更改为实际完成日期的日期。
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# 项目、任务和问题的预计完成日期概览

预计完成日期是一个实时的计算指标，用于指明项目、任务或问题何时完成。 当项目、任务或问题标记为已完成时，预计完成日期将更改为实际完成日期的日期。

以下各节介绍如何为项目、任务和问题确定预计完成日期，以及如何找到它。

## 访问要求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>For current licenses: 
   <ul><li><p>Contributor or higher to view the Projected Completion Date in a report</p></li> <li><p>A Standard license to create a report</p></li> </ul>
   
   <p>For legacy licenses: 
   <ul><li><p>Review or higher to view the Projected Completion Date in a report</p></li> 
   <li><p>A Plan license to create a report</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>You must have Edit access to Reports, Dashboards, Calendars to create a report</p> <p>You must have Edit access to Filters, Views, Groupings to create a report or modify a list view</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>在报表中查看预计完成日期的审核或更高版本</p> <p>用于创建报表的计划许可证</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限访问项目</p> <p>您必须拥有对报表、功能板、日历的编辑访问权限才能创建报表</p> <p>您必须拥有“过滤器”、“视图”、“分组”的“编辑”访问权限，才能创建报表或修改列表视图</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目的或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## Adobe Workfront如何确定预计完成日期

“预计完成日期”是一个计算字段，不能人工更改。

用于确定预计完成日期的标准因您正在查看的对象而异：

* **项目：** 项目的预计完成日期等于项目最新任务的预计完成日期。
* **任务：** 任务的预计完成日期根据以下标准确定：

   * **任务受分派人对任务进行的进度更新：** 进度更新包括对完成百分比的更改和任务状态的更改。
   * **提交日期：** 如果任务受分配人指定了提交日期，则预计完成日期将更改为与提交日期匹配。

      有关提交日期的更多信息，请参阅文章 [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **前置任务：** 如果前置任务没有延迟，则预计完成日期应与计划完成日期匹配。 当延迟发生时，相关任务显示的预计完成日期大于计划完成日期。

      有关任务的计划完成日期的详细信息，请参阅 [任务计划完成日期概览](../../../manage-work/tasks/task-information/task-planned-completion-date.md).
   >[!IMPORTANT]
   >
   >当任务的前置任务具有实际完成日期时，从属任务将收到预计完成日期，如以下方案中所述：
   >
   >
   >如果项目具有任务A、任务B和任务C，并且任务B是任务A的后继者，则任务C是任务B的后继者，并且将实际完成日期添加到任务A，则系统将自动重新计算任务B的预计完成日期(前提是 **更新类型** 项目的预计完成日期设置为“自动”和“更改时”)，但不会为任务C重新计算。目前，由于性能原因，Workfront会计算与更新任务相比处于一个层或以下的任务的预计完成日期。 

* **问题：**问题预计完成日期最初设置为与问题计划完成日期匹配。

   如果问题任务分配人指定了提交日期，则“预计完成日期”和“计划完成日期”都将更改为与“提交日期”匹配。

   有关提交日期的更多信息，请参阅文章 [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## 查看预计完成日期

您可以在报表中查看项目、任务和问题的预计完成日期。 您可以查看Workfront其他区域中项目和任务的预计完成日期。 

* [查看项目的预计完成日期](#view-the-projected-completion-date-of-a-project)
* [查看任务的预计完成日期](#view-the-projected-completion-date-of-a-task)
* [查看问题的预计完成日期](#view-the-projected-completion-date-of-an-issue)

### 查看项目的预计完成日期 {#view-the-projected-completion-date-of-a-project}

1. 转到要查看预计完成日期的项目。
1. 单击 **项目详细信息** 中。
1. 找到 **预计完成日期** 字段 **概述** 中。

### 查看任务的预计完成日期 {#view-the-projected-completion-date-of-a-task}

1. 转到要查看预计完成日期的任务。
1. 单击 **任务详细信息** 中。
1. 找到 **预计完成日期** 字段 **概述** 中。

### 查看问题的预计完成日期 {#view-the-projected-completion-date-of-an-issue}

您只能在问题报表或列表视图中查看问题的预计完成日期。 创建列表视图与在报表中创建视图类似。

要创建包含预计完成日期的问题报表，请执行以下操作：

1. 创建问题报告，如文章中所述 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 选择 **列（视图）** 选项卡。
1. 单击 **添加列**，然后开始键入 **预计完成日期** 在 **在此列中显示：** 字段。

1. 当它显示在列表中时，在 **问题** 对象。 
1. 单击 **保存并关闭**.

   的 **预计完成日期** 列。 

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
