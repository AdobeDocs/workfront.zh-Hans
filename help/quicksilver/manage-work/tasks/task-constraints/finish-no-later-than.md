---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '任务限制概述：完成时间不晚于'
description: “完成时间不晚于(FNLT)”是一种任务限制，它计划任务在您指定的日期之前完成。
author: Alina
feature: Work Management
exl-id: ea0e74fb-45a0-4466-b57d-294a9babb340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# 任务限制概述：完成时间不晚于

“完成时间不晚于(FNLT)”是一种任务限制，它计划任务在您指定的日期之前完成。

## 完成时间不晚于约束条件的概览

为任务使用“完成时间不晚于(FNLT)”限制时，请考虑以下事项：

* 当从开始日期开始安排项目时，您应使用此限制。 在这种情况下，您可以先对任务提供软约束，然后再强制其他依赖任务显示为处于风险中。
* 如果将FNLT约束与“计划自完成日期”项目一起使用，则此约束会计划尽可能晚的任务。
* 在将具有FNET约束的任务移动或复制到另一个项目时，任务的约束或项目的日期可能会根据约束日期以及项目的开始日期和完成日期而更改。 存在以下情况：

   * 当目标项目计划为从开始日期起时：

      * 当任务的限制日期早于项目的计划开始日期时，任务限制会尽快更改为。
      * 当任务的限制日期晚于项目计划完成日期时，项目计划完成日期将更改为匹配任务的完成限制日期。

      * 当目标项目计划为从完成开始时：

         * 当任务的限制日期晚于项目完成日期时，任务限制会变为“尽可能晚于”。
         * 当任务的限制日期早于项目的计划起始日期时，项目计划起始日期将更改为匹配任务的起始限制日期。

      * 无论项目计划如何，当任务的限制日期在项目的开始日期和完成日期之内时，任务限制日期或项目日期都不会发生更改。

  有关移动任务的信息，请参阅[移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md)。 有关复制任务的信息，请参阅[复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

有关如何更新任务的任务限制的信息，请参阅[更新任务的任务限制](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Finish No Later Than constraint</h2>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Finish No Later Than</strong>.</p> <p> <img src="assets/fnlt-350x266.png" alt="FNLT.png" style="width: 350;height: 266;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>You must complete the task on and not later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
