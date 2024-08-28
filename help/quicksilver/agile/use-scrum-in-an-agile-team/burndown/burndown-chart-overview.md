---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Agile燃尽图概述
description: 燃尽图以可视化形式呈现故事在迭代或项目中的进度。 实际燃尽率是根据迭代或项目时间线的理想燃尽率测量的。
author: Lisa
feature: Agile
exl-id: 414e3315-35ed-4aa4-a2d8-be42ec585f29
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# 敏捷燃尽图概述

燃尽图直观地显示了故事在迭代中的进度。 实际燃尽率是根据迭代时间线的理想燃尽率来测量的。

燃尽图根据选定的日期进行调整。 默认值为当天。 当选择前一天时，将重新计算燃尽图中的所有数据以及燃尽图上方[!UICONTROL 完成状态]部分中的所有值，以表示选定日期结束时的数据。 （您可以选择过去日期或当前日期；但不能选择将来的日期。）

![](assets/agile-iteration-burndown-350x88.png)

## 视觉指示器

燃尽图包含以下可视指示器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt=""> </td> 
   <td> <p>基于迭代开始时间的理想燃尽率。</p> <p>如果迭代的范围从不更改（小时或点从不添加或删除），则不显示此行。</p> <p>此线条在休息日完成工作时显示为平坦。 有关详细信息，请参阅<a title="使用敏捷燃尽图" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">休息日如何影响燃尽图</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt=""> </td> 
   <td> <p>基于当前情景或任务的理想燃尽率。</p> <p>在迭代开始后，向迭代添加小时或点或从迭代中删除点时，当前理想燃尽率（实心蓝线）不同于原始理想燃尽率（虚蓝线）。</p> <p>此线条在休息日完成工作时显示为平坦。</p> <p>有关详细信息，请参阅<a title="使用敏捷燃尽图" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">休息日如何影响燃尽图</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt=""> </td> 
   <td> <p>当燃尽率小于理想值（每天剩余的点数或小时数多于理想燃尽计算）时，实际燃尽率以红色显示。</p> <p>以下公式用于计算实际燃尽率：</p> <p>[SUM（正在进行的工作的点或小时值*完成百分比）+已完成工作的点或小时值]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt=""> </td> 
   <td> <p>当燃尽率等于或高于理想值（等于或低于理想燃尽计算的每天剩余点数）时，实际燃尽率以绿色显示。</p> <p>以下公式用于计算实际燃尽率：</p> <p>[SUM（正在进行的工作的点或小时值*完成百分比）+已完成工作的点或小时值]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>范围更改（在迭代中添加或删除小时或点）。</p> <p>范围更改始终在白天中间显示为垂直线。 此外，如果发生范围更改，则会在任何一天的中间显示一个蓝色圆点。</p> <p>燃尽图的垂直轴显示故事点或小时。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>日期范围的更改（迭代持续时间增加或减少）。</p> <p>在迭代持续时间发生更改的任何一天的中间会显示一个蓝色圆点。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>每当工作燃尽时，实际燃尽率上都会显示一个绿色或红色圆点。 （当当当天的实际燃尽率为红色时，圆点为红色；当当当天的实际燃尽率为绿色时，圆点为绿色。）</p> <p>出现以下任何情况时，工作都会被烧毁：</p> 
    <ul> 
     <li> [！UICONTROL完成百分比]在文章中会增加。<br>[！UICONTROL完成百分比]在以下情况下增加： 
      <ul> 
       <li> <p>手动更改</p> </li> 
       <li> <p>在文章中更新了点数或小时数</p> </li> 
      </ul></li>  
     <li>故事的状态已更改为[！UICONTROL结束]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 休息日对燃尽图的影响 {#how-days-off-affect-the-burndown-chart}

[!DNL Workfront]中定义的默认计划通过从燃尽中排除休息日（周末和假日）而影响燃尽图。 燃尽图使用默认时间表来定义工作日（如中所述）  [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

Agile团队可以通过定义替代计划来合并团队特定的非工作日（如文章[使用燃尽图的替代团队计划](../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md)中所述）。 然后，此备用计划会反映在分配给团队的任何迭代的燃尽图中。 替代计划仅影响燃尽图。

只有符合以下条件时，燃尽图才会反映休息日：

* 工作以前是休息日登录的。 （显示记录工作的日期。）

  在休息日登录工作时：

   * 在计算理想燃尽时，不会包括记录的任何工作，因为团队未计划进行任何工作。
   * 理想的燃尽线（实心蓝线和虚线蓝线）在燃尽图中显示为平坦，即工作完成时或查看燃尽图时（如果您在休息日查看）的任何一天。
   * 在计算其他燃尽统计数据（如估计完成情况以及每天的平均点数或小时数）时，包括记录的工作。

* 您正在休息日查看燃尽图。 （您查看的日期显示在燃尽图上。）
* 您在休息日完成迭代的总剩余工作。

  当用户休息日完成迭代的总剩余工作时，[!UICONTROL 预计完成]字段显示迭代完成的日期。

  在计划迭代时，如果您为非工作日设置迭代结束日期，并且迭代正在跟踪按时完成，则将[!UICONTROL 预计完成]日期设置为您设置的迭代结束日期之前的最后一个工作日（因为未计划在非工作日烧毁工作）。

  在计划迭代时指定迭代的结束日期，如[创建迭代](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)一文中所述。
