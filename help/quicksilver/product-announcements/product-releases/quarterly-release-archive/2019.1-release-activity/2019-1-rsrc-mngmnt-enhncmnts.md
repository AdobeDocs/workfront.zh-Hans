---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1资源管理增强功能
description: 本页介绍了2019.1版本中包含的所有资源管理增强功能。 该功能现已在“生产”环境中可用。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6eed6023-96cc-45d7-8dae-a36d45e92068
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# 2019.1资源管理增强功能

本页介绍了2019.1版本中包含的所有资源管理增强功能。 该功能现已在“生产”环境中可用。

有关2019.1版中所做所有更改的列表，请参阅[2019.1版活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md)。

## 更新了资源规划者中的默认筛选器

资源规划者中的默认筛选器不再按项目组进行筛选。

现在，在查看资源规划者时，您只能看到当前且默认情况下对日期敏感的项目。 默认情况下，将包含来自以下项目的信息：

* 计划完成日期在当月第一个日期之后。
* 计划开始日期早于从今天开始的第四个月的最后日期。
* 状态为“当前”或“计划”。

以前，默认过滤器会从以下其他项目中检索信息：

* 计划完成日期在当月第一个日期之后。
* 计划开始日期早于从今天开始的第四个月的最后日期。
* 状态为“当前”或“计划”。
* 与已登录用户的主组匹配的组。

有关将过滤器应用于资源规划者的信息，请参阅资源规划者中的[过滤器信息](../../../../resource-mgmt/resource-planning/filter-resource-planner.md)。

## 将通配符用于资源规划者筛选器

现在，在资源规划者中构建过滤器时可以使用通配符。 例如，可以使用$$USER.ID筛选已登录的用户信息，或使用$$USER.companyID筛选与已登录用户属于同一公司的所有用户信息。 有关基于用户的变量的完整列表，请参阅[通配符筛选器变量](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)中的[基于用户的通配符筛选器变量](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables)部分。

以前，通配符不可用于资源规划者过滤器。

有关在资源规划者中进行筛选的信息，请参阅资源规划者中的[筛选信息](../../../../resource-mgmt/resource-planning/filter-resource-planner.md)。

<!--
<iframe class="mt-media" src="assets/290697527?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>
-->

## 在资源规划程序中支持基于日期的通配符筛选器变量

在资源规划者中构建过滤器时，您现在可以使用任何版本的$$TODAY通配符过滤器变量。

在此增强功能之前，您只能使用基于用户的通配符筛选器变量。

有关在资源规划者中进行筛选的信息，请参阅资源规划者中的[筛选信息](../../../../resource-mgmt/resource-planning/filter-resource-planner.md)。

有关通配符筛选器变量的信息，请参阅[通配符筛选器变量](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。

## 资源规划者中角色视图的导出选项

现在，您可以从角色视图的资源规划者中选择要导出哪些级别的信息。 您可以导出以下任何一项：

* 仅角色
* 角色和项目
* 角色、项目和用户

在此增强功能之前，已在“角色”视图中导出所有级别的信息。 在以前的版本中，这些选项已引入到“项目”和“用户”视图中。

有关从资源规划者导出信息的信息，请参阅[从资源规划者导出信息](../../../../resource-mgmt/resource-planning/export-resource-planner.md)。

## 用于导出资源规划者的数据格式选项

现在，您可以选择在从资源规划者导出时如何在Excel文件中显示信息。

您可以通过以下方式显示从资源计划员导出的信息的可用性和分配：

* 按其所属对象的名称取消分组。 在这种情况下，其所属对象的名称将显示在每行数据上。 （这是默认选项）
* 按其所属对象的名称分组。 在这种情况下，导出的文件中的信息会显示在Workfront中。

在此增强功能之前，导出的文件中的信息显示为Workfront中的信息。

有关从资源规划者导出信息的信息，请参阅[从资源规划者导出信息](../../../../resource-mgmt/resource-planning/export-resource-planner.md)。

## 持续性计划时间表

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器计划资源的信息，请参阅[工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

现在，当您刷新时间线或导航离开页面时，计划时间线会保留您选择的时间范围。

在此增强功能之前，当您刷新页面或离开页面导航时，计划时间表返回到默认时间范围。

此增强功能在以下区域提供：

* “人员”区域中的“计划”选项卡
* “团队正在处理”选项卡
* 项目的“人员配备”标签上的“计划”子标签

有关在“资源计划”区域中使用时间线的信息，请参阅“开始使用资源计划”。

## 资源规划者中的新导出选项

您现在可以从资源规划者中选择要导出的信息级别。 在“项目”视图中，可以导出以下任意内容：

* 仅项目
* 项目和角色
* 项目、角色和用户

在“用户视图”中，可以导出以下任何内容：

* 仅限用户
* 用户和项目
* 用户、项目、角色、任务和问题

在此增强功能之前，默认情况下，所有级别的信息导出到资源规划者的所有视图中。

有关从资源规划者导出信息的信息，请参阅[从资源规划者导出信息](../../../../resource-mgmt/resource-planning/export-resource-planner.md)。

## 更新至资源规划者中的用户视图

现在，系统中的所有用户都显示在资源规划者的用户视图中，但只有与已筛选项目关联的用户也显示小时信息。

在此更新之前，只有分配到所筛选项目中工作项的用户会显示在资源规划者的用户视图中。

您可以使用基于用户的筛选器来减少“用户视图”中显示的用户数，仅限分配给要显示的项目的用户。

有关资源规划者中过滤器的信息，请参阅资源规划者中的[过滤器信息](../../../../resource-mgmt/resource-planning/filter-resource-planner.md)。
