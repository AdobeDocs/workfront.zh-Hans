---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '任务约束概览：最早可用时间'
description: 最早可用时间是一个任务限制，它计划在考虑任何前置任务关系后的最早可用时间开始任务。
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# 任务约束概览：最早可用时间

最早可用时间是一个任务限制，它计划在考虑任何前置任务关系后的最早可用时间开始任务。

有关如何更新任务的任务限制的信息，请参阅 [更新任务的任务限制](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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

## 最早可用时间与尽可能早之间的时间差

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

当存在以下所有条件时，“最早可用时间”约束与“尽可能早”约束不同：

* 项目计划自完成开始
* 项目中的任务具有前置任务关系
* 前置任务具有灵活的任务限制

在这种情况下：

* **最早可用时间：** 对后继任务使用最早可用时间限制会优先处理前继任务的灵活限制。

   **示例**

   任务A是任务B的前置任务。任务B具有最早可用时间限制，而任务A具有尽可能晚的时间限制。 在此情况下，任务B被安排在尽可能接近项目完成的阶段。

   ![当任务的日期接近项目的完成日期时，最早可用时间限制](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **尽快：** 在此场景中，对后续任务使用“越早越好”限制可为后续任务赋予优先级。

   **示例**

   任务A是任务B的前身。任务B具有尽可能早的限制条件，而任务A具有尽可能晚的限制条件。 在这种情况下，任务B的计划时间应尽可能接近项目的开始时间。

   ![尽快限制当任务的日期接近项目的开始日期时](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
