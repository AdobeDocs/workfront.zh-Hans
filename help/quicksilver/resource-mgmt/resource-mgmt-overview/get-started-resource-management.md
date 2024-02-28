---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: 资源管理入门
description: 资源管理允许您配置系统，以便根据资源的可用性准确预测资源的使用情况，从而按时和按预算完成必须完成的工作。
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: c80d9b0b7eb2a638af9e0a11ca3038ed99ecf1ee
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 0%

---

# 资源管理入门

<!-- Audited: 12/2023 -->

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

资源管理允许您配置系统，以便根据资源的可用性准确预测资源的使用情况，从而按时和按预算完成必须完成的工作。

## Adobe Workfront中的资源管理概述

资源管理是指由Adobe Workfront管理员、资源经理和项目所有者执行的所有活动，这些活动用于计划（资源或方案计划）和计划（工作负载均衡器）组织的资源，并根据它们的可用性将其分配给需要完成的工作。 此外，资源管理还指在报表视图（“利用率”报表）中查看有关计划和实际资源分配的信息。

Workfront有几组用于管理资源的工具。 每个工具都有一个单独的范围。 目前，您可以在Workfront中使用以下资源管理工具，具体取决于您处于哪个资源管理阶段：

* 要在项目实际工作开始之前，计划如何在更高级别分配资源，请使用以下工具：

   * **资源规划者**：您可以使用资源管理第一阶段的资源规划者，根据资源的计划可用性来预算资源的项目时间。 在资源计划阶段，您可以在资源池中组织用户，并将多个资源池分配给一个项目。

     有关资源计划的详细信息，请参阅 [资源计划：文章索引](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **场景规划器**：这是一个更高级别的资源规划，可让您跨多个计划管理这些资源，这些计划可以跨一个、三个或五年计划并包含多个项目。 您可以使用最佳方案以充分利用其可用性和预算。

     除Workfront许可证外，Scenario Planner还需要一个单独的许可证。 有关Workfront Scenario Planner的信息，请参阅 [Scenario Planner概述](../../scenario-planner/scenario-planner-overview.md).

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* 要计划或分配资源给实际工作（任务和问题），请使用以下工具：

   * **工作负载均衡器**：这属于资源管理的较低级别阶段，您可以在该阶段根据完成资源所需的小时数和可用性将资源分配给资源必须完成的实际工作（任务和问题）。 使用工作负载均衡器，您可以将用户分配到当前未分配或分配给工作角色的实际工作。

     有关Workfront均衡器的信息，请参阅 [工作负载均衡器：文章索引](../../resource-mgmt/workload-balancer/workload-balancer.md).

<!--

  * **Scheduling** (deprecated <span class="preview">and removed from the Preview environment</span>): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This happens at a lower-level in the process of managing resources, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.  

     For more information about resource scheduling, see the section [Resource Scheduling](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

    >[!CAUTION]
    >
    >
    >We are no longer supporting the Resource Scheduling tools and they will be removed from Workfront in **January 2023**. We recommend that you use the Workload Balancer for scheduling your resources. 
    >
    >
    >* For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
    >
    >
    >* For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* 要分析多个项目中的预算、计划和实际分配，请使用以下工具：

   * **利用率报告**：使用此报告可以查看项目的资源利用率。 您可以比较项目的预算、计划和实际分配及其对项目成本和收入的影响。

     有关利用率报表的信息，请参阅 [查看资源利用率信息](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## 资源管理进程的组成部分

>[!NOTE]
>
>在Workfront中，资源管理绝不是停滞不前的过程。 随着项目的计划、用户的可用性或其角色的变化，您必须不断调整有关资源、其分配及其分配给项目、任务和问题的信息。

在Workfront中管理资源的过程包括以下阶段：

* **配置**：作为系统管理员、资源管理器或项目所有者，您必须在管理资源之前配置Workfront实例中的某些字段和对象。 有关开始在Workfront中管理资源所需的先决条件的更多信息，请参阅 [准确资源管理的先决条件](#prerequisites-for-accurate-resource-management) 部分。\
  除了具有包含工作项的项目外，还必须在Workfront中配置以下项：

   * 用户\
     有关创建用户的更多信息，请参阅文章 [添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * 职位角色\
     有关创建工作角色的更多信息，请参阅文章 [创建和管理职位角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * 计划\
     有关创建时间表的详细信息，请参阅文章 [创建计划](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * 项目首选项

     >[!TIP]
     >
     >只有系统或组管理员才能修改系统或组的项目首选项。

     有关定义项目首选项的更多信息，请参阅文章 [配置系统范围的项目首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * 资源池

     有关创建资源池的详细信息，请参见 [创建资源池](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * 资源管理首选项

     作为系统，您必须决定Workfront如何计算系统级别的用户可用性，无论使用用户计划还是系统的默认计划。

     有关更多信息，请参阅 [配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **资源分配**：作为资源管理器或项目所有者，您可以为项目定义资源分配并分配工作。 对于此步骤，您可以使用资源规划者或场景规划者管理资源的估计分配，并在工作负载均衡器中将实际工作分配给用户。

  有关资源规划和分配工作的详细信息，请参阅以下部分：

   * [资源计划：文章索引](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Adobe Workfront Scenario Planner](../../scenario-planner/scenario-planning.md)
   * [工作负载均衡器：文章索引](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Workload Balancer overview](../workload-balancer/overview-workload-balancer.md). 
-->

* **分析**：作为资源经理、项目所有者或人员经理，查看利用率报告，了解资源的预算和计划分配与实际分配的对比情况。 按小时、成本或收入查看信息。 有关“利用率”报告的信息，请参阅 [查看资源利用率信息](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## 使用Workfront中的资源管理工具查看和管理资源所需的访问权限

以下用户有权访问Workfront中的资源管理工具：

您必须是以下用户之一，并且具有以下访问和权限才能访问资源管理工具：

* 系统管理员。
* 具有Plan许可证的用户。

  具有工作许可证的用户可以使用项目的工作负载均衡器并管理分配和分配。

  除了拥有工作许可证或更高许可证之外，还必须具备以下内容才能使用特定的资源管理工具：

   * 编辑对资源管理的访问权限（在工作负载均衡器中进行分配时不需要）
   * 编辑对财务数据的访问权限以在资源规划者中显示成本信息
   * 查看对财务数据的访问以查看利用率报告中的成本和收入信息（仅限拥有计划许可证的用户）

* Contribute或更高权限，包括在要为其管理资源的项目上进行“工作总揽”。

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

有关预算资源所需访问权限的信息，请参阅文章 [预算资源所需的访问权限](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

有关管理工作负载均衡器中的资源所需访问的信息，请参见 [在工作负载均衡器中管理资源所需的访问权限](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## 准确资源管理的先决条件  {#prerequisites-for-accurate-resource-management}

您必须满足一系列要求，然后才能有效地使用Workfront中的资源管理工具。

有关Workfront中每个资源管理工具的要求的信息，请参阅以下内容：

* 部分 [在资源规划者中工作的先决条件](../../resource-mgmt/resource-planning/get-started-resource-planner.md#prerequisites-for-working-in-the-resource-planner) 在文章中 [资源规划者概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
  <!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* 部分 [使用工作负载均衡器的最佳实践](../../resource-mgmt/workload-balancer/overview-workload-balancer.md#best-practices-for-using-the-workload-balancer) 在文章中 [工作负载均衡器概述](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [在Adobe Workfront中预算资源所需的访问权限](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [在工作负载均衡器中管理资源所需的访问权限](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and replaced with the links to each prerequisites instead) </p>
<p> We recommend that the following settings exist before starting to manage resources for your organization: </p>
<ul>
<li> You must have users in the system who have active accounts. </li>
<li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
Although you can assign work to a Reviewer or a Requestor, they cannot complete it.
<br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in Workfront, see
<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>.
</note></li>
<li> You must have job roles configured in the system.<br>For information about adding job roles to Workfront, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
<li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li>
<li> You must associate at least one job role with your users. </li>
<li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li>
<li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
<li>The Time Off calendar of the users must be up to date. </li>
<li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p>
<ul>
<li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates</a>.</p> </li>
</ul> </li>
<li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> </li>
<li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li>
<li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li>
</ul>
</div>
-->
