---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront用户凭据与 [!DNL SAML] 用户凭据
description: 创建用户后，可以编辑用户并启用“仅允许SAML 2.0身份验证”，以便其用户和密码由SAML系统控制。 启用此选项后，用户仅允许通过SAML登录。 当他们转到 [!DNL Workfront] URL时，会自动重定向到SAML系统并提示输入他们的SAML用户名和密码。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Adobe Workfront用户凭据与SAML用户凭据

本文专门针对[!DNL Adobe Workfront]和SAML，并未介绍其他SSO身份验证方法。

在数据库中，[!DNL Workfront]将eawch用户的电子邮件地址作为其[!DNL Workfront]用户名以及其[!DNL Workfront]密码存储。 这些凭据在“预览”和“自定义刷新”沙盒中复制。

在用户创建期间，如果[!DNL Workfront]检测到已配置SAML 2.0，它将默认为用户的“仅允许SAML 2.0身份验证”。 如果启用了“向此人发送邀请电子邮件”框，[!DNL Workfront]将禁用“仅允许SAML 2.0身份验证”并隐藏此选项。 启用“向此人发送邀请电子邮件”后，该用户将成为非SAML [!DNL Workfront]用户。

创建用户后，您可以编辑用户并启用&#x200B;**[!UICONTROL 仅允许SAML 2.0身份验证]**，以便其用户和密码由SAML系统控制。

完成后，用户只能通过SAML登录。 当他们转到[!DNL Workfront] URL时，会自动重定向到SAML系统并提示输入他们的SAML用户名和密码。

SAML凭据存储在外部SAML系统中，如Microsoft的ADFS，而不是存储在Workfront中。
