---
content-type: release-notes
keywords: 注释，季度，更新，发行
navigation-topic: 2021-2-release-activity
title: 21.2资源管理增强
description: 本页介绍了在“预览”环境中21.2版本中所做的所有资源管理增强。 这些增强功能将于2021年5月10日这一周的生产环境中提供。 有关21.2版本中可用的所有更改的列表，请参阅21.2版本概述。
author: Luke
feature: Product Announcements
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# 21.2资源管理增强

本页介绍了在“预览”环境中21.2版本中所做的所有资源管理增强。 这些增强功能将于2021年5月10日这一周的生产环境中提供。 有关21.2版本中可用的所有更改的列表，请参阅 [21.2版本概述](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 工作负载平衡器中的月级视图

为了帮助您管理较长时间的资源分配，我们现在为工作负载平衡器实施了月级视图。 您一次最多可以查看三个月并更新每月的资源分配。 在进行此更改之前，您只能按天或按周查看工作负载平衡器。

有关信息，请参阅 [导航工作负载平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 方案规划器、负载平衡器和任务列表之间的连接

>[!NOTE]
>
>仅在新的Adobe Workfront体验中可用。

为了帮助您对项目进行战略规划并确保这些计划与方案规划器的全局计划保持一致，我们在项目上创建了一个新区域，该区域显示了方案中的职务职责要求以及项目工作项上预计的计划时间。 此区域适用于项目级负载平衡器以及新Workfront体验中的任务列表。 在经典体验中，此功能仅适用于项目工作负载平衡器。

有关信息，请参阅以下文章：

* [协调项目和举措之间的资源分配的概述](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [导航工作负载平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>所有用户都可在新体验和经典Workfront体验中看到此新功能。 此外，对于尚未购买Workfront方案计划员许可证的客户，也可以查看此信息。

## 在资源计划员中计算净值时使用计划小时数

资源计划器中的新设置允许您在计算净值时使用计划小时数。

在此增强之前，Workfront仅使用预算小时数计算净值。 净值显示“可用”与“预算”或“计划小时数”、“FTE”或“成本”之间的差值。 在计算净值时，“预算小时数”仍是默认设置。

有关信息，请参阅 [资源计划员的“项目”和“职责”视图中的工时、FTE和成本信息概览](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## 工作负载平衡器中的12周视图

您现在可以在工作负载平衡器中查看长达12周的信息。 在进行此次增强之前，您可以查看2、4和6周的信息。

有关查看工作负载平衡器的信息，请参阅 [导航工作负载平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)导航工作负载平衡器。

## 在工作负载平衡器的“未分配”区域中更改作业角色筛选器的工作方式

为了改进工作负载平衡器中作业角色过滤器的工作方式并满足用户的期望，我们修改了“未分配”区域中过滤器的功能。 现在，您只能查看分配给您在筛选器中指定的作业角色的小时数。

在此增强之前，在将“作业角色”过滤器应用到“未分配”区域时，负载平衡器会显示与分配给作业角色的工作项目关联的所有小时。

有关在工作负载平衡器中过滤信息的信息，请参阅 [在工作负载平衡器中管理过滤器](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
