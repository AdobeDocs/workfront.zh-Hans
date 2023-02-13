---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: “任务约束概述：必须在“”时完成
description: 您可以使用“必须完成(MFO)任务约束”来安排任务在特定日期结束。
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# 任务约束概述：必须完成

您可以使用“必须完成(MFO)任务约束”来安排任务在特定日期结束。

“必须完成”(Must Finish On)约束计划任务，以完成您在 **计划完成日期** 字段。

>[!TIP]
>
>人工更新任务的计划完成日期会将任务的约束更改为必须完成。

## 任务约束必须完成的概述

在计划具有“必须完成”(Must Finish)约束的任务时，请考虑以下事项：

* 前置关系不强制重新计划任务。 Adobe Workfront实际上忽视了前身关系。
* 任务显示为 **面临风险** 如果前任们开始落后或迟到。

* 在将具有MFO约束的任务移动或复制到另一个项目时，任务的约束或项目日期可能会根据约束日期和项目的开始和完成日期而改变。 存在以下情形：

   * 当目标项目计划从开始时：

      * 当任务的约束日期早于项目计划起始日期时，任务约束将变为“尽快”。
      * 当任务的约束日期晚于项目计划完成日期时，项目计划完成日期将更改以匹配任务的完成约束日期。

      * 当目标项目计划完成时：

         * 当任务的约束日期晚于项目完成日期时，任务约束将变为“尽可能晚”。
         * 当任务的约束日期早于项目的计划起始日期时，项目计划起始日期会更改以匹配任务的起始约束日期。
      * 无论项目的计划如何，当任务的约束日期在项目的“开始”和“完成”日期之内时，“任务约束”或项目日期都不会发生更改。

   有关移动任务的信息，请参阅 [移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md). 有关复制任务的信息，请参阅 [复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

有关如何更新任务上的任务约束的信息，请参阅 [更新任务的任务约束](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Must Finish On Task Constraint</h2>
<p>To update the Task Constraint to Must Finish On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Finish On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete by this date, and no later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
