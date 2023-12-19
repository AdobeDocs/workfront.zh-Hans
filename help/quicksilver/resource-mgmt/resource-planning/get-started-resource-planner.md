---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: 资源规划者概述
description: 您可以使用资源计划程序来估计和预算分配给其所分配项目的资源，并预测其未来工作的可用性。
author: Alina
feature: Resource Management
exl-id: 06cd2226-f94d-4b6a-8692-6d35210782f2
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 0%

---

# 资源规划者概述

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: this used to be the beginning of Planning in the Resource Planner - consider restructuring it further? Merging some of this information with information about Understanding Navigation in the RP?!)</p>
-->

您可以使用资源计划程序来估计和预算分配给其所分配项目的资源，并预测其未来工作的可用性。

有关Adobe Workfront中资源规划的一般概述，请参阅文章 [资源规划入门](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## 资源规划者概述

您可以使用资源规划者轻松地了解用户和工作角色的可用性，以及完成项目工作所需的计划时间。 然后，您可以决定如何根据用户可用时间将用户及其工作角色分配给他们分配到的项目。

>[!IMPORTANT]
>
>您不能使用资源规划者将实际工作（任务和问题）分配给用户。 您只能估计用户或工作角色完成项目所需的时间，而不管他们被分配到什么任务和问题。\
>要将实际工作分配给用户，必须使用工作负载均衡器。 有关工作负载均衡器的详细信息，请参见 [工作负载均衡器概述](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

您可以使用三个不同的视图在资源规划程序中查看信息。 您可以使用每个视图来实现以下目的之一：

* 为需要使用“项目”和“角色”视图完成的工作预算您的资源时间或成本。 这是资源规划者的主要用途。\
  有关资源规划者中预算的更多信息，请参阅文章 [使用项目和角色视图的资源规划者中的预算资源](../resource-planning/budget-resources-project-role-views-resource-planner.md).

* 要使用“用户”视图查看以下信息，请执行以下操作：

   * 根据用户的计划提供的可用性
   * 根据项目计划完成工作所需的计划时间。
   * 用户已登录实际工作项的时间。

  有关查看资源规划者中用户的可用小时、计划小时数和实际小时数或FTE的更多信息，请参阅文章 [使用用户视图时查看资源规划者中的可用、计划和实际小时数或FTE](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md#using).

## 资源规划者注意事项

* 您可以优先处理正在处理的项目，并根据优先顺序来预算资源分配，以确保先将资源分配给最重要的项目。

  有关在资源规划程序中排列项目优先顺序的信息，请参阅 [在资源规划者中排定项目的优先级](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* 您可以显示来自项目任务和问题的小时、FTE和成本信息。

  >[!NOTE]
  >
  >任务和问题未显示在资源规划者中。 但是，任务上资源分配中的小时数、FTE和成本信息在资源规划程序中显示为项目的总数。

* 父任务的小时、FTE和成本信息从资源规划者中显示的项目中排除。 如果您想在资源规划者中管理这些资源的时间或成本，我们建议仅将资源分配给子任务。

  有关父任务的信息，请参阅以下文章：

   * [任务概述](../../manage-work/tasks/task-information/tasks-overview.md)
   * [创建子任务](../../manage-work/tasks/create-tasks/create-subtasks.md)

  >[!TIP]
  >
  >父任务显示子任务的总小时数和成本。 因此，计算子任务和父任务的小时数、FTE和成本将计算这些金额两次。 这就是从资源规划者中排除父任务信息的原因。

* 您无法在资源规划者中管理其具有任务或问题的项目上的团队分配。
* 您可以使用资源规划程序一次为多个项目预算资源，或使用业务案例的资源预算区域为单个项目预算资源。 您为一个项目编制预算的信息也会显示在资源规划者中。

  有关如何为单个项目预算资源的信息，请参阅文章 [业务案例中的预算资源](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

  有关如何一次在资源规划者中为多个项目预算资源的信息，请参阅文章中的“资源规划者中的预算资源”部分 [使用项目和角色视图的资源规划者中的预算资源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

## 在资源规划者中工作的先决条件 {#prerequisites-for-working-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(<b>THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!</b> - do NOT ADD the variable here, because it might break this link!)</p>
-->

要成功地使用资源规划者对资源进行预算，您必须首先确保您、您的项目和您的任务满足一组先决条件。 要在资源规划者中显示正确的信息并准确管理资源，必须满足这些先决条件。

>[!IMPORTANT]
>
>如果缺少以下任何先决条件，您可能会发现有关资源分配或可用性的某些信息缺失或具有零值。\
>有关了解字段为何缺少数据或值为零的详细信息，请将鼠标悬停在这些字段上。

![](assets/no-users-with-this-role-in-the-res-pool-350x57.png)

>[!NOTE]
>
>只有在按项目或按工作角色查看资源规划者或在项目的业务案例中预算资源时，才需要满足以下前提条件。

在按项目或按角色查看资源规划者时，需要以下类型的先决条件才能使其功能正确：

* [用户先决条件](#user-prerequisites)
* [项目先决条件](#project-prerequisites)
* [任务和问题先决条件](#tasks-and-issues-prerequisites)
* [系统级先决条件](#system-level-prerequisites)

### 用户先决条件 {#user-prerequisites}

在开始使用资源规划者之前，确保存在以下用户设置：

* 您对预算资源具有正确的访问权限。

  有关预算资源所需访问权限的信息，请参阅文章 [在Adobe Workfront中预算资源所需的访问权限](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* 分配给任务的用户将添加到与项目关联的资源池中。

  有关将用户添加到资源池的信息，请参见 [将资源池与用户关联](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

  >[!NOTE]
  >
  >当用户未添加到资源池时，可能会存在以下情况：
  >
  >   
  >   
  >   * 尽管这些用户可能被分配到项目中的任务，但他们未出现在资源规划者中。
  >   * 如果它们关联的任务具有计划小时数，则这些小时数不会显示在资源规划者中的项目上，除非用户还与这些任务上的工作角色关联。
  >   * 如果用户与项目上任务的工作角色关联，则计划小时数显示在工作角色的资源规划者中，但无法预算工作角色。
  >   
  >

* 分配到工作和资源池的用户必须具有与其配置文件关联的时间表和职位角色。

  有关将时间表和职位角色与用户关联的信息，请参见 [编辑用户配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >与计划无关联但位于项目的资源池中的用户无法在资源规划者中预算。

* 要获得准确的可用小时数信息，请确保与用户关联的计划已更新计划例外和空闲时间。

  >[!NOTE]
  >
  >对于资源规划者而言，如果用户未与计划关联，则默认情况下Workfront系统的默认计划与该用户关联。

  有关创建时间表的信息，请参阅文章 [创建计划](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* 如果要按“成本”预算资源，则必须将职务职责与成本/小时关联。 费率。 与分配给资源池中用户的工作角色关联的成本用于计算项目的预算劳力成本和预算成本。\
  有关将工作角色与费率关联的信息，请参阅文章 [创建和管理职位角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
  有关计算预算劳力成本的信息，请参阅文章 [了解项目的预算劳力成本和预算小时数](../../manage-work/projects/project-finances/budgeted-labor-cost.md).\
  有关计算预算成本的信息，请参阅文章 [计算预算成本](../../manage-work/projects/project-finances/budgeted-cost.md).

### 项目先决条件 {#project-prerequisites}

在开始使用资源规划者之前，确保存在以下项目设置：

* 您的项目与资源池相关联。\
  有关将资源池添加到项目的详细信息，请参阅 [将资源池与项目和模板关联](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md).

  >[!IMPORTANT]
  >
  >没有资源池的项目不会在资源规划者中显示计划小时数或工作分配信息。

### 任务和问题先决条件 {#tasks-and-issues-prerequisites}

虽然您不能在资源规划者中显示任务和问题，但其信息将转移到资源规划者中显示的项目。

在资源规划者中开始预算资源之前，确保存在以下任务和问题设置：

* 您正在为其编制预算资源的项目的任务或问题将分配给以下实体之一：

   * 项目资源池中与职位角色关联的用户
   * 职位角色

  >[!NOTE]
  >
  >分配给工作角色的任务和问题的已计划小时数显示在资源规划者中，但这些小时数无法进行预算，除非与工作角色关联的用户列在与项目关联的资源池中。

* 您不应将父任务分配给用户或角色。

  要在资源规划者中显示与父任务相关联的用户或角色的小时信息，还必须将他们分配给子任务。 资源规划者不显示父任务的信息。

* 任务和问题的规划小时数值大于零。
* 任务和问题的持续时间值大于零。
* 问题的计划日期在项目的时间表内。

### 系统级先决条件 {#system-level-prerequisites}

您必须了解Workfront实例如何根据系统中的资源管理首选项计算用户可用性。 Workfront可以使用用户时间表（如其“用户配置文件”页面中所定义）或系统的“默认时间表”来计算用户可用性。

![](assets/resource-management-preferences-section-in-setup-350x89.png)

Workfront管理员配置您的资源管理首选项。

有关更多信息，请参阅 [配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## 找到资源规划者

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This became another standalone article; drfat this section here when article is live.)</p>
-->

您可以在Workfront的两个区域中找到资源规划者，具体取决于您是要为多个项目还是仅为一个项目预算资源。

有关查找资源规划者的信息，请参见 [找到资源规划者](../../resource-mgmt/resource-planning/locate-resource-planner.md).

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

## 资源规划者的区域

您可以在资源计划程序中查看以下信息或执行以下操作：

* 有关在常规时间线的资源规划者中分配给项目的资源的信息。
* 资源规划者中的资源过度分配或利用率不足。
* 手动或自动为资源分配工作预算。

有关资源规划者中显示哪些区域以及如何配置这些区域中显示哪些信息的更多信息，请参阅文章 [资源规划者导航概述](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## 在资源规划者中显示信息时的限制

为了提高性能，Workfront会限制您可在资源规划者中显示的项目数量。

有关这些限制的更多信息，请参阅文章 [资源规划者显示限制](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md) .

## 在资源规划者中计算FTE

您可以在资源计划程序中按小时数、FTE或成本显示可用性、分配和计划值。

有关更改在资源规划者中显示的信息的信息，请参阅部分 [按小时、FTE或成本查看信息](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu) 在文章中 [使用Adobe Workfront资源规划者审查资源可用性和分配](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

有关如何在Workfront中计算用户和角色的小时数和FTE的更多信息，请参阅文章 [计算资源规划者中用户和角色的小时数和FTE的概述](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## 在资源规划者中计算成本

您必须具有项目上的“查看财务数据”和“查看财务”权限才能在资源规划者中按成本查看信息。

除了在资源计划员中显示小时数和FTE中的可用性、分配和计划值外，您还可以按成本显示它们。

>[!TIP]
>
>您必须将用户和职位角色与每小时成本费率相关联，以便在资源规划者中按成本显示信息。

有关将每小时成本费率与工作角色关联的更多信息，请参阅文章 [创建和管理职位角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
有关将每小时成本费率与用户关联的更多信息，请参阅文章 [编辑用户配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

在资源计划员中按成本查看信息时，请考虑以下事项：

* 每种小时类型（计划、可用、预算、用户、角色或项目的实际）的成本使用不同的成本费率计算。
* 计划成本受项目上任务的成本类型影响。
* 在将用户视图应用于资源计划员时，您不能按成本显示分配和可用性信息。

有关如何在“资源规划者”中为用户和角色计算成本的更多信息，请参阅文章 [在资源规划者中计算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

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

## 资源规划者中的筛选信息

您可以通过创建过滤器来减少资源规划者中显示的项目、角色或用户数量。\
有关更多信息，请参阅文章 [资源规划者中的筛选信息](../../resource-mgmt/resource-planning/filter-resource-planner.md).
