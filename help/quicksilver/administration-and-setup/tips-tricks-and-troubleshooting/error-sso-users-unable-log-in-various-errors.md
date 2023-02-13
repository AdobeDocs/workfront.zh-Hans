---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '错误：SSO用户无法登录到 [!DNL Adobe Workfront] 由于各种错误'
description: 当您收到有关联合单点登录、用户名/密码组合或 [!DNL Workfront], the problem might be that your [!DNL Workfront] 实例使用单点登录(SSO)，而您尝试使用不正确的URL登录。 确保使用正确的URL登录，而“.com”之后没有任何内容。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 13%

---

# 错误：SSO用户无法登录到 [!DNL Adobe Workfront] 由于各种错误

## 问题

我无法登录 [!DNL Workfront] 并收到以下错误之一：

* 抱歉，您无法访问 [!DNL Workfront] 通过此登录屏幕。 [!DNL Workfront] 已为使用SAML 2.0的联合单点登录设置。请与 [!DNL Workfront] 管理员。
* 该用户名/密码组合不太正确。确保您的大写锁定没有打开。
* 抱歉，您无权访问 [!DNL Workfront]. 请联系您的 [!DNL Workfront] 管理员以获取用户名和密码。

## 解决方案

您的 [!DNL Workfront] 实例使用单点登录，而您尝试通过不正确的URL登录。 确保您使用正确的URL登录，而“.com”之后没有任何内容

>[!TIP]
>
>删除任何现有的具有无效URL的书签。
