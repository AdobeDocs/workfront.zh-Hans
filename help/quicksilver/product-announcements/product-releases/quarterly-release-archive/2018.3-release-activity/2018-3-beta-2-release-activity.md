---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.3 Beta 2发行版活动
description: 本页介绍了2018.3 Beta 2版本在“预览”环境中最近提供的所有更改。 该功能将于2018年8月1日在预览环境中可用。 Beta 2中发布的校对增强功能将于7月18日星期三在“预览”环境中提供。 该版本将于2018年11月在生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# 2018.3 Beta 2发行版活动

本页介绍了2018.3 Beta 2版本在“预览”环境中最近提供的所有更改。 该功能将于2018年8月1日在预览环境中可用。 Beta 2中发布的校对增强功能将于7月18日星期三在“预览”环境中提供。 该版本将于2018年11月在生产环境中提供。

>[!NOTE]
>
> 此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2018.3版中所做所有更改的列表，请参阅  [2018.3发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md)。

2018.3 Beta 2版本包含面向Workfront管理员和其他用户的增强功能：

管理员的&#x200B;**&#x200B;**

* [以组管理员身份更新用户配置文件中的电子邮件地址](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

所有用户&#x200B;**&#x200B;**

* [在主页区域查看委托给我的审批](#view-approvals-delegated-to-me-in-the-home-area)
* [导出资源规划者中给定期间的数据](#export-data-for-a-given-period-in-the-resource-planner)
* 当用户分配过多时，[每日总计现在显示为红色](#daily-totals-now-display-in-red-when-the-user-is-overallocated)
* 当最小化时，[任务和问题在计划时间线上处于隐藏状态](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [在验证查看器中按用户过滤评论和回复](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [对视频校对中的一系列素材进行评论](#comment-on-a-range-of-footage-in-a-video-proof)
* [校对查看器中评论标记的新折线工具](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [为报表、日历和文档共享删除Flash](#flash-removal-for-report-calendar-and-document-sharing)

## 以组管理员身份更新用户配置文件中的电子邮件地址 {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

您现在可以更新属于您管理的组的用户的电子邮件地址。 

以前，只有Workfront管理员才能更新其他用户的电子邮件地址。 

有关详细信息，请参阅[组管理员](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)。

## 查看主页区域委托给我的审批 {#view-approvals-delegated-to-me-in-the-home-area}

您现在可以使用“主页”区域查看已委派给您的项目、任务和问题的审批。

在此更改之前，您只能在“我的工作”区域查看已委托的审批。

有关详细信息，请参阅[委托审批请求](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md)。

## 在资源规划者中导出给定期间的数据 {#export-data-for-a-given-period-in-the-resource-planner}

现在，在资源规划者中导出信息时会显示一个新窗口，允许您为导出的文件选择特定时间范围。

在此增强功能之前，您只能导出屏幕上显示的信息。

有关从资源规划者导出数据的更多信息，请参阅文章[资源规划者导航概述](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)中的[资源规划者导航概述](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)。

## 当用户分配过度时，每日总计现在以红色显示 {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器计划资源的信息，请参阅[工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

当用户分配过多时，用户分配过量的天数的每日总计现在显示为红色。 仅当在计划时间线设置中启用了显示每日计划小时数总计选项时，才会显示此选项。 在此增强功能之前，存在红色条形指示符，用于指示用户过度分配的日期，但显示每日总计时没有红色高亮。

有关用户分配的更多信息，请参阅“在计划区域管理用户分配”。

## 最小化时，任务和问题会在计划时间线上隐藏 {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

当您将计划时间轴上的任务和问题最小化时，如果在设置中启用了显示每日计划小时数总计选项，用户和角色现在会隐藏这些任务和问题。 未分配区域中的任务和问题以压缩视图显示。

以前，在最大限度地减少任务和问题时，任务和问题将保留在用户和角色的时间表上，但将以压缩视图显示。

有关在计划时间表中最大程度地减少任务和问题的更多信息，请参阅  “开始使用资源计划”。

## 在验证查看器中按用户过滤注释和回复 {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

现在，您可以在过滤由您指定的用户所做的评论时包含回复。 如果您希望重点关注重要审核者（如客户或项目经理）提出的所有反馈，则此功能非常有用。

以前，按用户过滤仅限于由您指定的审阅人创作（开始）的评论。

## 对视频校对中的一系列素材的评论 {#comment-on-a-range-of-footage-in-a-video-proof}

您可以为视频校样中的一系列素材创建评论。 例如，当您需要指明需要对素材段进行重新拍摄或移除时，这非常有用。

以前，您只能为视频时间轴上的单个点创建注释。

## 校对查看器中注释标记的新折线工具 {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

现在，向验证添加注释时，可以使用折线标记来绘制分段线条和形状。 您可以创建开放的分段线或闭合的形状。 在处理复杂的图像（如技术图像或体系结构图像）时，此工具特别有用。

以前，在标记验证以添加注释时，您可以绘制矩形、直线、手绘线或形状或箭头。

## 为报表、日历和文档共享删除Flash {#flash-removal-for-report-calendar-and-document-sharing}

我们已从Workfront中的以下“共享”对话框删除Flash：

* 报告
* 日程表
* 文档

您仍然可以像以前一样共享这些对象，但现在，体验不再依赖于Flash。
