---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 任务限制概览：尽可能迟
description: 尽可能迟(ALAP)是一种Adobe Workfront任务限制，它使任务的完成时间尽可能接近项目的结尾。
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# 任务限制概览：尽可能迟

尽可能迟(ALAP)是一种Adobe Workfront任务限制，它使任务的完成时间尽可能接近项目的结尾。

使用此约束可能导致前置任务或从属任务被重新计划。

有关前置任务关系的详细信息，请参阅[使用前置任务：文章索引](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md)。

如果项目使用的计划模式为“从完成日期开始计划”，并且任务的“起始日期”的系统或组默认值基于项目计划日期，则“尽可能晚于”为默认约束。

有关在何处为新任务设置默认约束的信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

有关如何更新任务的任务限制的信息，请参阅[更新任务的任务限制](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## 最新可用时间和尽可能晚之间的差异

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
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
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
