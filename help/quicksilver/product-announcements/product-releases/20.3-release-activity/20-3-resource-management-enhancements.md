---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3资源管理增强功能
description: 本页介绍了20.3版本对生产环境所做的所有资源管理增强。 这些增强功能在2020年8月10日这一周的生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# 20.3资源管理增强功能

本页介绍了20.3版本对生产环境所做的所有资源管理增强。 这些增强功能在2020年8月10日这一周的生产环境中提供。

有关20.3版本的所有可用更改列表，请参阅[20.3版本概述](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md)。

## 在工作负载均衡器的已分配工作区域包括问题的小时数

为了让您全面了解您的所有人员的工作负载，我们引入了一个设置，允许您在工作负载均衡器的已分配工作区域包含问题的小时数。

有关使用工作负载均衡器的信息，请参阅[导航工作负载均衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

## 在工作负载均衡器中调整非工作日的分配

您可以使用工作负载均衡器调整非工作日资源的分配。

有关管理工作负载均衡器中的分配的信息，请参阅[管理工作负载均衡器中的用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。

## 工作负载均衡器中可用的变量过滤器

为了改进您的体验并在您共享信息时为您提供更大的灵活性，我们现在为工作负载均衡器实施了变量过滤器。 以下过滤器已添加到工作负载均衡器：

* “我”（按用户筛选时）
* “我的主要角色”（按角色过滤时）
* “我的主团队”或“我的所有团队”（按团队筛选时）。

这些筛选器将替换$$USER.ID、$$USER.roleID、$$USER.homeTeamID和$$USER.teamIDs的通配符筛选器变量

当您应用这些过滤器之一，然后共享工作负载均衡器或将其置于仪表板时，所有其他用户都将看到他们自己的信息。

有关将过滤器应用于工作负载均衡器的信息，请参阅工作负载均衡器中的[过滤器信息](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)。

## 在工作负载均衡器中对项目进行新排序

工作负载均衡器现在首先根据用户显示在屏幕上的时间范围内发生的最早规划开始日期对项目进行排序，其次根据项目中任务的最晚规划完成日期进行排序。 这允许您以树状层次结构来组织工作，这有助于您更轻松地识别一天的工作。

有关在工作负载均衡器中查看项目和工作项的信息，请参阅[在工作负载均衡器中导航](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

## 在工作负载均衡器中显示实际工作进度

为了让您准确了解工作负载的进度，我们在工作负载均衡器中引入了一个新设置，该设置根据任务的预计日期显示任务和问题的时间线。 您可以启用显示预计日期设置以查看工作项的预计时间线以及计划时间线。

此外，通过这种改进，如果任务或问题在计划完成日期之前完成，则剩余天数中的分配小时数将被删除，以指明它们不计入用户的整体分配。

有关导航工作负载均衡器和启用设置的信息，请参阅[导航工作负载均衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

## 工作负载均衡器功能以前在20.2版本中作为发行版本进行介绍

* [在工作负载均衡器中调整每日和每周分配](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [在工作负载均衡器中更新任务已计划小时数](#update-task-planned-hours-in-the-workload-balancer)
* [在工作负载均衡器中更新分配的更简便方法](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### 在工作负载均衡器中调整每日和每周分配 {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

为避免资源燃尽，您现在可以使用工作负载均衡器调整用户的每日和每周分配以便工作。

在此增强功能之前，只能使用“资源计划”工具实现此功能。

有关管理工作负载均衡器中的分配的信息，请参阅[管理工作负载均衡器中的用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。

**在以下环境中可用：**

* Adobe Workfront Classic
* 新的Adobe Workfront体验

### 在工作负载均衡器中更新任务已计划小时数 {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>此增强功能将在2020.2版本发布后不久在生产中可用。

访问级别的资源管理区域中的新选项现在允许具有此访问权限的用户从工作负载均衡器编辑已计划小时数。 在工作负载均衡器调整分配时，每日分配总数无需与任务的已计划小时数匹配。 保存分配后，分配小时总数将成为任务的计划小时数。 这仅适用于具有简单持续时间类型的任务。

有关管理工作负载均衡器中的分配的信息，请参阅[管理工作负载均衡器中的用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。

有关授予对资源管理的访问权限的信息，请参阅[授予对资源管理的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)。

### 在工作负载均衡器中更新分配的更简便方法 {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

为了更便于管理工作负载均衡器中对工作项的分配，您现在可以双击该工作项。 您仍然可以使用现有的“编辑分配”菜单选项。 此外，您不再需要启用显示分配才能更新它们。

有关管理工作负载均衡器中的分配的信息，请参阅[管理工作负载均衡器中的用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。
