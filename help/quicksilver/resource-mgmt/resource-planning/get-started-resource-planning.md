---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: 资源规划入门
description: 您可以使用资源计划工具来管理您的工作角色、工作角色的可用性以及基于此可用性的项目常规分配。
author: Lisa
feature: Resource Management
exl-id: 0db9fbb3-4e94-47bd-b272-00b3ca4decaf
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# 资源规划入门

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(**** THIS WILL BE LINKED TO THE PRODUCT UI IN THE PLANNER AREA***DO NOT DELETE OR CHANGE URL FOR THIS ARTICLE****) </p>
<p>(Alina ***Keep the pink blurb for all articles in this NEW section.***More prerequisites for Users (with later releases): - users have an accurate number for their FTE field; The Prerequisites section: (this is linked to other articles, do not change name and link/ anchor))</p>
</div>
-->

您可以使用Adobe Workfront资源管理工具来预测资源的分配，以便准确了解项目是否按时、按预算交付。 有关Workfront中资源管理的概述，请参阅[资源管理入门](../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)。

您可以使用资源计划工具来管理您的工作角色、工作角色的可用性以及基于此可用性的项目常规分配。

预算用户对项目的一般分配不会为他们分配实际工作（任务和问题）。 您必须使用工作负载均衡器分配要使用的资源。

有关使用工作负载均衡器在Workfront中计划资源的更多信息，请参阅[工作负载均衡器概述](../workload-balancer/overview-workload-balancer.md)。

## Workfront中的资源规划工具

要为计划分配项目的资源预算时间，您可以使用以下工具：

* 要编制系统层多个项目的分配预算并设置其优先级：请使用系统层资源规划者。

  您可以通过转到资源区域中的Planner部分来访问资源规划者。

  有关资源规划者的信息，请参阅[资源规划者概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

* 对于单个项目的预算分配：在项目的业务案例的资源预算区域中使用项目层资源规划者。 有关为一个项目预算资源的信息，请参阅文章[商业案例中的预算资源](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

  要根据通用技能或部门结构管理用户并将他们组织到池中，然后管理他们分配给项目的分配，您必须创建资源池。 有关创建资源池的详细信息，请参阅[创建资源池](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)。

  >[!TIP]
  >
  >项目的资源预算区域是项目层的资源规划者。 在项目的业务案例中预算资源时，该信息也会反映在系统级别资源规划者中。

* 要在高级别跨多个计划管理资源，并使您的工作与贵组织的战略保持一致，请使用Adobe Workfront Scenario Planner。 Scenario Planner需要额外的许可证。 有关Workfront Scenario Planner的信息，请参阅[Scenario Planner概述](../../scenario-planner/scenario-planner-overview.md)。

  您可以在系统层、多个项目中使用资源规划者，也可以在业务案例的资源预算区域中为单个项目预算资源。 有关业务案例中项目预算资源的详细信息，请参阅业务案例中的[预算资源](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

## 资源规划工具的用途

* 使用资源计划程序，您可以执行以下操作：

   * 排定项目的优先级，以决定哪些项目应首先接收资源。 （仅在资源规划者中）
   * 根据用户计划了解资源的可用性。
   * 为资源（用户和职位角色）分配项目的预算小时、FTE或成本分配。

  有关使用资源规划者的信息，请参阅文章[资源规划者概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

* 使用Scenario Planner，您可以跨多个计划构建企业级计划，这些计划概述公司的总体战略成果。 有关详细信息，请参阅[Scenario Planner入门](../../scenario-planner/get-started-with-scenario-planning.md)。

  Scenario Planner需要额外的许可证。 有关Workfront Scenario Planner的信息，请参阅[Scenario Planner概述](../../scenario-planner/scenario-planner-overview.md)。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Prerequisites for resource planning</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This section drafted because it was moved to the "Resource Planner overview" article instead. But this used to be true: THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To successfully use the Resource Planner for budgeting your resources, you must first ensure that you, your projects, and your tasks meet a set of prerequisites. These prerequisites are mandatory to display the correct information in the Resource Planner and to accurately manage your resources. </p>
-->

<!--
<note type="important">  If any of the following prerequisites are missing, you might find that some of the information about the allocation or the availability of the resources is missing or has a zero value.
<br>For more information understanding why fields are missing data or have zero values, hover over the fields.
</note>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no-users-with-this-role-in-the-res-pool-350x57.png" style="width: 350;height: 57;"> </p>
-->

<!--
<note type="note">
The following prerequisites are required only when viewing the Resource Planner by project or by job role or when budgeting resources in the Business Case of a project.
<br>For more information about the views in the Resource Planner, see the "Project/ Role/ User view" selection section in the article
<a href="../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.
<br>
</note>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following types of prerequisites are required for the correct functionality of the Resource Planner: </p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user-prerequisites" class="MCXref xref">User prerequisites</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#project-prerequisites" class="MCXref xref">Project prerequisites</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#tasks-and-issues-prerequisites" class="MCXref xref">Tasks and issues prerequisites</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user-prerequisites">User prerequisites</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Ensure the following user setup exists before starting using the Resource Planner:</p>
<li>  <ul>   <li> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have the correct access to budget resources.</p><p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p>   </li>  </ul> </li>
-->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Users who are assigned to tasks are added to the Resource Pools associated with the project.</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about adding users to Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associate resource pools with users </a> and <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a>.</p>
  -->

<!--
  >[!NOTE]
  >
  >
  >
  ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">When users are not added to Resource Pools, the following scenarios may exist: </p>  >
  >
  >
  >   
  >   
  >   
  >     <li style="font-style: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">The users do not appear in the Resource Planner although they might be assigned to tasks on the projects. </li>  >   
  >     <li style="font-style: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">If the tasks they are associated with have Planned Hours, those hours do not appear for the project in the Resource Planner, unless the user is also associated with a job role on those tasks. </li>  >   
  >     <li style="font-style: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">If the users are associated with a job role on a task on the project, the Planned Hours display in the Resource Planner for the job role, but the job role cannot be budgeted. </li>  >
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Users who are assigned to work and Resource Pools must have Schedules and Job Roles associated with their profile.</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about associating Schedules and Job Roles with users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a></p>
  -->

<!--
  <note type="note">  Users who are not associated with a Schedule but are in the Resource Pool of the project cannot be budgeted in the Resource Planner.
  </note>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For accurate Available Hours information, ensure that the schedules associated with your users have the schedule exceptions and time off updated.</p>
  -->

<!--
  <note type="note">  If a user is not associated with a Schedule, the Default Schedule of your Workfront system is associated with the user by default, for the purposes of the Resource Planner.
  </note>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about creating schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.<br></p>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to budget your resources by Cost, you must associate Job Roles with Cost/Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.<br>For information about associating job roles with rates, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.<br>For information about calculating Budgeted Labor Cost, see the article <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>.<br>For information about calculating Budgeted Cost, see the article <a href="../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calculate Budgeted Cost</a>.</li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="project-prerequisites">Project prerequisites</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Ensure the following project setup exists before starting using the Resource Planner:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> Your projects are associated with Resource Pools.<br>For more information about adding Resource Pools to projects, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref">Associate resource pools with projects and templates</a>.<br>
  <note type="important">  Projects without Resource Pools do not display Planned Hour or assignments information in the Resource Planner.
  </note>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have the correct access to budget resources.</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="tasks-and-issues-prerequisites">Tasks and issues prerequisites</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Ensure the following tasks and issues setup exists before starting budgeting resources in the Resource Planner:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> The tasks or issues on the projects for which you are budgeting resources are assigned to one of these entities:<br>
  <ul>
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Users in the Resource Pools of the project who are also associated with Job Roles</li>
  <li>
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Job Roles</p>
  </li>  
  </ul>
  <note type="note">
  Teams assigned to tasks or issues do not display in the Resource Planner. The Planned Hours of tasks and issues assigned to job roles display in the Resource Planner, but these hours cannot be budgeted unless a user who is associated with the job role is listed in a Resource Pool associated with the project.
  </note>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Parent tasks should not be assigned to users or roles. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This will impact the value of Planned Hours for the project. </p>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Tasks and issues have a value for Planned Hours which is greater than zero. </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Tasks and issues have a value for their Duration which is greater than zero. </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Planned Dates of the issues are within the timeline of the project. </li>
  -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Access resource planning tools in&nbsp;Workfront</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can access the Planner from the  People Planner section  of the Resourcing area. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about accessing the Planner, see <a href="../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Create Resource Pools</h2>
<p>(drafted because it's redundant with the user prerequisites above) </p>
<p>You can manage your user resources by adding users to Resource Pools. Having users organized in Resource Pools and associating the pools with your projects are prerequisites to Resource Planning.</p>
<p>For information about adding users to Resource Pools and associating them with projects, see <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a> and <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associate resource pools with users </a>.</p>
</div>
-->
