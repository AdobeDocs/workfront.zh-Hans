---
title: 22.2集成增强功能
description: 22.2集成增强功能
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# 22.2集成增强功能

本页介绍了在“预览”环境的22.2版本中所做的所有集成增强。 这些增强功能将在生产环境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日这一周。

有关2.2版本中可用的所有更改的列表，请参阅 [22.2版本概述](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Adobe Workfront与Anaplan集成现已可用

为了让您能够更灵活地对Workfront项目的财务方面进行分析，Workfront现在可以与您的Anaplan帐户集成。 通过将Workfront对象链接到Anaplan对象，您可以自动更新两个帐户之间的信息，以确保两者中的信息都是最新的且相同。 您还可以在Anaplan中根据Workfront中的操作触发自动化流程（反之亦然）。

例如，您可以在Anaplan中创建营销活动，然后创建链接到该营销活动的Workfront项目或项目群。 然后，可以将在Workfront中跟踪的任何成本上传回Anaplan，以查看促销活动效果。

您可能考虑使用Workfront与Anaplan集成的其他工作流包括：

* 从新的Workfront项目创建Anaplan预算请求
* 从新的Anaplan列表项创建Workfront项目
* 从Workfront项目启动Anaplan供应商请求

有关更多信息，请参阅 [Adobe Workfront和Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Workfront for Experience Manager增强的连接器更新

Workfront for Experience Manager增强连接器现在包括以下更新：

* 现在，即使存在多个项目链接文件夹配置，您也可以在Adobe Workfront和Adobe Experience Manager Assets之间as a Cloud Service创建链接文件夹。
* 添加了对事件订阅分页的支持
* 添加了对AEM 6.4.x的支持
* 添加了对代理环境的支持
* 根据合作伙伴和客户反馈进行的若干错误修复

有关更多信息，请参阅 [Workfront for Experience Manager增强连接器概述](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>此连接器的部署和配置需要经过认证的合作伙伴。 请参阅 [安装Workfront for Experience Manager增强连接器](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install.html?lang=en#) 以了解更多信息。

## Adobe Creative Cloud集成现在使用OAuth2

为了提高安全性并在集成中提供更加一致的体验，我们更新了Adobe Creative Cloud集成以使用OAuth2身份验证，这是一种行业标准的用户身份验证方式。 现在，当您的用户登录时，他们可以看到集成有权访问和允许访问的特定操作和区域。 在此之后，用户无需频繁登录。

有关更多信息，请参阅 [使用适用于Illustrator的Workfront扩展和InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## 请参阅自定义OAuth2或JWT集成的客户端密钥详细信息

为了在使用自定义OAuth2和JWT集成时提供透明度，我们允许您查看集成使用的客户端密钥的详细信息。 现在，您可以看到客户端密钥的创建日期和上次使用日期。 您还可以添加和查看您自己有关客户端密钥的说明。

以前，这些详细信息不可用。

有关OAuth2或JWT自定义集成中客户端密钥的更多信息，请参阅 [为Workfront集成创建OAuth2应用程序](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## 请参阅自定义OAuth2应用程序列表中的身份验证类型

现在，在查看组织中的自定义OAuth2应用程序列表时，您可以查看每个应用程序是使用用户身份验证还是服务器身份验证。

以前，您只能通过转到每个应用程序上的编辑选项来查看此信息。

有关更多信息，请参阅 [为Workfront集成创建OAuth2应用程序](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## 在您的自定义OAuth2集成中为刷新令牌设置过期时间

为更好地控制自定义OAuth2集成的访问和安全性，您现在可以自定义刷新令牌的有效期。 用户的刷新令牌过期后，他们将需要再次登录到集成。

有关更多信息，请参阅 [为Workfront集成创建OAuth2应用程序](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## 在您的自定义OAuth2集成中为服务器到服务器应用程序使用公钥和私钥

您现在可以在自定义集成中设置服务器到服务器OAuth2应用程序。 通过设置公钥和私钥，您可以允许Workfront与其他应用程序通信，而无需使用登录凭据。

以前，您的自定义OAuth2应用程序中的所有身份验证都使用用户的登录凭据。

有关更多信息，请参阅 [为Workfront集成创建OAuth2应用程序](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Google G包集成现在使用OAuth2

为了提高安全性，并在各个集成之间提供更一致的体验，我们更新了Google G Suite集成，以使用OAuth2身份验证（一种用于身份验证用户的行业标准方法）。 现在，当您的用户登录时，他们可以看到集成有权访问和允许访问的特定操作和区域。 在此之后，用户无需频繁登录。

有关更多信息，请参阅 [登录和退出Adobe Workfront for G Suite](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
