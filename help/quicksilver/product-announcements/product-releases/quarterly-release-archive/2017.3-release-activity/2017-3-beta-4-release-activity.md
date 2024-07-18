---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 4发行版活动
description: 本页介绍了2017.3 Beta 4版本在“预览”环境中最近提供的所有更改。 此页面上的功能在2017年9月25日这一周的“预览”环境中提供。 该版本将于2017年11月初在“生产”环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 0%

---

# 2017.3 Beta 4发行版活动

本页介绍了2017.3 Beta 4版本在“预览”环境中最近提供的所有更改。 此页面上的功能在2017年9月25日这一周的“预览”环境中提供。 该版本将于2017年11月初在“生产”环境中提供。

>[!IMPORTANT]
>
> 此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2017.3版中所做所有更改的列表，请参阅  [2017.3发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md)。

2017.3 Beta 4版本包含面向Workfront管理员和其他用户的增强功能：

管理员的&#x200B;****

* [在设置区域新建资源管理首选项区域](#new-resource-management-preferences-area-in-the-setup-area)

所有用户&#x200B;****

* [重复的任务](#duplicate-tasks)
* 在计划资源时[自动执行分配](#automate-assignments-when-scheduling-resources)
* 在计划资源时[修改多个任务的分配](#modify-assignments-for-multiple-tasks-when-scheduling-resources)
* [将FTE分配应用于资源规划者](#apply-fte-distribution-to-the-resource-planner)
* 用户设置的[工作角色部分包含FTE可用性的百分比](#job-role-section-for-user-settings-includes-percentage-of-fte-availability)
* [在项目的利用率报告中保存和管理筛选器](#save-and-manage-filters-in-the-utilization-report-on-a-project)
* [利用率报告中的其他筛选选项](#additional-filtering-options-in-the-utilization-report)
* [按项目或Portfolio查看使用情况报告](#view-the-utilization-report-by-program-or-portfolio)
* [在项目和任务报告中显示原始问题信息](#show-original-issue-information-in-project-and-task-reports)
* 更新流中的[筛选器系统更新现在跨对象持续存在](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [报告Workfront中的活动验证阶段](#report-on-active-proof-stages-within-workfront)
* [将自定义Workfront Proof权限配置文件分配给Workfront中的用户](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront)
* [添加到事件订阅的小时资源](#hour-resource-added-to-event-subscriptions)

## 重复任务 {#duplicate-tasks}

您现在可以快速复制项目中的一项任务或一组任务。 此操作创建一个与原始任务相同的任务。 在复制过程中，没有其他选项可让您对新创建的任务进行任何更改。  

在此更改之前，您可以将任务复制到新项目或现有项目，并在复制时修改某些信息。

对象  有关复制任务的详细信息，请参阅[复制和复制任务](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

## 在计划资源时自动执行分配 {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器计划资源的信息，请参阅[工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

现在，在计划多个项目的资源时（从“计划”选项卡）或在计划单个项目的资源时（从“人员配备”选项卡），您可以允许Workfront自动为未分配的任务和问题建议分配。

Workfront会分析可用用户中的当前工作分配，并为任何尚未分配的任务或问题建议智能的逻辑分配。 在最终确定分配之前，您可以修改任何建议或现有分配。

有关更多信息，请参阅“在计划区域中手动分配未分配的任务和问题”。

## 在计划资源时修改多个任务的分配 {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

在计划资源时（通过“计划”选项卡或“人员配备”选项卡），如果批量分配、交换或取消分配用户，您现在可以修改在一个或多个项目中指定的特定任务（包括所有子任务和关联问题）的分配。

在此更改之前，您只能在整个项目中修改任务和问题的分配（您不能在项目中指定特定任务）。

有关更多信息，请参阅“在计划区域中手动分配未分配的任务和问题”。

## 将FTE分配应用于资源规划者 {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>此功能当前并非在所有群集的“预览”中可用。

当用户有多个角色时，您现在可以根据每个角色的FTE可用性百分比显示用户每个角色的正确可用小时数。

例如，如果用户计划表明他们在一个月内可工作100小时，并且他们对于主要角色的FTE可用性百分比为75%，而他们其它角色的FTE可用性百分比为25%，则资源规划者将列出主要角色下具有75可用小时并且其它角色下具有25可用小时数的用户。

在此更改之前，资源规划者中显示的用户的名称仅与主要角色相关联，并且用户的完全可用性根据其计划（100小时）仅与主要角色相关联。 仅当将用户分配给该角色中的任务，且其他角色中的用户的可用小时数为零时，才会在“资源规划者”中显示用户的“其他角色”。

有关如何为资源规划者中的用户和角色计算可用小时数和可用FTE的更多信息，请参阅资源规划者中计算用户和角色的小时数和可用FTE的[概述](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)。

## 用户设置的“工作角色”部分包含FTE可用性的百分比 {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>此功能当前并非在所有群集的“预览”中可用。

现在，在更新用户配置文件时，您可以向用户添加其他工作角色，并定义分配给每个工作角色的FTE的百分比。

在此更改之前，您无法将特定数量的FTE分配给与该用户关联的任何工作角色。

有关更新用户工作角色的FTE可用性百分比的详细信息，请参阅[编辑用户的配置文件](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)或[配置我的设置](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)。

## 在设置区域新建资源管理首选项区域 {#new-resource-management-preferences-area-in-the-setup-area}

您现在可以在安装程序中找到一个名为资源管理的新区域。 在此方面，我们引入了一个设置，该设置允许您指定如何在资源规划者中计算用户可用性。 可以使用以下方法计算此值：

* 人工：除了用户的单个FTE之外，系统的默认计划还用于确定资源规划者中用户的小时可用性。 用户的计划将被忽略。
* 自动：用户计划用于确定用户在资源规划者中的可用小时数。 FTE可用性是根据用户计划和默认计划计算的。 忽略用户FTE的值。 

有关为系统配置资源管理首选项的详细信息，请参阅[配置资源管理首选项](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

## 在项目的利用率报告中保存和管理筛选器 {#save-and-manage-filters-in-the-utilization-report-on-a-project}

现在，您可以保存在“利用率”报表中创建的过滤器。 此外，还可以重命名保存的筛选器、复制保存的筛选器、删除保存的筛选器或修改保存的筛选器。

以前，每次过滤利用率报告时都必须指定单独的过滤器选项。

有关在利用率报告中保存和管理过滤器的详细信息，请参阅[资源利用率报告概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)中的[资源利用率报告概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 利用率报告中的其他过滤选项 {#additional-filtering-options-in-the-utilization-report}

现在，运行利用率报告时，除了之前可用的“任务”、“问题”和“Portfolio”字段外，创建过滤器时，现在还提供针对“角色”、“项目”的新过滤字段。

在此更改之前，您只能通过添加新的筛选规则来按项目组合、项目和项目进行筛选。

有关详细信息，请参阅[资源利用率报告概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)中的[资源利用率报告概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 按项目或Portfolio查看利用率报告 {#view-the-utilization-report-by-program-or-portfolio}

您现在可以按项目或项目组合查看利用率报告。 这使您可以在单个利用率报告中查看多个项目的信息。

为便于进行此更改，现可在Workfront的报表区域以及单个项目中使用“利用率”选项卡。

在此更改之前，只能在项目中访问利用率报告。

有关更多信息，请参阅  [资源利用率报告概述](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。 

## 在项目和任务报告中显示原始问题信息 {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>此功能当前并非在所有群集的“预览”中可用。

对于通过转化问题而创建的项目和任务，您现在可以在项目或任务报告中找到关于原始问题的以下信息：

* 原始问题输入日期
* 原始问题名称
* 原始问题创建者ID

通过在文本模式下构建自定义视图，此信息可以显示在任务或项目报表或列表中。

在此更改之前，您无法报告此信息。

有关构建自定义文本模式视图（从原始问题中捕获信息）的更多信息，请参阅[视图：在任务和项目列表上显示原始问题信息](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md)。

## 更新流中的过滤器系统更新现在可以跨对象持续进行 {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>此功能未发布到Beta 4的“预览”环境。 它将在10月上半月的预览版中提供。

过滤器系统更新选项现在可以跨整个Workfront站点的对象持续使用。 这允许您隐藏系统更新并仅查看某个对象更新流中的用户注释，并在浏览到其他对象时保留该设置。

在此更改之前，您必须选择在浏览Workfront站点时筛选掉每个对象的系统更新。

有关详细信息，请参阅[更新工作](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

## 报告Workfront中的主要验证阶段 {#report-on-active-proof-stages-within-workfront}

在Workfront中创建文档版本报告时，现在有名为“主要验证阶段”的列。 此列允许您查看报告中每个文档版本上当前处于活动状态的验证阶段。 阶段的名称显示在“主要验证阶段”列中。 如果文档版本上当前没有处于活动状态的阶段，则该列为空。

有关视图和报告中可用字段的更多信息，请参阅[Adobe Workfront术语词汇表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

## 将自定义Workfront Proof权限配置文件分配给Workfront中的用户 {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

现在，在Workfront中为用户启用验证功能时，您可以分配自定义Workfront Proof权限配置文件。 

在此更改之前，只有以下权限配置文件可用：主管、经理、管理员。

## 添加到事件订阅的小时资源 {#hour-resource-added-to-event-subscriptions}

使用新的小时资源，您现在可以创建事件订阅，以使您的计费应用程序与Workfront保持同步。

若要了解有关事件订阅的更多信息，请参阅[事件订阅API](../../../../wf-api/general/event-subs-api.md)。
