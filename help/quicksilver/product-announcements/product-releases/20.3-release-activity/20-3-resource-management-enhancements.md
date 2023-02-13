---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3资源管理增强
description: 本页介绍了在生产环境的20.3版本中所做的所有资源管理增强。 这些增强功能已于2020年8月10日这一周的生产环境中提供。
author: Luke
feature: Product Announcements
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# 20.3资源管理增强

本页介绍了在生产环境的20.3版本中所做的所有资源管理增强。 这些增强功能已于2020年8月10日这一周的生产环境中提供。

有关20.3版本中可用的所有更改的列表，请参阅 [20.3版本概述](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## 在工作负载平衡器的“已分配工作”区中包含问题的小时数

为了让您能够看到所有人员工作负载的完整画面，我们引入了一个设置，允许您在工作负载平衡器的“已分配工作”区域中包含几个小时的问题。

有关在工作负载平衡器中工作的信息，请参阅 [导航工作负载平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 在负载平衡器中调整非工作日的分配

您可以使用负载平衡器调整非工作日的资源分配。

有关在负载平衡器中管理分配的信息，请参阅 [在工作负载平衡器中管理用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## 工作负载平衡器中可用的变量筛选器

为了改进您的体验，并在您共享信息时提供更大的灵活性，我们现在为工作负载平衡器实施了变量过滤器。 以下过滤器已添加到工作负载平衡器：

* “我”（按用户过滤时）
* “我的主要角色”（按角色过滤时）
* “我的主团队”或“我的所有团队”（按团队过滤）。

这些过滤器将替换通配符过滤器变量$USER.ID、$USER.roleID、$USER.homeTeamID和$USER.teamID

当您应用其中一个过滤器，然后共享工作负载平衡器或将其置于功能板上时，所有其他用户都将看到他们自己的信息。

有关将过滤器应用到工作负载平衡器的信息，请参阅 [在工作负载平衡器中筛选信息](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## 负载平衡器中项目的新排序

现在，负载平衡器首先根据最早的计划起始日期对项目进行排序，然后根据用户在屏幕上显示的时间范围内发生的项目中任务的最新计划完成日期对项目进行排序。 这样，您就可以按照类似树的层次结构来组织工作，从而更轻松地识别一天的工作。

有关在工作负载平衡器中查看项目和工作项的信息，请参阅 [导航工作负载平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 显示工作负载平衡器中的实际工作进度

为了让您准确地了解工作负载的进度，我们在工作负载平衡器中引入了新设置，该设置根据任务和问题的预计日期显示任务和问题的时间表。 您可以启用“显示预计日期”设置，以查看工作项的预计时间轴以及计划的时间轴。

此外，通过这项改进，如果任务或问题在计划完成日期之前完成，则从剩余天数开始分配的小时数将被划到，以表明它们不会计入用户的整体分配。

有关导航工作负载平衡器和启用设置的信息，请参阅 [导航工作负载平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 工作负载平衡器功能先前已与20.2版本通信为已发布

* [在工作负载平衡器中调整每日和每周分配](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [在工作负载平衡器中更新任务计划小时数](#update-task-planned-hours-in-the-workload-balancer)
* [更便于在负载平衡器中更新分配的方法](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### 在工作负载平衡器中调整每日和每周分配 {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

为避免资源耗尽，您现在可以使用负载平衡器调整用户的每日和每周分配，以便工作。

在进行此增强之前，只能使用资源计划工具进行此增强。

有关在负载平衡器中管理分配的信息，请参阅 [在工作负载平衡器中管理用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**可在以下环境中使用：**

* Adobe Workfront Classic
* 新的Adobe Workfront体验

### 在工作负载平衡器中更新任务计划小时数 {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>在2020.2版本发布后不久，此增强功能即将在生产环境中提供。

访问级别的“资源管理”区域中的新选项现在允许具有此访问权限的用户从负载平衡器编辑计划小时数。 在工作负载平衡器中调整分配时，每日分配的总数不需要与任务的计划小时数匹配。 保存分配后，分配小时总数将成为任务的计划小时数。 仅对于具有简单持续时间类型的任务可以执行此操作。

有关在负载平衡器中管理分配的信息，请参阅 [在工作负载平衡器中管理用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

有关授予对资源管理的访问权限的信息，请参阅 [授予对资源管理的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### 更便于在负载平衡器中更新分配的方法 {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

为了更方便地在负载平衡器中管理用户对工作项的分配，您现在可以双击该工作项。 您还可以使用现有的编辑分配菜单选项。 此外，您不再需要启用显示分配才能更新它们。

有关在负载平衡器中管理分配的信息，请参阅 [在工作负载平衡器中管理用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
