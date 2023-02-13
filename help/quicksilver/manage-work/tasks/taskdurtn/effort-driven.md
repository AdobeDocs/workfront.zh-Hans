---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: “持续时间类型概述：努力驱动”
description: “工作驱动”是一种持续时间类型，您可以在Adobe Workfront中为任务设置该持续时间类型。 有关Workfront中持续时间类型的常规信息，请参阅任务持续时间和持续时间类型概述。
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# 持续时间类型概述：努力驱动

“工作驱动”是一种持续时间类型，您可以在Adobe Workfront中为任务设置该持续时间类型。 有关Workfront中持续时间类型的常规信息，请参阅 [任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## 工作驱动的持续时间类型概述

您的Workfront或组管理员可以将系统或组的默认持续时间类型设置为“工作驱动”。 在这种情况下，将使用此持续时间类型创建所有新任务。 有关更改任务和发布首选项作为系统级别或组级别项目首选项的一部分的信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

在此情景中，可能会任意缩短项目计划，除非您作为项目经理需要时间考虑该任务是否实际是“工作驱动”任务。

使用工作驱动：

* 根据可用于处理任务的资源数确定计划持续时间。 持续时间等于“计划小时数”。 计划持续时间等于计划小时数除以受分配者数量。

   应用于任务的工作量决定了分工和持续时间。

* 跟踪在分配了多个资源时任务所花费的总小时数。

   添加资源后，任务的计划持续时间会减少。 （“多手轻工”原则说明此持续时间类型对任务计划持续时间的影响。）

以下各节提供了更详细的信息，说明Workfront如何计算工作驱动型任务的计划持续时间，以及添加资源对具有此持续时间类型的任务的影响。

## 工作驱动的持续时间类型公式概述

对于持续时间类型为“工作驱动型”的任务，其计划持续时间的计算公式取决于分配给该任务的每个资源的分配百分比。 对于“工作驱动”任务，Workfront会计算任务的“计划小时数”，它们始终与任务的“持续时间”相同：

```
Planned Hours (in hours) = Duration (in days)
```

您可以手动调整任务的持续时间。

Workfront假定一天有8个工作小时。 您的Workfront或组管理员使用设置中的项目首选项中的“每个工作日的典型小时数”设置定义每个工作日的小时数。 有关更改任务和问题首选项作为系统级别项目首选项的一部分的详细信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfront考虑分配给任务的每个资源的计划，以确定该任务的每个资源的分配百分比。 有关创建计划并将其分配给用户的信息，请参阅 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

请考虑以下情况：

* [100%的资源被分配给任务](#resources-are-allocated-100-to-the-task)
* [资源会按任务时间的不同百分比分配](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### 100%的资源被分配给任务 {#resources-are-allocated-100-to-the-task}

此公式假定所有资源均分配给任务100%。

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

此计算假定正常工作日的小时数为8。 公式包含此值，因此计划持续时间以天为单位显示。

### 资源会按任务时间的不同百分比分配 {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

由于每个已分配的资源可以具有唯一的分配级别，因此实际公式会考虑以下分配值：

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

此计算假定正常工作日的小时数为8。 公式包含此值，因此计划持续时间以天为单位显示。

## 向任务添加更多资源的效果

在向具有“工作驱动的持续时间类型”、“持续时间”和“计划小时数”的任务添加或移除任务的任务时，任务不会更改。 但是，计划持续时间确实会发生变化。

在以下示例中，在系统设置的项目首选项中，将每个工作日的典型小时数设置为8。 由于持续时间为3天，因此“计划小时数”设置为24（3天x每个工作日8小时= 24计划小时数）。

>[!NOTE]
>
>在使用固定日期任务约束时，在添加或删除受分配者时，计划持续时间保持不变，而是会调整持续时间和计划小时数。 使用“固定日期”以外的任何任务约束时，将调整计划持续时间。

下表说明了在向任务添加资源时，计划持续时间的变化情况：

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>受分配人数（每100%分配）</strong> </p> </th> 
   <th> <p><strong>持续时间</strong> </p> </th> 
   <th> <p><strong>计划小时</strong> </p> </th> 
   <th><strong>计划持续时间</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3天</p> </td> 
   <td> <p>24 小时</p> <p>（3天x每个工作日8小时= 24个计划小时）</p> </td> 
   <td> <p>3天</p> <p>（24计划时数/ 1受让人= 3天）</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3天</p> </td> 
   <td> <p>24 小时</p> <p>（3天x每个工作日8小时= 24个计划小时）</p> </td> 
   <td> <p>1.5天</p> <p>（24个计划时间/ 2个受让人= 12小时或1.5天）</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3天</p> </td> 
   <td> <p>24 小时</p> <p>（3天x每个工作日8小时= 24个计划小时）</p> </td> 
   <td> <p>1天</p> <p>（24个计划时间/ 3个受让人= 8小时或1天）</p> </td> 
  </tr> 
 </tbody> 
</table>

## 将任务的持续时间类型更改为工作驱动

有关更改任务的持续时间类型的信息，请参阅 [更新任务的持续时间类型](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Effort Driven</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong><strong>Changes</strong>.</li>
</ol>
-->
