---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 启用Outlook for Office以用于 [!DNL Adobe Workfront] 和SAML 2.0
description: 如果您的 [!DNL Adobe Workfront] 系统与SAML 2.0集成，则必须为Office加载项启用SAML 2.0身份验证，以便用户能够使用其SAML 2.0凭据进行身份验证。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 72ffceb3-50f0-486e-92b5-0bea4c9a99c8
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# 启用[!DNL Outlook for Office]以与[!DNL Adobe Workfront]和SAML 2.0一起使用

>[!IMPORTANT]
>
>[Microsoft正在禁用对旧版Exchange联机令牌](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支持，Workfront Outlook加载项当前使用这些令牌进行身份验证。 Microsoft的这一更改已开始影响客户，并将在2025年10月之前继续分阶段推出。
>
>* **在Microsoft完全禁用这些令牌后，Workfront for Microsoft Outlook集成将无法再正常使用。**
>
>作为此更改的一部分，Microsoft已决定更改令牌的重新启用方式。 在&#x200B;**2025年6月30日**&#x200B;之后，管理员将无法再自行重新启用令牌 — 只有Microsoft支持部门可以授予例外。 **在2025年10月1日，将为所有租户关闭旧版令牌。 将不会授予例外。**

如果您的[!DNL Adobe Workfront]系统与SAML 2.0集成，则必须为[!DNL Office]加载项启用SAML 2.0身份验证，以便用户能够使用其SAML 2.0凭据进行身份验证。

如果您在使用SAML登录到[!DNL Workfront]时遇到问题，请联系您的[!DNL Workfront]管理员以确保正确配置SAML。

有关如何启用Office加载项以使用SAML 2.0解决方案进行身份验证的信息，请参阅[使用SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)配置Adobe Workfront文章中的部分。
