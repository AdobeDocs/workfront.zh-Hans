---
title: 20.4资源管理增强
description: 20.4资源管理增强
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 9f660a38-4a59-4135-8178-0841088cc7d6
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 0%

---

# 20.4资源管理增强

本页介绍了在“预览”环境中20.4版本中所做的所有资源管理增强。 这些增强功能将于2020年11月9日这一周的生产环境中提供。

有关20.4版本中可用的所有更改的列表，请参阅 [20.4版本概述](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## 使用工作量而不是计划小时来规划工作

为了在您计划项目工作时提供灵活性，我们引入了任务工作量的新概念。 您可以估计任务的工作量是小、中还是大，而无需人工估计任务的计划时数。 每个工作量级别都根据实例中配置的每天典型小时数的百分比计算。

现在，这项新功能提供了以下改进功能：

* 为项目和模板启用此设置，以使其可用于任务和模板任务
* 使用简单持续时间类型更新每个任务的此设置，该类型可自动更新任务的计划时间
* 对于希望继续使用计划小时的用户，请使用布局模板来禁用此设置。
* 在任务列表或报表中显示此新字段的值。

有关工作量的信息，请参阅 [工作概述](../../../manage-work/tasks/task-information/work-effort.md).

此功能现在包含在 [计划员基础知识，第2部分学习路径](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-2-plan-a-project-20Y0z000000bm79EAA) Workfront一号。

## 工作负载平衡器中工作项的项目基于状态的颜色

为了在负载平衡器中更好地显示和增强体验的自定义功能，您现在可以更改项目及其工作项的颜色以匹配项目状态。 颜色与组级别或系统级别的项目状态相对应。 显示的颜色可以与系统和自定义项目状态相对应。

有关在工作负载平衡器中自定义视图的信息，请参阅 [导航工作负载平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 使用工作负载平衡器中的百分比值调整用户分配

您现在可以使用百分比而不是小时在负载平衡器中管理用户的分配。

有关在负载平衡器中管理分配的信息，请参阅 [在工作负载平衡器中管理用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## 在工作负载平衡器中显示或隐藏已完成的工作

现在，通过新设置，您可以在负载平衡器中显示或隐藏已完成的工作项。 默认情况下，该设置处于启用状态，并且已完成的工作项与筛选条件匹配，并且所选时间范围在工作负载平衡器中显示。

在此增强之前，已完成的工作项始终显示在工作负载平衡器中。

有关在工作负载平衡器中调整设置的详细信息，请参阅 [导航工作负载平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 工作负载平衡器的可用性改进

为确保在负载平衡器中管理资源时获得简化且用户友好的体验，现在提供了以下可用性改进：

* 现在，您可以从“摘要”图标（而不是“更多”菜单）中打开问题和任务的摘要。 此体验现在与列表体验一致。

   >[!NOTE]
   >
   >此选项仅在新的Adobe Workfront体验中可用。

* 您可以访问对象栏左侧的“更多”菜单，而不是对象栏的末尾。 这样可以更轻松地查找对象跨越较长时间的时间。
* 您可以使用键盘快捷键访问分配功能。 以前，只能从“更多”菜单中使用。
* 通过单击“加载更多”，您可以加载用户名下的所有其余项目，而不是仅加载以下20个项目。

有关导览工作负载平衡器的详细信息，请参阅 [导航工作负载平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 工作负载平衡器中的用户分配图表

为了让您能够在给定时间范围内以高级别的可视化方式显示用户分配，现在，新设置可以启用图表视图，以了解分配在工作负载平衡器中的显示方式。 启用此设置后，将在折线图中显示用户的分配情况，该分配情况以红色块表示过度分配，以蓝色表示过度分配。

有关在工作负载平衡器中配置设置的详细信息，请参阅 [导航工作负载平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 可视化工作负载平衡器中已完成的工作

为了让您轻松识别已完成的工作，以便您能够正确管理用户分配，我们在工作负载平衡器中启用了一个可视指示器，该指示器显示选定时间范围的项目何时完成。 您现在可以看到任务的绿色复选标记，以及任务完成时出现的问题。 当在屏幕上显示的时间范围内完成了工作项时，项目还会显示绿色复选标记。

有关在工作负载平衡器中查看信息的信息，请参阅 [导航工作负载平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 为工作负载平衡器中的“已分配工作”区域新增了默认筛选器

工作负载平衡器中“已分配的工作”区域的“默认”筛选器现在只显示属于您作为登录用户关联的所有团队的成员的用户。 默认情况下，新过滤器现在会显示与您最相关的信息。

在此增强功能之前，您有权查看的所有用户都会显示在此区域中。

有关在工作负载平衡器中使用过滤器的信息，请参阅 [在工作负载平衡器中管理过滤器](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## 用于在工作负载平衡器中的小时和百分比值之间切换，或分配和剩余时间之间切换的新图标

我们添加了新设置，允许您在查看工作负载平衡器时在分配的小时数和百分比之间进行切换。 使用此新图标，我们还消除了“设置”面板中的“用户工作量”部分。 工作负载平衡器默认显示已分配的时间，我们已将“剩余小时”设置移到新的“百分比”或“小时”图标。

这项改进消除了点击，使工作负载平衡器导航更简单、更高效。

有关管理工作负载平衡器设置的信息，请参阅 [导航工作负载平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 工作负载平衡器的新内置过滤器：项目用户

为了提高您在工作负载平衡器中的过滤体验的效率，我们在“已分配的工作”区域中添加了新的内置过滤器。 您现在可以应用项目上的用户筛选器，该筛选器可显示分配给您指定项目中的任务和问题的用户。

有关在工作负载平衡器中使用过滤器的信息，请参阅 [在工作负载平衡器中筛选信息](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

