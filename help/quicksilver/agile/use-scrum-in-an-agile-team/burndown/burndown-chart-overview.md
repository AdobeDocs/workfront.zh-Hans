---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: 敏捷燃耗图概述
description: 燃耗图直观地显示了故事在迭代或项目中的进展情况。 实际燃耗率是根据迭代或项目时间表的理想燃耗率测量的。
author: Lisa
feature: Agile
exl-id: 414e3315-35ed-4aa4-a2d8-be42ec585f29
source-git-commit: 373f2522b85196d6395f189ae6cfe03449cac61a
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# 敏捷燃耗图概述

燃耗图直观地显示了故事在迭代过程中的进展情况。 实际燃耗率是根据迭代时间线的理想燃耗率测量的。

燃耗图根据选定的日期进行调整。 当天是默认日期。 选择前一天时，燃耗图中的所有数据以及 [!UICONTROL 完成状态] 将重新计算燃耗图上方的部分，以表示在选定日期结束时的数据。 (您可以选择过去的日期或当天；您不能选择将来的日子。)

![](assets/agile-iteration-burndown-350x88.png)

## 可视指标

燃耗图包含以下可视指示器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt=""> </td> 
   <td> <p>基于迭代开始时的理想燃耗率。</p> <p>如果小版本的范围从未更改（从未添加或删除小时或点），则不会显示此行。</p> <p>当一天下班后工作完成时，此行将显示为平整。 有关更多信息，请参阅 <a title="使用敏捷燃耗图" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">休息天数如何影响燃耗图</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt=""> </td> 
   <td> <p>理想的燃耗率基于当前的故事或任务。</p> <p>当小时或点在迭代开始后被添加到迭代或从迭代中移除时，当前理想燃耗率（实蓝线）与原始理想燃耗率（虚蓝线）不同。</p> <p>当一天下班后工作完成时，此行将显示为平整。</p> <p>有关更多信息，请参阅 <a title="使用敏捷燃耗图" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">休息天数如何影响燃耗图</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt=""> </td> 
   <td> <p>当燃耗率小于理想值时，实际燃耗率以红色显示（比理想燃耗计算多点或多小时）。</p> <p>下列公式用于计算实际燃耗率：</p> <p>[SUM（正在进行的工作的点值或小时值*完成百分比）+已完成工作的点值或小时值]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt=""> </td> 
   <td> <p>当燃耗率等于或优于理想值时，实际燃耗率以绿色显示（等于或小于理想燃耗计算的每日剩余点）。</p> <p>下列公式用于计算实际燃耗率：</p> <p>[SUM（正在进行的工作的点值或小时值*完成百分比）+已完成工作的点值或小时值]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>范围更改（在小时或小时点中添加或删除小时或点）。</p> <p>范围更改始终在一天中间显示为一条垂直线。 此外，在发生范围更改的任何一天的中间，都会显示一个蓝色圆点。</p> <p>燃耗图的垂直轴显示故事点或小时。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>日期范围的更改（迭代持续时间会增加或减少）。</p> <p>更改迭代持续时间的任何一天的中间都会显示一个蓝色圆点。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>每当工作被烧毁时，实际燃尽率上都会显示一个绿色或红色圆点。 (当日实际燃耗率为红色时，圆点为红色；当当天的实际燃耗率为绿色时，圆点为绿色。)</p> <p>当发生以下任何情况时，工作会被烧毁：</p> 
    <ul> 
     <li> 文章中增加了[!UICONTROL Percent Complete]。<br>[!UICONTROL完成百分比]会在以下情况下增加： 
      <ul> 
       <li> <p>手动更改</p> </li> 
       <li> <p>文章中更新的点数或小时数</p> </li> 
      </ul></li>  
     <li>文章的状态将更改为[!UICONTROL Complete]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 休息天数如何影响燃耗图 {#how-days-off-affect-the-burndown-chart}

在中定义的默认计划 [!DNL Workfront] 从燃耗中排除休息天数（周末和节假日）会影响燃耗图。 燃耗图使用默认计划来定义工作日(如  [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md))。

敏捷团队可通过定义备用计划（如文章中所述）来整合特定于团队的非工作日 [为燃耗图使用备用团队计划](../../../agile/use-scrum-in-an-agile-team/burndown/use-alt--team-schedule-burndown-charts.md))。 然后，此备用计划将反映在分配给团队的任何小版本的燃尽图中。 备用计划仅影响燃耗图。

仅当满足以下条件时，燃尽图中才会反映休息天数：

* 工作以前在休息日记录。 （显示记录工作的日期。）

   休息日登录工作时：

   * 在计算理想燃耗时记录的任何工作都不包括在内，因为团队没有安排进行任何工作。
   * 理想的燃耗线（实蓝线和虚蓝线）在完成工作的任何一天或查看燃耗图的当天（如果您在休息日查看），燃耗图中都显示为平面。
   * 在计算其他燃耗统计时（如估计完成和每天的平均点数或小时数）时，将包括已记录的工作。

* 你在休息一天看燃耗图。 （您正在查看的日期显示在燃耗图表上。）
* 在休息日完成小版本的剩余工作总数。

   当用户在休息日完成小版本的剩余工作总数时， [!UICONTROL 估计完成] 字段会显示小版本的完成日期。

   在计划小版本时，如果为非工作日设置小版本结束日期，并且小版本正在跟踪以按时完成，则 [!UICONTROL 估计完成] 日期是在您设置的迭代结束日期之前的最后一个工作日设置的（因为工作未计划在非工作日被刻录）。

   在计划迭代时指定迭代的结束日期，如文章中所述 [创建迭代](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
