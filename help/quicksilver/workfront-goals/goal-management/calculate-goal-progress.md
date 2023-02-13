---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront目标中的目标进度和条件概述
description: 目标进展由活动、结果或儿童目标等进展指标驱动。 目标条件由目标在当前时刻的进度决定。
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# Adobe Workfront目标中的目标进度和条件概述

<!--drafted for P&P release: the note at the top will need to be replaced with this:

Your organization must have the following to use the functionality described in this article:

* For the legacy plan and license structure: 

  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans). 
  * An Adobe Workfront Goals license in addition to a Workfront license.

* For the current plan and license structure:

  * An Ultimate plan 
    
    Or
    
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>

Contact your Workfront account manager to learn about a Workfront Goals license.

For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

>[!NOTE]
>
>贵组织必须具备以下条件才能使用本文中描述的功能：
>
>* 专业或更高级 [Adobe Workfront计划](https://www.workfront.com/plans).
>* 除了Adobe Workfront许可证之外，还具有Workfront许可证。
>
>请联系您的Workfront客户经理以了解Workfront Target许可证。
>有关访问Workfront目标的其他信息，请参阅 [使用Workfront目标的要求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

Adobe Workfront根据其进度指标的进度自动计算目标进度。

## 先决条件

在开始之前，您必须具备以下条件：

* 包含主菜单中“目标”区域的布局模板。

## 目标进度和阈值概述

在您激活目标后，Workfront目标会开始计算其进度和条件，并在您将鼠标悬停在进度字段上时显示以下指标：

| 指标 | 指标描述 |
|---|---|
| 实际完成百分比 | 到目前为止，已经完成了多少目标。 Workfront目标通过平均与目标关联的所有进度指标的完成百分比来计算此值。 |
| 预期完成百分比 | 目标到目前为止应该完成多少，以便目标能够按时完成。 Workfront Goals通过查看目标的持续时间和当前时间来计算此值。 如果要按时完成，则目标应当在当前时间显示此值。 |
| 进度 | 一个标签，用于指示目标是按时完成，还是目标有风险或无法完成。 |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [实际完成百分比](#actual-percent-complete)
* [预期完成百分比](#expected-percent-complete)
* [进度和条件](#progress)

### 实际完成百分比 {#actual-percent-complete}

Workfront目标可根据目标进度指标的完成百分比平均值自动计算目标的实际完成百分比。

以下项目被视为目标的进度指标：

* 结果

   有关将结果添加到目标的信息，请参阅 [将结果添加到Adobe Workfront目标中的目标](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* 活动

   有关将活动（包括项目）添加到目标的信息，请参阅 [将活动添加到Adobe Workfront目标中的目标](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* 协调儿童目标

   有关父项和子项目标的信息，请参阅 [在Adobe Workfront目标中通过将目标连接起来来调整目标](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

   Workfront Target使用以下公式计算实际完成百分比：

   ```
   Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
   ```

   例如，如果目标的结果为完成20%，手动进度条为完成30%，项目完成10%，子项目标为完成40%，则目标完成百分比为25%。

### 预期完成百分比 {#expected-percent-complete}

Workfront目标会根据目标持续期间的总天数以及自目标开始日期以来经过的天数，自动计算目标的预期完成百分比。

Workfront Target使用以下公式计算预期完成百分比：

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

例如，如果目标将在90天内完成，而今天是该持续时间的第45天，则预期完成百分比为50%。

### 进度和条件 {#progress}

Workfront Goals会根据当前时间已达到预期完成百分比的百分比，计算进度百分比并为目标分配进度标签。 目标完成百分比栏的颜色会发生更改以指示目标的进度。

此外，还会相应地更新目标的条件，以指示目标是按时完成，还是滞后。

Workfront目标使用以下公式计算目标的进度百分比：

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

例如，如果当前时间的预期完成百分比为53%，而实际完成百分比为30%，则目标进度完成百分比为56%。 Workfront目标将此目标标记为“遇到问题”条件。

下图说明了条件标签与进度百分比之间的关系：

![](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

下表列出了目标条件标签以及与每个标签关联的目标进度百分比。

>[!TIP]
>
>目标条件标签与Workfront项目条件名称和颜色匹配。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>目标进度名称</b></td> 
   <td><b>目标进度定义</b></td> 
   <td><b>目标进度百分比</b></td> 
   <td><b>百分比完整条的颜色</b></td> 
   <td><b>条件指示器图标</b></td> 
  </tr> 
  <tr> 
   <td>新</td> 
   <td> <p>目标是新创建的，尚未记录进度。 目标进度显示为“新”，直到有人首次更新其进度。 </p> <p>有关更新目标进度的信息，请参阅 <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">更新Adobe Workfront目标中的目标进度</a>.</p> </td> 
   <td>无百分比</td> 
   <td>无栏</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_goal_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>准时</span> </p> </td> 
   <td>目标按预期执行，很有可能会按时完成。 </td> 
   <td>90-100%</td> 
   <td>绿色</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>处于风险中</span> </p> </td> 
   <td>目标滞后，但仍有可能按时完成。 </td> 
   <td>70-89.99%</td> 
   <td>黄色</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>存在问题</span> </p> </td> 
   <td> <p>目标很可能无法按时完成。 </p> </td> 
   <td>0-69.99%</td> 
   <td>红色</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_trouble_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>