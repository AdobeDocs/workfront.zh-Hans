---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: “任务约束概述：尽可能晚”
description: 尽可能晚(ALAP)是Adobe Workfront任务约束，它将任务的完成时间放在尽可能靠近项目结束的位置。
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# 任务约束概述：尽可能晚

尽可能晚(ALAP)是Adobe Workfront任务约束，它将任务的完成时间放在尽可能靠近项目结束的位置。

使用此约束可能会导致重新计划前置任务或从属任务。

有关前身关系的更多信息，请参阅 [使用任务前置任务](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

如果项目使用计划模式“从完成日期开始计划”，并且任务的起始日期默认为“基于项目计划日期”，则“尽可能晚”是默认约束。

有关在何处为新任务设置默认约束的信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

有关如何更新任务上的任务约束的信息，请参阅 [更新任务的任务约束](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible:&nbsp;</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click&nbsp;<strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the&nbsp;<strong>Overview</strong>&nbsp;section, expand the&nbsp;<strong>Task Constraint</strong>&nbsp;drop-down menu.</p> </li>
<li value="4"> <p>Select&nbsp;<strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.&nbsp;</li>
</ol>
</div>
-->

## 最新可用时间与尽可能晚一些的时间之差

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
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
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest&nbsp;Available Time constraint differs from the As Late&nbsp;As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest&nbsp;Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest&nbsp;Available Time constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close&nbsp;to the start&nbsp;of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late&nbsp;As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late&nbsp;As Possible&nbsp;constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close to the end&nbsp;of the project as possible.</p> </li>
</ul>
</div>
-->
