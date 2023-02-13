---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任务切换日期概述
description: “切换日期”是任务可用于工作的日期。 这通常意味着其前任任务已解决，任务的受让人可以开始处理它。
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: 39efbf1d678cf85e9b6b61744fb046664992370c
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 3%

---

# 任务切换日期概述

“切换日期”是任务可用于工作的日期。 这通常意味着其前任任务已解决，任务的受让人可以开始处理它。

>[!TIP]
>
>问题和项目不存在切换日期。

## Adobe Workfront如何计算切换日期

>[!NOTE]
>
>仅当项目状态等于以下状态时，才计算切换日期：
>
>* 保持
>* 目前
>* 完成
>* 废弃
>


Workfront使用以下规则计算任务的切换日期：

* **当任务的前置任务不完整时**:任务的切换日期为空。
* **当任务具有完整的前置任务时**:切换日期与前置任务的实际完成日期相同。 如果前置任务存在滞后，Workfront将使用以下公式计算后续任务的切换日期：

   `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

   有关滞后时间的信息，请参阅 [滞后类型概述](../use-prdcssrs/lag-types.md).

   如果后继任务具有多个前置任务，则根据前置任务的最近实际完成日期计算切换日期。 例如，如果两个前任的实际完成日期分别是2022年11月8日和2022年11月20日，则后继者的切换日期为2022年11月20日。

   >[!NOTE]
   >
   >   根据实际完成日期或前置任务计算后续任务的切换日期时，无论前置任务是否被强制执行，都是相同的。 有关强制前置任务的详细信息，请参阅 [强制前置任务](../use-prdcssrs/enforced-predecessors.md).


* **当任务没有前置任务和**:

   * **计划开始日期为过去**:切换日期与项目的计划开始日期相同。
   * **计划开始日期为将来（当前日期之后的任何日期）**:切换日期与项目的计划开始日期相同。

>[!NOTE]
>
>当任务具有跨项目前置任务时，只有在发生以下任一情况时，后继任务的切换日期才会重新计算：
>
>* 您可以手动重新计算后续项目的时间轴。 您必须拥有项目的“管理”权限，才能重新计算时间轴。
>* 后续项目的时间表将在晚上自动重新计算。
>
>有关重新计算项目时间轴的信息，请参阅 [重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **当任务对计划日期具有强制约束时**:切换日期始终与约束设置的日期相同，而不考虑任何其他条件。\
   以下是任务的强制限制：

   * 必须开始时间
   * 必须完成时间
   * 开始时间不早于
   * 开始时间不晚于
   * 固定日期

## 找到切换日期

您可以在任务报表或任务列表视图中显示任务的切换日期。\
有关构建报表的更多信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
