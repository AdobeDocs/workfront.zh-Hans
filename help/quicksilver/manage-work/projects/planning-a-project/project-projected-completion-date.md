---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 项目、任务和问题的预计完成日期概述
description: 预计完成日期是一个实时计算指示器，指示项目、任务或问题的完成时间。 将项目、任务或问题标记为完成时，预计完成日期将更改为实际完成日期的日期。
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: d71ee30378c39975366f4f257e3f7b17aba0c0ae
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# 项目、任务和问题的预计完成日期概述

<!-- Audited: 1/2024 -->

预计完成日期是一个实时计算指示器，指示项目、任务或问题的完成时间。 将项目、任务或问题标记为完成时，预计完成日期将更改为实际完成日期的日期。

以下部分介绍了如何确定项目、任务和问题的预计完成日期，以及如何查找该日期。

## 访问要求

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
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>新增： 
   <ul><li><p>参与者或更高版本以便在报告中查看预计完成日期</p></li> <li><p>用于创建报告的标准许可证</p></li> </ul>

<p>当前： 
   <ul><li><p>查看或更高版本以查看报告中的预计完成日期</p></li> 
   <li><p>用于创建报告的计划许可证</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看项目或授予更高的项目访问权限</p> <p>您必须对报告、功能板和日历具有编辑权限才能创建报告</p> <p>您必须对筛选器、视图、分组具有编辑权限才能创建报告或修改列表视图</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或更高权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Adobe Workfront如何确定预计完成日期

预计完成日期是一个计算字段，不能手动更改。

根据您查看的对象，用于确定“预计完成日期”的标准有所不同：

* **项目：** 项目的预计完成日期等于项目上最新任务的预计完成日期。

  例如，完成百分比越高，任务的预计完成日期就越接近当天。 如果任务的状态为“新建”，且任务计划完成日期已关闭或已过，则预计完成日期将进一步移至未来。

* **任务：** 任务的预计完成日期基于以下标准确定：

   * **任务被分派人对任务所做的进度更新：** 进度更新包括对完成百分比的更改和任务状态的更改。
   * **提交日期：** 如果任务被分配人指定了提交日期，则预计完成日期将更改以匹配提交日期。

     有关提交日期的详细信息，请参阅文章 [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **前置任务：** 如果前置任务没有延迟，则预计完成日期应与计划完成日期匹配。 在发生延迟时，依赖任务显示的预计完成日期晚于计划完成日期。

     有关任务的规划完成日期的详细信息，请参阅 [任务计划完成日期概览](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >当任务的前置任务具有实际完成日期时，相关任务将收到预计完成日期，如以下方案所述：
  >
  >
  >如果项目具有任务A、任务B和任务C，并且任务B是任务A的后继任务，任务C是任务B的后继任务，并且任务A中添加了实际完成日期，则系统会自动为任务B重新计算预计完成日期(前提是 **更新类型** 项目的IP地址设置为“自动”和“发生更改时”)，但不会为任务C重新计算它。目前，出于性能原因，Workfront会为更新任务中向上或向下一级的任务计算预计完成日期。 

* **问题：** 问题预计完成日期最初设置为与问题计划完成日期匹配。

  如果问题被分派人指定了提交日期，则预计完成日期和计划完成日期都将更改以匹配提交日期。

  有关提交日期的详细信息，请参阅文章 [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## 查看预计完成日期

您可以在报告中查看项目、任务和问题的预计完成日期。 您可以在Workfront的其他区域中查看项目和任务的预计完成日期。

### 查看项目的预计完成日期 {#view-the-projected-completion-date-of-a-project}

1. 转到要查看预计完成日期的项目。
1. 单击 **项目详细信息** 在左侧面板中。
1. 找到 **预计完成日期** 中的字段 **概述** > **项目日期** 部分。

### 查看任务的预计完成日期 {#view-the-projected-completion-date-of-a-task}

1. 转到要查看预计完成日期的任务。
1. 单击 **任务详细信息** 在左侧面板中。
1. 找到 **预计完成日期** 中的字段 **概述** > **任务日期和限制** 部分。

### 查看问题的预计完成日期 {#view-the-projected-completion-date-of-an-issue}

您只能在问题报告或列表视图中查看问题的预计完成日期。 创建列表视图与在报告中创建视图类似。

要创建包括预计完成日期的问题报表，请执行以下操作：

1. 创建问题报告，如文章所述 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 选择 **列（视图）** 选项卡。
1. 单击 **添加列**，并开始键入 **预计完成日期** 在 **显示在此列中：** 字段。

1. 当它出现在列表中时，将其选中 **问题** 对象。 
1. 单击 **保存+关闭**.

   此 **预计完成日期** 列将被填充。 

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
