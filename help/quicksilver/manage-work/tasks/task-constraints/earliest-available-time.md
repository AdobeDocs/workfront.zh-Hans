---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: “任务约束概述：最早可用时间”
description: 最早可用时间是任务约束，它将任务安排为在考虑任何前置任务关系后的最早可用时间开始。
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# 任务约束概述：最早可用时间

最早可用时间是任务约束，它将任务安排为在考虑任何前置任务关系后的最早可用时间开始。

有关如何更新任务上的任务约束的信息，请参阅 [更新任务的任务约束](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above) </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To update the Task Constraint to Earliest Available Time:</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit Task</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Earliest Available Time</strong>.</p>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save Changes</strong>.</li>
   -->

## 最早可用时间与尽快可用的时间之差

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

当存在以下所有条件时，“最早可用时间”约束与“尽快”约束不同：

* 项目计划完成
* 项目中的任务具有前置关系
* 前置任务具有灵活的任务约束

在这种情况下：

* **最早可用时间：** 在后续任务上使用最早可用时间约束优先于先前任务的灵活约束。

   **示例：** 任务A是任务B的前身。任务B具有最早的可用时间约束，任务A具有尽可能晚的约束。 在这种情况下，任务B将安排在尽可能接近项目完成的时间。

   ![当任务的日期接近项目的完成日期时，“最早可用时间”约束](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **尽快：** 在此方案中，对后续任务使用“尽快”约束将优先级赋予后续任务。

   **示例：**  任务A是任务B的前身。任务B具有尽快的约束，任务A具有尽快的约束。 在这种情况下，任务B将安排在尽可能靠近项目开始的位置。

   ![任务的日期接近项目的开始日期时，尽快设置约束](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
