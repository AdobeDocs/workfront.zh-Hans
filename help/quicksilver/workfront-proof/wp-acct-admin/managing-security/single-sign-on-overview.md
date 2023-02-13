---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: 单点登录 [!DNL Workfront Proof]
description: 单点登录(SSO)允许您的用户登录 [!DNL Workfront Proof] 使用贵组织的现有用户名和密码。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# 单点登录 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

安 [!UICONTROL 企业] [!DNL Workfront] 使用此功能需要计划。 有关各种可用计划的更多信息，请参阅 [Workfront计划](https://www.workfront.com/plans).

单点登录(SSO)允许您的用户登录 [!DNL Workfront Proof] 使用贵组织的现有用户名和密码。

要提供此功能，我们使用 [!DNL Security Assertion Markup Language] (SAML)2.0，一种基于XML的协议，允许您授权数据并在身份提供者与Web服务之间进行身份验证和交换身份验证。

这意味着您将针对自己的登录系统进行身份验证，而不是针对 [!DNL Workfront Proof]的登录页面。

您必须在 [!DNL Workfront] 用于启用SAML的校样帐户：

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* 有关完全自定义域的更多信息，请参阅  [品牌 [!DNL Workfront Proof] 站点 — 高级](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

请参阅 [为配置单点登录 [!DNL Workfront Proof] 用户](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) 有关在帐户中设置单点登录的信息。
