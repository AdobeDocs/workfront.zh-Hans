---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任务计划起始日期概览
description: 任务的“计划起始日期”是您作为任务创建者决定任务的工作应开始的日期。 计划任务日期会影响项目的日期和时间表。 有关项目计划起始日期的信息，请参阅项目计划起始日期概览。
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 2%

---

# 任务计划起始日期概览

任务的“计划起始日期”是您作为任务创建者决定任务的工作应开始的日期。 计划任务日期会影响项目的日期和时间表。 有关项目计划起始日期的信息，请参阅 [项目计划开始日期概览](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## 任务的计划起始日期

您可以指定任务的计划起始日期，也可以将其留给Adobe Workfront，以根据特定标准计算。 

* [人工设置任务的计划起始日期](#manually-set-the-planned-start-date-of-a-task)
* [如何计算任务的计划开始日期](#how-the-planned-start-date-is-calculated-for-a-task)

### 人工设置任务的计划起始日期 {#manually-set-the-planned-start-date-of-a-task}

设置任务的计划起始日期取决于您分配给任务的任务约束类型。 

您可以在创建任务时手动设置计划起始日期，如文章中所述 [在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

在选择以下任一任务约束时，您可以手动指定计划起始日期： 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任务约束类型</strong> </p> </th> 
   <th> <p><strong>人工更改计划完成日期的影响</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>必须开始时间</p> <p>开始时间不早于</p> <p>开始时间不晚于</p> </td> 
   <td> <p><span class="s1">为保持持续时间相同，将调整计划完成日期。</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定日期</p> </td> 
   <td> <p>为保持计划完成日期相同，将调整持续时间。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 如何计算任务的计划开始日期 {#how-the-planned-start-date-is-calculated-for-a-task}

当系统自动计算任务时，以下内容可能会影响任务的计划起始日期：

* “设置”的“任务和问题”区域中的“开始日期”首选项设置

   您的Workfront或组管理员可以确定新任务是在项目计划起始日期的同一日期开始，还是在您创建任务的当天开始。

   有关“任务和问题”首选项的信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* 任务限制

   有关任务约束的详细信息，请参阅文章 [任务约束概述](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)

* 任务前置关系

   有关任务前置任务的详细信息，请参阅文章 [任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* 项目开始日期，从开始日期开始计划项目。
* 任务的主要受分派人的计划时间。

   如果主要任务负责人在任务期间计划了休息时间，则任务的计划日期会相应地调整 **考虑任务持续时间中的用户休息时间** 为 **用户关机时间** 字段。 新项目将从“项目首选项”区域继承此设置，但您可以在项目级别编辑该设置。

   例如，如果具有“尽快约束”的任务计划在6月1日开始，并在6月3日完成，并且主要受分配人已将6月1日标记为“超时”，则“计划起始日期”将变为6月2日。

   有关 **用户关机时间** 首选项，请参阅文章  [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) 或 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

自动设置后，计划起始日期将根据以下计算确定： 

```
Planned Start Date = Planned Completion Date - Task Duration
```

例如，如果任务的完成日期为9月16日，持续时间为10天，则计划起始日期为9月6日。

>[!NOTE]
>
> 项目的更新类型还必须设置为“自动和更改时”或“自动”，以便自动调整计划小时数和持续时间。\
有关更新类型的详细信息，请参阅文章 [选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md).
