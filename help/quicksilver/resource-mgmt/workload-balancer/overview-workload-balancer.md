---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: 工作负载均衡器概述
description: 项目经理通过创建任务来计划项目工作之后，以及资源经理将工作角色资源分配给资源规划者中的项目之后，项目所有者和团队经理可以使用工作负载均衡器将工作项分配给用户。
author: Lisa
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 0%

---

# 工作负载均衡器概述

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

项目经理通过创建任务来计划项目工作之后，以及资源经理将工作角色资源分配给资源规划者中的项目之后，项目所有者和团队经理可以使用工作负载均衡器将工作项分配给用户。

>[!IMPORTANT]
>
>您可以使用工作负载均衡器将实际工作（任务和问题）分配给用户。
>
>您必须使用资源规划者而不是工作负载均衡器来在高级别估计项目的工作角色分配。 有关资源规划者的详细信息，请参阅 [资源规划者概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

本文介绍了工作负载均衡器的常规用途以及如何设置项目和资源以成功使用它的一些最佳实践。

要查看工作负载均衡器的视频教程，请转到 [WorkfrontTutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html) 页面。 在左侧菜单中，选择 **管理资源** > **工作负载均衡器** 并选择教程。

## 找到工作负载均衡器

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

我们建议在以下区域使用工作负载均衡器来计划资源：

* 在系统级别，在“资源”区域。
* 在项目级别的项目的工作负载均衡器部分。
* 在团队级别，在团队的工作负载均衡器部分。

有关定位工作负载均衡器的更多信息，请参阅 [找到工作负载均衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## 工作负载均衡器的好处

使用工作负载均衡器时请考虑以下优势：

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* 获取对所有利益相关者都透明的资源过度分配和利用率不足的清晰直观映射。
* 作为人员经理，您可以保护人员免于倦怠，并使他们能够通过提高专注、质量和参与度来做好他们的最佳工作。 您可以确保它们的充分利用、打破各自为政的局面，并实现跨团队工作的一致性。
* 在任务或问题级别分配工作时，您不会了解用户可能有多忙。 使用工作负载均衡器时，您可以查看哪些用户在其工作负载中具有可用性，以按时完成任务或问题。 这包括他们的休息时间和计划例外详细信息。

  有关更多信息，请参阅 [在工作负载均衡器中分配工作概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

  您还可以批量分配工作项，这样更容易同时跨多个项目分配多个工作项。 有关更多信息，请参阅 [使用工作负载均衡器批量分配工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* 执行官可以通过透明地了解组织内部人员的利用情况，及时作出人员配置决定。
* 团队成员从更好的协作中获益，因为他们都可以随时查看同事正在做什么。 有关在工作负载均衡器中查看或管理资源所需访问的信息，请参见 [在工作负载均衡器中管理资源所需的访问权限](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* 通过在自定义选项卡中嵌入指向资源区域的链接，可与无权访问资源区域的任何人共享。 有关信息，请参阅 [使用链接共享工作负载均衡器](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)
* 在全球、项目或团队级别以一个视图可视化和管理人员的工作负载和需求，具体取决于您的角色。 在管理项目时，这不仅包括项目的资源分配，还包括从Adobe Workfront Scenario Planner可视化资源分配。 人员经理使用Workfront Scenario Planner管理整个组织的工作技能。 Scenario Planner仅在新的Adobe Workfront Experience中可用。

  >[!NOTE]
  >
  >  Scenario Planner需要额外的许可证。 有关Workfront Scenario Planner的信息，请参阅 [Scenario Planner概述](../../scenario-planner/scenario-planner-overview.md).


## 使用工作负载均衡器的最佳实践

我们建议在开始使用工作负载均衡器计划资源之前，采用以下最佳实践来规划项目、配置用户和使用过滤器。

* [在工作负载均衡器中显示信息的最佳实践](#best-practices-for-displaying-information-in-the-workload-balancer)
* [设置用户的最佳实践](#best-practices-for-setting-up-users)
* [设置任务和问题的最佳实践](#best-practices-for-setting-up-tasks-and-issues)

### 在工作负载均衡器中显示信息的最佳实践 {#best-practices-for-displaying-information-in-the-workload-balancer}

我们建议您使用过滤器，以便只显示与您相关的未分配工作项和已分配工作项的信息。

有关在工作负载均衡器中创建和使用过滤器的信息，请参见 [工作负载均衡器中的过滤器信息](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### 设置用户的最佳实践

* 作为为他人安排工作的用户，您必须具有安排工作资源的正确访问和权限。

  有关在工作负载均衡器管理资源的工作负载所需的访问权限的信息，请参阅 [在工作负载均衡器中管理资源所需的访问权限](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* 要管理其工作量的用户必须满足以下条件，以便有关其可用性和技能的信息准确无误：

   * 将时间表和职位角色与其配置文件关联。

     有关将时间表和工作角色与用户关联的详细信息，请参阅 [添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * 如果用户未与时间表关联，则出于资源管理目的，默认情况下Workfront系统的默认时间表与该用户关联。
   * 在其计划中更新计划例外。

     有关创建调度的详细信息，请参见 [创建计划](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * 在个人资料中更新其休息时间日历。

     有关更新用户休息时间日程表的信息，请参阅 [配置个人休息时间](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* Workfront管理员必须确定Workfront计算用户可用性的方式。 他们可以决定Workfront是使用系统默认计划，还是使用用户的计划通过调整Workfront设置区域中的资源管理首选项来计算用户可用的时间。

  有关更多信息，请参阅 [配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### 设置任务和问题的最佳实践 {#best-practices-for-setting-up-tasks-and-issues}

开始在工作负载均衡器中将工作分配给用户之前，确保存在以下任务和问题设置：

* 父级任务未分配给用户或角色。 父任务未显示在工作负载均衡器中。
* 任务和问题的规划小时数值大于零。

* 任务和问题的持续时间值大于零。
* 问题的计划日期在项目的时间表内。

## 开始使用工作负载均衡器之前

* 在开始使用工作负载均衡器之前，请查看以下文章：

   * 本文向您介绍如何导航工作负载均衡器以执行以下操作： [导航工作负载均衡器](../workload-balancer/navigate-the-workload-balancer.md).

   * 以下文章将指导您逐步了解如何分配工作和管理用户分配：

      * [在工作负载均衡器中分配工作概述](../workload-balancer/assign-work-in-workload-balancer.md).
      * [管理工作负载均衡器中的用户分配](../workload-balancer/manage-user-allocations-workload-balancer.md).

* 工作负载均衡器可以在Workfront的多个不同区域找到。 有关可在何处找到工作负载均衡器的信息，请参见 [找到工作负载均衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## 使用工作负载均衡器所需的访问权限

您必须对特定项目具有正确的Workfront访问权限和权限才能查看和使用Workfront中的工作负载均衡器。 有关使用工作负载均衡器所需访问的信息，请参阅文章 [在工作负载均衡器中管理资源所需的访问权限](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
