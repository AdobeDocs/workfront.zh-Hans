---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 任务限制概览：完成时间不早于
description: “完成时间不早于(FNET)”是一种任务限制，它计划在指定日期之后完成任务。
author: Alina
feature: Work Management
exl-id: b1dbf5c9-34b6-4c25-b582-ce9454501e03
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 任务限制概览：完成时间不早于

“完成时间不早于(FNET)”是一种任务限制，它计划在指定日期之后完成任务。

## 完成时间不早于约束条件的概览

为任务使用不早于(FNET)完成限制时，请考虑以下事项：

* 当项目计划自完成日期开始时，您应使用此限制。 在这种情况下，您可以先对任务提供软约束，然后再强制其他依赖任务显示“处于风险中”。
* 当您对计划为&#x200B;**从开始日期**&#x200B;开始的项目使用FNET时，约束将计划该任务，就像在约束尽可能快的情况下计划任务一样。
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
<h2>Use the Finish No Earlier Than constraint</h2>
<p>(NOTE: replaced with new article linked above)&nbsp;</p>
<p>To update the Task Constraint to Finish No Earlier Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>Finish No Earlier Than</strong>.</p> <p> <img src="assets/fnet-350x267.png" alt="FNET.png" style="width: 350;height: 267;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete no earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes.</strong> </li>
</ol>
</div>
-->
