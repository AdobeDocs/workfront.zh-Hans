---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: ' [!DNL Workfront Proof]中的单点登录'
description: 单点登录(SSO)允许您的用户使用您组织的现有用户名和密码登录 [!DNL Workfront Proof] 。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# [!DNL Workfront Proof]中的单点登录

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

需要[!UICONTROL Enterprise] [!DNL Workfront]计划才能使用此功能。 有关各种可用计划的详细信息，请参阅[Workfront计划](https://www.workfront.com/plans)。

单点登录(SSO)允许您的用户使用您组织的现有用户名和密码登录[!DNL Workfront Proof]。

为了提供此功能，我们使用[!DNL Security Assertion Markup Language] (SAML) 2.0，它是一种基于XML的协议，允许您在身份提供程序和Web服务之间授权数据和交换身份验证。

这意味着您将针对自己的登录系统，而不是[!DNL Workfront Proof]的登录页面进行身份验证。

您必须在[!DNL Workfront]验证帐户上设置自定义子域或域才能启用SAML：

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* 您可以在[品牌 [!DNL Workfront Proof] 站点 — 高级](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md)中阅读有关完全自定义域的详细信息。

有关在您的帐户上设置SSO的信息，请参阅[为 [!DNL Workfront Proof] 用户配置单点登录](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md)。
