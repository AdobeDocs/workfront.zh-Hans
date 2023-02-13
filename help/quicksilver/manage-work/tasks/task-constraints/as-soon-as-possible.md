---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: “任务约束概述：尽快”
description: “尽快”是一项任务约束，它将任务的开始时间尽可能靠近项目的开始时间。
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# 任务约束概述：尽快

“尽快”是一项任务约束，它将任务的开始时间尽可能靠近项目的开始时间。

## 使用尽快约束的注意事项

* 如果项目使用从起始日期开始的计划模式，并且新任务的系统默认起始日期设置为基于项目计划日期，则“尽快”是默认约束。

* 如果项目使用从开始日期开始计划的计划模式，并且新任务的系统或组默认的开始日期设置为今天，则默认的任务约束为不早于开始。

   有关在何处为新任务设置默认约束的信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

有关如何更新任务上的任务约束的信息，请参阅 [更新任务的任务约束](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Soon As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Soon As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## 最早可用时间与尽快可用的时间之差

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

当存在以下所有条件时，“最早可用时间”约束与“尽快”约束不同：

* 项目已计划完成。
* 项目中的任务具有前置关系。
* 前置任务具有灵活的任务约束。

在这种情况下：

* **最早可用时间：** 在后续任务上使用最早可用时间约束优先于先前任务的灵活约束。

   例如，假定任务A是任务B的前身。任务B具有最早可用时间约束，任务A具有尽可能晚的约束。 在这种情况下，任务将安排在尽可能接近项目完成的位置。

* **尽快：** 在此方案中，对后续任务使用“尽快”约束将优先级赋予后续任务。

   例如，假定任务A是任务B的前身。任务B具有尽快约束，任务A具有尽可能晚的约束。 在这种情况下，任务会安排在尽可能靠近项目开始的位置。
