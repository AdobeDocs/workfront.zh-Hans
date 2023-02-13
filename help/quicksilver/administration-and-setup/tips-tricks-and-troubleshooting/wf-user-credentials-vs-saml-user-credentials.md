---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront用户凭据与 [!DNL SAML] 用户凭据
description: 在用户创建后，您可以编辑用户并启用“仅允许SAML 2.0身份验证”，以便其用户和密码由SAML系统控制。 启用此选项后，用户只能通过SAML登录。 当他们转到 [!DNL Workfront] URL中，SAML系统会自动将其重定向到SAML系统，并提示输入其SAML用户名和密码。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Adobe Workfront用户凭据与SAML用户凭据

本文特别着重于 [!DNL Adobe Workfront] 和SAML，且不涵盖其他SSO身份验证方法。

在数据库中， [!DNL Workfront] 将eawch用户的电子邮件地址作为 [!DNL Workfront] 用户名及其 [!DNL Workfront] 密码。 这些凭据会复制在“预览”和“自定义刷新”沙箱中。

在用户创建期间(如果 [!DNL Workfront] 检测到已配置SAML 2.0，则该SAML 2.0默认为用户的“仅允许SAML 2.0身份验证”。 如果启用了“向此人发送电子邮件邀请”框， [!DNL Workfront] 禁用“仅允许SAML 2.0身份验证”并隐藏此选项。 启用“向此人发送邀请电子邮件”后，用户将变为非SAML [!DNL Workfront] 用户。

用户创建后，您可以编辑用户并启用 **[!UICONTROL 仅允许SAML 2.0身份验证]** 以便其用户和密码由SAML系统控制。

完成后，用户只能通过SAML登录。 当他们转到 [!DNL Workfront] URL中，SAML系统会自动将其重定向到SAML系统，并提示输入其SAML用户名和密码。

SAML凭据存储在外部SAML系统(如Microsoft的ADF)中，而不存储在Workfront中。
