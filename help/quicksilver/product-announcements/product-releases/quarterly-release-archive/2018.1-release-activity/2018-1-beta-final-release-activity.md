---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta最终发行版活动
description: 本页介绍了2018.1 Beta Final版本在“预览”环境中最近提供的所有更改。 2018年1月31日，该功能在“预览”环境中提供。 该版本将于2018年3月在生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 35bd3604-5452-4b46-afb1-78bc2fbb48ec
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# 2018.1 Beta最终发行版活动

本页介绍了2018.1 Beta Final版本在“预览”环境中最近提供的所有更改。 2018年1月31日，该功能在“预览”环境中提供。 该版本将于2018年3月在生产环境中提供。

>[!IMPORTANT]
>
> 此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2018.1版中所做所有更改的列表，请参阅  [2018.1版本活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md)。

2018.1 Beta最终版本包含面向Workfront管理员和其他用户的增强功能：

管理员的&#x200B;****

* [配置资源可用性和用户分配，以根据用户计划进行计算](#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule)

所有用户&#x200B;****

* [移动增强功能](#mobile-enhancements)
* [Jira集成](#jira-integration)
* [更新到验证查看器名称](#update-to-proofing-viewer-names)
* 从校对生产环境同步到预览时[更改为同步节奏](#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview)
* [在资源计划员中达到2,000个项目限制时显示警告消息](#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner)

## 移动设备增强功能 {#mobile-enhancements}

以下功能将于2018年3月初在移动应用商店推出：

* 新导航：我们的移动应用程序主页已重新设计。
* 移动主页：我们的新主页功能现在也在移动应用程序上进行了更新。

iOS和Android平台均支持新功能。

## Jira集成 {#jira-integration}

您现在可以通过安装和配置适用于Jira的Workfront加载项将Jira问题链接到Workfront任务或问题。 利用此集成，您的项目经理可以继续在Workfront中工作，而开发工程师可以继续在Jira中工作，同时他们的单个项目通过Workfront与Jira的集成变得关联。

您可以通过此集成配置以下内容：

* 为Workfront分配建立触发器，以便在发生Jira问题时自动创建。
* 手动将Jira问题链接到之前已创建的Workfront任务或问题。
* 指定在其中一个应用程序中更新某个链接项后立即在链接项上同步的字段。

Workfront加载项将适用于Jira的内部部署和按需版本。 此加载项是免费的，将于2018年3月初在Atlassian Marketplace中下载。

有关适用于Jira的Workfront加载项的更多信息，包括下载该加载项的链接，请参阅[将Workfront与Jira结合使用。](https://support.workfront.com/hc/en-us/sections/115001130053)

## 校对查看器名称更新 {#update-to-proofing-viewer-names}

在整个Workfront系统中，基于HTML5的验证查看器和基于Flash的验证查看器的名称已重新命名。 以前的和更新的名称如下： 

| **以前的名称** | **已更新名称** |
|---|---|
| HTML5验证查看器 | 新验证查看器 |
| Flash验证查看器 | 旧版验证查看器 |

{style="table-layout:auto"}

 有关使用新校对查看器的更多信息，请参阅[在校对查看器中查看校对。](https://support.workfront.com/hc/en-us/sections/115000275214)

## 配置资源可用性和用户分配，以根据用户计划进行计算 {#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule}

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器计划资源的信息，请参阅[工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

Workfront管理员现在可以确定Workfront如何在系统级别计算资源可用性和用户分配（考虑小时数和FTE可用性）。 Workfront管理员可以配置要使用默认计划或用户计划计算的资源可用性和用户分配。

在计划资源时，此设置会影响以下情况下的用户可用性：

* 当允许Workfront自动分配资源时，如“在计划区域中手动分配未分配的任务和问题”中所述。

* 显示分配指标时，如计划区域中的管理用户分配中所述。

有关更多信息，请参阅配置Workfront如何计算计划区域的资源小时和FTE可用性。

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器计划资源的信息，请参阅[工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。


## 从验证生产环境同步到预览时更改为同步节奏 {#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview}

>[!NOTE]
>
>此更改将于2018年2月11日生效。

现在，Workfront Proof生产环境中的数据每周都会同步到Workfront Proof预览环境。

在此更改之前，数据每月会从Workfront Proof生产环境同步到预览环境，而来自Workfront生产环境的数据每周会同步到Workfront预览环境。 在Workfront预览环境中使用验证功能时，此差异会导致出现一些同步错误。 

有关详细信息，请参阅[预览Sandbox测试环境 — Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md)。 

## 在资源计划员中达到2,000个项目限制时显示警告消息 {#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner}

由于我们当前正在努力寻找更永久的解决方案以改进资源规划者中的性能，因此我们为您可应用于资源规划者的每个视图引入了2,000个项目的限制：

* “用户视图”仅显示2,000个分配
* 项目视图仅显示2,000个项目
* “角色视图”仅显示2,000个角色

当资源规划者尝试加载超过2,000个项目时，会显示一条通知，提醒您只能显示2,000个项目。

有关这些限制以及它们如何影响资源规划者的更多信息，请参阅[资源规划者显示限制](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our beta program for the Resource Planner performance, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a>.</p>
-->
