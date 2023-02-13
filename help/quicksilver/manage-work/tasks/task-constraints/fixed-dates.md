---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: “任务约束概述：固定日期的
description: 如果希望具体说明任务的确切开始日期和结束日期，可以使用固定日期任务约束。 有关任务约束的详细信息，请参阅任务约束概述。
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 任务约束概述：固定日期

如果希望具体说明任务的确切开始日期和结束日期，可以使用固定日期任务约束。 有关任务约束的详细信息，请参阅 [任务约束概述](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## 固定日期约束概述

使用固定日期约束时请考虑以下事项：

* 选择固定日期(FIXT)任务约束时，必须指定任务的计划起始日期和计划完成日期。 在这种情况下，将忽略任务的前置关系。
* 使用FIXT约束时，任务的“持续时间”字段不可编辑。 持续时间计算为任务的计划起始日期和计划完成日期之间的差值。
* 如果任务的“持续时间类型”为“工作驱动”，则任务上的受分配者数量也会影响任务的持续时间。
* 在将具有FIXT约束的任务移动或复制到另一个项目时，任务的约束或项目日期可能会根据约束日期和项目的开始和完成日期而改变。 存在以下情形：

   * 当目标项目计划从开始时：

      * 当任务的任何约束日期早于项目开始日期时，任务约束将变为“尽快”。
      * 当任务的任意或两个约束日期晚于项目的计划完成日期时，项目计划完成日期将更改以匹配任务的完成约束日期。
   * 当目标项目计划完成时：

      * 当任务的任何约束日期晚于项目完成日期时，任务约束将变为“尽可能晚”。
      * 当任务的任何或两个约束日期早于项目的计划起始日期时，项目计划起始日期会更改以匹配任务的起始约束日期。
   * 无论项目的计划如何，当任务的约束日期在项目的“开始”和“完成”日期之内时，“任务约束”或项目日期都不会发生更改。

   有关移动任务的信息，请参阅 [移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md). 有关复制任务的信息，请参阅 [复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

有关如何更新任务上的任务约束的信息，请参阅 [更新任务的任务约束](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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
