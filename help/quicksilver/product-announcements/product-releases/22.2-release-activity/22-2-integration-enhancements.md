---
title: 22.2集成增强
description: 22.2集成增强
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 22.2集成增强

本页介绍了22.2版本对“预览”环境的所有集成增强。 这些增强功能将在“生产”环境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日这一周。

有关22.2版本的所有可用更改列表，请参阅[22.2版本概述](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md)。

## Adobe Workfront与Anaplan集成现已可用

为了让您更灵活地了解Workfront项目的财务方面，Workfront现在可以与您的Anaplan帐户集成。 通过将Workfront对象链接到Anaplan对象，您可以自动更新这两个帐户之间的信息，确保这两个帐户中的信息都是最新且相同的。 您还可以根据Workfront中的操作在Anaplan中触发自动流程（反之亦然）。

例如，您可以在Anaplan中创建营销策划，然后创建链接到该营销策划的Workfront项目或项目。 在Workfront中跟踪的任何成本都可以上传回Anaplan以审查营销活动效果。

您可能考虑使用Workfront将Anaplan集成用于的其他工作流包括：

* 根据新的Workfront项目创建Anaplan预算请求
* 通过新的Anaplan列表项创建Workfront项目
* 从Workfront项目启动Anaplan供应商请求

有关详细信息，请参阅带有Anaplan的[Adobe Workfront](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md)。

## 用于Experience Manager增强型连接器更新的Workfront

Workfront for Experience Manager增强型连接器现在包含以下更新：

* 现在，即使存在多个项目链接文件夹配置，您也可以在Adobe Workfront和Adobe Experience Manager Assetsas a Cloud Service之间创建链接文件夹。
* 添加了对事件订阅分页的支持
* 添加了对AEM 6.4.x的支持
* 添加了对代理环境的支持
* 基于合作伙伴和客户反馈的多项错误修复

有关详细信息，请参阅[Workfront的Experience Manager增强型连接器概述](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md)。

>[!NOTE]
>
>此连接器的部署和配置需要经过认证的合作伙伴。 有关详细信息，请参阅[为Experience Manager增强型连接器安装Workfront](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install.html?lang=en#)。

## Adobe Creative Cloud集成现在使用OAuth2

为了提高安全性和跨集成实现更一致的体验，我们更新了Adobe Creative Cloud集成，以使用OAuth2身份验证（一种行业标准对用户进行身份验证的方式）。 现在，当您的用户登录时，他们可以看到集成有权访问的特定操作和区域，并且可以允许访问。 之后，他们无需频繁登录。

有关详细信息，请参阅[使用Workfront Extension for Illustrator和InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md)。

## 查看自定义OAuth2或JWT集成的客户端密钥的详细信息

为了让您透明地使用自定义OAuth2和JWT集成，我们让您能够查看集成使用的客户端密钥的详细信息。 现在，您可以查看客户端密钥的创建日期和上次使用日期。 您还可以添加和查看您自己的有关客户端密钥的注释。

以前，这些详细信息不可用。

有关OAuth2或JWT自定义集成中的客户端密钥的更多信息，请参阅[为Workfront集成创建OAuth2应用程序](../../../administration-and-setup/configure-integrations/create-oauth-application.md)。

## 在自定义OAuth2应用程序列表中查看身份验证类型

现在，当您查看组织中的自定义OAuth2应用程序列表时，可以查看每个应用程序是使用用户身份验证还是服务器身份验证。

以前，您只能通过进入每个应用程序上的编辑选项来查看此信息。

有关详细信息，请参阅[为Workfront集成创建OAuth2应用程序](../../../administration-and-setup/configure-integrations/create-oauth-application.md)。

## 在自定义OAuth2集成中设置刷新令牌的过期时间

为了更好地控制自定义OAuth2集成的访问和安全性，您现在可以自定义刷新令牌的有效期。 用户的刷新令牌过期后，他们需要再次登录到集成。

有关详细信息，请参阅[为Workfront集成创建OAuth2应用程序](../../../administration-and-setup/configure-integrations/create-oauth-application.md)。

## 在用于服务器到服务器应用程序的自定义OAuth2集成中使用公钥和私钥

您现在可以在自定义集成中设置服务器到服务器OAuth2应用程序。 通过设置公钥和私钥，您可以允许Workfront与另一个应用程序通信，而无需使用登录凭据。

以前，您的自定义OAuth2应用程序中的所有身份验证都使用用户的登录凭据。

有关详细信息，请参阅[为Workfront集成创建OAuth2应用程序](../../../administration-and-setup/configure-integrations/create-oauth-application.md)。

## Google Google Workspace集成现在使用OAuth2

为了提高安全性和跨集成实现更一致的体验，我们更新了Google Google Workspace集成，以使用OAuth2身份验证（一种行业标准对用户进行身份验证的方式）。 现在，当您的用户登录时，他们可以看到集成有权访问的特定操作和区域，并且可以允许访问。 之后，他们无需频繁登录。

有关详细信息，请参阅[登录和注销Google Workspace的Adobe Workfront](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md)。
