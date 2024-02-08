---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 项目完成百分比概述
description: 项目的完成百分比值根据项目中任务的计划持续时间或计划小时数来计算。 您的Adobe Workfront管理员或组管理员定义在项目偏好设置区域中配置信息时，在您的系统中计算完成百分比时要考虑的值。 有关配置项目首选项的信息，请参阅配置系统范围项目首选项。
author: Alina
feature: Work Management
exl-id: d2395569-9fe5-42e7-a392-cff49eb519d9
source-git-commit: 816fd70642ffb7b24095602ce160421aa947e2a6
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# 项目完成百分比概述

<!-- Audited 01/2024 -->

项目的完成百分比值根据项目中任务的持续时间或计划小时数来计算。 您的Adobe Workfront管理员或组管理员定义在项目偏好设置区域中配置信息时，在您的系统中计算完成百分比时要考虑的值。

有关配置项目首选项的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

父任务的完成百分比基于其每个子任务的持续时间或计划小时数。

同样，项目的完成百分比基于项目中每个主任务的持续时间或计划小时数。

主要任务为父任务和没有子任务的独立任务。

>[!TIP]
>
>主任务未在项目计划中缩进。

## Workfront如何计算完成百分比

### 更新任务的完成百分比 {#update-the-percent-complete-on-a-task}

您可以手动修改任务的完成百分比。 这不是算计。

Workfront使用单个任务的完成百分比来计算其父任务的完成百分比或项目的完成百分比。

有关更新任务的完成百分比的信息，请参阅 [查看和更新任务的完成百分比](../../../manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

### Workfront如何计算父任务的完成百分比 {#how-workfront-calculates-percent-complete-on-a-parent-task}

根据系统或组级别的Workfront或组管理员在项目首选项中选择的内容，父任务的完成百分比基于任务的持续时间或计划小时数计算。

请考虑以下情况：

* 如果系统根据计划小时数计算完成百分比，则父任务完成百分比使用以下公式计算：

  `Parent Task Percent Complete = (((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of Parent)*100`

  父级的总计划小时数表示每个子级的所有计划小时数的总和。

  ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

* 如果系统根据“持续时间”计算完成百分比，则父任务完成百分比使用以下公式计算：

  `Parent Task Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/ Total Duration of Parent)*100`

  ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!IMPORTANT]
  >
  >父任务的总持续时间是子任务的所有持续时间的总和。 例如，如果父任务有两个子任务，其各自的“持续时间”为1天和2天，则“总持续时间”为3天，即使这两个子任务可以在同一天开始。


### Workfront如何计算项目的完成百分比 {#how-workfront-calculates-percent-complete-on-a-project}

根据您的Workfront或组管理员在系统或组级别的项目首选项中选择的内容，项目的完成百分比基于项目上主要任务的持续时间或计划小时数来计算。

* 如果系统根据计划小时数计算完成百分比，则使用下列公式计算项目完成百分比：

  `Project Percent Complete =(((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of the Project)*100`

  项目的总计划小时数是项目中所有主要任务的计划小时数的总和。

  ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

  >[!NOTE]
  >
  >任务1或任务2只能是父任务或独立任务。 此计算中不使用子任务的计划小时数和完成百分比。

* 如果系统根据“持续时间”计算完成百分比，则使用以下公式计算项目完成百分比：

  `Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

  >[!IMPORTANT]
  >
  >项目持续时间是显示完成百分比的所有主任务的总持续时间。 例如，对于工期为2天的独立任务和工期为5天的父任务，如果在其上已完成工作，则项目的总工期为7天，即使这两个任务可以在同一天开始。

  ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!NOTE]
  >
  >任务1或任务2只能是父任务或独立任务。 此计算中不使用子任务的持续时间和完成百分比。

## 使用持续时间的项目完成百分比示例

使用任务的持续时间计算项目的完成百分比时，请考虑以下示例：

![](assets/project-with-tasks-percent-complete-duration-calculation.png)

以下信息用于计算项目的完成百分比

* 独立任务的完成百分比（任务1 - 20%）
* 父任务的完成百分比（任务2 - 25%）
* 任务1的持续时间（5天）
* 任务2的持续时间（2天）
* 项目持续时间（7天）


要使用持续时间计算项目的完成百分比，请执行以下操作：

`Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

或

`(((5*0.2)+(2*0.25))/7)*100= 21.43%`


<!--drafted, this was the old example:

When using the Planned Duration of the tasks to calculate the percent complete of a project, consider the following example:

percent_complete_on_project_example.png

Only the parent task (Task 1) and the standalone task (Task 8) are used to calculate the percent complete of the project.

The secondary parents of Task 1 are used to calculate the percent complete of the main parent (Task 1).

To calculate the percent complete of the main parent (Task 1), first calculate the percent complete of its secondary parents:

Task 5 Percent Complete = ((14 * 0.75 + 12 * 0.25)/(12 + 14))*100 = 51.92%

Task 2 Percent Complete = ((5 * 0.7 + 2 * 0.5)/(5 + 2))*100 = 64.29 %

Then, to calculate the percent complete of the main parent (Task 1), use the following formula:

Task 1 Percent Complete =((56 * 0.5192 + 7 * 0.6429)/63)*100 = 53.29%

To calculate the percent complete of the project, you will need to have the following numbers ready:

Task 1 Duration (63 hours) and Percent Complete (53.29%)
Task 8 Duration (100 hours) and Percent Complete (4%)
Now, to calculate the percent complete of the project, use the following formula:

Project Percent Complete =((100 * 0.04 + 63 * 0.5329))/163)*100 = 23.05%
-->