---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront目标中的目标状态概述
description: 目标状态指示目标是否处于活动状态且当前正在记录进度，或者目标是否处于非活动状态、已起草或已实现。
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 4%

---

# Adobe Workfront目标中的目标状态概述

<!--Audited: 4/2025-->

>[!IMPORTANT]
>
>您的组织必须具备以下条件才能使用本文中所述的功能：
>
>* 对于新计划和许可证结构：
>
>   * Ultimate Workfront计划
>    
>* 对于当前计划和许可证结构：
>
>   * Pro或更高版本Workfront计划
>   * 除了Adobe Workfront许可证之外，还提供了Workfront目标许可证。
>
>请联系您的Workfront客户经理，了解有关Workfront Goals许可证的信息。
> 
>有关访问Workfront目标的更多信息，请参阅[使用Workfront目标的要求](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md)。

## 在Workfront目标中更新目标状态时的注意事项

* 您无法手动更新已创建或与您共享的目标状态。 目标的状态会根据您对目标执行的操作而更新。 例如，激活目标会将草稿状态更改为活动。
* 根据以下规则，存在某些限制，有时无法将目标的状态更改为其他状态：

  | 从/到 | 草稿 | 活动 | 非活动 | 已关闭 |
  |---|---|---|---|---|
  | 草稿 | - | 是 | 否 | 否 |
  | 活动 | 否 | - | 是 | 是 |
  | 非活动 | 否 | 是 | - | 否 |
  | 已关闭 | 否 | 是 | 否 | - |

* 打开已关闭的目标也会更新目标的进度。
* 您对目标执行的某些操作也会更新其状态。 有关如何更新目标状态的信息，请参阅以下文章：

   * [在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md)
   * [在Adobe Workfront目标中激活目标](../../workfront-goals/goal-management/activate-goals.md)
   * [删除和停用Adobe Workfront目标中的目标](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [在Adobe Workfront目标中关闭和重新打开目标](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Workfront目标中的目标状态概述

有关创建Workfront目标的信息，请参阅[在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md)。

有关激活目标的信息，请参阅[在Adobe Workfront目标中激活目标](../../workfront-goals/goal-management/activate-goals.md)。

在Workfront目标中，目标可以具有以下状态之一：

* [草稿](#draft)
* [活动](#active)
* [不活动](#inactive)
* [已关闭](#closed)

### 草稿 {#draft}

* 这是新创建目标的默认状态。 有关创建目标的信息，请参阅[在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md)。
* Workfront目标不记录起草目标的进度。
* 您无法更新起草目标的进度。
* 您不能关闭或停用草稿目标，因为它们缺少进度信息。
* 起草的目标不会有助于其他目标的进度计算，图表也不会考虑这些目标。
* 起草的目标显示在Workfront目标的以下领域：

   * 目标列表
   * 目标对齐部分（仅作为对齐的目标）


>[!IMPORTANT]
>
>将目标的状态更改为任何其他状态后，该目标再也不能置于草稿状态。

### 活动 {#active}

* 仅当将草稿目标与结果、活动相关联或将其他目标与其对齐时，才能激活草稿目标。 激活目标会将其状态更改为活动。 有关激活目标的信息，请参阅[在Adobe Workfront目标中激活目标](../../workfront-goals/goal-management/activate-goals.md)。
* Workfront目标记录活动目标的进度。
* 活动目标有助于其他目标的进度计算，并且会在图形中考虑这些目标。
* 活动目标显示在Workfront目标的以下区域中：

   * 目标列表
   * “目标对齐方式”部分
   * 活动目标的进度以图形显示

* 您可以重新激活“已关闭”或“不活动”目标。

### 非活动 {#inactive}

* 当所有者临时或永久停止处理某个活动目标时，您可以停用该活动目标。 您可以保存它以获取历史信息。 这会将目标的状态更新为非活动。

  有关停用目标的信息，请参阅文章[在Adobe Workfront目标中删除和停用目标](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)中的“停用目标”部分。

* 您不能停用草稿或已关闭的目标。
* 您可以重新激活不活动的目标并继续处理该目标。
* Workfront目标不会计算不活动目标的进度。
* 您无法更新非活动目标的进度。
* 非活动目标不会有助于其他目标的进度计算，并且图表不会考虑这些目标。
* 非活动目标具有进度历史，因为它们曾经是活动目标，不同于草拟的目标。
* 非活动目标显示在Workfront目标的以下区域中：

   * 目标列表
   * 目标对齐部分（仅作为对齐的目标）

### 已关闭 {#closed}

* 如果您希望表明已实现某个目标，或者您不再致力于该目标，而且将来也不会致力于该目标，则可以关闭该目标。 有关关闭目标的信息，请参阅[在Adobe Workfront目标中关闭和重新打开目标](../../workfront-goals/goal-management/close-and-reopen-goals.md)。

  >[!TIP]
  >
  >如果您计划稍后处理尚未实现的目标，我们建议您将状态更改为“非活动”而不是“已关闭”。

* 您无法关闭从未激活的目标，例如草稿目标。
* 您可以重新打开已关闭的目标并继续处理它。
* Workfront目标停止记录已关闭目标的进度。
* 您无法更新已关闭目标的进度。
* 已关闭的目标显示在Workfront目标的以下区域：

   * 目标列表
   * 目标对齐部分（仅作为对齐的目标）
   * 来自已关闭目标的信息也会在图形部分中考虑。
