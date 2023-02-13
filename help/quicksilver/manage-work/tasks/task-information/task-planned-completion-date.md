---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任务计划完成日期概览
description: 任务的计划完成日期是任务设置为完成的日期。
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 1%

---

# 任务计划完成日期概览

任务的计划完成日期是任务设置为完成的日期。

您可以指定任务的计划完成日期，也可以将任务保留给Adobe Workfront，以根据特定标准计算任务。 

项目任务的计划完成日期确定项目计划完成日期（从开始日期开始）。 有关项目计划完成日期的详细信息，请参阅 [设置项目计划完成日期](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>任务的计划完成日期与任务的提交日期或任务的预计完成日期不同，具体方式如下：
>
>* “提交日期”是指分配给任务的人员人工估计其已完成任务的日期。 有关更多信息，请参阅以下文章：
   * [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [提交日期与计划完成日期之间的交互](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* 预计完成日期是Workfront计算的日期，它考虑了任务延迟、任务或其前期的时间表，以及确定实际完成任务的实际日期的其他因素。 有关更多信息，请参阅 [项目、任务和问题的预计完成日期概览](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## 人工设置任务的计划完成日期

您必须具有任务的编辑访问权限和任务的管理权限，才能更新任务的计划完成日期。

设置任务的计划完成日期取决于您分配给任务的任务约束类型。 

您可以在Workfront的以下区域中手动设置计划完成日期：

* 在“编辑任务”框中，创建或编辑任务时。 有关信息，请参阅 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* 在“任务详细信息”区域。 有关信息，请参阅 [在“任务详细信息概览”区域中管理任务信息](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* 在“主页”区域中，如果查看任务时显示计划完成日期。 有关信息，请参阅 [在“主页”区域更新或编辑工作项](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* 在任务标题中。 有关信息，请参阅 [新对象标头](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* 在任务列表或报表中，“计划完成日期”字段显示在视图中。

   有关信息，请参阅 [在列表中编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

在选择以下任一任务约束时，您可以人工指定计划完成日期： 

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
   <td> <p>必须完成时间</p> <p>完成时间不晚于</p> <p>完成时间不早于</p> </td> 
   <td> <p><span class="s1">为保持持续时间相同，将调整计划起始日期。</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定日期</p> </td> 
   <td> <p>为保持计划起始日期相同，会调整持续时间。</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront如何自动计算任务的计划完成日期

当系统自动计算任务完成日期时，以下内容可能会影响任务的计划完成日期：

* 任务限制

   有关任务约束的详细信息，请参阅文章 [任务约束概述](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* 任务前置关系

   有关任务前置任务的详细信息，请参阅文章 [任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* 项目完成日期，从完成日期开始计划项目。
* 任务的主要受分派人的计划时间。

   如果主要任务负责人在任务期间计划了休息时间，则任务的计划日期会相应地调整 **考虑任务持续时间中的用户休息时间** 为 **用户关机时间** 字段。 新项目将从“项目首选项”区域继承此设置，但您可以在项目级别编辑该设置。

   例如，如果具有“尽快约束”的任务计划在6月1日开始，并在6月3日完成，而主要受分配人已将6月2日标记为“超时”，则任务“计划完成日期”将变为6月4日。

   有关 **用户关机时间** 首选项，请参阅文章 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) 或 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

* 与审批设置关联的任务与审批关联的时间。 有关更多信息，请参阅 [配置全局批准设置](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

自动设置后，计划完成日期将根据以下计算确定： 

```
Planned Completion Date = Planned Start Date + Duration
```

例如，如果任务的起始日期为9月16日，持续时间为10天，则计划完成日期为9月26日。

>[!NOTE]
 项目的更新类型必须设置为“自动”和“更改时”或“自动”，以便“计划小时数”和“持续时间”自动调整。\
有关更新类型的详细信息，请参阅文章 [选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md).
