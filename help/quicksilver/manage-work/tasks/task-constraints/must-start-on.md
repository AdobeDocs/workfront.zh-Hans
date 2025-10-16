---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 任务限制概述：必须开始于
description: 使用“必须开始日期(MSO)”任务限制可以将任务计划为在特定日期完全开始。
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# 任务限制概述：必须开始时间

使用“必须开始日期(MSO)”任务限制可以将任务计划为在特定日期完全开始。

必须开始日期约束计划任务完全按照您在&#x200B;**计划开始日期**&#x200B;字段中指定的时间和日期开始。

>[!TIP]
>
>手动更新任务的计划开始日期会将任务的限制更改为必须开始于。

## 必须开始于任务限制的概述

在计划具有“必须开始于”限制的任务时，请考虑以下事项：

* 前置任务关系不会强制重新计划此任务。 Workfront实质上会忽略具有此约束的任务的任何前置任务关系。
* 如果前置任务开始落后或延迟，则任务显示&#x200B;**处于风险中**。

* 当您将具有MSO限制的任务移动或复制到另一个项目时，任务的限制或项目的日期可能会根据限制日期以及项目的开始和完成日期而更改。 存在以下情况：

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
<h2>Use the Must Start On Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Must Start On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Start On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start by this date, and no later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
