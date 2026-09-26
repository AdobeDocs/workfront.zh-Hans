---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScaler设置可能会导致性能降低
description: 创建用户后，可以编辑用户并启用“仅允许SAML 2.0身份验证”，以便其用户和密码由SAML系统控制。 启用此选项后，用户仅允许通过SAML登录。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
TQID: 'https://experienceleague.adobe.com/-3-p8fzXIiV-gnjIjhRzBmLfspAEEVAuD2lpmcsVjLA'
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
source-wordcount: '107'
ht-degree: 44%
---
# Workfront：ZScaler 设置可能会导致性能下降

>[!NOTE]
>
>这是 ZScaler 的问题，Workfront 不会修复。

ZScaler 的 Web 服务默认使用 `http/1.1`，这会导致 Workfront 的性能下降。

要检查并解决此问题，请将ZScaler软件配置为使用`http/2`。 这无法在 Workfront 中配置。

您可以在 ZScaler 文档中找到有关 `http/2` 的信息。
