---
title: 项目限制概述
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront对可与项目关联的对象数进行了限制。 设定项目限制以提高产品性能并增强您对Workfront的使用体验。
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 8be7534dfc0a1227bd2274ad093a88ae19b4691d
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# 项目限制概述

Adobe Workfront对可与项目关联的对象数进行了限制。 设定项目限制以提高产品性能并增强您对Workfront的使用体验。

以下与项目关联的对象具有以下限制：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>任务</p></td> 
   <td>  <p>每个项目的最大任务数为5,000。 当任务数接近此最大值时，会显示警告消息。 当达到最大时，会显示一条错误消息，并且无法将其他任务添加到项目中。</p> <p>要避免达到此最大值，请将已关闭的任务移动到为已关闭任务指定的其他项目。 这些项目报告可能需要进行调整。</p>

<b>重要</b>

对于任务具有大量依赖关系的项目，在计算时间表或在项目中工作时，性能可能会降低。

因此，我们建议具有复杂依赖关系的项目中的任务数量应远远低于允许的最大数量5,000个任务。

一些可能会影响或阻止重新计算项目时间线的任务依赖项示例包括：

<ul><li>子项数量</li>
   <li>多级任务缩进</li>
   <li>前置任务数量</li>
   <li>多个分配</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>问题</p></td> 
   <td>  <p>每个项目的最大问题数为10,000。 当问题数接近此最大值时，会显示警告消息。 当达到最大时，会显示一条错误消息，并且无法将其他问题添加到项目中。</p> <p>要避免达到此最大值，请将已关闭的问题移动到为已关闭问题指定的另一个项目。 这些项目报告可能需要进行调整。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>持续时间</p></td> 
   <td> <p>项目的最长持续时间必须为15年，Workfront才能自动计算其时间线。 当项目持续时间接近最大值时，会显示警告消息。 当达到最大值时，会显示警告消息，并且不再进行自动时间线计算。</p> <p>一旦通过调整项目中任务的日期将项目的持续时间缩短到15年以下，将自动恢复时间表计算。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>时间线计算</p></td> 
   <td>Workfront不会为6个月内未更新的项目执行自动时间表计算，并且在进行更新之前不会恢复。<p>对于在3个月内未更新的项目，Workfront会每周执行时间线计算，而不是每晚执行。</p><p>有关计算项目时间线的信息，请参阅 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">重新计算项目时间表</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->