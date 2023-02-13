---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任务进度状态概述
description: Adobe Workfront通过查看任务在其时间线中的进度来确定任务的“进度状态”。 您可以配置Workfront，以根据任务的进度状态值确定项目的条件。 有关配置项目条件的更多信息，请参阅项目条件和条件类型概述一文。
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 65f25a3b1198f491f7357efef11e2ae075e9721a
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 1%

---

# 任务进度状态概述

Adobe Workfront通过查看任务在其时间线中的进度来确定任务的“进度状态”。 您可以配置Workfront，以根据任务的进度状态值确定项目的条件。 有关配置项目条件的详细信息，请参阅文章 [项目条件和条件类型概述](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## 确定任务进度状态的标准

有关项目进度状态的信息，请参阅 [项目进度状态概述](../../../manage-work/projects/planning-a-project/project-progress-status.md).

有关跟踪任务进度的信息，请参阅 [任务跟踪模式概述](../../../manage-work/tasks/task-information/task-tracking-mode.md).

以下标准确定任务的进度状态：

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>进度状态</strong> </p> </th> 
   <th> <p><strong>确定标准</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>准时</strong> </p> </td> 
   <td scope="col"> <p>考虑任务 <strong>开始时间</strong> 当所有计划日期与预计日期匹配时。 此进度状态还可能意味着项目提前，并且预计日期可能早于计划日期。</p> <p>有关预计日期的详细信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">项目、任务和问题的预计完成日期概览</a>.</p> <p>有关任务计划完成日期的详细信息，请参阅以下文章：</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">任务计划起始日期概览</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任务计划完成日期概览</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>处于风险中</strong> </p> </td> 
   <td><p>考虑任务 <strong>面临风险</strong> 当预计完成日期迟于计划完成日期且迟于预计完成日期时。 当任务的约束为 <strong>必须完成</strong> 或 <strong>必须开始</strong> 但是，任务的完成百分比或前置关系表明它不能在指定日期完成或开始。 </p><p> 将任务约束设置为 <strong>必须完成</strong> 手动将计划完成日期设置为特定日期。 在这种情况下，预计完成日期与计划完成日期匹配。 对于此约束，Workfront会分析任务以根据完成百分比计算任务何时完成。 此计算将存储为预计到期日期。 如果预计到期日在预计完成日期之后，则任务将被视为有延迟的风险。 </p> <p> 将任务约束设置为 <strong>必须开始</strong> 手动将计划开始日期设置为特定日期。 在这种情况下，预计起始日期与计划起始日期匹配。 对于此约束，Workfront会分析任务，以根据其前身关系计算何时开始。 此计算将存储为估计开始日期。 如果有强制的前置任务不允许任务在指定的起始日期开始，则预计起始日期可以在预计完成日期之后。 这项任务被认为有迟到的危险。 </p> <p>注意：通常，预计日期与预计日期匹配，但 <strong>必须开始</strong> 或 <strong>必须完成</strong> 中，将使用。 在这些情况下，预计日期会继续根据完成百分比和其他因素（前置关系）进行计算，而预计日期将被强制与人工设置的计划日期匹配。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>滞后</strong> </p> </td> 
   <td> <p>任务被视为 <strong>后面</strong> 当预计完成日期迟于或等于计划完成日期且早于预计完成日期时。</p> <p>预计完成日期是根据先前进度实时查看任务完成时间。 虽然任务启动时间较晚，但它尚未被视为延迟，因为计划完成日期和预计完成日期仍在将来，并且任务可能仍可按时完成。</p> <p>注意：的 <strong>后面</strong> 和 <strong>面临风险</strong> 进度状态几乎相同。 但是， <strong>面临风险</strong> 指示在其中一个或两个计划日期上存在一些强制任务限制（必须完成、必须开始、固定日期）。 如果任务没有强制约束，则预计日期与预计日期相同，并反映系统根据任务当前进度计算完成日期。 任务尚未被视为延迟，因为计划完成日期和预计完成日期仍在将来，并且任务可能仍可按时完成。<br>有关预计日期和预计日期的详细信息，请参阅 <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">预计日期和预计日期之间的差异 </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>延迟</strong> </p> </td> 
   <td> <p>任务是 <strong>延迟</strong> 计划完成日期早于今天日期时。<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## 任务进度状态随时间的变化如何更新

我们项目中的不同日期类型告诉我们任务在一段时间内的进展情况：

* 准时

   ![](assets/on-time-progress-status-350x233.png)

* 处于风险中

   ![](assets/at-risk-progress-status-350x233.png)

* 滞后

   ![](assets/behind-progress-status-350x233.png)

* 延迟

   ![](assets/late-progress-status-350x233.png)
