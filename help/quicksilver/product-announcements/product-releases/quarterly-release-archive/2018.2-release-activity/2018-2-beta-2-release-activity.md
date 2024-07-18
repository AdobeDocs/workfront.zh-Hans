---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 2发行版活动
description: 本页介绍了2018.2 Beta 2版本在“预览”环境中最近提供的所有更改。 该功能已于2018年4月5日在预览环境中提供。 该版本将于2018年6月在生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c8ef68f5-53db-4c3c-af0f-e1c98521ec27
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# 2018.2 Beta 2发行版活动

本页介绍了2018.2 Beta 2版本在“预览”环境中最近提供的所有更改。 该功能已于2018年4月5日在预览环境中提供。 该版本将于2018年6月在生产环境中提供。

>[!IMPORTANT]
>
> 此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2018.2版中所做所有更改的列表，请参阅  [2018.2发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md)。

2018.2 Beta 2版本包含以下增强功能：

* [直接从主页区域编辑字段](#edit-fields-directly-from-the-home-area)
* [以天为单位记录时间](#log-time-in-days)
* [在项目列表中的甘特图上查看跨项目前置任务关系](#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects)
* [使用Portfolio优化程序中的预算成本计算Portfolio财务](#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances)
* [利用率报告：从新资源预算区域](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area)填充预算小时数（仅预览）

* [利用率报告：查看项目上按用户的预算小时数](#utilization-report-view-budgeted-hours-by-user-on-a-project)（仅预览）

* [文档列表中的验证进度可供非验证用户使用](#proof-progress-from-the-document-list-available-to-non-proofing-users)
* [移动改进](#mobile-improvements)

## 直接从主页区域编辑字段 {#edit-fields-directly-from-the-home-area}

现在，当您在“主页”区域中选择对象时，可以直接从“主页”区域的右侧面板编辑与该对象关联的字段。 

在此更改之前，只能在“主页”区域查看信息，不能进行编辑。

有关详细信息，请参阅文章中的[在主页区域](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)更新或编辑工作项  [更新或编辑主页区域中的工作项](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)。

## 以天为单位记录时间 {#log-time-in-days}

Workfront管理员现在可以配置其组织中的用户是记录时间（以天还是以小时为单位）。 拥有Planner许可证的用户可以自己配置此设置。

在此更改之前，用户只能以小时为单位记录时间。

您可以通过编辑用户配置文件来配置此设置。 有关详细信息，请参阅[配置时间是以小时还是天数记录](../../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)。

有关用户如何在此设置更新后记录时间（以天为单位）的信息，请参阅[记录时间](../../../../timesheets/create-and-manage-timesheets/log-time.md)。

## 在项目列表的甘特图上查看跨项目前置任务关系 {#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects}

您现在可以在甘特图上的以下项目列表中查看跨项目前置任务关系：

* 项目组合或项目群中的“项目”选项卡
* 在项目报告中

在此更改之前，您只能查看项目级别单个任务的跨项目前置任务关系。

有关详细信息，请参阅[配置信息在甘特图上的显示方式](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)。 

## 使用Portfolio优化程序中的预算成本计算Portfolio财务 {#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances}

新的Portfolio优化程序现在使用业务案例的新资源预算区域或资源规划程序中的预算成本来计算以下字段：

* 净值
* 投资回报率(ROI)
* 成本

以前，新旧版Portfolio优化器都使用旧版预算成本。 旧版Portfolio优化器仍使用旧版预算成本计算净值、投资回报和成本。

我们还在Portfolio财务字段中添加了两个新字段：旧版ROI和旧版净值，以便从新的资源管理工具中获取新的价值。

有关详细信息，请参阅文章中的[Portfolio优化器概述](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)  [Portfolio优化程序概述](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)。

## 利用率报表：从新资源预算区域填充预算小时数 {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
>此功能将不会包含在2018.2版的“预览”环境的正式版本中。 它将在2018.3版本的Beta测试期间重新引入，并将在2018.3版本中发布到“生产”环境。 

利用率报表中的预算小时数现在由业务案例的新资源预算编制区域中的可用信息填充。

在此更改之前，使用旧版资源估算区域中的信息。

有关详细信息，请参阅文章中的[资源利用率报告概述](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)  [资源利用率报告概述](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 利用率报表：按用户在项目上查看预算小时数 {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>此功能将不会包含在2018.2版的“预览”环境的正式版本中。 它将在2018.3版本的Beta测试期间重新引入，并将在2018.3版本中发布到“生产”环境。 

项目的利用率报告现在按用户显示预算小时数。

在此更改之前，“利用率”报告仅按工作角色显示预算小时数。 

有关详细信息，请参阅[资源利用率报告概述](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)一文中的[资源利用率报告概述](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 文档列表中的验证进度可供非验证用户使用 {#proof-progress-from-the-document-list-available-to-non-proofing-users}

现在，当查看文档列表时，将为所有用户显示验证进度指示器（已发送、已打开、已作出评论和决策）。 这包括无法生成验证的用户(有关允许用户生成验证的更多信息，请参阅部分。

在此更改之前，验证进度指示器仅适用于可以生成验证的用户。

有关详细信息，请参阅[校对进度和状态概述](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md)。

## 移动改进 {#mobile-improvements}

移动设备应用程序包含以下增强功能：

* 现在，在其他移动设备应用程序中与您共享的链接会在Workfront移动设备应用程序中打开。

  有关共享链接的更多信息，请参阅。

  此更新现已在iOS和Android上可用。

* 我们更新了对iOS平台的支持要求以支持iPhone X。

  有关支持的移动设备和操作系统的更多信息，请参阅。 
