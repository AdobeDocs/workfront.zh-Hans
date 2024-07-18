---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 项目实际完成日期概览
description: 在Adobe Workfront中，项目、任务和问题具有实际完成日期。 这是将项目、任务或问题标记为完成的日期。
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# 项目实际完成日期概览

在Adobe Workfront中，项目、任务和问题具有实际完成日期。 这是将项目、任务或问题标记为完成的日期。

## 实际完成日期

实际完成日期表示完成工作的实际日期和时间。 当任务或问题标记为完成或完成时，Workfront会自动将项目状态更改日期设置为任务或问题的实际完成日期。 如果该日期不能准确反映任务或问题实际完成的时间，则可以手动编辑实际完成日期。

例如，您可以将任务或问题标记为已在星期一完成，但您知道该工作已在上个星期五完成。 将任务或问题标记为“完成”后，您可以手动将任务或问题的实际完成日期更新为上个星期五的日期，以反映实际完成日期。

您不能手动编辑项目的实际完成日期，但可以手动更改项目的状态，这会触发对其实际完成日期的更改。

通过以下方式设置项目的实际完成日期：

* 通过人工更新项目的状态：如果项目的“完成模式”设置为“人工”，并且您人工将项目的状态更改为“完成”，这会触发要更新为上次完成任务的日期和时间的项目的实际完成日期。
* 当项目的最后一个任务完成时，系统会自动更新：如果项目的“完成模式”设置为“自动”，并且您已将最后一个任务标记为“完成”或更新最后一个任务的“实际完成日期”，则项目的“实际完成日期”也会更新为该日期。

  有关设置项目完成模式的信息，请参阅文章[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。

  >[!NOTE]
  >
  >Workfront使用上次完成的项目任务的实际完成日期作为整个项目的实际完成日期。

当任务或问题的计划完成日期设置为“完成”或“关闭”时，Workfront或组管理员会确定Workfront使用的是当天日期还是使用这些日期。 有关设置任务和问题首选项的信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## 查找实际完成日期

实际完成日期位于Workfront的以下区域：

* 项目、任务和问题详细信息区域
* 编辑项目、任务和问题框
* 作为系统更新的“项目”、“任务”和“问题更新”区域。
* 项目、任务或问题列表或报告。

有关创建报告的详细信息，请参阅文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
