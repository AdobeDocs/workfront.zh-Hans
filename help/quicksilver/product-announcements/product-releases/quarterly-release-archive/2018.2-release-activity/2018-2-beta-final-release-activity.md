---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta最终发行版活动
description: 本页介绍了2018.2 Beta Final版本在“预览”环境中最近提供的所有更改。 2018年6月20日，该功能在预览环境中提供。 该版本将于2018年7月在生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 36001571-bf8c-4fe8-a66b-09d3726f66d3
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# 2018.2 Beta最终发行版活动

本页介绍了2018.2 Beta Final版本在“预览”环境中最近提供的所有更改。 2018年6月20日，该功能在预览环境中提供。 该版本将于2018年7月在生产环境中提供。

>[!IMPORTANT]
>
> 此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2018.2版中所做所有更改的列表，请参阅  [2018.2发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md)。

以下新功能将在18.2生产版本发布时发布：

* [指定用于回复Workfront电子邮件通知的邮件传递服务](#specify-mail-delivery-services-for-replying-to-workfront-email-notifications)
* [接收有关文档评论的电子邮件通知](#receive-email-notifications-for-comments-on-documents)
* [系统跟踪的更新不再包含图标](#system-tracked-updates-no-longer-contain-an-icon)
* 将评论转换为任务的[选项已删除](#option-to-convert-a-comment-to-a-task-was-removed)
* 用于Salesforce的[Workfront](#workfront-for-salesforce)
* [WorkfrontSlack改进](#workfront-for-slack-improvements)
* [移动改进](#mobile-improvements)

## 指定用于回复Workfront电子邮件通知的邮件传递服务 {#specify-mail-delivery-services-for-replying-to-workfront-email-notifications}

现在，在配置Workfront以允许用户通过电子邮件回复对对象进行注释时，Workfront管理员可以选择邮件投放服务。 可以将Workfront配置为使用默认电子邮件服务或POP电子邮件帐户。

在此更新之前，Workfront管理员需要为每个用户设置POP帐户。 

有关配置POP电子邮件帐户的信息，请参阅。

有关默认邮件服务的更多信息，请参阅。

## 接收文档评论的电子邮件通知 {#receive-email-notifications-for-comments-on-documents}

现在，当有人对您拥有的文档发表评论时，您将收到电子邮件通知。 此选项默认处于启用状态。 您可以使用“我的文档中添加了注释”通知设置来禁用电子邮件通知选项。

在此更改之前，当有人对您拥有的文档发表评论时，您未收到任何通知。 

有关详细信息，请参阅[修改您自己的电子邮件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

>[!NOTE]
>
>最初发布此功能时，用户除了收到电子邮件通知外，还会收到应用程序内通知。 当有人对您拥有的文档发表评论时，您将不再收到应用程序内通知。 

## 系统跟踪的更新不再包含图标 {#system-tracked-updates-no-longer-contain-an-icon}

每当Workfront系统在对象（例如项目中的）的更新区域中创建更新时，该更新不再包含相应的图标。

在此更改之前，任何系统更新还包括一个图标，表示已进行的更新。

有关系统更新的详细信息，请参阅[系统跟踪的更新](../../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)。

## 将评论转换为任务的选项已删除 {#option-to-convert-a-comment-to-a-task-was-removed}

已删除将评论转换为任务的选项。

以前，您可以在对象的“更新”区域将注释转换为任务。

## 适用于Salesforce的Workfront {#workfront-for-salesforce}

我们将发布Salesforce与Workfront之间全新的现成集成。 您将能够执行以下操作：

* 当Salesforce Opportunity达到某个阶段、将新Product添加到Opportunity或更新帐户类型时，自动创建新的Workfront项目。
* 从Salesforce Opportunity或Account创建Workfront请求。

此集成将可供拥有Workfront Pro版本或更高版本的所有客户使用，并且将是免费的。

有关Workfront for Salesforce的更多信息，请参阅  用于Salesforce的[Adobe Workfront](../../../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce.md)。

## WorkfrontSlack改进 {#workfront-for-slack-improvements}

您可以将配置为在SlackWorkfront渠道中接收Workfront通知。

也可以将以下Workfront通知配置为以Slack发送：

* 当有人在评论或更新中为您标记时。
* 当您分配到新任务或问题时。
* 您收到批准项目的请求时。

在此改进之前，您无法在Slack中接收Workfront通知。

有关Slack中Workfront通知的更多信息，请参阅[在Slack中接收Adobe Workfront通知](../../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md)。

## 移动改进 {#mobile-improvements}

18.2生产版本发布时，以下新功能将会发布到移动商店：

* 对象名称的内联编辑 

  您现在可以在移动应用程序中内联编辑字段，例如项目、任务或问题的名称。

* 上传文档 

  您现在可以将文档上传到Workfront移动设备应用程序中的对象。

* 上传个人资料图片 

  您现在可以在iOS移动应用程序中上传用户档案照片。

  此功能将仅适用于iOS移动设备应用程序。

以下功能已发布到Android Beta版本的Workfront移动应用程序，并且还将发布到公共Android和iOS移动应用程序。 iOS平台的Experience与已发布的Android体验包含以下差异：

* 新的iOS底部导航栏 

* iOS的新教程体验 

有关这些功能的更多信息以及观看演示这些功能的视频，请参阅[2018.2 Beta 4发布活动](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-beta-4-release-activity.md)和[2018.2 Beta 5发布活动](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-beta-5-release-activity.md)。
