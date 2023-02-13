---
product-area: resource-management
navigation-topic: resource-scheduling
title: 在“计划”区域中管理用户分配
description: 本文介绍了如何使用“资源计划”区域更新分配给任务或问题的用户的每日每小时分配。
author: Alina
feature: Resource Management
exl-id: c8ddb250-145e-4321-8747-4f4967fcce41
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2944'
ht-degree: 0%

---

# 在“计划”区域中管理用户分配

>[!IMPORTANT]
>  
><span class="preview">自2023年1月的23.1版本开始，本文中描述的计划功能已弃用并从Adobe Workfront中删除。   </span>
>  
> <span class="preview"> 2023年初23.1版发布后不久，也将删除本文。 此时，我们建议您相应地更新任何书签。 </span>
> 
><span class="preview"> 您现在可以使用负载平衡器来计划资源的工作。 </span>
>  
> <span class="preview">有关使用工作负载平衡器计划资源的信息，请参阅一节 [工作负载平衡器](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--  

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 

-->

用户分配是指用户在某一给定日期完成工作项所花费的时间（小时）。 它们包含在工作项的“计划时间”中。

本文介绍了如何使用“资源计划”区域更新分配给任务或问题的用户的每日每小时分配。 有关管理用户和任务作业角色的总体分配的信息，请参阅 [管理任务的用户和角色分配小时数](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md). 您无法更新用户的总体分配和问题的作业角色。

您可以在Adobe Workfront的以下区域中显示用户分配：

* 在“资源”区域的“计划”部分。
* 在项目的“计划”部分（为单个项目计划资源时）。
* 在团队的“计划”部分（为团队计划资源时）。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>查看或更高程度地访问项目、任务和问题</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>对项目、任务和问题拥有权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 计划区域中的用户分配

在您开始按照本文所述将时间分配给用户之前，请熟悉资源计划在Workfront中的工作方式，如 [资源计划入门](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

您可以安排资源处理您所属的单个团队的任务和问题，也可以安排资源处理您所属的单个项目的任务和问题，或者安排资源处理您所属的项目团队成员的多个项目的任务和问题。

以下各节介绍如何在Workfront中启用和管理用户分配：

* [使用“计划”区域来分配工作](#use-the-scheduling-areas-to-assign-work)
* [在“编辑任务”或“编辑问题”框中设置的分配与在“计划”区域中设置的分配](#allocations-set-on-the-edit-task-or-the-edit-issue-boxes-vs-in-the-scheduling-areas)
* [分配指标](#allocation-indicators)
* [计划小时数的默认分配](#default-allocation-for-planned-hours)
* [谁可以查看和修改分配？](#who-can-view-and-modify-allocations)
* [计划区域中的时区注意事项](#time-zone-considerations-in-the-scheduling-areas)

### 使用“计划”区域来分配工作 {#use-the-scheduling-areas-to-assign-work}

在计划时间线上为用户分配新工作时，您可以确定如何将任务或问题的计划时间分配给用户。\
有关“计划时数”的详细信息，请参阅 [计划时数概述](../../manage-work/tasks/task-information/planned-hours.md).

计划时数可按以下方式划分：

* 在分配给任务或问题的用户中
* 任务或问题的整个持续时间\
   例如，在任务持续时间结束时，与销售相关的任务可能需要进行更多工作。 您可以计划任务中时数分配的不均衡。

>[!TIP]
>
>在从“计划”区域为多个项目计划资源时，并非所有用户和工作项都显示在计划时间轴上。 有关计划时间轴上显示哪些信息的信息，请参阅 [资源计划入门](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

### 在“编辑任务”或“编辑问题”框中设置的分配与在“计划”区域中设置的分配 {#allocations-set-on-the-edit-task-or-the-edit-issue-boxes-vs-in-the-scheduling-areas}

您可以在Workfront中从以下位置修改任务或问题的用户分配：

* 计划时间轴\
   计划时间轴位于以下区域：

   * 在“资源”区域的“计划”部分。
   * 在项目的“计划”部分（为单个项目计划资源时）。
   * 在团队的“计划”部分（为团队计划资源时）。

   当您从计划时间轴修改用户分配时(如 [修改用户分配](#modify-user-allocations) 部分)，您可以为任务或问题中的每个用户定义分配，以及为任务或问题持续时间内的每一天定义分配。\
   ![scheduling_contours.png](assets/scheduling-contours-350x139.png)

* 编辑任务或编辑问题对话框。\
   在“编辑任务”或“问题”对话框中修改用户分配时(如 [管理任务的用户或角色分配百分比](../../manage-work/tasks/assign-tasks/manage-allocation-percentage-on-tasks.md))，则您只能为每个用户定义任务或问题的整体分配。 如果要按天管理这些分配，则必须修改计划时间轴中的分配，如 [修改用户分配](#modify-user-allocations) 章节。

   >[!IMPORTANT]
   >
   >在“编辑任务”或“问题”对话框中修改用户分配时，之前在“计划时间轴”中配置的分配将被覆盖。 此外，您对计划时间轴中的分配所做的任何更改都不会反映在“编辑任务”或“问题”对话框中。

我们建议从计划时间轴而不是编辑任务或问题中管理用户分配，以便从以下优势中受益：

* 您可以使用分配指示器清楚地了解用户何时被过度分配，如 [分配指标](#allocation-indicators) 中。
* 您可以为一个用户分配更多时间，而不是为另一个用户。\
   分配指示器提供如何将分配的用户与其他用户进行比较的直观表示，如 [分配指标](#allocation-indicators) 中。

* 您可以为一天的工作分配更多时间，而不是一天的工作。\
   分配指标直观地显示了已分配用户在给定日期的方式，如 [分配指标](#allocation-indicators).

* 您可以在计划时间轴上的一个位置执行所有资源分配责任。

### 分配指标 {#allocation-indicators}

各种可视指示器可用于提供关于用户在指定日期工作所分配到的级别的快速信息。

系统管理员确定Workfront如何在系统级别计算用户可用性（考虑工时和FTE可用性）。 根据此系统范围的设置，可使用默认计划或用户的计划来计算用户可用性。 有关更多信息，请参阅 [配置Workfront如何计算“计划”区域的资源小时数和FTE可用性](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).

* **分配底纹**
在以明暗形式分配给用户的任务上，会以可视方式显示分配情况。 较深的底纹表示分配的小时数，以指定日期分配用户FTE（相当全职）的百分比表示。 (有关如何在Workfront中配置FTE的详细信息，请参阅 [配置Workfront如何计算“计划”区域的资源小时数和FTE可用性](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).)\
   例如，将单个用户分配给具有4个计划小时和1天持续时间的任务。 用户的FTE在系统中定义为1（这意味着用户计划以全时状态工作，或者是每周工作40小时，或每天工作8小时）。 给定日期的任务的底纹占任务垂直空间的一半，这表示用户在该日被分配了其FTE（4小时）的一半。\
   ![](assets/scheduling-shading-allocation.png)\
   任务或问题显示分配给工作项的所有用户的累计分配。 您可以展开工作项以查看更多详细信息，包括分配给工作项的人员以及分配给每个用户的小时数。\
   底纹不显示在 **未分配** 的上方。\
   ![resource_allocation_expanded.png](assets/resource-allocation-expanded-350x192.png)

* **每个用户的每日总计：** 您可以显示每天分配给给定用户的总计划小时数。 此信息显示在计划时间轴上每个用户行的顶部。 默认情况下，不显示此信息。 您可以按照 [启用用户分配](#enable-user-allocations). 确定每日总计时，将包含具有以下任何状态的项目中的任务：当前、计划或已批准。\
   ![resource_daily_totals.png](assets/resource-daily-totals-350x55.png)

* **超额分配指标**
如果在给定日期分配给用户的计划小时数总数超过用户在一天（跨所有任务）中工作的小时数，则该用户在该日会被视为被过度分配。\
   当用户被过度分配时，会显示一个红色栏，勾勒当天每项任务的轮廓。\
   在确定用户的过度分配时，将包含具有以下任何状态的项目中的任务：当前、计划或已批准。\
   用户一天中的工作小时数通过每个用户配置文件中的FTE字段定义，如 [配置Workfront如何计算“计划”区域的资源小时数和FTE可用性](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).\
   ![resource_over_allocation.png](assets/resource-over-allocation-350x72.png)\
   当您启用 **显示每日计划时数的合计** 和 **显示资源分配突出显示** 选项时，当用户被过度分配时，计划小时数的每日总数将以红色显示。 默认情况下，小时数显示在最接近的第十位（例如，1.3）。\
   ![RS_planned_hours_in_red_with_decimals__1_.png](assets/rs-planned-hours-in-red-with-decimals--1--350x56.png)

### 计划小时数的默认分配 {#default-allocation-for-planned-hours}

Workfront尝试在分配的用户和天数之间分配计划小时数，如下所示：

* 当将多个用户分配给任务或问题时，将在用户之间平均分配小时数。\
   分配反映已对任务进行的任何高级分配。\
   有关高级分配的详细信息，请参阅 [创建高级分配](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

* 当任务或问题的持续时间跨越多天时，计划小时数会根据用户的计划在各天之间以及分配给任务的所有用户之间平均分配。
* 当任务的计划小时数跨越多天时，从不同时区查看任务的用户可能会看到任务持续时间或计划起始日期或计划完成日期之间存在差异。

默认情况下，小时数显示为最接近的百分位值（例如，1.33）。 您可以滚动到右侧以查看更多内容。\
![RS_Planed_Hours_with_two_decimals_in_contour_screen__1___1_.png](assets/rs-planned-hours-with-two-decimals-in-contour-screen--1---1--350x252.png)

### 谁可以查看和修改分配？ {#who-can-view-and-modify-allocations}

以下类型的用户可以在Workfront中查看或修改用户分配：

* **资源管理器：** 您可以查看和修改任何项目（您为其资源管理器）中任务和问题的用户分配。 您可以在“人员”区域的“计划”时间轴中，或在项目的“人员配备”选项卡中执行此操作。\
   有关资源管理器如何更改项目中的任务和问题的信息，请参阅 [在“计划”区域中手动分配未分配的任务和问题](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

* **计划和工作用户：** 您可以使用新的“我的工作日历”或您所属团队的“工作日历”来查看分配给您的任何任务和问题的分配。\
   除了查看分配之外，如果您对任务和问题具有Contribute访问权限，则还可以修改分配。

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Article is conditioned to classic.)
  </MadCap:conditionalText>
  -->

### 计划区域中的时区注意事项  {#time-zone-considerations-in-the-scheduling-areas}

在极少数情况下，查看计划时间轴的用户可能会看到不一致的情况，即任务的计划时间不等于每天分配的总时间。 当一个用户的操作系统时区设置使得计划起始日期或计划完成日期与另一个用户不同时，就会发生这种情况。

例如，如果任务的“计划完成日期”在11/3/18 MST的上午11:00设置为，则在澳大利亚查看任务的用户将在次日11/4/18的上午1:00看到“计划完成日期”。 如果澳大利亚的用户在11/4/18年分配小时数，则这些分配的小时数在MST上对用户不可见。 但是，这些小时始终考虑项目的计划小时数。

## 启用用户分配 {#enable-user-allocations}

默认情况下，计划时间轴上会禁用用户分配功能。 您必须先启用用户分配功能，然后才能使用本节中介绍的用户分配功能。

>[!NOTE]
>
>只有在将计划时间轴配置为使用计划日期时，才能启用用户分配。 如果将计划时间轴配置为使用预计日期，则无法显示用户分配。 有关配置计划时间轴以使用计划日期或预计日期的详细信息，请参阅 [在“计划”区域中配置设置](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md).

要在计划时间轴上启用用户分配，请执行以下操作：

1. 转到多个项目、单个项目或团队的计划时间轴：

   * **对于多个项目**:  单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **资源配置>工作负载平衡器**，然后选择 **计划** 中。
   * **对于单个项目**:转到项目，单击 **工作负载平衡器** ，然后选择 **计划** 从左上角的下拉菜单中。
   * **对于团队**:单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **团队**，选择团队，单击&#x200B;**工作负载平衡器** 在左侧面板中，选择&#x200B;**计划** 从左上角的下拉菜单中。

   ![](assets/scheduling-tab-global-resourcing-area-nwe-350x145.png)

1. 单击 **设置** 图标。\
   ![scheduling_settings_icon.png](assets/scheduling-settings-icon-350x169.png)\
   此时将显示“资源计划设置”对话框。\
   ![RS_scheduling_tab_all_settings__4_.png](assets/rs-scheduling-tab-all-settings--4--350x348.png)

1. 启用以下一个或两个选项，以在计划时间轴上显示用户分配：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">突出显示资源分配</td> 
      <td> <p>在计划时间轴上显示任务和问题的用户分配底纹。 </p> <p>默认情况下，此选项处于禁用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">显示每日计划小时数的总数</td> 
      <td>显示计划时间线上每天分配给每个用户的计划小时总数。 “计划时数”显示为最接近的十分点（例如，1.3）。<br>默认情况下，此选项处于禁用状态。</td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）在 **包括问题** 部分，选择是否希望问题显示在计划时间轴上。\
   默认情况下，此选项处于禁用状态。

1. 单击 **返回计划**.\
   用户分配现在显示在计划时间轴上。\
   ![RS_daily_planed_totals_and_allocation_highlighting__1_.png](assets/rs-daily-planned-totals-and-allocation-highlighting--1--350x123.png)

## 修改用户分配 {#modify-user-allocations}

您可以从计划时间轴（如本节所述）或编辑任务或问题对话框中修改任务或问题的用户分配。 有关更多信息，请参阅 [在“编辑任务”或“编辑问题”框中设置的分配与在“计划”区域中设置的分配](#allocations-set-on-the-edit-task-or-the-edit-issue-boxes-vs-in-the-scheduling-areas).

默认情况下，用户会平均分配到任务或分配给任务，或分配给任务或分配给任务的时间，或分配给分配给任务的时间，如 [计划小时数的默认分配](#default-allocation-for-planned-hours).

要从计划时间轴修改任务或问题的用户分配，请执行以下操作：

1. 转到多个项目、单个项目或团队的计划时间轴：

   * **对于多个项目**:  单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **资源配置>工作负载平衡器**，然后选择 **计划** 中。
   * **对于单个项目**:转到项目，单击 **工作负载平衡器** ，然后选择 **计划** 从左上角的下拉菜单中。
   * **对于团队**:单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **团队**，选择团队，单击&#x200B;**工作负载平衡器** 在左侧面板中，选择&#x200B;**计划** 从左上角的下拉菜单中。

   ![scheduling_contours.png](assets/scheduling-contours-350x139.png)

1. 确保在计划时间轴上启用用户分配，如 [启用用户分配](#enable-user-allocations) 章节。
1. 展开要管理用户分配的任务。\
   默认情况下，计划小时数在分配的用户和任务持续时间的天数之间平均分配。 周末（星期六和星期日）不增加小时数。 有关更多信息，请参阅 [计划小时数的默认分配](#default-allocation-for-planned-hours) 章节。

1. 单击要在给定日期调整其小时数的用户的字段。

   >[!NOTE]
   >
   >要在修改小时后维护原始分发，请单击 **取消**.

1. 指定调整后的小时数。
1. 单击&#x200B;**保存**。\
   仅当任务的总小时数等于原始计划小时数时，才能保存更改。 此数字显示在 **计划小时数** 字段。 当总数不等于总计划小时数时，该数字以红色显示。\
   ![resource_allocation_expanded_modified_png](assets/resource-allocation-expanded-modified-350x226.png)

## 重置用户分配的标准

Workfront会重置当任务或项目发生大量操作时，您在计划时间轴中手动编辑的用户分配。 通常，如果任务和问题的计划小时数在此过程中发生更改，则Workfront会在重新计算项目时间表的任何时候重置用户分配。\
有关重新计算项目时间表的详细信息，请参阅 [重新计算项目时间表](../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

在计划时间轴中，一些最常见的可能重置用户分配的标准包括：

* 将任务添加到迭代。\
   由于迭代具有固定日期，因此将重新计算任务和分配的日期。\
   有关迭代如何影响任务日期的信息，请参阅 [将文章添加到现有小版本](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

* 将任务的持续时间类型更改为“工作驱动”。
* 将任务的持续时间类型更改为在分配了1人以上时的“计算分配”。\
   有关任务持续时间的信息，请参阅 [任务持续时间和持续时间类型概述](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* 更改项目计划起始日期和计划完成日期。\
   有关项目计划日期的信息，请参阅 [项目计划开始日期概览](../../manage-work/projects/planning-a-project/project-planned-start-date.md) 和 [设置项目计划完成日期](../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

   有关任务计划完成日期的信息，请参阅 [任务计划完成日期概览](../../manage-work/tasks/task-information/task-planned-completion-date.md).

* 如果“任务约束”是灵活约束，则更改前置任务的日期。\
   例如，尽快或尽快。\
   有关任务约束的信息，请参阅 [任务约束概述](../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* 更改任务或问题的计划小时数。

   有关Workfront中的计划时数的信息，请参阅 [计划时数概述](../../manage-work/tasks/task-information/planned-hours.md).
