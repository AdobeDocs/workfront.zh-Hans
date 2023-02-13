---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: “任务约束概述：最新可用时间”
description: “最新可用时间(LAT)”是Adobe Workfront中的一种任务约束类型。
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 任务约束概述：最新可用时间

“最新可用时间(LAT)”是Adobe Workfront中的一种任务约束类型。

## 使用最新可用时间任务约束

如果您希望计划在项目中考虑前置 — 后继关系后，在最晚的可用时间开始任务，则可以使用LAT约束。

此约束与“尽快”不同，因为它不会强制重新计划前置任务或后置任务。 相反，它只会影响与其关联的任务的计划，并根据与其他任务的关系将其设置为最新的可用时间。

有关如何更新任务上的任务约束的信息，请参阅 [更新任务的任务约束](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To update the Task Constraint to Latest Available Time:</p>
<p>(NOTE:&nbsp;replaced with new article linked above)&nbsp;</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Latest Available Time</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## 最新可用时间与尽可能晚一些的时间之差

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
-->

当存在以下条件时，“最新可用时间”约束与“尽可能晚一些”约束不同：

* 项目计划从开始日期开始
* 项目中的任务具有前置关系
* 后续任务具有灵活的任务约束

在这种情况下：

* **最新可用时间：** 在前置任务上使用“最新可用时间”(Latest Available Time)约束时，优先考虑后置任务的灵活约束。

   **示例：** 例如，任务A是任务B的前身。任务A具有最新的可用时间约束，任务B具有尽快约束。 在这种情况下，任务A将安排在尽可能靠近项目开始的位置。

   ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **尽可能晚：** 在此方案中，对前置任务使用“尽可能晚”(As Late Ap Possiby)约束将优先考虑前置任务。

   **示例：** 例如，任务A是任务B的前身。任务A具有尽可能晚的约束，任务B具有尽可能快的约束。 在这种情况下，任务A将安排在尽可能靠近项目结束的位置。

   ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
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
