---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: “持续时间类型概述：计算工作”
description: “计算工作”是一种持续时间类型，您可以在Adobe Workfront中为任务设置该类型。 有关Workfront中持续时间类型的常规信息，请参阅任务持续时间和持续时间类型概述。
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 1%

---

# 持续时间类型概述：计算量度

“计算工作”是一种持续时间类型，您可以在Adobe Workfront中为任务设置该类型。 有关Workfront中持续时间类型的常规信息，请参阅 [任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## 计算的工作持续时间类型概述

计算工作确定完成任务所需的工作量（计划小时数）。 如果分配给任务的资源在整个任务期间被分配，我们建议您使用计算的工作持续时间类型。

您的Workfront或组管理员可以将系统或组的默认持续时间类型设置为计算量度。 在这种情况下，将使用此持续时间类型创建所有新任务。 有关更改任务和发布首选项作为系统级别或组级别项目首选项的一部分的信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

在将资源添加到任务中时，项目经理可能会看到计划工作量的增加。 为了说明这一点，一个包含三个资源的一小时计划会议代表总共需要三个工作小时，一个包含十个资源的一小时计划会议代表需要十个工作小时。 这假定每个资源都已分配到分配了100%的任务。

## 复查在使用计算的工作持续时间类型时计算所需工作的公式

在任务上使用“计算的工作持续时间类型”时，Workfront会使用以下两个公式计算每个任务的工作量。 公式会因每个资源分配到任务的时间百分比以及您分配给每个任务的资源数量而异：

* 简化公式：如果您为任务分配了一个资源，并且这些资源在任务可用时间的100%内被分配给任务，则使用以下公式计算每个任务的“需要工作”值：

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* 复杂公式：如果您为每个资源分配了各种分配，则公式会将这些分配考虑在内，并考虑这些变量：

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## 查看在任务中添加或删除资源的效果

在向具有“计算的工作持续时间”类型的任务添加或删除受分配者时，可以手动编辑“持续时间”。 在任务中添加或删除任务分配者时，“计划小时数”会发生更改。

在以下示例中，“设置”的“项目首选项”中的“每个工作日的典型小时数”设置为8。 每个任务的持续时间为1天。 随着受分配人数的变化，计划小时数会根据给定任务上的受分配人数而变化：

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>受分配人数（每100%分配）</strong> </p> </th> 
   <th> <p><strong>持续时间</strong> </p> </th> 
   <th> <p><strong>计划小时</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1天</p> </td> 
   <td> <p>8 小时</p> <p>（1天x每个工作日8小时x 1代理人= 8计划小时）</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1天</p> </td> 
   <td> <p>16小时</p> <p>（1天x每个工作日8小时x 2个受派人= 16个计划小时）</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1天</p> </td> 
   <td> <p>24 小时</p> <p>（1天x每个工作日8小时x 3个受派人= 24个计划小时）</p> </td> 
  </tr> 
 </tbody> 
</table>

在这种情况下，每个受分配人将100%分配给“计算工作”任务。

![](assets/calcwork-350x71.png)

## 将任务的持续时间类型更改为计算工作

有关更改任务的持续时间类型的信息，请参阅 [更新任务的持续时间类型](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
