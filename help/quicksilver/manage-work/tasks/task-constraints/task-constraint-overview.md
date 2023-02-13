---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: 任务约束概述
description: 任务约束决定了任务何时应在项目上开始和结束。
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 10%

---

# 任务约束概述

任务约束决定了任务何时应在项目上开始和结束。

## 任务约束概述

在构建项目计划时，您可以根据项目任务的顺序和时间范围做出决策。 任务可以独立于任何任务序列运行，但它们可能会影响项目时间轴。 任务约束允许项目经理在项目上开始或完成某些任务时进行规划。

根据您使用的约束，您可能必须为任务指定计划起始日期、计划完成日期或两者。

要求定义日期的约束类型会影响前置关系。

>[!TIP]
>
>如果在任务之间使用前置关系，请考虑使用不需要特定日期的约束类型。

下表显示了每个约束及其缩写。 在创建Kick-Start导入文件时，任务列表中使用缩写。 单击每个任务约束的链接标题可了解有关该类型约束的详细信息。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>约束名称</strong> </p> </th> 
   <th> <p><strong>缩写</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">任务约束概述：尽快</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">任务约束概述：尽可能晚 </a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">任务约束概述：最早可用时间</a> </p> </td> 
   <td scope="col"> <p>EAT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">任务约束概述：最新可用时间</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">任务约束概述：开始时间不早于</a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">任务约束概述：开始时间不晚于</a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">任务约束概述：不早于完成</a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">任务约束概述：不迟于完成</a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">任务约束概述：必须开始</a> </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">任务约束概述：必须完成</a> </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">任务约束概述：固定日期</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
  </tr> 
 </tbody> 
</table>

## 默认约束概述

创建新任务时，任务约束将由Workfront自动选择。

Workfront使用两个变量来确定为新任务默认选择的任务约束：

* 的 **项目计划自** 字段。

   有关“项目计划自”字段的信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

* 的 **开始日期** 首选项由您的Workfront或组管理员在 **任务和问题** 面积 **设置**.

   有关任务和问题首选项的信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

下表显示了在为项目和新任务选择不同变量时默认的任务约束：

| 项目计划自 | 任务开始日期 | 任务约束默认值 |
|---|---|---|
| 开始日期 | 基于项目计划日期 | 尽可能早 |
| 开始日期 | 今天 | 开始时间不早于 |
| 完成日期 | 基于项目计划日期 | 尽可能晚 |
| 完成日期 | 今天 | 开始时间不晚于 |
