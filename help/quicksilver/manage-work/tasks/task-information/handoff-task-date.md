---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任务移交日期概述
description: 移交日期是任务可供工作的日期。 这通常意味着其前置任务已解决，并且任务的被分派人可以开始处理它。
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 2%

---

# 任务移交日期概述

移交日期是任务可供工作的日期。 这通常意味着其前置任务已解决，并且任务的被分派人可以开始处理它。

>[!TIP]
>
>问题和项目的移交日期不存在。

## Adobe Workfront如何计算移交日期

>[!NOTE]
>
>仅当项目状态等于以下状态时，才会计算移交日期：
>
>* 暂停
>* 目前
>* 完成
>* 已停止
>

Workfront使用以下规则计算任务的移交日期：

* **当任务具有未完成的前置任务时**：任务的移交日期为null。
* **当任务具有完整的前置任务时**：移交日期与前置任务的实际完成日期相同。 如果前置任务有延迟，Workfront会使用以下公式计算后续任务的移交日期：

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  有关滞后时间的信息，请参阅[滞后类型概述](../use-prdcssrs/lag-types.md)。

  如果后续任务有多个前置任务，则根据前置任务的最近实际完成日期计算移交日期。 例如，如果两个前置任务的实际完成日期分别为2022年11月8日和2022年11月20日，则后续任务的移交日期为2022年11月20日。

  >[!NOTE]
  >
  >   不管是否强制前置任务，根据实际完成日期或前置任务计算后续任务的移交日期是相同的。 有关强制前置任务的详细信息，请参阅[强制前置任务](../use-prdcssrs/enforced-predecessors.md)。


* **当任务没有前置任务和**&#x200B;时：

   * **计划开始日期在过去**：如果任务没有强制设置约束，则移交日期与项目的计划开始日期相同。 有关任务具有强制限制的情况，请参阅下面的“当任务具有计划日期的强制限制时”部分。
   * **计划开始日期是将来的日期（当前日期之后的任何日期）**：如果任务未设置强制约束，则移交日期与任务的计划开始日期相同。 有关任务具有强制限制的情况，请参阅下面的“当任务具有计划日期的强制限制时”部分。

>[!NOTE]
>
>当任务具有跨项目前置任务时，仅当出现以下任一情况时，才会重新计算后置任务的移交日期：
>
>* 您可以手动重新计算接替者项目的时间表。 您必须具有项目的管理权限才能重新计算时间线。
>* 后继项目的时间表在夜间自动重新计算。
>
>有关重新计算项目时间表的信息，请参阅[重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)。

* **当任务具有计划日期的强制限制时**：切换日期因限制类型以及任务是否具有实际开始日期而有所不同。\
  以下是对任务的强制约束：

   * 必须开始时间
   * 必须完成时间
   * 开始时间不早于
   * 开始时间不晚于
   * 固定日期

  存在以下情况：

   * **当任务具有必须开始日期或开始日期不早于**&#x200B;的限制时：如果任务限制日期是过去的，并且任务没有实际开始日期（任务尚未开始），则移交日期是任务可以开始工作的最近日期。 如果任务已开始，则移交日期等于项目的开始日期。
   * **当任务的限制为“必须完成于”或“开始时间不晚于**”时：如果任务限制日期是未来的日期，并且任务没有实际开始日期（任务尚未开始），则移交日期是任务的计划开始日期。 如果任务具有实际开始日期，则移交日期是项目的开始日期。
   * **当任务具有固定日期的限制时**：移交日期是任务的计划开始日期，无论任务是否有前置任务，也无论前置任务是否已完成。

<!--these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## 找到移交日期

您可以在任务报告或任务列表视图中显示任务的移交日期。\
有关生成报告的详细信息，请参阅[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
