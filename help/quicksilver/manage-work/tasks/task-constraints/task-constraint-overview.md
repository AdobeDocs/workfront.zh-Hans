---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: 任务限制概述
description: 任务约束决定了任务在项目中的开始和结束时间。
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 6%

---

# 任务限制概述

<!-- Audited: 12/2023 -->

任务约束决定了任务在项目中的开始和结束时间。

## 任务约束概览

在构建项目计划时，您可以根据项目任务的顺序和时间范围做出决策。 任务可以独立于任何任务序列运行，但它们可能会影响项目的时间表。 任务约束允许项目经理计划特定任务何时可以在项目上开始或完成。

根据您使用的约束条件，您可能需要为任务指定计划起始日期、计划完成日期或同时指定两者。

需要定义日期的限制类型会影响前置任务关系。

>[!TIP]
>
>如果在任务之间使用前置任务关系，请考虑使用不需要特定日期的限制类型。

下表显示了每个约束及其缩写。 任务列表和创建Kick-Start导入文件时使用缩写。 单击每个任务限制的链接标题，以了解有关该类型限制的更多信息。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col>
 <thead> 
  <tr> 
   <th> <p><strong>约束名称</strong> </p> </th> 
   <th> <p><strong>缩写</strong> </p> </th> 
   <th> <p><strong>描述</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">任务限制概述：尽快</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td>
   <td scope="col"> <p>将任务的开始时间尽量放置在项目开始时间附近。</p> 
   <p>如果项目从开始日期开始使用计划模式，并且新任务的系统默认开始日期设置为基于项目计划日期，则它是默认限制。 </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">任务限制概览：尽可能迟 </a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
   <td scope="col"> <p>使任务的完成时间尽可能接近项目的结尾。</p> 
   <p>当项目“计划模式”为“完成日期”，并且任务的“开始日期”的系统或组默认值设置为“基于项目计划日期”时，这是默认约束。 </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">任务约束概览：最早可用时间</a> </p> </td> 
   <td scope="col"> <p>EAT</p> </td> 
 <td scope="col"> <p>在考虑任何前置任务关系后，将任务调度为在最早可用时间开始。</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">任务限制概述：最新可用时间</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
   <td scope="col"> <p>考虑项目中的前置任务 — 后续任务关系后，将任务安排在最新的可用时间开始。</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">任务限制概览：开始时间不早于</a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
   <td scope="col"> <p>将任务安排在您指定的日期之后开始。</p> 
   <p>如果项目计划模式为起始日期，并且系统或组将新任务的默认起始日期设置为今天，则这是默认限制。   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">任务限制概述：开始时间不晚于</a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
   <td scope="col"> <p>将任务安排在您指定的日期之前开始。</p> 
   <p>如果项目“计划模式”是从“完成日期”开始，并且任务的“开始日期”的系统或组默认值设置为“今天”，则这是默认限制。 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">任务限制概览：完成时间不早于</a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td>
   <td scope="col"> <p>安排在指定日期之后完成的任务。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">任务限制概述：完成时间不晚于</a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
   <td scope="col"> <p>安排在指定日期之前完成的任务。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">任务限制概述：必须开始时间</a> </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
   <td scope="col"> <p>将任务计划为恰好在特定日期开始。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">任务限制概述：必须完成日期</a> </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
   <td scope="col"> <p>安排在特定日期结束的任务。</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">任务限制概览：固定日期</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
   <td> <p>将任务安排在特定日期开始和结束。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 默认约束概览

创建新任务时，Workfront会自动选择任务限制。

Workfront使用两个变量来确定默认情况下，为新任务选择哪个任务限制：

* 此 **项目时间表开始日期** 项目中的字段。

  有关“项目计划起始日期”字段的信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

* 此 **开始日期** 由Workfront或组管理员在 **任务和问题** 面积 **设置**.

  有关任务和问题首选项的信息，请参阅 [新任务默认值](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#new-task-defaults) 中的部分 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

下表显示了为项目和新任务选择不同变量时的默认任务限制：

| 项目时间表开始日期 | 任务开始日期 | 任务限制默认值 |
|---|---|---|
| 开始日期 | 基于项目计划日期 | 尽可能早 |
| 开始日期 | 今天 | 开始时间不早于 |
| 完成日期 | 基于项目计划日期 | 尽可能迟 |
| 完成日期 | 今天 | 开始时间不晚于 |
