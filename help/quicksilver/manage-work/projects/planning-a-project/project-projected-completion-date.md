---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 项目、任务和问题的预计完成日期概述
description: 预计完成日期是一个实时计算指示器，指示项目、任务或问题的完成时间。 将项目、任务或问题标记为完成时，预计完成日期将更改为实际完成日期的日期。
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: 4897f165a7316a52b968601b45f95f7045f63840
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---

# 项目、任务和问题的预计完成日期概述

<!-- Audited: 11/2025 -->

预计完成日期是一个实时计算指示器，指示项目、任务或问题的完成时间。 将项目、任务或问题标记为完成时，预计完成日期将更改为实际完成日期的日期。

以下部分介绍了如何确定项目、任务和问题的预计完成日期，以及如何查找该日期。

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
   <ul><li><p>参与者或更高版本以便在报告中查看预计完成日期</p></li> <li><p>用于创建报告的标准许可证</p></li> </ul>
   或
   <ul><li><p>查看或更高版本以查看报告中的预计完成日期</p></li> 
   <li><p>用于创建报告的计划许可证</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别</td> 
   <td> <p>查看项目或授予更高的项目访问权限</p> <p>编辑对报告、功能板和日历的访问权限以创建报告</p> <p>编辑对筛选器、视图、分组的访问权限以创建报告或修改列表视图</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或更高权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## Adobe Workfront如何确定预计完成日期

预计完成日期是一个计算字段，不能手动更改。

根据您查看的对象，用于确定“预计完成日期”的标准有所不同：

* **项目：**&#x200B;项目的预计完成日期等于项目上最新任务的预计完成日期。

  例如，完成百分比越高，任务的预计完成日期就越接近当天。 如果任务的状态为“新建”，且任务计划完成日期已关闭或已过，则预计完成日期将进一步移至未来。

* **任务：**&#x200B;任务的预计完成日期基于以下条件确定：

   * **任务接受者对任务所做的进度更新：**&#x200B;进度更新包括对完成百分比的更改和任务状态的更改。
   * **提交日期：**&#x200B;如果任务分派人指定了提交日期，则预计完成日期将更改以匹配提交日期。

     有关提交日期的详细信息，请参阅文章[提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)。

   * **前置任务：**&#x200B;如果前置任务没有延迟，则预计完成日期应与计划完成日期匹配。 在发生延迟时，依赖任务显示的预计完成日期晚于计划完成日期。

     有关任务计划完成日期的更多信息，请参阅[任务计划完成日期概览](../../../manage-work/tasks/task-information/task-planned-completion-date.md)。

  >[!IMPORTANT]
  >
  >当任务的前置任务具有实际完成日期时，相关任务将收到预计完成日期，如以下方案所述：
  >
  >
  >如果项目具有任务A、任务B和任务C，并且任务B是任务A的后继任务，任务C是任务B的后继任务，并且任务A中添加了实际完成日期，则系统会自动为任务B重新计算预计完成日期（如果项目的&#x200B;**更新类型**&#x200B;设置为“自动”和“发生更改时”），但不会为任务C重新计算预计完成日期。目前，出于性能原因，Workfront会计算从更新任务中上移或下移一层的任务的预计完成日期。

* **问题：**&#x200B;问题预计完成日期最初设置为与问题计划完成日期匹配。

  如果问题被分派人指定了提交日期，则预计完成日期和计划完成日期都将更改以匹配提交日期。

  有关提交日期的详细信息，请参阅文章[提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)。

## 查看预计完成日期

您可以在报告中查看项目、任务和问题的预计完成日期。 您可以在Workfront的其他区域中查看项目和任务的预计完成日期。

### 查看项目的预计完成日期 {#view-the-projected-completion-date-of-a-project}

1. 转到要查看预计完成日期的项目。
1. 单击左侧面板中的&#x200B;**项目详细信息**。
1. 在&#x200B;**概述** > **项目日期**&#x200B;部分中找到&#x200B;**预计完成日期**&#x200B;字段。

### 查看任务的预计完成日期 {#view-the-projected-completion-date-of-a-task}

1. 转到要查看预计完成日期的任务。
1. 单击左侧面板中的&#x200B;**任务详细信息**。
1. 在&#x200B;**概述** > **任务日期和限制**&#x200B;部分中找到&#x200B;**预计完成日期**&#x200B;字段。

### 查看问题的预计完成日期 {#view-the-projected-completion-date-of-an-issue}

您只能在问题报告或列表视图中查看问题的预计完成日期。 创建列表视图与在报告中创建视图类似。

要创建包括预计完成日期的问题报表，请执行以下操作：

1. 创建问题报告，如[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)一文中所述。
1. 选择&#x200B;**列（视图）**&#x200B;选项卡。
1. 单击&#x200B;**添加列**，然后在&#x200B;**显示在此列：**&#x200B;字段中开始键入&#x200B;**预计完成日期**。

1. 当它出现在列表中的&#x200B;**问题**&#x200B;对象下时，将其选中。
1. 单击&#x200B;**保存+关闭**。

   ![报告列中的问题预计完成日期](assets/issue-projected-completion-date-in-view-nwe-350x148.png)


   已填充报表中的&#x200B;**预计完成日期**&#x200B;列。


