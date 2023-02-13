---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: 在Adobe Workfront目标中开始使用结果和活动
description: 您必须将结果、活动或目标与目标一致地添加才能激活它。 这会将目标状态从“草稿”更新为“活动”，并开始记录目标的进度。
author: Alina
feature: Workfront Goals
exl-id: 64fa0aef-cb92-465a-9b74-d863fc232fd1
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# 在Adobe Workfront目标中开始使用结果和活动

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
>  请联系您的Workfront客户经理以了解Workfront Target许可证。
>
>有关访问Workfront目标的其他信息，请参阅 [使用Workfront目标的要求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


在创建目标时，目标的状态为“草稿”。 有关创建目标的信息，请参阅 [在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md).

要开始记录目标的进度，必须将其激活。 要激活您的目标并将其状态更改为“活动”，您必须先向其添加以下内容：

* 结果
* 活动
* 项目
* 一致的目标

在至少添加其中一个项目后，您可以激活目标。 您必须更新目标的结果和活动，以指示目标的进度。


>[!IMPORTANT]
>
> 目标不能包含超过1000个活动、结果、项目或一致目标。</span>

本文概述了活动和结果。 有关协调目标的信息，请参阅 [Adobe Workfront目标中的目标协调](../../workfront-goals/goal-alignment/goal-alignment.md). 有关将项目连接到目标的信息，请参阅 [将项目添加到Adobe Workfront目标中的目标](../results-and-activities/connect-projects-to-goals-overview.md).

## 结果概述

<!--
<p> This will have additional types in the future - add another section for types?)</p>
-->

结果衡量目标的进度或目标实现的距离。 作为目标所有者，您还可以拥有结果。 您的目标结果也可能会分配给其他用户。

有关将结果添加到目标的信息，请参阅 [将结果添加到Adobe Workfront目标中的目标](../../workfront-goals/results-and-activities/add-results-to-goals.md).

您可以将结果添加到您自己的目标或目标中，这些目标属于您组织中的其他实体。

处理结果时请考虑以下事项：

* 他们回答了“我如何知道我的目标何时完成？”
* 它们是量度指标。 您可以从以下选项中进行选择，以指示结果的进度：

   <!--
  this might change (jira, Salesforce, etc))
  -->

   * 货币
   * 数字
   * 百分比

有关结果的更多信息，请参阅部分中结果和活动之间的相似性列表 [结果、活动和项目之间的相似性](#similarities-between-results-activities-and-projects) 在本文中。

## 活动概述

<!--
This will have additional types in the future - add another section for types?
-->

活动（如成果）是具体和可衡量的，通常包括完整百分比指标。 作为目标所有者，您还可以拥有与目标关联的活动。 此外，还可以将您目标上的活动分配给其他用户。

有关将活动添加到目标的信息，请参阅 [将活动添加到Adobe Workfront目标中的目标](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

将活动与目标关联时，请考虑以下事项：

* 他们回答了“当目标完成时，我将实现什么？”
* 活动是自定义条目，在完整或不完整方面可以认为是更多内容。 必须手动更新它们，以指示迄今为止已完成的活动百分比。

<!--
* You can associate the following activities with goals:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Manual progress bar </td> 
     <td> <p>Custom entries that can be thought of more in terms of complete or incomplete. They must be manually updated.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><p>Project</p></td> 
     <td> <p>Existing projects that you have at least permissions to View and are not in a status of Dead. They are updated automatically, based on the progress of their work items. </p> <p>The projects must exist before associating them with the goal. You can associate a project with multiple goals. For information about adding projects to goals, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</p>
     <p><span class="preview">In the Preview environment, projects are separate progress indicators, independent from activities. Adding projects to a goal in the Preview environment is different from adding activities. For more information, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</span></p>
      </td> 
    </tr> 
   </tbody> 
  </table>
-->
<!--drafted for goal redesign: For THE PRODUCTION RELEASE: remove the projects in this article altogether.-->

有关结果和活动的更多信息，请参阅部分中结果和活动之间的相似性列表 [结果、活动和项目之间的相似性](#similarities-between-results-activities-and-projects) 在本文中。

## 结果、活动和项目之间的相似性 {#similarities-between-results-activities-and-projects}

成果、活动和项目是目标进度指标。

与管理结果和活动的方式相比，您管理项目的方式存在一些差异。 有关将项目添加到目标的信息，请参阅 [将活动添加到Adobe Workfront目标中的目标](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 有关与目标关联的项目的信息，请参阅 [将项目添加到Adobe Workfront目标中的目标](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

除了结果、活动和项目之外，您还可以将子目标与目标相关联。 儿童目标也是目标的一种进度指标。 有关信息，请参阅 [在Adobe Workfront目标中通过将目标连接起来来调整目标](../goal-alignment/align-goals-by-connecting-them.md). 儿童目标的进度指标的进展也推动了父目标的进展。

下表显示了结果、活动和项目之间的相似之处和差异，作为目标指标：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b><p>功能</p></b></td> 
   <td><b><p>结果</p></b></td> 
   <td><b><p>活动</p></b></td> 
   <td> <p><strong>项目</strong> </p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td><span style="font-weight: normal;">您可以在Workfront界面中自定义对象名称</span> </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>您可以将它们添加到过去的目标中。</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>您可以将多个结果、活动或项目与同一目标相关联。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>您可以将其中一个目标与多个目标相关联。</td> 
   <td> </td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>在计算目标进度时，会考虑其进度。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>必须在Workfront Target中手动更新它们</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>它们将在目标的结束日期完成</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>它们只能分配给用户，而不能分配给团队、组或公司。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>这些量度是具体的、可衡量的，并且通常包括用于指示其进展的设定数字。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>它们提供开始值和结束值之间的一系列值，以说明您接近于实现这些值。 与结束值的接近度计算目标的进度值。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
 </tbody> 
</table>
