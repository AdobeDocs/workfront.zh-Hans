---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront用户凭据与SAML用户凭据
description: 创建用户后，可以编辑用户并启用“仅允许SAML 2.0身份验证”，以便其用户和密码由SAML系统控制。 启用此选项后，用户仅允许通过SAML登录。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
TQID: https://experienceleague.adobe.com/8paS2GIumamOltxTC8Gw2mBZ4bKB6TOgbly7IBPKhDw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 0%

---

# Adobe Workfront用户凭据与SAML用户凭据

本文专门针对[!DNL Adobe Workfront]和SAML，并未介绍其他SSO身份验证方法。

在数据库中，[!DNL Workfront]将eawch用户的电子邮件地址作为其[!DNL Workfront]用户名以及其[!DNL Workfront]密码存储。 这些凭据在“预览”和“自定义刷新”沙盒中复制。

在用户创建期间，如果[!DNL Workfront]检测到已配置SAML 2.0，它将默认为用户的“仅允许SAML 2.0身份验证”。 如果启用了“向此人发送邀请电子邮件”框，[!DNL Workfront]将禁用“仅允许SAML 2.0身份验证”并隐藏此选项。 启用“向此人发送邀请电子邮件”后，该用户将成为非SAML [!DNL Workfront]用户。

创建用户后，您可以编辑用户并启用&#x200B;**[!UICONTROL 仅允许SAML 2.0身份验证]**，以便其用户和密码由SAML系统控制。

完成后，用户只能通过SAML登录。 当他们转到[!DNL Workfront] URL时，会自动重定向到SAML系统并提示输入他们的SAML用户名和密码。

SAML凭据存储在外部SAML系统中，如Microsoft的ADFS，而不是存储在Workfront中。
