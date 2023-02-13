---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: 资源计划员概述
description: 您可以使用“资源计划员”估算和预算资源分配给分配给项目的分配情况，并预测其可用性以供将来工作使用。
author: Alina
feature: Resource Management
exl-id: 06cd2226-f94d-4b6a-8692-6d35210782f2
source-git-commit: ec49a7d3adeb24c1b8df0ff5fafe650d18d92280
workflow-type: tm+mt
source-wordcount: '2077'
ht-degree: 0%

---

# 资源计划员概述

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: this used to be the beginning of Planning in the Resource Planner - consider restructuring it further? Merging some of this information with information about Understanding Navigation in the RP?!)</p>
-->

您可以使用“资源计划员”估算和预算资源分配给分配给项目的分配情况，并预测其可用性以供将来工作使用。

有关Adobe Workfront中资源规划的一般概述，请参阅 [资源规划入门](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## 资源计划员概述

您可以使用资源计划器轻松了解用户和职务角色的可用性以及完成项目工作所需的计划时间。 然后，您可以根据用户的可用时间，决定如何在分配给他们的项目上分配用户及其工作角色。

>[!IMPORTANT]
>
>您不能使用资源计划员将实际工作（任务和问题）分配给用户。 您只能估计用户或作业角色完成项目所需的时间量，而不考虑它们被分配给的任务和问题。\
>要向用户分配实际工作，您必须使用工作负载平衡器。 有关工作负载平衡器的详细信息，请参阅 [工作负载平衡器概述](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

您可以使用三个单独的视图在资源计划器中查看信息。 您可以使用每个视图来实现以下目的之一：

* 对资源的时间或成本进行预算，以便使用“项目”和“角色”视图完成需要完成的工作。 这是资源计划员的主要用途。\
   有关资源计划员中预算的详细信息，请参阅文章 [使用“项目”和“职责”视图在资源计划员中预算资源](../resource-planning/budget-resources-project-role-views-resource-planner.md).

* 要使用“用户”视图查看以下信息，请执行以下操作：

   * 根据用户的日程安排，用户的可用性
   * 根据项目计划完成工作所需的计划时间。
   * 用户已登录实际工作项目的时间。

   有关在资源计划器中查看用户的可用小时数、计划小时数和实际小时数或FTE的详细信息，请参阅文章 [使用“用户”视图时，在资源计划器中查看可用、计划和实际工时或FTE](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md#using).

## 资源计划员注意事项

* 您可以对正在处理的项目进行优先排序，并根据其优先级对资源分配进行预算，以确保先将资源分配给最重要的项目。

   有关在资源计划器中对项目进行优先级排序的信息，请参阅 [在资源计划器中排定项目优先级](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* 您可以显示项目任务和问题中的小时数、FTE和成本信息。

   >[!NOTE]
   >
   >任务和问题不显示在资源计划器中。 但是，任务上资源分配中的小时数、FTE和成本信息将在资源计划器中显示为项目的总数。

* 从资源计划器中显示的项目中排除父任务中的小时、FTE和成本信息。 如果您要在资源计划器中管理这些资源的时间或成本，我们建议仅将资源分配给子任务。

   有关父任务的信息，请参阅以下文章：

   * [任务概述](../../manage-work/tasks/task-information/tasks-overview.md)
   * [创建子任务](../../manage-work/tasks/create-tasks/create-subtasks.md)

   >[!TIP]
   >
   >父任务显示子任务的总小时数和成本。 因此，从子任务和父任务中计数小时数、FTE和成本将计算这些金额两次。 这就是为什么从资源计划器中排除父任务信息的原因。

* 您不能在资源计划器中管理其任务或问题所在项目上的小组分配。
* 您可以使用“资源计划员”一次为多个项目预算资源，或使用“业务案例”的“资源预算”区域为单个项目预算资源。 您对一个项目进行预算的信息也会显示在资源计划器中。

   有关如何为单个项目预算资源的信息，请参阅文章 [业务案例中的预算资源](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   有关如何在资源计划器中为一次多个项目预算资源的信息，请参阅文章中的“资源计划器中的预算资源”部分 [使用“项目”和“职责”视图在资源计划员中预算资源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

## 在资源计划器中工作的先决条件 {#prerequisites-for-working-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(<b>THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!</b> - do NOT ADD the variable here, because it might break this link!)</p>
-->

要成功使用资源计划员对资源进行预算，您必须首先确保您、项目和任务满足一组先决条件。 在资源计划器中显示正确的信息和准确管理资源时，必须满足这些先决条件。

>[!IMPORTANT]
>
>如果缺少以下任何先决条件，您可能会发现有关资源分配或资源可用性的某些信息缺失或具有零值。\
>有关了解字段为何缺少数据或具有零值的更多信息，请将鼠标悬停在字段上。

![](assets/no-users-with-this-role-in-the-res-pool-350x57.png)

>[!NOTE]
>
>只有在按项目或职务职责查看资源计划员时，或在项目业务案例中对资源进行预算时，才需要满足以下先决条件。

在按项目或按职责查看资源计划员时，需要以下类型的先决条件才能使其正常运行：

* [用户先决条件](#user-prerequisites)
* [项目先决条件](#project-prerequisites)
* [任务和问题先决条件](#tasks-and-issues-prerequisites)
* [系统级别先决条件](#system-level-prerequisites)

### 用户先决条件 {#user-prerequisites}

在开始使用资源计划器之前，请确保存在以下用户设置：

* 您有权正确访问预算资源。

   有关预算资源所需访问权限的信息，请参阅文章 [在Adobe Workfront获得预算资源所需的资源](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* 分配给任务的用户将添加到与项目关联的资源池中。

   有关将用户添加到资源池的信息，请参阅 [将资源池与用户关联](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

   >[!NOTE]
   >
   >当用户未添加到资源池时，可能会存在以下情况：
   >
   >   
   >   
   >   * 虽然可能会将用户分配给项目上的任务，但用户不会显示在资源计划器中。
   >   * 如果与之关联的任务具有计划小时数，则这些小时数不会在“资源计划器”中为项目显示，除非用户也与这些任务上的任务职责相关联。
   >   * 如果用户与项目任务上的任务职责相关联，则“计划时数”将显示在任务职责的资源计划员中，但无法编入任务职责预算。


* 分配到工作池和资源池的用户必须具有与其配置文件关联的计划和作业角色。

   有关将计划和作业角色与用户关联的信息，请参阅 [编辑用户的配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   >[!NOTE]
   >
   >未与计划关联但位于项目资源池中的用户无法在资源计划器中预算。

* 要获取准确的可用小时数信息，请确保与用户关联的计划具有计划例外和更新时间。

   >[!NOTE]
   >
   >如果用户未与计划关联，则为了资源计划员的目的，Workfront系统的默认计划默认与用户关联。

   有关创建计划的信息，请参阅文章 [创建计划](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* 如果要按成本对资源进行预算，则必须将任务职责与成本/人力资源相关联。 比率。 与分配给资源池中用户的任务职责关联的成本用于计算项目的预算人工成本和预算成本。\
   有关将任务职责与费率关联的信息，请参阅文章 [创建和管理作业角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
   有关计算预算人工成本的信息，请参阅文章 [了解项目的预算人工成本和预算工时](../../manage-work/projects/project-finances/budgeted-labor-cost.md).\
   有关计算预算成本的信息，请参阅文章 [计算预算成本](../../manage-work/projects/project-finances/budgeted-cost.md).

### 项目先决条件 {#project-prerequisites}

在开始使用资源计划器之前，请确保存在以下项目设置：

* 您的项目与资源池相关联。\
   有关将资源池添加到项目的更多信息，请参阅 [将资源池与项目和模板关联](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md).

   >[!IMPORTANT]
   >
   >没有资源池的项目不会在资源计划器中显示计划小时或分配信息。

### 任务和问题先决条件 {#tasks-and-issues-prerequisites}

虽然您不能在资源计划器中显示任务和问题，但它们的信息会传输到在资源计划器中显示的项目。

在资源计划员中启动预算资源之前，请确保存在以下任务和发放设置：

* 您为其预算资源的项目的任务或问题会分配给以下实体之一：

   * 项目资源池中也与“作业角色”关联的用户
   * 职位角色

   >[!NOTE]
   >
   >分配给任务职责的计划工时和问题将显示在资源计划器中，但是这些工时不能编入预算，除非与任务职责关联的用户在与项目关联的资源池中列出。

* 您不应将父任务分配给用户或角色。

   要在资源计划员中显示与父任务关联的用户或角色的小时信息，您还必须将它们分配给子任务。 资源计划员不显示父任务中的信息。

* 任务和问题的“计划小时数”值大于零。
* 任务和问题的持续时间值大于零。
* 问题的计划日期在项目的时间线内。

### 系统级别先决条件 {#system-level-prerequisites}

您必须了解Workfront实例如何根据系统中的资源管理首选项计算用户可用性。 Workfront可以使用用户配置文件页面中定义的用户计划或系统的默认计划来计算用户可用性。

![](assets/resource-management-preferences-section-in-setup-350x89.png)

Workfront管理员配置您的资源管理首选项。

有关更多信息，请参阅 [配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## 查找资源计划员

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This became another standalone article; drfat this section here when article is live.)</p>
-->

您可以在Workfront的两个区域中找到资源计划器，具体取决于您是要为多个项目预算资源，还是只为一个项目预算资源。

有关查找资源计划员的信息，请参阅 [查找资源计划员](../../resource-mgmt/resource-planning/locate-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(this is drafted and moved to its own article: locate-resource-planner) </p>
<p>Ensure that all prerequisites are met before starting to use the Resource Planner. This way, you ensure that the Resource Planner displays the correct information before you start budgeting your resources.<br>For information about the prerequisites that must be met before you can start using the Resource Planner, see the <a href="#prerequisites-for-working-in-the-resource-planner" class="MCXref xref">Prerequisites for working in the Resource Planner</a> section in this article. </p>
<p>You can locate the Resource Planner in two areas of Workfront, depending on whether you want to budget your resources for multiple projects, or for just one project.</p>
<ul>
<li><a href="#use-the-resource-planner-for-multiple-projects" class="MCXref xref">Use the Resource Planner for multiple projects</a> </li>
<li> <p><a href="#use-the-resource-planner-for-one-project" class="MCXref xref">Use the Resource Planner for one project</a> </p> </li>
</ul>
<p><strong>Use the Resource Planner for multiple projects</strong></p>
<p>When using the Resource Planner for multiple projects, the allocation numbers for your resources represent numbers across multiple projects. </p>
<p>To access the  Planner section  in the  Resourcing area: </p>
<ol>
<li value="1">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.  </li>
<li value="2"> <p>  Click <strong>Resourcing</strong>. The Resource Planner displays by default.  For information about budgeting resources in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> <p> <img src="assets/qs-resource-management-area-with-planner-as-default-350x152.png" style="width: 350;height: 152;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">  Hover over the left panel, and click <strong>Resource Pools</strong>. <br>For information about creating new resource pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a>.</li>
</ol>
<p><strong>Use the Resource Planner for one project</strong></p>
<p>When using the Resource Planner for one project, the allocation numbers for your resources represent numbers for the selected project. </p>
<ol>
<li value="1"> <p>Go to a project you want to budget resources for.</p> </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Business Case</strong> in the left panel.</p> </li>
<li value="3"> <p>Scroll to the <strong>Resource Budgeting</strong> section of the Business Case.</p> </li>
<li value="4"> <p>Click <strong>Edit Resource Budgeting</strong> to add resource pools to your project and start budgeting your resources. </p> <note type="tip">
You can only add a resource pool in the Resource Budgeting area of the Business Case when the project has no resource pools associated with it. When the project already has a resource pool, the users in the pool and their job roles display in the Resource Budgeting area by default.
</note> <p> <img src="assets/resource-budgeting-area-on-project-350x70.png" style="width: 350;height: 70;"> </p> <p>For information about budgeting resources for one project, see the article <a href="../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md" class="MCXref xref">Budget resources in the Business Case</a>.</p> </li>
</ol>
</div>
-->

## 资源计划员的区域

您可以在资源计划员中查看以下信息或执行以下活动：

* 有关在一般时间轴中分配给资源计划器中项目的资源的信息。
* 在资源计划器中过度分配或资源利用率不足。
* 手动或自动对资源进行预算以使其正常工作。

有关资源计划器中显示哪些区域以及如何配置这些区域中显示哪些信息的详细信息，请参阅文章 [资源计划员导航概述](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## 在资源计划器中显示信息时的限制

为了提高性能，Workfront会限制您在资源计划器中显示的物料数量。

有关这些限制的更多信息，请参阅文章 [资源计划员显示限制](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md) .

## 在资源计划员中计算FTE

您可以在资源计划员中以小时、FTE或成本显示可用性、分配和计划值。

有关更改在资源计划器中显示的信息的详细信息，请参阅部分 [按小时、FTE或成本查看信息](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu) 在文章中 [使用Adobe Workfront资源计划员复查资源可用性和分配](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

有关如何在Workfront中计算用户和角色的小时数和FTE的更多信息，请参阅文章 [资源计划员中用户和角色的小时数和FTE计算概述](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## 在资源计划员中计算成本

您必须具有查看财务数据的访问权限和查看项目的财务权限，才能在资源计划器中按成本查看信息。

除了按小时和FTE在资源计划员中显示可用性、分配和计划值外，您还可以按成本显示它们。

>[!TIP]
>
>您必须将用户和职务职责与每小时成本费率关联，以便按成本在资源计划器中显示信息。

有关将每小时成本费率与任务职责关联的详细信息，请参阅文章 [创建和管理作业角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
有关将每小时成本费率与用户关联的详细信息，请参阅文章 [编辑用户的配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

在资源计划器中按成本查看信息时，请考虑以下事项：

* 每种类型小时（“已计划”、“可用”、“已预算”、“用户”、“角色”或“项目”的“实际”）的成本使用不同的成本率计算。
* 计划成本受项目任务的成本类型的影响。
* 在将“用户视图”应用到资源计划员时，您无法按成本显示分配和可用性信息。

有关如何在资源计划器中为用户和角色计算成本的详细信息，请参阅文章 [在资源计划器中计算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the User View to view Available, Planned, and Actual Hours or FTE </h2>
<p>(this information is repeated from above where it exists in shorter form. Drafted to simplify the amount of info of this article.) </p>
<p>You can use the User View of the Resource Planner to display information about the Planned, Available, and Actual Hours or FTE values for projects and resources. </p>
<p>For information about using the Resource Planner to review the Available, Planned, and Actual Hours and FTE for resources, see the article <a href="../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md" class="MCXref xref">View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view</a>.</p>
<p><strong>Use the Project and Role Views to budget resources </strong></p>
<p> The main function of the Resource Planner is to budget your resources for the work that needs to be completed on the projects that you can manage. </p>
<p> You can budget your resources only if you apply the <strong>View by Project</strong> or <strong>View by Role</strong> views to the Resource Planner.</p>
<p>For information about budgeting resources using the Project and Role views in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md"><a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a></a>.</p>
</div>
-->

## 在资源计划器中筛选信息

您可以通过创建过滤器来减少在资源计划器中显示的项目、角色或用户数。\
有关更多信息，请参阅文章 [在资源计划器中筛选信息](../../resource-mgmt/resource-planning/filter-resource-planner.md).
