---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 任务限制概述：尽快
description: “尽快”是一种任务限制，它使任务的开始时间尽可能接近项目的开始。
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# 任务限制概述：尽快

“尽快”是一种任务限制，它使任务的开始时间尽可能接近项目的开始。

## 使用“尽快”约束的注意事项

* 如果项目使用的计划模式为从起始日期开始计划，并且新任务的系统默认起始日期设置为基于项目计划日期，则“尽快”为默认限制。

* 如果项目使用“从起始日期开始计划”的计划模式，并且系统或组将新任务的默认“起始日期”设置为“今天”，则默认的“任务限制”为“起始日期不早于”。

  有关在何处为新任务设置默认约束的信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

有关如何更新任务的任务限制的信息，请参阅[更新任务的任务限制](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)。

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

## 最早可用时间与尽快之间的差异

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

当存在以下所有条件时，“最早可用时间”约束条件与“尽可能早”约束条件不同：

* 项目被列入完成计划。
* 项目中的任务具有前置任务关系。
* 前置任务具有灵活的任务限制。

在这种情况下：

* **最早可用时间：**&#x200B;对后续任务使用最早可用时间约束会优先处理前置任务的弹性约束。

  例如，假设任务A是任务B的前置任务。任务B具有“最早可用时间”限制，而任务A具有“尽可能晚于”限制。 在这种情况下，任务的计划时间应尽可能接近项目的完成时间。

* **尽快：**&#x200B;在此方案中，对后续任务使用“尽快”限制可授予后续任务的优先级。

  例如，假设任务A是任务B的前置任务。任务B具有尽可能早的限制，而任务A具有尽可能晚的限制。 在这种情况下，任务的计划时间应尽可能接近项目的开始时间。
