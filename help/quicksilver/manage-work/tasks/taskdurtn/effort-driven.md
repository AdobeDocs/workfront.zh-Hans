---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '持续时间类型概述：投入比导向'
description: 投入比导向是可以为Adobe Workfront中的任务设置的持续时间类型。 有关Workfront中持续时间类型的一般信息，请参阅任务持续时间和持续时间类型概述。
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 1%

---

# 持续时间类型概述：投入比导向

投入比导向是可以为Adobe Workfront中的任务设置的持续时间类型。 有关Workfront中持续时间类型的一般信息，请参阅[任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

## 投入比导向的持续时间类型概述

您的Workfront或组管理员可以将系统或组的默认持续时间类型设置为投入比导向。 在这种情况下，将使用此持续时间类型创建所有新任务。 有关将任务和问题首选项作为系统级或组级项目首选项的一部分进行更改的信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

在此情景中，除非您作为项目经理花时间考虑该任务是否实际上是一个投入比导向任务，否则存在着武断地缩短项目计划的风险。

使用投入比驱动可以：

* 根据可用于处理任务的资源数确定计划持续时间。 持续时间等于计划小时数。 计划持续时间等于计划小时数除以被分配人数量。

  应用于任务的工作量级别决定了分工和持续时间。

* 在分配了多个资源时跟踪在任务上花费的总小时数。

  当添加资源时，任务的计划持续时间会缩短。 （“多手轻工”的原则说明了此持续时间类型对任务的计划持续时间的影响。）

以下部分提供了有关Workfront如何计算投入比导向任务的计划持续时间以及添加资源对具有此持续时间类型的任务产生的影响的更多详细信息。

## 投入比导向的持续时间类型公式概述

工期类型为投入比导向的任务计划工期的计算公式取决于分配给任务的每个资源的分配百分比。 对于投入比导向任务，Workfront会计算任务的已计划小时数，这些小时数始终与任务的持续时间相同：

```
Planned Hours (in hours) = Duration (in days)
```

您可以手动调整任务的持续时间。

Workfront假定每天有8个工作小时。 您的Workfront或组管理员使用“设置”中“项目首选项”的“每个工作日的典型小时数”设置来定义每个工作日的小时数。 有关将任务和问题首选项作为系统级项目首选项的一部分进行更改的详细信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

>[!TIP]
>
>Workfront会考虑分配给任务的每个资源的计划，以确定任务每个资源的分配百分比。 有关创建计划并将其分配给用户的信息，请参阅[创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

请考虑以下情况：

* [资源100%分配给任务](#resources-are-allocated-100-to-the-task)
* [资源按任务的不同时间百分比分配](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### 资源100%分配给任务 {#resources-are-allocated-100-to-the-task}

此公式假定所有资源都分配给100%的任务。

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

此计算假定正常工作日的小时数为8。 方程式包含此值，因此计划持续时间以天为单位显示。

### 资源按任务的不同时间百分比分配 {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

由于每个分配的资源可以具有唯一的分配层，因此实际公式会考虑这些分配值：

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

此计算假定正常工作日的小时数为8。 方程式包含此值，因此计划持续时间以天为单位显示。

## 向任务添加更多资源的影响

向具有投入比驱动持续时间类型的任务添加或移除被分配人时，持续时间和已计划小时数不会更改。 但是，计划持续时间会发生变化。

在以下示例中，系统设置中的项目首选项将每个工作日的典型小时数设置为8。 由于持续时间为3天，因此计划小时数设置为24（3天x8小时每工作日= 24计划小时数）。

>[!NOTE]
>
>使用固定日期任务限制时，在添加或删除被分配人时，计划持续时间保持不变，而是调整持续时间和计划小时数。 使用固定日期以外的任何任务限制时，将调整计划持续时间。

下表说明了计划持续时间如何随着将资源添加到任务而变化：

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>受分配人数量（每100%分配）</strong> </p> </th> 
   <th> <p><strong>持续时间</strong> </p> </th> 
   <th> <p><strong>计划小时数</strong> </p> </th> 
   <th><strong>计划持续时间</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3天</p> </td> 
   <td> <p>24 小时</p> <p>（3天x每个工作日8小时= 24计划小时）</p> </td> 
   <td> <p>3天</p> <p>（24个计划小时数/ 1个被分派人= 3天）</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3天</p> </td> 
   <td> <p>24 小时</p> <p>（3天x每个工作日8小时= 24计划小时）</p> </td> 
   <td> <p>1.5天</p> <p>（24个计划小时数/ 2个受让人= 12小时或1.5天）</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3天</p> </td> 
   <td> <p>24 小时</p> <p>（3天x每个工作日8小时= 24计划小时）</p> </td> 
   <td> <p>1天</p> <p>（24个计划小时数/ 3个受让人= 8小时或1天）</p> </td> 
  </tr> 
 </tbody> 
</table>

## 将任务的持续时间类型更改为投入比导向

有关更改任务的持续时间类型的信息，请参阅[更新任务的持续时间类型](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)。

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
