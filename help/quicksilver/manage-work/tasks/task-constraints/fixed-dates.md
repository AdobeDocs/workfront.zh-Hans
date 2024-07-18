---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '任务限制概述：固定日期'
description: 当您想要明确了解任务的确切开始日期和结束日期时，可以使用固定日期任务限制。 有关任务限制的详细信息，请参阅任务限制概述。
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 任务限制概览：固定日期

当您想要明确了解任务的确切开始日期和结束日期时，可以使用固定日期任务限制。 有关任务限制的更多信息，请参阅[任务限制概述](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)。

## 固定日期约束概览

使用固定日期限制时，请考虑以下事项：

* 在选择固定日期(FIXT)任务限制时，必须指定任务的计划起始日期和计划完成日期。 在这种情况下，任务的前置任务关系将被忽略。
* 使用FIXT约束时，任务的持续时间字段不可编辑。 持续时间计算为任务的计划开始日期和计划完成日期之间的差值。
* 如果任务的工期类型为投入比导向，则任务上的任务接受者数量也会影响任务的工期。
* 在将具有FIXT约束的任务移动或复制到另一个项目时，任务的约束或项目的日期可能会根据约束日期以及项目的开始日期和完成日期而更改。 存在以下情况：

   * 当目标项目计划为从开始日期起时：

      * 当任务的任何限制日期早于项目开始日期时，任务限制会尽快更改为。
      * 当任务的任何或两个限制日期晚于项目的计划完成日期时，项目计划完成日期将更改以匹配任务的完成限制日期。

   * 当目标项目计划为从完成开始时：

      * 当任务的任何限制日期晚于项目完成日期时，任务限制会尽可能晚地更改。
      * 当任务的任何或两个限制日期早于项目的计划起始日期时，项目计划起始日期将更改为匹配任务的起始限制日期。

   * 无论项目计划如何，当任务的限制日期在项目的开始日期和完成日期之内时，对任务限制日期或项目日期均没有更改。

  有关移动任务的信息，请参阅[移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md)。 有关复制任务的信息，请参阅[复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

有关如何更新任务的任务限制的信息，请参阅[更新任务的任务限制](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Fixed Dates</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start on this date. </p> </li>
<li value="6"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete on this date. </p> </li>
<li value="7">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
