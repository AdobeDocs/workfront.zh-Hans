---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 1发行版活动
description: 本页介绍了2017.2 Beta 1版本在“预览”环境中提供的所有更改。 2017年5月10日，预览环境中提供了此页面上的功能。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

# 2017.2 Beta 1发行版活动

本页介绍了2017.2 Beta 1版本在“预览”环境中提供的所有更改。 2017年5月10日，预览环境中提供了此页面上的功能。

>[!IMPORTANT]
>
>此页面上描述的功能在生产环境中可用之前可能会发生更改。

2017.2 Beta 1版本包含面向Workfront管理员和其他用户的增强功能：

管理员的&#x200B;**：**

* [还原文档](#restore-documents)
* [新预览横幅及发行信息](#new-preview-banner-with-release-information) 
* [API 7可用性](#api-7-availability)

所有用户&#x200B;**：**

* [订阅任务和问题](#subscribe-to-tasks-and-issues)
* [资源计划改进](#resource-scheduling-improvements)
* [比较校样](#compare-proofs)
* [用户和项目资源池的新字段](#new-field-for-resource-pools-for-users-and-projects)
* [已更新仪表板列表中的外观](#updated-look-and-feel-in-the-dashboard-list)
* [在Workfront中删除签署功能](#removing-the-endorsements-functionality-in-workfront)
* [使用拖放操作对任何列表中的列重新排序（即将删除功能）](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## 恢复文档 {#restore-documents}

Workfront管理员现在可以恢复过去30天内删除的单个文档。 

在此更改之前，Workfront管理员只能恢复项目、任务和问题（包括随删除的项目、任务或问题一起删除的文档）。

有关详细信息，请参阅[还原已删除的项](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

## 包含发行信息的新预览横幅 {#new-preview-banner-with-release-information}

预览沙盒环境顶部的蓝色横幅现在显示预览环境的版本名称和版本号。 单击版本的名称将会转到帮助站点文章，您可以在该文章中找到有关当前预览版本的更多信息。 有关预览Sandbox环境的详细信息，请参阅[Adobe Workfront预览Sandbox环境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) 

## API 7可用性 {#api-7-availability}

API 7现已可用，其中包含新的和更新的对象。

有关详细信息，请参阅[API版本7](../../../../wf-api/api/new-api-version-7.md)中的新增功能。

## 订阅任务和问题 {#subscribe-to-tasks-and-issues}

Workfront会发送有关您分配到的项目或您拥有的项目的通知。

从当前版本开始，如果您希望关注未分配给您但可能影响工作的项目，则可以订阅这些项目。

您可以订阅您至少有权查看的问题和任务。 当新评论添加到您订阅的问题或任务时，您将收到有关该评论的电子邮件通知。

有关订阅问题和任务的更多信息，请参阅[在Adobe Workfront中订阅项目](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## 资源计划改进 {#resource-scheduling-improvements}

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器计划资源的信息，请参阅[工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

在计划资源时，有以下改进可用：

* [在单个视图中查看资源计划时间线上的更多项目](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [将项目名称配置为在计划时间线的任务和问题上显示](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [配置是否将父任务显示在计划时间线上](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline)
* [更轻松地展开或折叠计划时间线上的所有任务和问题](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [滚动时，角色和用户信息将保留在计划时间线的顶部](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### 在单个视图中查看资源计划时间线上的更多项目 {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

在为团队或您担任其资源管理器的任何项目计划资源时，任务和问题现在占用的计划时间表的垂直空间更少。 这允许您在单个视图中查看更多任务和问题。

如果您决定在时间表上显示每个任务和问题的项目名称，则会扩展每个任务和问题的垂直空间，从而减少在单个视图中显示的任务和问题。

有关计划资源的详细信息，请参阅  “开始使用资源计划”。

### 将项目名称配置为在计划时间线的任务和问题上显示 {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

在为团队或您担任其资源经理的任何项目计划资源时，您现在可以将项目名称配置为显示在计划时间线上的每个任务和问题中。 这样，用户就可以查看时间表以快速查看任务或问题所在项目的名称。

有关详细信息，请参阅“开始使用资源计划”。

### 配置是否将父任务显示在计划时间线上 {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

在为您是资源经理的项目计划资源时，您现在可以配置当项目的“摘要完成模式”选项设置为“手动”时，父任务是否显示在计划时间线上。

在此更改之前，当项目的“摘要完成模式”设置为“手动”时，父任务始终显示在计划时间线上。 

当项目的“摘要完成模式”设置为“自动”时，父任务不能显示在计划时间线上。 这种体验没有改变。

有关详细信息，请参阅“开始使用资源计划”。

### 更轻松地展开或折叠计划时间线上的所有任务和问题 {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

提供了一个新链接，通过该链接可以更轻松地折叠计划时间线上的所有任务和问题。

有关详细信息，请参阅“开始使用资源计划”。

### 滚动时，角色和用户信息将保留在计划时间线的顶部 {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

现在，当在计划时间轴上向下滚动以查看其他信息时，角色名称和用户名保持在计划时间轴上的用户和角色区域的顶部，从而更容易查看任务和问题相关联的用户和角色。

在此更改之前，角色名称和用户名将从当前视图中滚出。

有关计划资源的详细信息，请参阅  “开始使用资源计划”。

## 比较验证 {#compare-proofs}

现在，您可以在任意单个文档列表（如项目、任务、问题、项目组合中的“文档”选项卡）中或全局导航栏中的主“文档”区域中比较两个文档校样。 

这两个校样显示在审阅和批准工具中，您可以在并排视图中比较每个文档时对其进行校样。

有关详细信息，请参阅[比较验证](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md)。

## 用于用户和项目的资源池的新字段 {#new-field-for-resource-pools-for-users-and-projects}

R1.5版本在预览环境中引入了与资源规划相关的新功能。 此功能允许您创建新的资源池，这些资源池是用户的集合。

现在，您可以将这些资源池与项目以及用户关联。 现在，您将在项目以及用户对象中看到一个名为“资源池”的新字段。

有关新的资源池以及它们如何与项目和用户关联的更多信息，请参阅[资源池概述](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## 更新了“功能板列表”中的外观 {#updated-look-and-feel-in-the-dashboard-list}

现在，查看仪表板列表时，外观会更加新颖，而且可扩展性也更高。

此功能以前仅适用于已注册提前访问的用户。 该功能现在适用于预览环境中的所有用户。 该版本将在2017.2版本中提供给生产环境中的所有用户。 

有关仪表板的详细信息，请参阅[创建仪表板](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)。

## 删除Workfront中的认可功能 {#removing-the-endorsements-functionality-in-workfront}

在评估更新流中包含的功能时，我们已确定认可是一种低采用率和低使用率功能。 在2017.2中，从2017.2版本开始，将从Workfront中删除以下关于认可的功能（此功能在预览中不再可用）：

* 用户配置文件区域中的“认可”选项卡；
* 认可对象将从API Explorer中删除；如果您当前正在为对象“认可”或“认可共享”提取API报表，则在删除此对象后，调用将无效。

以下功能将继续保留在Web应用程序中：

* 在删除此功能之前由其他用户进行的用户认可，将保留在认可者的更新流中。 

认可不是可报告的对象，因此该对象的报告没有任何变化。

## 使用拖放操作对任何列表中的列重新排序（即将删除功能） {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

在2017.2版本中，通过将列从一个位置拖放到另一个位置来更改任何列表中列顺序的功能将从生产环境中的抢先访问中删除，并将不再可供任何用户使用。 

有关此功能的更多详细信息，请参阅[修改列宽和顺序](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)。
