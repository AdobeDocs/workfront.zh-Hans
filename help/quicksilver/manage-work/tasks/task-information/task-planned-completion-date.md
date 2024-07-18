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
source-wordcount: '782'
ht-degree: 1%

---

# 任务计划完成日期概览

任务的计划完成日期是任务设置为完成的日期。

您可以指定任务的规划完成日期，也可以将其留给Adobe Workfront根据特定条件进行计算。 

当项目计划于开始日期时，项目上任务的计划完成日期确定项目的计划完成日期。 有关项目计划完成日期的详细信息，请参阅[设置项目计划完成日期](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)。

>[!NOTE]
>
>任务的计划完成日期与任务的提交日期或任务的预计完成日期在以下方面不同：
>
>* 提交日期是分配任务的人员手动估计其将完成任务的日期。 有关更多信息，请参阅以下文章：
>
>   * [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * 提交日期和计划完成日期之间的[交互](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md)。
>
>* 预计完成日期是Workfront计算出的日期，它考虑了任务延迟、任务或其前置任务的时间表以及其他因素来确定实际完成任务的实际日期。 有关详细信息，请参阅[项目、任务和问题的预计完成日期概述](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)。
>

## 手动设置任务的计划完成日期

您必须具有任务的“编辑”访问权限和任务的“管理”权限才能更新任务的规划完成日期。

设置任务的计划完成日期取决于您分配给任务的任务限制类型。 

您可以在Workfront的以下区域中手动设置规划完成日期：

* 在编辑任务框中，创建或编辑任务时。 有关信息，请参阅[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。
* 在“任务详细信息”区域。 有关信息，请参阅[在任务详细信息概述区域](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)中管理任务信息。
* 如果在查看任务时显示计划完成日期，则位于主页区域。 有关信息，请参阅[在主页区域](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)更新或编辑工作项。
* 在任务标题中。 有关信息，请参阅[新对象标头](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md)。
* 在视图中显示“规划完成日期”字段时在任务列表或报告中。

  有关信息，请参阅[编辑列表中的任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)。

选择以下任何任务约束时，您可以人工指定计划完成日期： 

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
   <td> <p>必须完成时间</p> <p>完成时间不晚于</p> <p>完成时间不早于</p> </td> 
   <td> <p><span class="s1">计划开始日期已调整以使持续时间保持不变。</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定日期</p> </td> 
   <td> <p>持续时间会调整以使计划开始日期保持不变。</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront如何自动计算任务的规划完成日期

当系统自动计算此日期时，以下各项可能会影响任务的规划完成日期：

* 任务限制

  有关任务约束的详细信息，请参阅文章[任务约束概述](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)。

* 任务前置任务关系

  有关任务前置任务的更多信息，请参阅文章[任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

* 项目完成日期，从完成日期开始计划项目。
* 任务的主要被分配人的空闲时间计划。

  当主要被分配者在任务持续时间中计划了空闲时间时，如果为&#x200B;**用户空闲时间**&#x200B;字段选择了&#x200B;**考虑任务持续时间中的用户空闲时间**&#x200B;设置，则任务的计划日期将相应地调整。 新项目会从项目偏好设置区域继承此设置，但您可以在项目级别编辑此设置。

  例如，如果一项带有尽可能早限制的任务的计划于6月1日开始并在6月3日完成，而主要被分配人将6月2日标记为休假，则任务计划完成日期将变为6月4日。

  有关&#x200B;**用户休息时间**&#x200B;首选项的信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)或[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)文章。

* 如果任务与批准关联，则为与批准设置关联的时间量。 有关详细信息，请参阅[配置全局批准设置](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)。

在自动设置时，计划完成日期将根据以下计算确定： 

```
Planned Completion Date = Planned Start Date + Duration
```

例如，如果任务的开始日期为9月16日，持续时间为10天，则计划完成日期为9月26日。

>[!NOTE]
>
> 项目的更新类型必须设置为自动和更改时或自动以使计划小时数和持续时间自动调整。\
>有关更新类型的详细信息，请参阅文章[选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md)。
