---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '任务限制概述：开始时间不晚于'
description: “开始时间不晚于(SNLT)”是一种任务限制，它计划任务在指定的日期之前开始。
author: Alina
feature: Work Management
exl-id: 86139ce6-c6b1-4ac4-a5cb-fd4aa899a025
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# 任务限制概述：开始时间不晚于

“开始时间不晚于(SNLT)”是一种任务限制，它计划任务在指定的日期之前开始。

使用SNLT约束条件时，请考虑以下事项：

* 当从完成日期开始计划项目时，您应使用开始时间不晚于限制。 在这种情况下，您可以先对任务提供软约束，然后再强制其他依赖任务显示为处于风险中。
* 如果项目使用的计划模式为“从完成日期开始计划”，并且任务的“开始日期”的系统或组默认值是“今天”，则起始时间不晚于默认限制条件。 有关在何处为新任务设置默认约束的信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。
* 当您使用SNLT限制条件和“从开始日期开始计划”项目时，Adobe Workfront会像计划尽快任务一样计划该任务。
* 在将具有SNLT限制的任务移动或复制到另一个项目时，任务的限制或项目的日期可能会根据限制日期以及项目的开始日期和完成日期而更改。 存在以下情况：

   * 当目标项目计划为从开始日期起时：

      * 当任务的限制日期早于项目的计划开始日期时，任务限制会尽快更改为。
      * 当任务的限制日期晚于项目计划完成日期时，项目计划完成日期将更改为匹配任务的完成限制日期。

      * 当目标项目计划为从完成开始时：

         * 当任务的限制日期晚于项目完成日期时，任务限制会变为“尽可能晚于”。
         * 当任务的限制日期早于项目的计划起始日期时，项目计划起始日期将更改为匹配任务的起始限制日期。

      * 无论项目计划如何，当任务的限制日期在项目的开始日期和完成日期之内时，任务限制日期或项目日期都不会发生更改。

  有关移动任务的信息，请参阅[移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md)。

  有关复制任务的信息，请参阅[复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

有关如何更新任务的任务限制的信息，请参阅[更新任务的任务限制](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Start No Later Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Later Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>.<br></li>
</ol>
</div>
-->
