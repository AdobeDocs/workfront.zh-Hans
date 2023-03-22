---
title: 项目限制概述
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront对与项目关联的对象数量存在限制。 已设置项目限制，以提高产品性能并增强您的Workfront体验。
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 809f1c3629c343a55305c0c617f4974dc05439bf
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# 项目限制概述

Adobe Workfront对与项目关联的对象数量存在限制。 已设置项目限制，以提高产品性能并增强您的Workfront体验。

与项目关联的以下对象具有以下限制：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>任务</p></td> 
   <td>  <p>每个项目的最大任务数为5,000。 当任务数接近此最大值时，将显示一条警告消息。 达到最大值时，将显示一条错误消息，无法将其他任务添加到项目中。</p> <p>为避免达到此最大限度，请将已关闭的任务移动到为已结束任务指定的其他项目。 可能需要调整这些项目的报告。</p>

<b>重要信息</b>

对于任务具有大量依赖关系的项目，我们建议项目中的任务数应远远低于允许的最大5,000个任务数。

可能会影响或阻止重新计算项目时间轴的任务依赖关系的一些示例包括：

<ul><li>子项数量</li>
   <li>多级别任务缩进</li>
   <li>前置任务数</li>
   <li>多个分配</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>问题</p></td> 
   <td>  <p>每个项目的最大问题数为10,000。 当问题数量接近此最大值时，将显示一条警告消息。 达到最大值时，将显示一条错误消息，无法将其他问题添加到项目中。</p> <p>为避免达到此最大限度，请将已关闭的问题移动到指定用于已结束问题的其他项目。 可能需要调整这些项目的报告。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>持续时间</p></td> 
   <td> <p>项目的最长持续时间必须为15年，Workfront才能自动计算其时间轴。 当项目持续时间接近最大时，会显示一条警告消息。 达到最大值时，将显示一条警告消息，并且不再进行自动时间轴计算。</p> <p>通过调整项目中任务的日期，一旦项目的持续时间缩短到15年以下，将自动时间轴计算将立即恢复。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>时间轴计算</p></td> 
   <td>Workfront不会为6个月内未更新的项目执行自动时间轴计算，并且在进行更新之前不会恢复。<p>对于3个月内未更新的项目，Workfront每周（而不是夜间）执行时间轴计算。</p><p>有关计算项目时间轴的信息，请参阅 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">重新计算项目时间表</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->