---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScalar设置可能会导致性能降低
description: 创建用户后，可以编辑用户并启用“仅允许SAML 2.0身份验证”，以便其用户和密码由SAML系统控制。 启用此选项后，用户仅允许通过SAML登录。
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 806a4c4835e47da4fbbdb28ec0c35c990f70239e
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Workfront： ZScalar设置可能会导致性能降低

>[!NOTE]
>
>这是ZScalar的一个问题，Workfront不会修复此问题。

默认情况下，ZScalar的Web服务使用`http/1.1`，这会导致Workfront中的性能降低。

要检查并解决此问题，请将ZScalar软件配置为使用`http/2`。 无法在Workfront中配置此设置。

您可以在ZScalar文档中找到有关`http/2`的信息。
