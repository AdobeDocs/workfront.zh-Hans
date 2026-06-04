---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 项目进度状态概述
description: Adobe Workfront通过查看项目在时间线中的进度来确定项目的进度状态。 您可以配置Workfront以根据任务的进度状态的值确定项目的条件。 请参阅本文以了解有关项目进度状态的更多信息。
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
TQID: https://experienceleague.adobe.com/V9eyzkoYIREb4zUuDxmyDhnQa54YQaYTv2woNTOhq24
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 375
ht-degree: 2%

---

# 项目进度状态概述

<!--Audited: 12/2023-->

Adobe Workfront通过查看项目在时间线中的进度来确定项目的进度状态。 您可以配置Workfront以根据任务的进度状态的值确定项目的条件。 有关配置项目条件的更多信息，请参阅文章[项目条件和条件类型概述](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)。

以下是Workfront中项目的进度状态：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>准时</td> 
   <td> 如果符合以下条件，则项目的进度状态为<strong>开始时间</strong>：<ul><li>如果预计到期日和估计到期日均早于或等于项目的计划完成日期 <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p></li></ul>  </td> 
  </tr> 
  <tr> 
   <td>处于风险中</td> 
   <td> 如果以下<strong>全部</strong>为True，则项目的进度状态为<strong>有风险</strong>：<ul><li>估计完工日期和预计完工日期均在未来</li><li> 估计到期日期迟于计划完成日期和预计完成日期 <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p></li></ul> </td> 
  </tr> 
  <tr> 
   <td>滞后</td> 
   <td> 如果以下<strong>全部</strong>为True，则项目的进度状态为<strong>落后</strong>：<ul><li>估计完工日期和预计完工日期均在未来</li><li> 预计完成日期和预计完成日期均晚于项目的计划完成日期</li><li> 预计到期日期不晚于预计完成日期
   <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p></li></ul>  </td> 
  </tr> 
  <tr> 
   <td>迟到</td> 
   <td> 
     如果以下<strong>任一</strong>为True，则项目的进度状态为<strong>延迟</strong>：<ul><li>项目已完成，且实际完成日期迟于计划完成日期 <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>项目未完成，项目的计划完成日期为过去的日期 <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

请考虑以下事项：

* 项目的预计完成日期由关键路径上的任务以及最近的预计完成日期驱动。
* 项目的估计到期日由关键路径上带有最新估计到期日的任务驱动。

有关项目关键路径的信息，请参阅[项目关键路径概述](../../../manage-work/tasks/manage-tasks/critical-path.md)。

有关预计完成日期的信息，请参阅[项目、任务和问题的预计完成日期概览](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)。
