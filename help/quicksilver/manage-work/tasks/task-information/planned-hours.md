---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 计划小时数概述
description: 与任务、问题或项目关联的已计划小时数表示已分配用户完成任务、问题或项目所需的时间量。
author: Alina
feature: Work Management
exl-id: 0b86c760-691a-436e-9beb-31e9ac36440a
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '2815'
ht-degree: 0%

---

# 计划小时数概述

<!-- Audited: 01/2024 -->

与任务、问题或项目关联的已计划小时数表示已分配用户完成任务、问题或项目所需的时间量。

## 关于Adobe Workfront中计划小时数的注意事项

* 计划小时数主要与Adobe Workfront中的工作项（任务和问题）相关联。 工作项的计划小时数累计到其项目的计划小时数。
* 默认情况下，Workfront将任务和问题已计划小时数平均分发给任务或问题持续时间中的所有天。
* 将用户和角色分配给任务和问题后，任务和问题的已计划小时数将与用户或角色分配相关联。
* 如果要使用Workfront中的资源管理工具，则必须为任务和问题定义规划小时数的值。
* 您只能为某些持续时间类型修改任务的已计划小时数的值。

  有关修改与任务的持续时间类型相关的任务计划小时数的详细信息，请参阅本文中的[根据持续时间类型更新任务计划小时数](#update-task-planned-hours-based-on-duration-type)部分。

* 您可以随时修改问题的已计划小时数的值。
* 您无法修改项目或父任务的计划小时数的值，因为它们是其所有任务和子任务的所有计划小时数的计算总数。
* 使用资源管理工具管理用户分配可能会更改任务、问题和项目的计划小时数，以及与工作项关联的工作分配的数量。

## 任务的计划小时数与项目的计划小时数 {#planned-hours-on-tasks-vs-planned-hours-on-projects}

任务中的计划小时数累计到项目的计划小时数。 问题中的计划小时数并不总是累计到项目的计划小时数。

本节介绍任务和项目计划小时数之间的差异。 它还描述了您可以在何处查看汇总到项目的问题计划小时数。

### 任务的计划小时数 {#planned-hours-on-tasks}

任务的计划小时数表示估计任务的实际工时可能花费的时间。 默认情况下，Workfront会平均分配每个任务持续时间内每天的计划小时总数。 每日已计划小时数将成为任务的每日分配数。 如果将任务分配给多个资源，则默认情况下，每个资源分配的每日小时数相等。

使用工作负载均衡器，您可以修改分配给任务的用户的每日分配。 当任务持续时间类型为简单时，这还可以更新任务的已计划小时数。 有关详细信息，请参阅在工作负载均衡器[中的管理用户分派一文](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)中的“管理用户分派时更新任务已计划小时数”部分。

当任务包含子任务时，父任务的计划小时数是任何子任务上所有计划小时数的总和。 您无法更新父任务的已计划小时数。

>[!NOTE]
>
>与计划小时数不同，父任务的实际小时数是直接在父任务中记录的小时数。 它们不表示子任务的实际小时数总和。\
>有关实际小时数的详细信息，请参阅[查看实际小时数](../../../manage-work/tasks/task-information/actual-hours.md)。

### 项目计划小时数 {#planned-hours-on-projects}

您无法编辑项目中的计划小时数。 项目计划小时数是项目所有任务中所有计划小时数的计算总和。

是否在计划小时数计算中包括问题取决于您在项目中查看计划小时数的位置。 您可以在项目的以下位置查看项目计划小时数：

* **项目详细信息部分和“编辑项目”框**：只考虑项目上任务的计划小时数。 在项目详细信息部分或编辑项目框中查看项目的计划小时总数时，不考虑项目上问题的计划小时数。

* **工作负载均衡器**：项目的工作负载均衡器中仅显示与工作负载均衡器中可见的任务关联的已计划小时数。 用户每日分配可以在工作负载均衡器中更改项目每日已计划小时数。
* **利用率部分**：在利用率部分中查看项目的计划小时总数时，会考虑与分配给任务和项目问题之用户关联的计划小时数。
* 任务列表中的&#x200B;**角色分配面板**：在此区域显示分配给工作角色或与工作角色关联的用户的任务和项目问题的计划小时数。 与未分配或分配给团队的任务和问题关联的已计划小时数不显示在此区域中。 有关详细信息，请参阅[在角色分配面板](../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md)中查看项目计划小时数。

## 在任务持续时间内的计划小时数分布

默认情况下，Workfront在任务持续时间中平均分配已计划小时数，根据项目计划的可用性为任务的每天分配相同数量的已计划小时数。

例如，如果任务设置为在下午4点开始，并且时间表在任务的第一天余下一小时，Workfront在任务工期的第一天放置一个已计划小时数，然后将已计划小时数的剩余部分平均分配到任务工期的其余天中。

>[!NOTE]
>
>每日计划小时数或每日分配是在任务持续时间期间每天的计划小时数的分配。 如果任务有一个分配，则此数字表示每个分配的每日计划小时数。 如果任务有多个分配，则每个分配的每日计划小时数与任务的每日计划小时数不同。 对于具有多个分配的任务，Workfront中每个分配的每日计划小时数没有可视化表示形式。

## 查找并了解计划小时数值

您可以在Workfront的各个区域找到计划小时数值。

显示的已计划小时数源自项目上的工作项，或者计算方式有所不同，具体取决于您在中查看这些工作项的区域和对象。

您可以在Workfront的以下区域找到计划小时数：

* [项目、任务或问题的详细信息部分](#the-details-section-of-a-project-task-or-issue)
* [编辑任务或编辑问题框](#the-edit-task-or-edit-issue-box)
* [报告](#reports)
* [工作负载均衡器](#the-workload-balancer)
* [资源规划者](#the-resource-planner)
* [使用情况报告](#the-utilization-report)
* [“角色分配”面板](#the-role-allocation-panel)

### 项目、任务或问题的详细信息部分 {#the-details-section-of-a-project-task-or-issue}

![详细信息部分中的计划小时数](assets/planned-hours-on-details-for-project.png)

任务、问题或项目的详细信息部分中的计划小时数是与项目关联的计划小时数总计。

有关项目计划小时数的详细信息，请参阅本文中的[任务计划小时数与项目计划小时数](#planned-hours-on-tasks-vs-planned-hours-on-projects)部分。

### “编辑任务”或“编辑问题”框 {#the-edit-task-or-edit-issue-box}

![编辑任务框](assets/planned-hours-on-edit-task-box-nwe.png)

任务或问题的编辑框中的计划小时数是相应项目的总计划小时数。

有关项目计划小时数的详细信息，请参阅本文中的[任务计划小时数与项目计划小时数](#planned-hours-on-tasks-vs-planned-hours-on-projects)部分。

对于任务，只能编辑某些持续时间类型的已计划小时数。 有关信息，请参阅本文中的[根据持续时间类型更新任务已计划小时数](#update-task-planned-hours-based-on-duration-type)部分。

您可以在分配区域查看分配给任务或问题的每个用户或工作角色的单独计划小时数分配。

### 报告 {#reports}

![计划报告小时数](assets/planned-hours-on-task-report.png)

您可以在项目、任务和问题报告中添加规划小时数字段。

默认情况下，计划小时数列包含在任务列表的标准视图中。

任务、问题或项目报告中的计划小时数是相应项目在项目的“详细信息”部分或“编辑”框中显示的计划小时数总计。

有关创建报告的信息，请参阅[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

>[!NOTE]
>
>如果您创建项目（财务数据）报告并按日期对其进行分组，则计划小时数可能会显示项目计划小时数的一部分，具体取决于项目上任务的时间线。 默认情况下，Workfront会为任务持续时间的每天平均分配任务计划小时数。 特定时间范围的计划小时数与Workfront在项目（财务数据）报表中为该时间范围设置的相等分布相匹配。

<!--
### The Scheduling areas  {#the-scheduling-areas}

![](assets/task-detail-expanded-in-scheduler-with-planned-hours-and-adjusted-daily-allocations-nwe-350x323.png)

The Planned Hours for tasks and issues display in the Scheduling areas in the Planned Hours field.

You can view the daily allocation of Planned Hours for each user assigned to a task or an issue in the Scheduling areas.

The daily hour amount represents one of the following:

* the default amount equally distributed by Workfront for each day of the Duration of the tasks or issues
* the adjusted daily allocation managed by resource managers.

  For information about adjusting daily allocations in the Scheduling tools, see [Manage user allocations in the Scheduling areas](../../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).
-->

### 工作负载均衡器 {#the-workload-balancer}

工作负载均衡器中的![计划小时数](assets/planned-hours-on-wb-expanded-with-pti-info.png)

任务、问题和项目的以下已计划小时数显示在任务、问题或项目名称右侧的工作负载均衡器中：

* 对于任务和问题，显示与其关联的已计划小时数。
* 对于项目，屏幕中显示的任务和问题的计划小时总数。

  >[!TIP]
  >
  >工作负载均衡器未在项目详细信息区域显示项目的所有计划小时数。

您可以在工作负载均衡器中查看分配给任务或问题的每个用户的每日计划小时数分配。

计划小时数的每日小时数表示以下小时数之一： 

* Workfront在任务、问题或项目持续时间的每天平均分配的默认金额
* 由资源管理器管理的调整后的每日分配

  有关在工作负载均衡器中调整每日分配的信息，请参阅[在工作负载均衡器中管理用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。

### 资源规划者 {#the-resource-planner}

资源规划者中的![计划小时数](assets/planned-hours-on-all-objects-in-resource-planned-expanded.png)

资源规划者显示项目、任务和问题的计划小时数。

您可以在资源规划者的PLN列中查看与工作项关联的用户和工作角色的每周计划小时数分配。

>[!TIP]
>
>工作负载均衡器中的每日分配调整影响资源规划者中任务和问题的每周分配。

每个对象的计划小时数因应用于资源规划者的视图而异。 有关详细信息，请参阅资源规划者[的项目和角色视图中的](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)小时概述、FTE和成本信息。

任务和问题的每周计划小时数表示以下值之一：

* Workfront在任务或问题持续时间的每天平均分配的默认每周金额
* 由工作负载均衡器中的资源管理器管理的已调整每周分配

  有关在工作负载均衡器中调整每日分配的信息，请参阅[在工作负载均衡器中管理用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。

项目、用户和角色的每周金额受与其关联的任务和问题的每周计划小时数的影响。

### 利用率报告 {#the-utilization-report}

项目计划小时数是指与每个任务和问题的工作分配关联的小时数。

>[!IMPORTANT]
>
>请注意，“利用率”报告中的“计划小时数”与分配相关联，而不是与任务和问题本身相关联。 利用率报告中的计划小时数与项目任务和问题的计划小时数并不总是匹配。 但是，计划小时数与任务和问题的工作分配关联的小时数不匹配。

您可以在“利用率”报表中查看以下类型的计划小时数：

* 在包含项目的整个生命周期内，项目上所有工作分配的总计划小时数
* 指定日期范围内所有分配的总计划小时数（您可以指定单独的周或月）。

  当使用工作负载均衡器调整了用户每日小时分配时，如果在利用率报表中选择的日期仅包含任务或问题的持续时间的一部分，则特定日期范围的已计划小时数可能会受到影响。 有关调整用户每日分配的信息，请参阅[在工作负载均衡器中管理用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。

有关详细信息，请参阅[查看资源利用率信息](../../../resource-mgmt/resource-utilization/view-utilization-information.md)。

### “角色分配”面板

角色分配面板中的计划小时数表示在项目总持续时间中与分配给项目任务或问题的每个工作角色关联的计划小时数。 该数字与资源规划者中的角色“已计划小时数”匹配。

>[!TIP]
>
>请注意，与用户关联的已计划小时数未显示在角色分配面板中。

有关详细信息，请参阅[在工作负载均衡器](../../../scenario-planner/show-role-allocation-workload-balancer.md)中显示项目和计划的角色分配。

## 根据持续时间类型更新任务已计划小时数 {#update-task-planned-hours-based-on-duration-type}

仅当任务具有特定的持续时间类型时，才能在编辑任务时更新任务的总计划小时数。

存在以下情况：

* 只有在编辑任务时使用计算的分配或简单的持续时间类型时，您才能修改任务的已计划小时数。

  有关计算分配持续时间类型的详细信息，请参阅[持续时间类型概述：计算分配](../../../manage-work/tasks/taskdurtn/calculated-assignment.md)。

  有关简单持续时间类型的详细信息，请参阅[持续时间类型概述：简单](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)。

* 当管理用户对任务的分配时，您只能在工作负载均衡器中为简单持续时间类型任务更新任务已计划小时数。 有关管理工作负载均衡器中的用户分配的信息，请参阅[管理工作负载均衡器中的用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。
* 您无法修改工期类型为投入比导向或已计算工作的任务的已计划小时数。 在这些情况下，Workfront根据任务的持续时间确定计划小时数；但在这种情况下，计划小时数始终等于持续时间（以小时为单位），并且不受已分配资源的百分比分配的影响。

  有关投入比驱动的持续时间类型的详细信息，请参阅[持续时间类型概述：投入比驱动](../../../manage-work/tasks/taskdurtn/effort-driven.md)。

  有关计算的工作持续时间类型的详细信息，请参阅[持续时间类型概述：计算的工作量](../../../manage-work/tasks/taskdurtn/calculated-work.md)。

## 管理用户分派时更新任务已计划小时数

在手动更新任务的用户或工作角色分配时，您可以更新任务的已计划小时数。 仅当任务的持续时间类型为“简单”时，才可以执行此操作。

有关详细信息，请参阅[持续时间类型概述：简单](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)。

在使用工作负载均衡器时，您可以更新分配给任务的用户和角色的总体分配，也可以更新用户每日分配。

有关管理任务的总体用户和工作角色分配的信息，请参阅[管理任务和角色分配小时数](../../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md)。

有关管理任务的每日分配的信息，请参阅[在工作负载均衡器](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)中管理用户分配。

手动更新任务的用户或工作角色分配时，存在以下情况：

* 如果您未手动更新单个用户或角色分配以触发对任务计划小时数的更改，则在您添加、删除或替换任务上的分配时，计划小时数保持不变。 向任务添加新分配时，各个分配将在所有被分配者之间重新分配。
* 当您手动更新分配以触发对任务计划小时数的更改时，计划小时数会在您从任务中删除分配时减少。 当您替换分配时，它们保持不变。
* 当您手动更新分配以触发对任务计划小时数的更改并向任务添加分配时，新分配默认分配为0小时。 您必须手动更新他们到任务的分配，这可能会影响规划小时数。
* 如果您未手动更新分配以触发对任务计划小时数的更改，并且您删除了任务的所有分配，则计划小时数将保持不变。
* 当您手动更新分配以触发对任务计划小时数的更改并且删除任务的所有分配时，计划小时数也会被删除，任务的计划小时数变为0。

>[!NOTE]
>
>例如，如果一项任务具有10个计划小时数，而您有两个被分配人，则默认情况下会为每个人分配5小时。
>
>* 如果您未使用工作负载均衡器更新单个用户分配或每日分配，并且从任务中删除了任何或所有被分配人，则任务已计划小时数仍为10小时。
>* 如果您将分配分配分别手动更改为4小时和6小时，并且删除分配到6小时的用户及其工作角色，则任务计划小时数将更新为4小时。 如果您还删除分配给4小时的用户，但保留与已删除用户关联的工作角色，则任务的已计划小时数将保留4小时。 如果删除最后一个分配到4小时的用户及其工作角色，并且任务仍然未分配，则任务计划小时数将变为0。

## 使用工作投入自动更新任务已计划小时数

当您使用工作投入来估计完成任务所需的投入时，任务的已计划小时数将自动更新。 这仅适用于具有简单持续时间类型的任务。

有关使用工作投入估计任务投入的信息，请参阅[工作投入概述](../../../manage-work/tasks/task-information/work-effort.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this issue has the explanation of how Planned Hours should work - from Vazgen and Anna: https://hub.workfront.com/issue/6217dced00730b7034c4b808339a35ce/</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Details of their comments: </p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Anna Asatryan</p>
<p>3/22/2022 At 3:16 PM</p>
<p>&nbsp;</p>
<p>to Mark Paul, Corrie Butler, Arman Simonyan, Gagik Khalatyan, Alina Wilson, Artur Sargsyan, Vazgen Babayan, Anna Asatryan</p>
<p>I have done some rough calculations on what the planned hours/revenues should look like Book.xlsx . And if we look, for example at the 2 users highlighted in one of the screenshots their planned hours look way off from what the calculation looks like in the spreadsheet (i.e. equally distributed allocation). When looking at the Workload balancer (the second screenshot), as an example for the user Yashas Mitta, I can see that the allocation has been modified. Obviously the utilization report calculates the allocations based on the modified contouring using the new work per day calculation. The project financial report uses the old, equal distribution of allocation along the full duration of the task. Hence. there is a difference when grouping per periods.</p>
<p>Vazgen Babayan</p>
<p>I believe we will need to prioritise syncing the project financial data report with the new work per day.</p>
<p>Alina Wilson</p>
<p>@Anna Asatryan , do you have a definition of what we should say in documentation (glossary, for example) for how the Planned Hours (or Planned Revenue) is calculated, keeping in mind that we don't document the concept of "workPerDay". We call them "daily allocations", for example, but let me know if that's accurate, too.</p>
<p>Vazgen Babayan</p>
<p>Last Thursday at 3:13 PM</p>
<p>I think an important note here is that regardless the calculation, even if the both views used the same formula, they will not display the same data, because the underlying data sources are different. The Financial Data report does not respect user-entered allocations in Workload Balancer at this moment. So there will be a clear discrepancy, as Anna showed in her message. My recommendation for communication will be to explain that the data sources are different so there can be a mismatch in data and that we will look into addressing that on our roadmap.</p>
<p>Alina Wilson</p>
<p>So far, I hear you guys say this (with my questions for confirmation/ comments in bold):</p>
<p>- the utilization report calculates the allocations based on the modified contouring using the new work per day calculation (so this is what we see in the Workload Balancer, right?)</p>
<p>- the project financial report uses the old, equal distribution of allocation along the full duration of the task (this is before the daily allocations for example were modified in the WB, right?)</p>
<p>I have these additional questions:</p>
<p>- what does the Project Details show? Which Planned Hours, for instance - because earlier, we had a question about this also. - which numbers?</p>
<p>- what does any Planned Hours/ Planned Revenue field that can be pulled in any other report (outside of Financial Data and Utilization reports) show? - which numbers?</p>
<p>- are there any other areas I am not thinking of that we need to document, @Corrie Butler</p>
<p>I will try to document all the possible areas where these display but please help. Thanks!</p>
<p>Vazgen Babayan</p>
<p>Last Saturday at 3:41 PM</p>
<ul>
<li> <p>Confirming the first two points </p> </li>
</ul>
<p>For the following questions</p>
<ul>
<li> <p>Project details show an aggregated sum of task planned hours. It doesn't have anything to do with the work per day because it always deals with total numbers for the whole duration of the Project/Task.</p> </li>
<li> <p>Same thing applies to the Planned Hours and Planned Revenue fields in reports - they show totals for the whole Project/Task duration and thus have no use of work per day.</p> </li>
<li> <p>Can't think of any other fields related to this right now.</p> </li>
<li> <p>In general, if I were to summarize the system behavior, it's as follows:</p> </li>
<li> <p>Every area that only deals with total numbers of Planned Hours / Planned Revenue, uses the numbers entered on the tasks. Those are Task / Project Details, reports exposing those fields.</p> </li>
<li> <p>Areas that deal with time-sensitive portions of Planned Hours / Planned Revenue, use work per day. Those are all Resource Management tools - Workload Balancer, Resource Planner, Utilization Report, importing projects via Scenario Planner.</p> </li>
<li> <p>All the areas in the second point support user-edited allocations made in Workload Balancer.</p> </li>
<li> <p>Scheduling area and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from Workload Balancer.</p> </li>
<li> <p>Scheduling will be removed this year, and we need to do work to move the Project Financial Data reports to the new work per day sometime after Q3.</p> </li>
</ul>
<p>Alina Wilson</p>
<p>@Vazgen Babayan , one clarifying question: when you say "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" - you mean that those use the system default which spreads the allocations evenly, correct? Because you can edit (daily) allocations in Scheduling tools, but it doesn't use that, correct? It uses the default of the daily allocation that the system figures out when dividing the Planned Hours by the number of days in the Duration. Please let me know. And thanks!</p>
<p>Anna Asatryan</p>
<p>Yesterday at 11:42 AM</p>
<p>@Alina Wilson , that's correct, when saying "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" Vazgen meant that it spreads the allocation evenly.</p>
<p>As for the scheduling, the allocation modification that's being done there isn't reflected anywhere else in the application other than in the Scheduling itself. That's probably one of the reasons it's being deprecated.</p>
</div>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <br> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: everything below is drafted because I replaced it with the table above)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can find the Planned Hours information on tasks, issues, or projects in the following locations:</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours in the Details  section  of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours in the Details  section  is identical for tasks, issues, and projects. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the Planned Hours value on the Details  section  of a task: </p>
<ol>
<li value="1">Go to a task for which you want to review the Planned Hours.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Overview</strong> area and notice the Planned Hours value.</p> <p>This value represents the time it would take the user assigned to the task to complete it. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3> </h3>
<p>The Planned Hours in the Edit box of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours while editing a task or an issue is identical. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the value of Planned Hours while editing a task:</p>
<ol>
<li value="1">Go to the task or issue you want to view Planned Hours for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> <p>The Planned Hours are located in the <strong>Overview</strong> section. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours column is included in the Standard view of a task list, by default. For issues and projects, you can add it to the view, when you are editing the view or when you build a report. </p>
<p>The Planned Hours in a task, issue, or project report are the total Planned Hours of the respective item as they display in the Details  section  or the Edit box of the items. </p>
<p>Adding the Planned Hours column to a project view is similar to building a view in a project report. </p>
<p>To show Planned Hours in a project report:</p>
<ol>
<li value="1"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Workfront, then click <strong>Reports</strong>. </p> </li>
<li value="2">Click <strong>New Report</strong>, then choose <strong>Project</strong> as your object.</li>
<li value="3">Click <strong>Add Column</strong>, and start typing <strong>Planned Hours</strong> when the <strong>Show in this column</strong> drop-down field is displayed. Select the field when it appears in the list.</li>
<li value="4"> <p>Click <strong>Save + Close</strong> to save the report. </p> <p>The Planned Hours column shows the total number of Planned Hours on each project. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Planned Hours in Resource Management tools</p> <note type="important">
When viewing Planned Hours in the Resource Management tools by a specific time frame, the daily allocations for each work item and the daily allocations for the resources assigned to the work items during that time frame can influence the daily Planned Hours of projects or work items.
</note>
<p>You can see the value of Planned Hours for your tasks, issues, or projects when using the following Resource Management tools:</p>
<ul>
<li> <p>Resource Planner</p> <p>For information about using the Resource Planner, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</p> </li>
<li> <p>Utilization Report.</p> <p>For information about the utilization report, see <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Overview of the Resource Utilization report</a>.</p> </li>
<li>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Workload Balancer or Scheduling areas in the following sections:</p>
<ul>
<li>Scheduling or Workload Balancer sections in the Resourcing area</li>
<li>Scheduling or Workload Balancer section at the project level</li>
<li>Schedule or Workload Balancer section at the team level</li>
</ul>
</div> <p>For information about scheduling resources, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p> <p>For information about the Workload Balancer, see <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Workload Balancer overview</a>. </p> </li>
<li> <p><b>Role Allocation panel</b> in the project  task list or  Workload Balancer: The Planned Hours for the tasks and the issues on the project that are assigned to a job role or a user associated with a job role are taken into account in this area. For more information, see <a href="../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md" class="MCXref xref">View project Planned Hours in the Role Allocation panel</a>. </p> </li>
</ul>
</div>
-->
