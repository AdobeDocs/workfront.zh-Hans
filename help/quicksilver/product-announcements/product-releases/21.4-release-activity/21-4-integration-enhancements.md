---
title: 21.4集成增强功能
description: 21.4集成增强功能
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# 21.4集成增强功能

本页介绍了21.4版本对“预览”环境的所有集成增强。 这些增强功能将在2021年10月4日当周的生产环境中提供。

有关21.4版本可用的所有更改列表，请参阅 [21.4版本概述](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## 从Dropbox业务链接文档

我们已将Dropbox业务添加为可用的文档集成。 现在，您可以直接从Workfront内部访问存储在Dropbox业务中的文档。

Dropbox业务允许您链接共享文档并将文档上传到共享文件夹。 Dropbox(而非Dropbox业务)仅允许文档所有者在Workfront中查看文档。

您的Workfront管理员可以为贵组织启用此集成。

有关详细信息，请参阅 [链接来自外部应用程序的文档](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

有关Workfront管理员如何启用此选项的信息，请参阅 [配置文档集成](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## 更新了用于Slack的Workfront

用于Slack集成的Workfront中现在会显示以下更新：

* 适用于Slack的Workfront具有全新外观。
* 现在您会实时收到Workfront的Slack通知。

  例如，如果您被分配到某个任务，则会在分配后立即收到该通知。 以前，通知出现在Slack中之前可能会延迟。

此更新要求您重新授权Workfront以进行Slack集成。 有关授权集成的信息，请参阅 [为Slack配置Adobe Workfront](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

有关用于Slack通知的Workfront的更多信息，请参阅 [在Slack中接收Adobe Workfront通知](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## 在同意Adobe Workfront集成时，可以更清楚地查看帐户访问的详细信息

Adobe Workfront集成的同意屏幕现已更新。 现在，您可以查看集成有权访问的特定操作和区域，以便更好地了解您允许集成或应用程序访问的内容。

这个新的同意屏幕适用于任何使用OAuth 2.0的Adobe Workfront集成。

有关特定集成的详细信息，请参阅该集成的文档。

## 集成不再需要进行API密钥身份验证

Workfront集成最近开始使用OAuth2来提高安全性和可用性。 作为此移动的一部分，Workfront不再需要使用API密钥进行集成身份验证。
