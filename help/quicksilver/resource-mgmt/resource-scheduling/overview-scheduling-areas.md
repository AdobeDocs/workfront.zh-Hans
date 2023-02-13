---
content-type: overview
product-area: resource-management
navigation-topic: resource-scheduling
title: 计划区域概述
description: 以下各节介绍您在Adobe Workfront中访问计划区域的位置以及计划区域中提供的功能。
author: Alina
feature: Resource Management
exl-id: ed6f1db9-917d-4a19-9fd4-1ed5d2ca95fb
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1790'
ht-degree: 0%

---

# 计划区域概述

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 

-->


以下各节介绍您在Adobe Workfront中访问计划区域的位置以及计划区域中提供的功能。

## Workfront区域，用于计划资源

您可以在Workfront的以下区域计划资源：

* **对于您是其资源经理的任何项目** (从 **计划** 区域)Workfront中的“计划”区域使资源管理者能够跨多个项目进行资源分配。

* **当您是项目团队的成员时，用于单个项目** (从 **计划** 项目区域):

   项目中的“计划”区域允许项目团队成员将项目中的工作分配给项目团队的用户。

* **对于单个团队，您是** (从 **计划** 部分)团队中的计划部分允许团队成员将已从多个项目分配给团队的工作分配给各个团队成员。

## “计划”区域中可用的功能

计划区域显示任务和问题以及当前资源分配。\
![resource_scheduling_overview.png](assets/resource-scheduling-overview-350x237.png)

* [过滤和交换工具](#filter-and-swap-tools)
* [日期选择](#date-selection)
* [未分配区域](#unassigned-area)
* [用户和角色](#users-and-roles)
* [计划时间表](#scheduling-timeline)

### 过滤和交换工具 {#filter-and-swap-tools}

* **过滤器工具：** 允许您过滤在计划时间轴上显示的内容。 有关使用过滤器工具的更多信息，请参阅 [在“计划”区域中筛选信息](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).
* **交换工具：** （仅当从“计划”选项卡或“人员配备”选项卡中为项目计划资源时可用）使您能够跨多个项目快速分配、交换或取消分配用户的任务。 有关更多信息，请参阅 [在“计划”区域中手动分配未分配的任务和问题](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### 日期选择 {#date-selection}

您可以调整在计划时间轴上显示数据的日期范围。 默认情况下，日期范围为从当天开始的2周（连续14天，包括周末）。

### 未分配区域 {#unassigned-area}

* [在将资源计划为资源管理器时（对于“计划”区域中的多个项目）](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [将资源安排为项目团队的成员（来自项目）时](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [将资源安排为团队成员（来自团队）时](#when-scheduling-resources-as-a-team-member-from-a-team)

#### 在将资源计划为资源管理器时（对于“计划”区域中的多个项目） {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area}

的 **未分配** 计划时间轴上的区域仅显示满足以下所有条件的任务和问题：

* 未分配给用户。
* 未分配给团队。\
   如果任务或问题已分配给团队，则它仍会显示在 **未分配** 区域。\
   如果任务或问题具有用户未完成的其他职务角色分配，则也会显示这些任务或问题。\
   例如，任务被分配给3个作业角色：设计人员、产品经理和开发人员。 您将此任务分配给具有设计人员作业角色的用户A和具有产品经理作业角色的用户B。 在此方案中，任务仍显示在计划时间轴上的“未分配”区域中，因为未将开发人员作业角色分配给用户。

#### 将资源安排为项目团队的成员（来自项目）时 {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project}

的 **未分配** 计划时间轴顶部的区域显示满足以下条件的任务和问题：

* 与项目关联，但未分配给项目团队中的任何用户。\
   与项目关联并分配给项目团队中用户的任务将显示在向其分配任务的用户行中。
* 与项目关联，但分配给不在项目团队中的成员。

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! Is it even possible to have the task assigned to a member who is not part of the project team? If so, then would this end up in the Unassigned area?])</p>
  -->

#### **将资源安排为团队成员（来自团队）时** {#when-scheduling-resources-as-a-team-member-from-a-team}

的 **未分配** 计划时间轴顶部的区域显示满足以下条件的任务和问题：

* 分配给团队和团队中没有其他用户。\
   分配给团队和团队中用户的任务都会显示在分配给这些任务的用户的行中。
* 同时分配给团队和不是团队成员的用户。

### 用户和角色 {#users-and-roles}

* [在将资源计划为资源管理器时（对于“计划”区域中的多个项目）](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [将资源安排为项目团队的成员（来自项目）时](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [将资源安排为团队成员（来自团队）时](#when-scheduling-resources-as-a-team-member-from-a-team)

#### 在将资源计划为资源管理器时（对于“计划”区域中的多个项目） {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area-1}

任何有资格被分配其中一项未分配任务的用户都位于 **未分配** 的上界。 在以下情况下，可在计划时间表上为用户分配任务或问题：

* 默认情况下，仅当用户在系统中定义了作业角色（主作业角色或辅助作业角色），并且该作业角色与分配给当前在 **未分配** 的上方。 您可以禁用此功能，以便允许将任务和问题分配给任何用户，而不管该用户在其用户配置文件中定义的角色是否与分配给他们的任务或问题的角色分配相匹配。 有关更多信息，请参阅 [在“计划”区域中，不考虑角色和组成员资格，允许用户分配](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md).\
   如果用户在Workfront系统中指定了多个作业角色，则用户和用户分配的任务可能会在计划时间线上多次显示。\
   在为用户分配任务或问题后，即使没有具有匹配角色分配的剩余任务或问题，用户仍会停留在计划时间线上。 这允许您在分配后进行任何必要的更改。\
   如果未将任务分配给作业角色，则会显示符合筛选要求的所有用户。 有关过滤器的更多信息，请参阅 [在“计划”区域中筛选信息](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

* 它们已在 **用户** 字段 **过滤器** 选项卡。\
   有关过滤器的更多信息，请参阅 [在“计划”区域中筛选信息](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).\
   在计划团队的资源时(在“工作方式”(Working On)选项卡上)，还会显示团队分配。

分配给这些用户的任何其他任务或问题也会显示在时间轴上。

您可以查看在给定日期为用户分配的级别，如 [在“计划”区域中管理用户分配](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). 您至少没有Contribute权限的任务在计划时间轴上显示为灰色条。

#### 将资源安排为项目团队的成员（来自项目）时 {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project-1}

无论用户的作业角色分配和“未分配”区域中任务的角色分配如何，团队的每个成员始终都会显示在计划时间轴上。

如果用户在系统中定义了多个作业角色，则当满足以下任一条件时，该用户会在计划时间线上多次显示：

* 在 **未分配** 分配给与用户关联的作业角色的区域。
* 项目中有已分配作业角色的任务或问题，并且这些任务或问题被分配给在系统中定义了该作业角色的用户。

#### 将资源安排为团队成员（来自团队）时 {#when-scheduling-resources-as-a-team-member-from-a-team-1}

无论用户的作业角色分配和“未分配”区域中任务的角色分配如何，团队的每个成员始终都会显示在计划时间轴上。

您可以查看在给定日期为用户分配的级别，如 [在“计划”区域中管理用户分配](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). 您至少没有Contribute权限的任务，可在计划时间轴上显示为灰色条。

### 计划时间表 {#scheduling-timeline}

* **默认内容：** 默认情况下，所有满足部分中定义要求的任务 [任务和问题先决条件](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#task-and-issue-prerequisites) 在 [资源计划入门](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md) 所有状态为“当前”的项目的文章都会显示在计划时间线上。

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: [! true for teams? - Yes, but really we're focusing on tasks, and the team assignment.])
  </MadCap:conditionalText>
  -->

   要自定义计划时间轴上显示的内容（包括显示问题和具有不同状态的项目），请使用过滤器，如 [在“计划”区域中筛选信息](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

   给定用户每天最多显示10个任务。 您可以展开列表以查看当前分配给该用户的所有任务。

* **父任务：** 是否在时间轴上显示父任务取决于多个设置。 有关更多信息，请参阅 [在“计划”区域中配置设置](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) 文章。

* **颜色编码：** 计划时间轴上的任务和问题会根据其所属的项目进行颜色编码。 您无法自定义与特定项目关联的颜色。

   在计划团队工作时（从“人员配备”选项卡），仅当 **显示所有用户任务** 选项。 有关更多信息，请参阅 [在“计划”区域中配置设置](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) 文章。

* **任务持续时间：** 任务持续时间在每个任务的时间轴上表示（任务的实际跨越天数等于持续时间）。 您无法从计划时间轴调整任务持续时间。

* **结束时间：** 结束时间在计划时间线上由列中的浅灰色指示器表示，该指示器是为给定用户计划结束时间的当天。\
   将根据以下信息为每个用户配置休息时间：

   用户的个人休息日历。 有关个人休假日历的更多信息，请参阅 [在Adobe Workfront中配置个人休息时间](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

   分配给用户的计划。 这可能是默认计划或自定义计划。 有关计划的详细信息，请参阅 [创建计划](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **周末：** 周末在计划时间表中以星期六和星期日的浅灰色阴影表示。 在计划时间轴上设置为周末的一周中的天数是不可配置的。 您可以安排用户在周末工作。
