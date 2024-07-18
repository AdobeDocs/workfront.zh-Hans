---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '任务限制概述：最新可用时间'
description: 最新可用时间(LAT)是Adobe Workfront中的一种任务限制类型。
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
source-git-commit: c3abb5dce14c0b19ab2e5b82f159cd29f80f79e4
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 任务限制概述：最新可用时间

最新可用时间(LAT)是Adobe Workfront中的一种任务限制类型。

## 使用最新可用时间任务限制

当考虑项目中的前置任务 — 后续任务关系后，要计划任务在最新的可用时间开始时，可以使用LAT约束。

此限制与“尽快”的不同之处在于，它不会强制重新计划前置任务或后续任务。 相反，它只会影响与其关联的任务的计划，根据其与其他任务的关系将其设置为最新可用时间。

有关如何更新任务的任务限制的信息，请参阅[更新任务的任务限制](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To update the Task Constraint to Latest Available Time:</p>
<p>(NOTE: replaced with new article linked above) </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Latest Available Time</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## 最新可用时间和尽可能晚之间的差异

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
-->

当存在以下条件时，“最新可用时间”约束与“尽可能晚到”约束不同：

* 项目计划自开始日期起执行
* 项目中的任务具有前置任务关系
* 后续任务具有灵活的任务限制

在这种情况下：

* **最新可用时间：**&#x200B;对前置任务使用最新可用时间约束会优先使用后置任务的灵活约束。

  **示例：**&#x200B;例如，任务A是任务B的前置任务。任务A具有最新可用时间限制，而任务B具有“尽快”限制。 在此情况下，任务A被安排在尽可能接近项目开始的时间。

  ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **尽可能迟：**&#x200B;在此方案中，对前置任务使用尽可能晚的限制将优先处理前置任务。

  **示例：**&#x200B;例如，任务A是任务B的前置任务。任务A具有尽可能晚的限制，而任务B具有尽可能早的限制。 在这种情况下，任务A被安排在尽可能接近项目结束的时间。

  ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest Available Time constraint differs from the As Late As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
