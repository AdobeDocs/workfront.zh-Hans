---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 任务限制概览：开始时间不早于
description: 使用“开始时间不早于(SNET)任务限制”将任务调度为在指定的日期之后开始。
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# 任务限制概览：开始时间不早于

使用“开始时间不早于(SNET)任务限制”将任务调度为在指定的日期之后开始。

## 开始日期不早于任务限制的概览

使用“开始时间不早于任务限制”时，请考虑以下事项：

* 当从开始日期开始计划项目时，您应使用“开始时间不早于”约束条件。 在这种情况下，您可以先对任务提供软约束，然后再强制其他依赖任务显示为处于风险中。
* 如果项目计划为从起始日期开始，并且新任务的系统或组默认起始日期设置为今天，则起始日期不早于是默认约束条件。 有关为任务配置默认设置的信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

* 如果您计划项目起始日期，并且新任务的系统默认起始日期设置为基于项目计划日期，则新任务的默认限制为“尽快”。
* 如果计划项目自完成日期项目，并且新任务的系统默认起始日期设置为“今天”，则“起始日期不早于”约束将计划该任务，因为它将计划尽可能晚的任务。
* 在将具有SNET限制的任务移动或复制到另一个项目时，任务的限制或项目的日期可能会根据限制日期以及项目的开始日期和完成日期而更改。 存在以下情况：

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
<h2>Use the Start No Earlier Than Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above)&nbsp;</p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Earlier Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
