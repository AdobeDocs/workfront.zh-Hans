---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 2发行版活动
description: 本页介绍了2017.2 Beta 2版本在“预览”环境中提供的所有更改。 2017年5月24日，预览环境中提供了此页面上的功能。 该版本将于2017年7月底至8月初在“生产”环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# 2017.2 Beta 2发行版活动

本页介绍了2017.2 Beta 2版本在“预览”环境中提供的所有更改。 2017年5月24日，预览环境中提供了此页面上的功能。 该版本将于2017年7月底至8月初在“生产”环境中提供。

>[!IMPORTANT]
>
>此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2017.2版中所做所有更改的列表，请参阅[2017.2版活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md)。

2017.2 Beta 2版本包含面向Workfront管理员和其他用户的增强功能：

管理员的&#x200B;**：**

* [API增强功能：事件订阅](#api-enhancement-event-subscriptions)

所有用户&#x200B;**：**

* [订阅项目](#subscribe-to-projects)
* [取消订阅电子邮件中的项目](#unsubscribe-from-items-from-email)
* [配置里程碑在甘特图上的显示方式](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [资源池模板](#resource-pools-templates)
* [在Workfront中查看校对文档的版本](#view-versions-of-proofed-documents-within-workfront)
* [验证审批报告中的新请求者对象](#new-requester-object-in-proof-approval-report)

## API增强功能：事件订阅 {#api-enhancement-event-subscriptions}

当事件订阅支持的Workfront对象上发生操作时，您现在可以将Workfront配置为将响应发送到所需的端点。 这意味着您的集成可以与Workfront API实时交互。

有关详细信息，请参阅[事件订阅API](../../../../wf-api/general/event-subs-api.md)。 

## 订阅项目 {#subscribe-to-projects}

您现在可以订阅有关您不属于项目团队的项目的新注释。 在此版本之前，您只能订阅关于问题和任务的评论。

有关订阅项目的详细信息，请参阅[在Adobe Workfront中订阅项目](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## 取消订阅电子邮件中的项目 {#unsubscribe-from-items-from-email}

您可以使用订阅电子邮件中的“取消订阅”链接取消订阅项目。 以前，您只能从Workfront界面取消订阅项目。

有关取消订阅订阅电子邮件的更多信息，请参阅[Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md)中的“选择退出电子邮件通知”部分 

## 配置里程碑在甘特图上的显示方式 {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***更正&#x200B;**：此功能当前不在预览Sandbox环境中。 计划于稍后日期（2017年6月）发布。*

现在，可以使用两个选项来查看甘特图中的里程碑信息。 您可以配置以下里程碑指示器之一或两者：

* 里程碑菱形（图标）

  此图标显示在甘特图中与里程碑关联的任何任务之后。

* 里程碑线

  在甘特图的所有任务中，与里程碑关联的任何任务之后都会显示一条直线。

在此更改之前，只有一个选项允许里程碑显示在甘特图上，称为“里程碑”。 此选项同时启用了里程碑菱形图标和里程碑线。 无法分隔这些指示器。 这两个选项现在可用于所有甘特图，包括所有项目列表和报告。 

有关配置信息在甘特图中的显示方式的更多信息，请参阅[配置信息在甘特图中的显示方式](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)。

## 资源池模板 {#resource-pools-templates}

您现在可以为模板指定资源池。 在此版本之前，您只能将资源池与用户和项目相关联。

有关资源池的详细信息，请参阅[资源池概述](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## 在Workfront中查看校对文档的版本 {#view-versions-of-proofed-documents-within-workfront}

您现在可以在Workfront界面中查看已校对文档所有版本的校对。 

在此更改之前，您只能查看校对文档的最新版本。

没有验证许可证的用户可以：

* 在校对文档的先前版本上打开校对

拥有校对许可证的用户可以执行以下任一操作：

* 在校对文档的先前版本上打开校对
* 查看有关已验证文档的先前版本的验证详细信息

有关详细信息，请参阅[管理文档版本](../../../../documents/managing-documents/manage-document-versions.md)中的[管理文档版本](../../../../documents/managing-documents/manage-document-versions.md)。

## 验证审批报告中的新请求者对象 {#new-requester-object-in-proof-approval-report}

现在，创建验证审批报告时，存在新的请求者对象。 利用此对象，可报告有关请求验证审批的用户的信息。 

验证审批报告中的新请求者对象包含其他类型的对象报告中现有用户对象可用的所有字段。

>[!NOTE]
>
> 仅从首次将此功能引入相应的预览或生产环境开始，报告中才提供此信息；在引入此功能之前，报告中有关请求者对象的信息不可用。

您在创建验证审批报告时访问请求者对象，如[创建自定义报告](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中所述。

有关验证审批对象报告的详细信息，请参阅[了解Adobe Workfront中的对象](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)中的[了解Adobe Workfront中的对象](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)部分。
