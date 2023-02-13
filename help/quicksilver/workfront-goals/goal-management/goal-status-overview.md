---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront目标中的目标状态概述
description: 目标状态指示目标是处于活动状态且当前记录进度，还是处于不活动状态、草拟目标还是已实现目标。
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 4%

---

# Adobe Workfront目标中的目标状态概述

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

>[!NOTE]
>
>贵组织必须具备以下条件才能使用本文中描述的功能：
>
>* 专业或更高级 [Adobe Workfront计划](https://www.workfront.com/plans).
>* 除了Adobe Workfront许可证之外，还具有Workfront许可证。
>
>请联系您的Workfront客户经理以了解Workfront Target许可证。

有关访问Workfront目标的其他信息，请参阅 [使用Workfront目标的要求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


目标状态指示目标是处于活动状态且当前记录进度，还是处于不活动状态、草拟目标还是已实现目标。

## 更新Workfront目标中的目标状态时的注意事项

* 您无法手动更新您创建或与您共享的目标的状态。 根据您对目标执行的操作，目标的状态会发生更新。 例如，激活目标会将“草稿”状态更改为“活动”。
* 存在一些限制，有时您无法根据以下规则将目标状态更改为其他状态：

   | 从/到 | 草稿 | 活动 | 非活动 | 已关闭 |
   |---|---|---|---|---|
   | 草稿 | - | 是 | 否 | 否 |
   | 活动 | 否 | - | 是 | 是 |
   | 非活动 | 否 | 是 | - | 否 |
   | 已关闭 | 否 | 是 | 否 | - |

* 打开已结束的目标也会更新目标的进度。
* 您对目标执行的某些操作也会更新其状态。 有关如何更新目标状态的信息，请参阅以下文章：

   * [在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md)
   * [在Adobe Workfront目标中激活目标](../../workfront-goals/goal-management/activate-goals.md)
   * [删除和停用Adobe Workfront目标中的目标](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [在Adobe Workfront目标中关闭并重新打开目标](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Workfront目标中的目标状态概述

有关创建Workfront目标的信息，请参阅 [在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md).

有关激活目标的信息，请参阅 [在Adobe Workfront目标中激活目标](../../workfront-goals/goal-management/activate-goals.md).

目标在Workfront目标中可以具有以下状态之一：

* [草稿](#draft)
* [活动](#active)
* [非活动](#inactive)
* [已关闭](#closed)

### 草稿 {#draft}

* 这是新创建目标的默认状态。 有关创建目标的信息，请参阅 [在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md).
* Workfront目标没有记录起草目标方面的进展。
* 不能更新拟定目标的进度。
* 您无法关闭或停用已起草的目标，因为它们缺少进度信息。
* 起草的目标无助于其他目标的进度计算，图表中也未考虑这些目标。
* 起草的目标在Workfront目标的以下方面显示：

   * 目标列表
   * “目标对齐”部分（仅作为对齐的目标）


>[!IMPORTANT]
>
>将目标状态更改为任何其他状态后，再也不能将目标置于“草稿”状态。

### 活动 {#active}

* 仅当您将起草的目标与结果、活动或其他目标相关联时，才能激活该目标。 激活目标会将其状态更改为“活动”。 有关激活目标的信息，请参阅 [在Adobe Workfront目标中激活目标](../../workfront-goals/goal-management/activate-goals.md).
* Workfront目标记录了活动目标方面的进展。
* 积极目标有助于对其他目标的进度计算，图表中也考虑了这些目标。
* “Workfront目标”的以下区域显示了活动目标：

   * 目标列表
   * “目标对齐”部分
   * 活动目标的进度显示在图表中

* 您可以重新激活已关闭或不活动的目标。

### 非活动 {#inactive}

* 当所有者暂时或永久停止对活动目标工作时，您可以停用该目标。 您可以保留它以获取历史信息。 这会将目标的状态更新为“不活动”。

   有关取消激活目标的信息，请参阅文章中的“取消激活目标”部分 [删除和停用Adobe Workfront目标中的目标](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* 不能停用已起草或已关闭的目标。
* 您可以重新激活不活动的目标并继续处理该目标。
* Workfront目标不计算不活动目标的进度。
* 您无法更新不活动目标的进度。
* 不活跃的目标无助于其他目标的进度计算，图表中也未考虑这些目标。
* 不活动目标具有进展历史，因为它们曾经是活跃的，与起草的目标不同。
* 不活动的目标显示在Workfront目标的以下区域：

   * 目标列表
   * “目标对齐”部分（仅作为对齐的目标）

### 已关闭 {#closed}

* 当您想要表明您已实现目标，或者您不再致力于此目标时，您可以结束目标，以后也不会这样做。 有关结束目标的信息，请参阅 [在Adobe Workfront目标中关闭并重新打开目标](../../workfront-goals/goal-management/close-and-reopen-goals.md).

   >[!TIP]
   >
   >如果您计划在以后实现一个尚未实现的目标，我们建议您将状态更改为“不活动”，而不是“已关闭”。

* 不能像起草的目标那样关闭从未激活的目标。
* 您可以重新打开已关闭的目标并继续处理该目标。
* Workfront目标停止记录已关闭目标的进度。
* 无法更新已结束目标的进度。
* 已关闭的目标显示在Workfront目标的以下区域：

   * 目标列表
   * “目标对齐”部分（仅作为对齐的目标）
   * 图形部分还考虑来自已结束目标的信息。
