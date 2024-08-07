---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 预计日期和预计日期概览
description: 有多种类型的日期显示了任务从何时可以开始到何时可以完成之间的时间线。
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# 预计日期和预计日期概览

<!--Audited: 07/2024-->

有多种类型的日期显示了任务从何时可以开始到何时可以完成之间的时间线。 以下是显示任务时间线的一些日期：

* 计划开始日期和计划完成日期
* 预计起始日期和预计完成日期
* 估计开始日期和估计到期日期
* 实际开始日期和实际完成日期

本文介绍了项目的预计日期和预计日期之间的差异。

首次创建任务时，计划、预计和预计日期通常应该匹配。 存在一些例外。

有关Adobe Workfront中项目、任务和问题日期的详细信息，请参阅[Workfront中的项目、任务和问题日期概述](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md)。

## 计划日期概览

计划日期是项目所有者定义为任务的开始和结束日期的日期。 您或项目所有者可以手动修改任务的计划日期。

## 实际日期概览

首次创建任务时，该任务没有实际日期，因为任务尚未开始或完成。

## 预计日期和预计日期概览

在项目存留期内，“预计日期”和“预计日期”更加符合项目的实际情况，因为它们考虑到了哪些因素可能会影响任务的实际开始和结束。 这会导致他们从计划日期更改。

处理任务的预计日期和估计日期时，请考虑以下事项：

* 您不能手动修改任务的预计日期和预计日期。 两者均由Adobe Workfront计算。
* 在创建任务时，预计日期和预计日期应该相同，并且它们应该说明任务可以开始或结束的实际时间。\
  您对任务进行的某些更新会直接影响“预计日期”和“预计日期”的值。

  例如，如果用户开始或完成任务，则任务将显示影响任务预计日期和预计日期的实际开始日期和完成日期。 此外，如果任务的被分配人修改了提交日期，则此日期会影响任务的预计日期。

## 预计日期和估计日期之间的差异

预计日期和预计日期之间的差异为：

* 如果用户在任务中进行以下更新，则会影响预计日期：

   * 通过添加固定任务限制来添加限制日期
   * 添加提交日期

* 预计日期只考虑给定时间点内任务的实际进度。

**示例：**&#x200B;如果我们有一个任务的计划开始日期为9月20日，计划完成日期为9月24日，并且任务必须在限制时完成，即计划完成日期为9月24日。 此任务的工期为4天。

预计完成日期是根据任务工作的当前进度计算的。 因此，如果今天是9月23日，而任务尚未开始，则预计完成日期为9月27日（假设工作已在今天开始，则应在4天后完成）。

如果任务今天已完成50%，则预计完成日期为9月25日（应在2天后完成，即任务持续时间的一半）。


### 了解任务的预计日期何时更新 {#understand-when-projected-dates-update-on-tasks}

预计日期可以与其他任务日期匹配，也可以是Workfront根据任务的实际进度计算而得。

当任务的预计日期在项目生命周期内根据任务的实际发生情况发生更改时，以下列表显示了几种方案：

* 将任务标记为“完成”时：

  `Projected Dates = Estimated Dates = Actual Dates`

* 当任务具有实际开始日期时：

  `Projected Start Date = Estimated Start Date = Actual Start Date`

* 当任务没有实际开始日期，但计划开始日期（必须开始于）具有未来强制限制时：

  `Projected Start Date = Constraint Date`

  有关限制日期的信息，请参阅[Adobe Workfront术语词汇表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

* 当任务没有实际开始日期并且任务没有强制限制日期时：

  `Projected Start Date = the next available date in the future that falls within working schedule`

* 当被分派人更新提交日期时：

  `Projected Completion Date = Commit Date`

  有关提交日期的信息，请参阅[提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)。

* 当任务没有更新的提交日期，并且任务的计划完成日期为未来的强制约束（必须完成日期）时：

  `Projected Completion Date = Constraint Date`

* 当任务没有更新的提交日期、强制限制日期在将来或限制日期在过去时：

  `Projected Completion Date = system calculation for the Completion Date based on the current progress and the work left to be done`

### 了解任务的预计日期何时更新 {#understand-when-the-estimated-dates-update-on-tasks}

与上面所述的预计日期方案相比，预计日期始终反映Workfront对任务何时开始或完成的真实分析，而不管约束日期或提交日期如何。

## 影响任务时间线的因素

以下是一些可能影响任务真实时间线的示例：

* 与计划日期和当天相关的任务进度
* 迄今为止任务的完成百分比
* 前置任务关系
* 前置任务进度
* 用户分配

  >[!NOTE]
  >
  >如果用户分配影响任务的完成速度，则可能会影响任务的预计完成日期。 例如，如果任务持续时间类型为投入比导向，您可以通过添加被分配人来加快任务完成速度。 因此，预计完成日期会发生变化。
