---
title: 21.4集成增强功能
description: 21.4集成增强功能
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# 21.4集成增强功能

本页介绍了在“预览”环境的21.4版本中所做的所有集成增强。 这些增强功能将于2021年10月4日这一周的生产环境中提供。

有关21.4版本中可用的所有更改的列表，请参阅 [21.4版本概述](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## 从Dropbox业务链接文档

我们已将Dropbox业务作为可用的文档集成添加。 现在，您可以直接从Workfront内访问存储在Dropbox业务中的文档。

Dropbox业务允许您链接共享文档并将文档上传到共享文件夹。 Dropbox(非Dropbox业务)仅允许文档所有者在Workfront中查看文档。

您的Workfront管理员可以为您的组织启用此集成。

有关详细信息，请参阅 [从外部应用程序链接文档](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

有关Workfront管理员如何启用此选项的信息，请参阅 [配置文档集成](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## 更新了Workfront以供Slack

现在，Workfront中提供了以下更新以用于Slack集成：

* Workfront的Slack有了新的外观。
* 现在，您将实时收到Workfront以获取Slack通知。

   例如，如果您被分配到任务，则在您被分配后，您会立即收到该通知。 以前，在通知显示在Slack之前可能会有延迟。

此更新要求您重新授权Workfront以进行Slack集成。 有关授权集成的信息，请参阅 [配置Adobe Workfront以Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

有关WorkfrontSlack通知的更多信息，请参阅 [在Slack中接收Adobe Workfront通知](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## 在同意Adobe Workfront集成时，请更清楚地查看帐户访问的详细信息

现在，更新了Adobe Workfront集成的同意屏幕。 现在，您可以查看集成有权访问的特定操作和区域，以便更好地了解允许集成或应用程序访问的内容。

此新的同意屏幕适用于使用OAuth 2.0的任何Adobe Workfront集成。

有关特定集成的详细信息，请参阅该集成的文档。

## 集成不再需要API密钥身份验证

Workfront集成最近开始使用OAuth2，以提高安全性和可用性。 作为此步骤的一部分，Workfront不再需要API密钥来进行集成身份验证。
