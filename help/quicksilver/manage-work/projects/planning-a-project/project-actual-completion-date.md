---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 项目实际完成日期概览
description: 项目、任务和问题在Adobe Workfront中有实际完成日期。 这是将项目、任务或问题标记为已完成的日期。
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: 3a3dc541219706e3f6a4700889db344c110838bb
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# 项目实际完成日期概览

项目、任务和问题在Adobe Workfront中有实际完成日期。 这是将项目、任务或问题标记为已完成的日期。

## 实际完成日期

实际完成日期表示完成工作的实际日期和时间。 当任务或问题标记为完成或完成时，Workfront会自动将物料状态更改的日期设置为任务或问题的实际完成日期。 如果该日期不能准确反映任务或问题的实际完成时间，则可以人工编辑实际完成日期。

例如，您可以将任务或问题标记为在星期一完成，但您知道该工作已在上一个星期五完成。 将任务或问题标记为完成后，您可以人工将任务或问题的实际完成日期更新为上星期五的日期，以反映实际完成情况。

您无法手动编辑项目的实际完成日期，但可以手动更改项目的状态，以触发对其实际完成日期的更改。

项目的实际完成日期按以下方式设置：

* 通过手动更新项目的状态：如果项目的“完成模式”设置为“手动”，并且您手动将项目的状态更改为“完成”，则会触发项目的“实际完成日期”，该日期将更新为更改状态的日期和时间。
* 当项目的最后一项任务完成时，会自动：如果项目的“完成模式”设置为“自动”，并且您将最后一个任务标记为“完成”或更新最后一个任务的“实际完成日期”，则项目的“实际完成日期”也会随该日期更新。

   有关设置项目完成模式的信息，请参阅文章 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!NOTE]
   >
   >Workfront使用项目任务中最后完成的实际完成日期作为整个项目的实际完成日期。

Workfront或组管理员确定Workfront是使用今天的日期，还是任务的计划完成日期，还是将任务设置为“完成”或“关闭”时的问题。 有关设置任务和问题首选项的信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## 查找实际完成日期

实际完成日期位于Workfront的以下区域：

* 项目、任务和问题详细信息区域
* 编辑项目、任务和问题框
* 项目、任务和问题更新区域作为系统更新。
* 项目、任务或问题列表或报告。

有关创建报告的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
