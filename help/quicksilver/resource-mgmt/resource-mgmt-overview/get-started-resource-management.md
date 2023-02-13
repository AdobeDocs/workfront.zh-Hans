---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: 资源管理入门
description: Oracle Resource Management允许您配置系统，以根据资源的可用性准确预测资源的使用情况，以便必须按时按预算完成工作。
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 0%

---

# 资源管理入门

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

Oracle Resource Management允许您配置系统，以根据资源的可用性准确预测资源的使用情况，以便必须按时按预算完成工作。

## Adobe Workfront中的资源管理概述

资源管理是指由Adobe Workfront管理员、资源管理器和项目所有者执行的所有活动，以规划（资源或方案规划）和计划（工作负载平衡器）组织的资源，并将其分配给需要完成的工作，同时考虑其可用性。 此外，资源管理还指在报表视图（利用率报表）中查看有关计划和实际资源分配的信息。

Workfront有几套用于管理资源的工具。 每个工具都有一个单独的范围。 目前，您可以在Workfront中使用以下资源管理工具，具体取决于您处于的资源管理阶段：

* 要在项目实际工作开始之前计划如何在更高级别分配资源，请使用以下工具：

   * **资源计划员**:您可以在资源管理的第一阶段使用资源计划员，根据资源的计划可用性来预算项目时间。 在资源规划阶段，您可以组织资源池中的用户，并将多个资源池分配给一个项目。

      有关资源计划的详细信息，请参阅 [Adobe Workfront资源规划](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **方案计划员**:这是一个更高级别的资源规划，允许您跨多个计划管理资源，这些计划可跨一年、三年或五年计划，并包括多个项目。 您可以使用最佳方案充分利用其可用性和预算。

      除了Workfront许可证外，方案规划器还需要单独的许可证。 有关Workfront方案规划器的信息，请参阅 [方案计划员概述](../../scenario-planner/scenario-planner-overview.md).

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* 要计划资源或将资源分配给实际工作（任务和问题），请使用以下工具：

   * **工作负载平衡器**:这属于资源管理的较低级别阶段，在该阶段中，您可以根据完成资源所需的小时数及其可用性，将资源分配给必须完成的实际工作（任务和问题）。 使用工作负载平衡器，您可以将用户分配给当前未分配或分配给作业角色的实际工作。

      有关Workfront平衡器的信息，请参阅 [工作负载平衡器](../../resource-mgmt/workload-balancer/workload-balancer.md).

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
* 要分析跨多个项目的预算分配、计划分配分配和实际分配，请使用以下工具：

   * **利用率报表**:使用此报表可以查看项目资源的使用情况。 您可以比较项目的预算、计划和实际分配及其对项目成本和收入的影响。

      有关“利用率报表”的信息，请参阅 [查看资源利用信息](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## 资源管理流程的组成部分

>[!NOTE]
>
>在Workfront，资源管理从来不是一个停滞的过程。 随着项目计划、用户可用性或角色的更改，您必须持续调整有关资源、其分配以及对项目、任务和问题的分配的信息。

在Workfront管理资源的过程包括以下阶段：

* **配置**:作为系统管理员、资源管理器或项目所有者，您必须先在Workfront实例中配置某些字段和对象，然后才能管理资源。 有关在Workfront中开始管理资源所需先决条件的更多信息，请参阅 [准确资源管理的先决条件](#prerequisites-for-accurate-resource-management) 章节。\
   除了在Workfront中包含具有工作项的项目之外，您还必须配置以下项目：

   * 用户\
      有关创建用户的更多信息，请参阅文章 [添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * 职位角色\
      有关创建作业角色的更多信息，请参阅文章 [创建和管理作业角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * 计划\
      有关创建计划的详细信息，请参阅文章 [创建计划](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * 项目首选项

      >[!TIP]
      >
      >只有系统或组管理员才能修改系统或组的项目首选项。

      有关定义项目首选项的详细信息，请参阅文章 [配置系统范围的项目首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * 资源池

      有关创建资源池的详细信息，请参阅 [创建资源池](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * 资源管理首选项

      作为系统，您必须决定Workfront如何在系统级别计算用户可用性，无论是使用用户的计划还是系统的默认计划。

      有关更多信息，请参阅 [配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **资源分配**:作为资源管理者或项目所有者，您可以为项目定义资源分配并分配工作。 对于此步骤，您可以使用资源计划器或方案计划器管理资源分配的估计值，并在负载平衡器中将实际工作分配给用户。

   有关资源规划和分配工作的详细信息，请参阅以下章节：

   * [Adobe Workfront资源规划](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Adobe Workfront方案规划器](../../scenario-planner/scenario-planning.md)
   * [工作负载平衡器](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Overview of the Workload Balancer](../workload-balancer/overview-workload-balancer.md). 
-->

* **分析**:作为资源经理、项目责任人或人员经理，请复查“利用率报表”，以了解资源的预算分配和计划分配与实际分配的比较情况。 按小时、成本或收入查看信息。 有关“利用率”报表的信息，请参阅 [查看资源利用信息](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## 使用Workfront中的资源管理工具查看和管理资源所需的访问权限

以下用户有权访问Workfront中的资源管理工具：

您必须是以下用户之一，并且拥有以下访问资源管理工具的访问权限和权限：

* 系统管理员。
* 具有计划许可证的用户。

   具有工作许可证的用户可以使用项目的负载平衡器并管理分配和分配。

   除了拥有作品或更高许可证之外，您还必须具备以下条件才能使用特定的资源管理工具：

   * 编辑对资源管理的访问（在工作负载平衡器中进行分配时不需要）
   * 编辑对财务数据的访问权限，以在资源计划器中显示成本信息
   * 查看对财务数据的访问权限，以在利用率报表中查看成本和收入信息（仅限具有计划许可证的用户）

* 对要管理资源的项目包含“进行分配”的参与或更高权限。

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

有关预算资源所需访问权限的信息，请参阅文章 [获得预算资源所需的访问权限](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

有关在工作负载平衡器中管理资源所需的访问权限的信息，请参阅 [在工作负载平衡器中管理资源所需的访问权限](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## 准确资源管理的先决条件  {#prerequisites-for-accurate-resource-management}

您必须满足一组要求，然后才能高效使用Workfront中的资源管理工具。

有关Workfront中每个资源管理工具的要求信息，请参阅以下内容：

* 文章中的“在资源规划器中工作的先决条件”部分 [资源计划员概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

<!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* 文章中的“使用工作负载平衡器的最佳实践”部分 [工作负载平衡器概述](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [在Adobe Workfront获得预算资源所需的资源](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [在工作负载平衡器中管理资源所需的访问权限](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

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
