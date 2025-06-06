---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任务计划开始日期概述
description: 任务的计划开始日期是您作为任务创建者决定开始任务工作的日期。 计划任务日期会影响项目的日期和时间线。 有关项目计划开始日期的信息，请参阅项目计划开始日期概览。
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: 0ff02569d3c7fb532a2faafc46fe4235ce77acd4
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 2%

---

# 任务计划开始日期概述

<!-- Audited: 6/2025 -->

任务的计划开始日期是您作为任务创建者决定开始任务工作的日期。 计划任务日期会影响项目的日期和时间线。 有关项目计划开始日期的信息，请参阅[项目计划开始日期概览](../../../manage-work/projects/planning-a-project/project-planned-start-date.md)。

## 任务的计划开始日期

您可以指定任务的计划开始日期，也可以将其留给Adobe Workfront根据特定条件进行计算。 

* [手动设置任务的计划开始日期](#manually-set-the-planned-start-date-of-a-task)
* [如何为任务计算计划开始日期](#how-the-planned-start-date-is-calculated-for-a-task)

### 手动设置任务的计划开始日期 {#manually-set-the-planned-start-date-of-a-task}

设置任务的计划开始日期取决于您分配给任务的任务限制类型。 

创建任务时，您可以手动设置规划开始日期。 有关详细信息，请参阅[在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

选择以下任何任务约束时，您可以手动指定计划起始日期： 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任务限制类型</strong> </p> </th> 
   <th> <p><strong>手动更改计划完成日期的影响</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>必须开始时间</p> <p>开始时间不早于</p> <p>开始时间不晚于</p> </td> 
   <td> <p><span class="s1">计划完成日期已调整以使持续时间保持不变。</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定日期</p> </td> 
   <td> <p>持续时间会调整以使计划完成日期保持不变。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 如何为任务计算计划开始日期 {#how-the-planned-start-date-is-calculated-for-a-task}

当系统自动计算此日期时，以下各项可能会影响任务的计划起始日期：

* “设置”的“任务和问题”区域中的“开始日期”首选项设置

  您的Workfront或组管理员可以确定新任务的开始日期是与该项目的计划开始日期相同的日期，还是您创建任务的日期。

  有关任务和问题首选项的信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

* 任务限制

  有关任务约束的详细信息，请参阅[任务约束概述](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)。

* 任务前置任务关系

  有关任务前置任务的详细信息，请参阅[任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

* 项目开始日期，从开始日期开始计划项目。
* 任务的主要被分配人的空闲时间计划。

  如果主要被分配人在任务持续时间中计划了空闲时间，则当为用户空闲时间字段选择考虑用户在任务持续时间中的空闲时间设置时，任务的计划日期会相应地调整。 新项目会从项目偏好设置区域继承此设置，但您可以在项目级别编辑此设置。

  例如，如果一项带有尽可能早限制的任务的计划于6月1日开始并在6月3日完成，而主要被分配人在6月1日标记为休息时间，则任务计划开始日期将变为6月2日。

  有关用户休息时间首选项的信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)或[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。

在自动设置时，将根据以下计算确定计划起始日期： 

```
Planned Start Date = Planned Completion Date - Task Duration
```

例如，如果任务的完成日期为9月16日，持续时间为10天，则计划开始日期为9月6日。

>[!NOTE]
>
> 项目的更新类型还必须设置为自动和更改时或自动，以便自动调整计划小时数和持续时间。\
>有关更新类型的详细信息，请参阅[选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md)。
