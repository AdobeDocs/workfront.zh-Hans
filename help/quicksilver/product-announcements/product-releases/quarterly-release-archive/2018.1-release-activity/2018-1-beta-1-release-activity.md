---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 1发行版活动
description: 本页介绍了2018.1 Beta 1版本在“预览”环境中最近提供的所有更改。 2017年12月1日，预览环境中提供了此页面上的功能。 该版本将于2018年3月在生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 0%

---

# 2018.1 Beta 1发行版活动

本页介绍了2018.1 Beta 1版本在“预览”环境中最近提供的所有更改。 2017年12月1日，预览环境中提供了此页面上的功能。 该版本将于2018年3月在生产环境中提供。

>[!IMPORTANT]
>
> 此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2018.1版中所做所有更改的列表，请参阅  [2018.1版本活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md)。

2018.1 Beta 1版本包含面向Workfront管理员和其他用户的增强功能：

管理员的&#x200B;****

* [已更新布局模板以支持主区域](#updated-layout-template-to-support-the-home-area)
* [禁用从Workfront发送的校对电子邮件通知](#disable-proofing-email-notifications-sent-from-workfront)
* [添加到事件订阅的新资源](#new-resources-added-to-event-subscriptions)

所有用户&#x200B;****

* [主页区域（已更新我的工作区）](#home-area-updated-my-work-area)
* [在业务案例和更新的业务案例摘要下显示资源规划者数据](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary)
* [在资源规划者中显示计划小时数分配的百分比](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner)
* [“更改时自动更新”和“仅更改”更新类型会在更新任务的同时触发对父对象的更新](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated)
* [甘特图中可用的时间线快照](#timeline-snapshot-available-in-the-gantt-chart)

## 主页区域（已更新我的工作区） {#home-area-updated-my-work-area}

新的“主页”区域为当前在“我的工作”区域中可用的相同数据提供另一个增强视图。 与“我的工作”区域相比，“主页”区域具有以下优点：

* 更加精简和直观的界面
* 增强的性能
* 更新富文本格式的任务和问题

## 更新了布局模板以支持主页区域 {#updated-layout-template-to-support-the-home-area}

作为Workfront管理员，您可以通过配置用户所分配的布局模板来确定组织中的用户是否具有主页区域的访问权限。 未分配布局模板的用户始终可以访问“主页”区域。

有关详细信息，请参阅创建和管理布局模板。

## 禁用从Workfront发送的校对电子邮件通知 {#disable-proofing-email-notifications-sent-from-workfront}

您现在可以配置在对验证进行评论时，Workfront实例中的用户是否从Workfront接收电子邮件通知。

以前，当对验证进行评论时，始终从Workfront发送验证电子邮件。 如果还在Workfront Proof中启用了通知，则会导致用户收到重复通知。 

对于现有Workfront客户，Workfront默认配置为在对验证进行评论时发送电子邮件。

有关如何在Workfront中禁用验证的电子邮件通知以便仅从Workfront Proof发送验证电子邮件的信息，请参阅。  

## 在业务案例和更新的业务案例摘要下显示资源规划者数据 {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

现在，资源预算区域在项目的业务案例中可用。 在此区域中，您可以在资源规划者中查看为资源估算的预算小时数以及与其关联的预算劳力成本。

业务案例的资源评估区域已重命名为旧版资源评估。

作为此更改的一部分，业务案例摘要现在包括基于资源估计和资源预算的财务信息。

在此更改之前，您无法在项目的业务案例中看到资源规划者信息。 您只能查看在传统资源池的Capacity Planner中指定的资源估计信息。

有关创建业务案例的详细信息，请参阅[为项目创建业务案例](../../../../manage-work/projects/define-a-business-case/create-business-case.md)。

## 在资源规划者中显示计划小时数分配的百分比 {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

资源规划者的用户视图现在包括一个新列，允许您查看计划小时数分配占用户和工作角色的总可用小时数的百分比。

在此更改之前，您只能在单独的列中查看用户和工作角色的已计划小时数和可用小时数总计。

有关计划小时数分配百分比列的详细信息，请参阅[资源规划者概述](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)中的“查看可用小时数和计划小时数或FTE之间在资源规划者中的差异”部分。

## “更改时自动更新”和“仅更改”更新类型会在更新任务的同时触发对父对象的更新 {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

我们更改了在项目中更新较低级别对象时父任务和项目更新的方式。 父对象更新的时间由项目中的更新类型字段决定。 您可以从以下更新类型中进行选择：

* 更改时自动更新
* 仅在更改时更新
* 仅自动更新
* 仅手动

现在，当您选择“更改时自动更新”或“仅更改”更新类型时，应用到单个任务的更改也将立即应用到父任务和项目。

在此更改之前，您必须刷新页面以确保父对象和项目时间线也会更新。

有关项目更新类型的详细信息，请参阅[选择项目更新类型](../../../../manage-work/projects/manage-projects/select-project-update-type.md)。

## 甘特图中可用的时间线快照 {#timeline-snapshot-available-in-the-gantt-chart}

现在，您可以使用甘特图中的新时间线快照快速滚动到项目生命周期的某个时间点。

当您在查看任务或项目列表时为甘特图选择粒度更细的时间范围时，水平滚动条会显示在甘特图的底部。 单击滚动条允许您在快照中查看项目的整个时间线。 您可以单击甘特图快照中的任意位置，以导航到项目生命周期中的特定点。

在此更改之前，您必须在整个甘特图上水平滚动以找到特定时间点，或者必须缩小粒度视图。

有关信息如何在甘特图中显示的详细信息，请参阅[配置信息在甘特图上的显示方式](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)。

## 添加到事件订阅的新资源 {#new-resources-added-to-event-subscriptions}

现在，您可以为以下资源创建事件订阅：

* **费用：**&#x200B;在添加或修改费用时通知您。
* **工作分配：**&#x200B;在用户、工作角色或团队的任务或问题中添加或修改工作分配时通知您。
* **时间表：**&#x200B;在提交、拒绝或批准时间表时通知您。

若要了解有关事件订阅的更多信息，请参阅[事件订阅API](../../../../wf-api/general/event-subs-api.md)。
