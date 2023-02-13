---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 任务持续时间和持续时间类型概述
description: 任务持续时间是任务的计划完成日期与计划起始日期之间的差值。 持续时间表示任务完成所需的时间范围。
author: Alina
feature: Work Management
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1383'
ht-degree: 2%

---

# 任务持续时间和持续时间类型概述

任务持续时间是任务的计划完成日期与计划起始日期之间的差值。 持续时间表示任务完成所需的时间范围。

任务的持续时间类型标识分配给任务的资源数量、总工作量和任务的总持续时间之间的关系。

## 任务持续时间概述

>[!NOTE]
>
>考虑主要受让人在项目上的休息时间时，任务的计划日期可能会调整，但任务的持续时间保持不变。 有关在规划项目时考虑主要受让人的休假时间的信息，请参阅  [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

如果任务的实际起始日期和实际完成日期不在项目、主要任务负责人或默认计划的计划之外，则任务持续时间为零。

**示例：** 如果您有一个从上午9:00开始、在下午12:00结束的计划，以及一个计划在下午2:00开始、下午4:00结束的任务，则任务的持续时间为零。

以下是在Adobe Workfront中计算持续时间时存在的两种情况。

* 如果任务被分配给用户，则Workfront会使用以下计划之一，按此精确顺序计算持续时间：

   1. Workfront会考虑用户的计划。
   1. 如果用户未与计划关联，则Workfront会考虑项目的计划。
   1. 如果项目与计划未关联，则Workfront会考虑您系统的默认计划。 有关计划的信息，请参阅 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* 如果任务被分配给多个用户：

   Workfront考虑项目计划或主要受让人的计划。

   当将任务分配给多个用户时，Workfront管理员会确定Workfront使用的计划。 有关信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   这些步骤与了解Workfront用于计算持续时间的计划后的第一个方案类似。

## 任务持续时间的时间单位

您可以在正常时间和计划起始日期与计划完成日期之间经过的时间中指示任务持续时间。

在更新列表中任务的持续时间时，可以使用以下缩写来指示Workfront中的时间单位：

| 时间单位 | 缩写 |
|---|---|
| 分钟 | 一 |
| 小时 | H |
| 天数. 这是默认设置。 | D |
| 周 | 三 |
| 月 | 二 |
| 占用分钟数 | EM |
| 占用小时数 | EH |
| 占用天数 | ED |
| 占用周数 | EW |
| 占用月数 | ET |

{style=&quot;table-layout:auto&quot;}

**示例：** 如果要指明任务的持续时间为3已经过天，则应在任务列表的持续时间字段中键入“3 ED”。  在编辑任务时，或在“任务详细信息”部分，您还可以从可用的下拉菜单中选择“持续时间单位”的首选选项。 有关编辑任务的信息，请参阅 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

在指示任务的持续时间时，请考虑以下事项：

* 已用时间是任务持续时间的单位。 任务的“计划起始日期”和“计划完成日期”之间的时间（包括假日、周末和休假时间）。 换言之，已用时间即为日历日的过去。
* 常规时间考虑节假日、周末和休假时间，并从任务的“持续时间”中排除这些时间。

* 当您以周为单位指示任务的持续时间时，Workfront会根据Workfront管理员在“设置”的“项目首选项”区域中设置的每周典型工作日和每个工作日的典型小时数设置，计算持续时间（以天和小时为单位）。
* Workfront在计算持续时间（以月为单位）时，使用4周的默认持续时间（一个月）。

## 任务持续时间类型概述

通过管理任务的持续时间类型，您可以根据任务的需求设置一致的资源分配。

持续时间类型有助于回答以下问题：

* 我们要多忙？
* 这份工作有多大？
* 要花多久？

![duration_type_triangle.png](assets/duration-type-triangle-350x245.png)

## 定义持续时间类型

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row">持续时间类型 </th> 
   <th scope="col"> <p><strong>功能</strong> </p> </th> 
   <th scope="col"> <p><strong>资源对It的影响</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>计算的分配量</strong> </p> </th> 
   <td scope="col"> <p>计算任务上每个受分派人的分配百分比。 </p> <p>选择此持续时间类型时，您可以为任务输入单个持续时间和计划小时数。 Workfront将计划小时数除以任务持续时间内的小时数，再除以分配给任务的资源数，以计算每个受分配人的分配。</p> <p>有关更多详细信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">持续时间类型概述：计算分配</a>.</p> </td> 
   <td scope="col">在向任务添加或移除任务分配人时，持续时间和计划小时数不会更改。 </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>计算的工作量</strong> </p> </th> 
   <td scope="col"> <p>确定完成任务所需的计划小时数（工作量）。</p> <p>在为任务分配的资源在任务的整个持续时间内分配时通常使用。</p> <p>选择此持续时间类型时，您能够为任务输入单个持续时间。 Workfront计算任务的计划小时数，方法是将持续时间中的天数乘以计划中的工作小时数和任务的受分配者数。 </p> <p>您可以人工将每个受分配人的分配百分比更改为任务，以缩短计划小时数。</p> <p>有关更多详细信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">持续时间类型概述：计算量度</a>.</p> </td> 
   <td scope="col"> <p>将受分配者添加到任务后，计划小时数会增加。 </p> <p>从任务中删除任务分配人后，计划小时数会减少。</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p>投入比导向</p> </th> 
   <td scope="col"> <p>根据资源数确定计划小时数。</p> <p>选择此持续时间类型时，您能够为任务输入单个持续时间。 Workfront计算任务的计划小时数，方法是将持续时间中的天数乘以计划中的工作小时数，然后除以任务的受分配者数。 </p> <p>您可以人工将每个受分配人的分配百分比更改为任务，但计划小时数保持不变。</p> <p>有关更多详细信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">持续时间类型概述：努力驱动</a>.</p> </td> 
   <td scope="col"> <p>从任务中删除受分配人后，计划小时数会增加。</p> <p>在任务中添加受分配者时，计划小时数会减少。 </p> <p>持续时间不会更改，无论受分配人数或其计划如何更改。 </p> <p>持续时间等于“计划小时数”。 计划持续时间等于计划小时数除以受分配者数量。</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>简单</strong> </p> </th> 
   <td scope="col"> <p>根据每个受分配人分配的小时数确定计划小时数和持续时间（对于此持续时间类型，它们是相同的）。 </p> <p>Workfront通过为每个受分配人合计计划分配的小时数来计算计划小时数。 </p> <p>您可以人工更改每个受分配人分配的小时数，并且计划小时数和持续时间金额会相应地发生更改。 如果为所有受分配人选择分配的总小时数，则该小时数在每个受分配人之间平均分配。</p> <p>有关更多详细信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">持续时间类型概述：简单</a>.</p> </td> 
   <td scope="col"> <p>如果选择分配的总小时数，则小时数在分配者之间平均分配。 但是，作为项目经理，您可以手动调整每个受让人的小时数。 </p> <p>您可以在内联或任务层编辑具有简单持续时间类型的任务的计划小时数和持续时间。 </p> <p>如果将敏捷团队分配给任务，则持续时间类型会自动设置为简单，并且无法更改。 敏捷团队的任务持续时间必须大于0分钟。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 新任务的持续时间类型

新任务的持续时间类型与系统中设置的持续时间类型匹配。 默认的持续时间类型为“计算分配”。 您的Workfront管理员或组管理员可以更新系统或与项目关联的组的默认持续时间类型。 有关信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## 更改任务的持续时间类型

有关更改任务的持续时间类型的信息，请参阅 [更新任务的持续时间类型](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
