---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1校对增强功能
description: 本页介绍了2019.1版本中包含的所有验证增强功能。 该功能现已在“生产”环境中可用。
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 6b9b847c-dfb5-4285-b8fc-72f33c6a54d0
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# 2019.1校对增强功能

本页介绍了2019.1版本中包含的所有验证增强功能。 该功能现已在“生产”环境中可用。

有关2019.1版中所做所有更改的列表，请参阅 [2019.1发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## 适用于管理员

* [为打开验证的非收件人配置默认验证角色](#configure-default-proofing-role-for-non-recipients-who-open-a-proof)

## 适用于所有用户

* [在Web验证查看器中验证交互式内容](#proof-interactive-content-in-the-web-proofing-viewer)
* [现在，校对查看器中注释的默认排序顺序是从“最旧到最新”](#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest)
* [增强了在验证查看器中与一系列视频关联的评论的查看功能](#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video)
* [从验证通知或验证查看者链接到文档详细信息](#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer)
* [在验证查看器中更改电子邮件通知](#change-your-email-notifications-in-the-proofing-viewer)
* [在桌面校对查看器中更改背景颜色](#change-the-background-color-in-the-desktop-proofing-viewer)
* [在桌面验证查看器中从验证中清除缓存的浏览器数据](#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer)

## 为打开验证的非收件人配置默认验证角色 {#configure-default-proofing-role-for-non-recipients-who-open-a-proof}

Workfront管理员现在可以为以下用户配置默认验证角色：在验证工作流中不是指定的收件人，但可通过其Workfront对象（如项目、任务或问题）访问验证。

以前，当用户和访客有权访问验证而没有添加到其工作流时，他们的默认验证角色是查看者。

此功能仅适用于在Workfront中创建的验证，而不适用于Workfront Proof。

## 在Web验证查看器中验证交互式内容 {#proof-interactive-content-in-the-web-proofing-viewer}

如果贵组织的安全策略不允许使用独立的桌面验证查看器应用程序，则您的Workfront管理员现在可以在Web验证查看器中启用交互式内容。 在创建验证之前，必须将内容捆绑到ZIP文件中。

有关更多信息，请参阅文章中的。

视频

## 现在，校对查看器中注释的默认排序顺序是从“最旧到最新”  {#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest}

在验证查看器中，验证评论的默认排序顺序现在为“最旧到最新”，就像在口头对话中一样。

以前，默认排序顺序是最新到最旧。

您可以选择其他排序选项，系统会记住您打开的所有其他校样。

有关更多信息，请参阅文章中的部分。

## 增强了在验证查看器中与一系列视频关联的评论的查看功能 {#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video}

现在，当您在校对查看器中查看与一系列视频素材关联的注释时，可以单击“播放”来查看整个素材范围。 播放到达范围结尾时会暂停。 评论保持打开状态，这样您就不会丢失对位置的跟踪。

以前，打开一系列视频素材的注释时，您必须通过查看注释上显示的帧号来手动查找范围的起点，然后再单击“播放”。 否则，验证查看器将开始播放您上次在视频时间轴中单击的任何位置，并且未在范围结束时暂停。 此外，当您单击“播放”时，评论会折叠，因此不再清楚您正在查看哪条评论。

有关查看视频校样的信息，请参阅。

视频

## 从验证通知或验证查看者链接到文档详细信息 {#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer}

当您收到电子邮件邀请您查看验证，或者您在验证查看器中查看验证时，您现在可以快速访问验证的文档详情页面。 在此页面上，您可以看到与验证关联的Workfront对象（例如任务、项目或问题）。 这提供了上下文以帮助您了解需要对验证所做的工作。

此功能可能仅适用于您添加到系统的新用户。 此问题是暂时的。

有关更多信息，请参阅文章。

视频

## 在验证查看器中更改电子邮件通知 {#change-your-email-notifications-in-the-proofing-viewer}

现在，所有校对查看者都可以指定他们要接收哪些校对通知。 在与外部利益相关者合作时，这一点尤其重要。

以前，只有验证所有者或流量管理员可以为添加到验证的查看者配置验证的电子邮件警报。 外部协作者无法控制他们收到了哪些有关验证的电子邮件警报，因为他们既没有访问Workfront所需的权限，也没有适当的权限级别。

这些设置不同于您可以在Workfront中配置的电子邮件警报设置。

有关更多信息，请参阅 [管理验证评论和决策的通知](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md)

视频

## 在桌面校对查看器中更改背景颜色 {#change-the-background-color-in-the-desktop-proofing-viewer}

现在，您可以将桌面校对查看器的背景颜色从默认的近黑色更改为白色。 这使得查看具有透明背景的校对内容变得更容易。

有关更多信息，请参阅 [配置校对查看器设置](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

视频

## 在桌面验证查看器中从验证中清除缓存的浏览器数据 {#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer}

当浏览器的Cookie和缓存设置设置为阻止弹出窗口等内容时，这种阻止行为也会在桌面验证查看器中发生，使查看者无法看到验证中的弹出内容并进行评论。

现在，您可以清除可能随验证一起保存的浏览器缓存数据，以便所有内容都显示在桌面验证查看器中，并且查看者可以在该查看器中查看和评论。

有关更多信息，请参阅 [配置校对查看器设置](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

视频
