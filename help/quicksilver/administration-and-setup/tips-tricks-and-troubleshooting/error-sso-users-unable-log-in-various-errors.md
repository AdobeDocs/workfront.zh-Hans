---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 错误：由于各种错误，SSO用户无法登录到[!DNL Adobe Workfront]
description: 当您收到有关联合单一登录、用户名/密码组合或访问[!DNL Workfront]的登录错误时，问题可能是您的[!DNL Workfront]实例使用了SSO，而您尝试使用错误的URL登录。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
TQID: 'https://experienceleague.adobe.com/8L78zoOjC2KgtVKTorhvWDd8MvaficRL2pZKOfrlGSs'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 4%
---
# 错误：由于各种错误，SSO用户无法登录到[!DNL Adobe Workfront]

## 问题

我无法登录到[!DNL Workfront]，并收到以下错误之一：

* 抱歉，您不能通过此登录屏幕访问[!DNL Workfront]。 [!DNL Workfront]设置为使用SAML 2.0进行联合单点登录。 请联系您的[!DNL Workfront]管理员。
* 该用户名/密码组合不正确。 请确保大写锁定未打开，然后重试。
* 抱歉，您无权访问[!DNL Workfront]。 请联系您的[!DNL Workfront]管理员以获取用户名和密码。

## 解决方案

您的[!DNL Workfront]实例使用SSO，并且您正尝试通过错误的URL登录。 确保您使用URL登录，而不使用“.com”之后的任何内容

>[!TIP]
>
>删除包含无效URL的任何现有书签。
