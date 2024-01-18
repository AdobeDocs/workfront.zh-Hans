---
content-type: release-notes
keywords: 注释，季度，更新，版本
navigation-topic: 2021-2-release-activity
title: 21.2资源管理增强功能
description: 本页介绍了21.2版本对“预览”环境所做的所有资源管理增强功能。 这些增强功能将在2021年5月10日这一周的“生产”环境中提供。 有关21.2版本中可用的所有更改列表，请参阅21.2版本概述。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 21.2资源管理增强功能

本页介绍了21.2版本对“预览”环境所做的所有资源管理增强功能。 这些增强功能将在2021年5月10日这一周的“生产”环境中提供。 有关21.2版本可用的所有更改列表，请参阅 [21.2发行版概述](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 工作负载均衡器中的月级别视图

为了帮助您在更长的时段内管理资源分配，我们现在为工作负载均衡器实施了月级别视图。 您一次最多可以查看三个月，并更新每月资源分配。 在此更改之前，您只能按天或按周查看工作负载均衡器。

有关信息，请参阅 [导航工作负载均衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 场景规划器、工作负载均衡器和任务列表之间的连接

>[!NOTE]
>
>仅在新的Adobe Workfront Experience中可用。

为了帮助您制定项目的战略计划并确保它们与Scenario Planner的全局计划相符，我们在项目上创建一个新区域，该区域显示计划的工作角色要求以及在项目工作项上估计的计划小时数。 此区域适用于项目级别的工作负载均衡器以及新Workfront Experience中的任务列表。 在经典体验中，这仅适用于项目工作负载均衡器。

有关信息，请参阅以下文章：

* [在项目和计划之间协调资源分配概述](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [导航工作负载均衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>这项新功能对所有用户均可见，无论是在新版还是旧版Workfront Experience中。 对于未购买Workfront Scenario Planner许可证的客户也可看到此视图。

## 在资源规划者中计算净值时使用计划小时数

资源规划程序中的新设置允许您在计算净值时使用已计划小时数。

在此增强功能之前，Workfront仅使用预算小时数计算净值。 净值显示可用小时数和预算或计划小时数、FTE或成本之间的差异。 在计算净值时，预算小时数仍然是默认设置。

有关信息，请参阅 [资源规划者的“项目”和“角色”视图中的小时数、FTE和成本信息概览](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## 工作负载均衡器中的12周查看

您现在可以在工作负载均衡器中查看长达12周的信息。 在此增强功能之前，您可以查看2、4和6周的信息。

有关查看工作负载均衡器的信息，请参见 [导航工作负载均衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)导航工作负载均衡器。

## 更改工作角色过滤器在工作负载均衡器的未分配区域中的工作方式

为了改进工作角色过滤器在工作负载均衡器中的工作方式并满足用户的期望，我们修改了未分配区域中的过滤器的功能。 您现在只能查看分配给您在筛选器中指定的工作角色的小时数。

在此增强功能之前，当将工作角色过滤器应用于未分配区域时，工作负载均衡器显示与分配给工作角色的工作项关联的所有小时数。

有关在工作负载均衡器中过滤信息的信息，请参见 [在工作负载均衡器中管理过滤器](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
