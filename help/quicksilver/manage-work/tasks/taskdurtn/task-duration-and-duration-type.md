---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 任务工期和工期类型概览
description: 任务持续时间是任务的计划完成日期和计划开始日期之间的差值。 “持续时间”表示任务可以完成的时间范围。
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: b42436ad660642bd23638a8a44d9561513d748ed
workflow-type: tm+mt
source-wordcount: '1791'
ht-degree: 1%

---

# 任务工期和工期类型概览

<!-- Audited: 12/2023 -->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

任务持续时间是任务的计划完成日期和计划开始日期之间的差值。 “持续时间”表示任务可以完成的时间范围。

任务的持续时间类型确定分配给任务的资源数量、总工作量以及任务总持续时间之间的关系。

## 任务持续时间概述

如果任务的实际起始日期和实际完成日期不在项目、主要被分配人或默认计划的计划之内，则任务持续时间为零。

>[!BEGINSHADEBOX]

**示例**
如果您的计划从上午9:00开始到中午12:00结束，并且任务计划从下午2:00开始到下午4:00结束，则任务的持续时间为零。


>[!ENDSHADEBOX]

以下是计算Adobe Workfront中的持续时间时存在的两种方案：

* 如果任务分配给一个用户，则根据您使用的环境，存在以下情况：

   * 在生产环境中，Workfront使用以下计划之一，按此确切顺序计算持续时间：

   1. Workfront会考虑用户的计划。
   1. 如果用户未与计划关联，则Workfront会考虑项目的计划。
   1. 如果项目未与时间表关联，Workfront会考虑您的系统的默认时间表。 有关计划的信息，请参阅[创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

<div class="preview">

* 在“预览”环境中：

   1. Workfront会考虑项目计划或分配给任务的用户的计划。

      当任务分配给一个用户时，您的Workfront或组管理员会确定Workfront使用的计划。 有关信息，请参阅[配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

   1. 如果用户或项目没有计划，Workfront将使用系统默认计划。

      这些步骤类似于了解Workfront使用哪个计划计算持续时间后的第一个方案。

</div>

* 如果任务分配给多个用户：

   1. Workfront会考虑项目或主要受让人的日程安排。

      当任务分配给多个用户时，由Workfront或组管理员确定Workfront使用的计划。 有关信息，请参阅[配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

   1. 如果主要被分配人或项目没有时间表，Workfront使用系统默认时间表。

  这些步骤类似于了解Workfront使用哪个计划计算持续时间后的第一个方案。

>[!NOTE]
>
>当考虑到主要受让人在项目中的休息时间时，任务的计划日期可能会调整，但任务的持续时间保持不变。 有关在计划项目时考虑主要被分配人的空闲时间的信息，请参阅[配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

## 任务持续时间的时间单位

您可以按常规时间以及计划开始日期和计划完成日期之间的经过时间指明任务持续时间。

更新列表中的任务持续时间时，可以使用以下缩写来指示Workfront中的时间单位：

| 时间单位 | 缩写 |
|---|---|
| 分钟 | 一 |
| 小时 | H |
| 天。 这是默认设置。 | D |
| 周 | 星期- |
| 月 | T， MO |
| 经过的分钟数 | EM |
| 经过的小时数 | EH |
| 经过的天数 | ED |
| 经过的周数 | EW |
| 经过的月数 | ET |

{style="table-layout:auto"}

>[!BEGINSHADEBOX]

**示例**

如果要指示任务的持续时间是3天经过的时间，应在任务列表的“持续时间”字段中键入“3 ED”。  在编辑任务时，您还可以从可用下拉菜单或任务详细信息部分中选择持续时间单位首选选项。 有关编辑任务的信息，请参阅[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。


>[!ENDSHADEBOX]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

在指示任务的持续时间时，请考虑以下事项：

* 占用时间是任务持续时间的时间单位。 该时间是任务的计划开始日期与计划完成日期之间的时间，包括假日、周末和休息时间。 换言之，经过的时间就是行事历的日数。
* 天数表示系统中定义的工作日，可以在“设置”区域中配置该天数。 在大多数情况下，一天包含8小时。
* 常规时间（日或工作日）考虑假日、周末和休息时间，并将其排除在任务持续时间之外。
* 当您以周为单位指定任务的持续时间时，Workfront会根据Workfront管理员在“设置”的“项目首选项”区域中设置的每周典型工作日和每个工作日的典型小时数设置，以天和小时计算持续时间。
* 在计算以月为单位的持续时间时，Workfront使用4周的默认持续时间来表示一个月。

## 任务持续时间类型概述

通过管理任务的持续时间类型，您可以根据任务的需求设置一致的资源分配。

持续时间类型有助于回答以下问题：

* 我们要多忙啊？
* 这项工作有多大？
* 要花多久时间？

![duration_type_triangle.png](assets/duration_type_triangle.png)

## 定义持续时间类型

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row"><p><strong>持续时间类型</strong></p></th> 
   <th scope="col"> <p><strong>函数</strong> </p> </th> 
   <th scope="col"> <p><strong>资源如何影响它</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>计算的工作分配</strong> </p> </th> 
   <td scope="col"> <p>计算任务中每个被分配人的分配百分比。 </p> <p>选择此持续时间类型时，可以为任务输入单个持续时间和已计划小时数。 Workfront将计划小时数除以任务持续时间内的小时数，再除以分配给任务的资源数，从而计算每个被分配人的分配。</p> <p>有关更多详细信息，请参阅<a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">持续时间类型概述：计算的分配</a>。</p> </td> 
   <td scope="col">向任务添加或移除被分配者时，持续时间和已计划小时数未发生变化。 </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>计算的工作量</strong> </p> </th> 
   <td scope="col"> <p>确定完成任务所需的计划小时数（工作量）。</p> <p>通常用于为任务的整个持续时间分配分配给任务的资源时。</p> <p>选择此持续时间类型后，您能够为任务输入单个持续时间。 Workfront计算该任务的已计划小时数，方法是用工期的天数乘以计划中的工作小时数并乘以该任务的被分配人数。 </p> <p>您可以手动将每个被分配人的分配百分比更改为任务，这将缩短计划小时数。</p> <p>有关更多详细信息，请参阅<a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">持续时间类型概述：计算的工作量</a>。</p> </td> 
   <td scope="col"> <p>将受分配者添加到任务后，计划小时数增加。 </p> <p>从任务中删除被分配者时，计划小时数会减少。</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>投入比导向</strong></p> </th> 
   <td scope="col"> <p>基于资源数确定计划小时数。</p> <p>选择此持续时间类型后，您能够为任务输入单个持续时间。 Workfront计算该任务的已计划小时数，方法是用工期中的天数乘以计划中的工作小时数，然后除以该任务的被分配人数。 </p> <p>您可以手动将每个被分配人的分配百分比更改为任务，但计划小时数保持不变。</p> <p>有关详细信息，请参阅<a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">持续时间类型概述：投入比导向</a>。</p> </td> 
   <td scope="col"> <p>从任务中删除被分配者时，计划的小时数增加。</p> <p>将受分配者添加到任务后，计划小时数会减少。 </p> <p>无论被分配人数量或其时间表如何变化，持续时间都不会改变。 </p> <p>持续时间等于计划小时数。 计划持续时间等于计划小时数除以被分配人数量。</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>简单</strong> </p> </th> 
   <td scope="col"> <p>根据每个被分配人分配的小时数确定计划小时数和持续时间（对于此持续时间类型是相同的）。 </p> <p>Workfront通过将每个被分配人的计划分配小时数相加来计算计划小时数。 </p> <p>您可以手动更改每个被分配人的分配小时数，计划小时数和持续时间量会相应地更改。 如果您为所有被分配人选择分配的总小时数，则该数字将平均分配给每个被分配人。</p> <p>有关详细信息，请参阅<a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">持续时间类型概述：简单</a>。</p> </td> 
   <td scope="col"> <p>如果选择分配的总小时数，则小时数平均分配给被分派人。 但是，作为项目经理，您可以手动调整每个被分配人的小时数。 </p> <p>您可以内联或在任务级别编辑具有“简单持续时间类型”的任务的已计划小时数和持续时间。 </p> <p>如果将Agile团队分配给任务，则“持续时间类型”自动设置为“简单”，且无法更改。 Agile团队的任务持续时间必须大于0分钟。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 新任务的持续时间类型

新任务的持续时间类型与系统中设置的持续时间类型匹配。 默认持续时间类型为计算分配。 Workfront管理员或组管理员可以更新系统或与项目关联的组的默认持续时间类型。 有关信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

## 父任务的原始持续时间

任务的原始持续时间是指任务在成为父任务之前的原始持续时间（以分钟为单位）。

当任务成为父任务时，最早子任务的计划开始日期与最后一个子任务的计划完成日期之间的持续时间将累计到父任务，并成为父任务的持续时间。 这将替换原始任务的持续时间。

当子级使用经过天数的持续时间单位并且父级使用天数的持续时间单位时，Workfront计算父级任务的持续时间的方式可能存在差异。

请考虑以下事项：

* 持续时间单位“经过天数”表示日历日，该日历日始终由每天24小时组成。
* 持续时间单位“天数”表示在系统中定义的工作日，并且可以对其进行配置。 在大多数情况下，包括每天8小时。
* 用于计算父任务持续时间的公式如下：

  `Parent task duration = Planned Completion Date of the child task that is planned to end the latest - Planned Start Date of the child task that starts the earliest`

* 在计算父任务的持续时间时，系统首先按上述公式计算持续时间，然后应用计划。


有关详细信息，请参阅[任务原始持续时间概述和原始计划小时数](/help/quicksilver/manage-work/tasks/task-information/task-original-duration-and-original-planned-hours.md)。

## 更改任务的持续时间类型

有关更改任务的持续时间类型的信息，请参阅[更新任务的持续时间类型](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)。
