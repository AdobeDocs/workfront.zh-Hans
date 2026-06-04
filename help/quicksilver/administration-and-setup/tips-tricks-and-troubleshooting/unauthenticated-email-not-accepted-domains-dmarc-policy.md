---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 由于域的DMARC策略，未接受未经身份验证的电子邮件
description: 如果由于域的DMARC策略而不接受从 [!DNL Workfront] 系统发送的电子邮件，则电子邮件管理员可以通过将您的电子邮件系统配置为允许来自workfront.com的所有电子邮件来修复此问题。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
TQID: https://experienceleague.adobe.com/f44Wkid-gwfXgHKmSKa6oevhN5jA6720JTlOcH8kJKY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 177
ht-degree: 1%

---

# 由于域的DMARC策略，未接受未经身份验证的电子邮件

## 问题

[测试]我收到以下退回电子邮件：

550-5.7.1由于以下原因，不接受来自“customer domain.com”的未经身份验证的电子邮件\
550-5.7.1域的DMARC策略。 请联系“customer domain.com”的管理员\
550-5.7.1域（如果这是合法邮件）。 请访问\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690)了解DMARC\
550 5.7.1倡议。

## 解决方案

DMARC是在您公司的电子邮件系统中配置的，不是[!DNL Adobe Workfront]的一部分。 如果您收到此电子邮件，则需要联系电子邮件管理员。

您的电子邮件管理员应将您的电子邮件系统配置为允许/信任来自noreply@workfront.com的电子邮件，或最好是所有来自workfront.com的电子邮件。

有关DMARC的详细信息，请参阅[https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
