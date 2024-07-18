---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '持续时间类型概述：计算的工作量'
description: 计算的工作量是一种持续时间类型，您可以在Adobe Workfront中为任务设置此类型。 有关Workfront中持续时间类型的一般信息，请参阅任务持续时间和持续时间类型概述。
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 1%

---

# 持续时间类型概览：计算的工作量

计算的工作量是一种持续时间类型，您可以在Adobe Workfront中为任务设置此类型。 有关Workfront中持续时间类型的一般信息，请参阅[任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

## 计算的工作持续时间类型概述

计算的工作量确定完成任务所需的工作量（计划小时数）。 当分配给任务的资源被分配用于任务的整个持续时间时，我们建议您使用计算的工作持续时间类型。

您的Workfront或组管理员可以将系统或组的默认持续时间类型设置为计算的工作量。 在这种情况下，将使用此持续时间类型创建所有新任务。 有关将任务和问题首选项作为系统级或组级项目首选项的一部分进行更改的信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

在将资源添加到任务时，项目经理可能会看到计划的工作量增加。 举例来说，一个有三种资源的1小时规划会议代表总共需要3个小时的工作，一个有十种资源的1小时规划会议代表需要10个小时的工作。 这假定每个资源都按100%的分配分配给任务。

## 查看使用计算的工作持续时间类型时用于计算所需工作的公式

在任务上使用“计算的工作持续时间类型”时，Workfront会使用以下两个公式计算每个任务的工作量。 根据每个资源分配给任务的时间百分比以及分配给每个任务的资源数量，公式会有所不同：

* 简化公式：假设您有一个资源分配给任务，并且这些资源在任务可用时间的100%内分配给任务，则可以使用以下公式计算每个任务的“所需工作”值：

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* 复杂公式：如果您使用各种分配分配分配每个资源，则公式会将这些分配考虑在内，并计入这些变化：

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## 查看在任务中添加或删除资源的效果

在具有“已计算的工作持续时间”类型的任务中添加或删除被分配人时，可以手动编辑持续时间。 当在任务中添加或删除被分配人时，计划小时数会发生更改。

在以下示例中，在“设置”的项目首选项中，将每个工作日的典型小时数设置为8。 每项任务的工期均为1天。 随着被分配人数量的变化，计划小时数也会根据给定任务的被分配人数量而变化：

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>受分配人数量（每100%分配）</strong> </p> </th> 
   <th> <p><strong>持续时间</strong> </p> </th> 
   <th> <p><strong>计划小时数</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1天</p> </td> 
   <td> <p>8 小时</p> <p>（1天x每个工作日8小时x 1被分派人= 8计划小时）</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1天</p> </td> 
   <td> <p>16小时</p> <p>（1天x每个工作日8小时x 2被分派人= 16计划小时）</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1天</p> </td> 
   <td> <p>24 小时</p> <p>（1天x每个工作日8小时x 3被分配人= 24计划小时）</p> </td> 
  </tr> 
 </tbody> 
</table>

在这种情况下，每个被分派人100%分配给“计算的工作”任务。

![](assets/calcwork-350x71.png)

## 将任务的持续时间类型更改为计算的工作量

有关更改任务的持续时间类型的信息，请参阅[更新任务的持续时间类型](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Work</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
