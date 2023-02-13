---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 项目进度状态概述
description: Adobe Workfront通过查看项目在其时间轴中的进度来确定项目的进度状态。 您可以配置Workfront，以根据任务的进度状态值确定项目的条件。 有关配置项目条件的更多信息，请参阅项目条件和条件类型概述一文。
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---

# 项目进度状态概述

Adobe Workfront通过查看项目在其时间轴中的进度来确定项目的进度状态。 您可以配置Workfront，以根据任务的进度状态值确定项目的条件。 有关配置项目条件的详细信息，请参阅文章 [项目条件和条件类型概述](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

以下是Workfront中项目的进度状态：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>开始时间</td> 
   <td> <p>如果预计完成日期和预计完成日期都早于或等于项目的计划完成日期，则项目的进度状态为 <strong>开始时间</strong>.</p> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>处于风险中</td> 
   <td> <p>如果预计完成日期和预计完成日期都在将来但迟于项目的计划完成日期，并且预计完成日期迟于预计完成日期，则项目进度状态为 <strong>面临风险</strong>. </p> <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>滞后</td> 
   <td> <p>如果预计完成日期和预计完成日期都在将来但迟于项目的计划完成日期，但预计完成日期不迟于预计完成日期，则项目进度状态为 <strong>后面</strong>.</p> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>延迟</td> 
   <td> 
    <ul> 
     <li> <p>如果项目已完成且实际完成日期晚于计划完成日期，则项目的进度状态为 <strong>延迟</strong>. </p> <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>如果项目未完成，并且项目的计划完成日期已过，则项目进度状态为 <strong>延迟</strong>. </p> <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

请考虑以下事项：

* 项目的预计完成日期由关键路径上的任务（具有最新的预计完成日期）决定。
* 项目的预计完成日期由关键路径上的任务驱动，并且最近的预计完成日期。

有关项目关键路径的信息，请参阅 [项目关键路径概述](../../../manage-work/tasks/manage-tasks/critical-path.md).

有关预计完成日期的信息，请参阅 [项目、任务和问题的预计完成日期概览](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
