---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 疑难解答：使用Workfront for Outlook时出现outlookIdentityToken错误
description: 如果使用Workfront for Outlook时出现outlookIdentityToken错误，则必须为贵组织启用Microsoft 365旧版令牌。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 43%

---

# 疑难解答：使用Workfront for Outlook时出现outlookIdentityToken错误

>[!IMPORTANT]
>
>[Microsoft已禁用对旧版Exchange Online令牌的支持](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)，Workfront Outlook加载项已使用这些令牌进行身份验证。 Microsoft的此更改将分阶段推出，并自2025年10月1日起完成。
>
>**由于Microsoft已禁用这些令牌，因此Workfront for Microsoft Outlook集成不再起作用。**

使用Workfront for Outlook时，您可能会看到以下错误：

```
Unexpected error
Unable to get the outlookIdentityToken
```

要解决此错误，您必须为您的组织启用 Microsoft 365 旧版令牌。因为这必须在 Microsoft 365 中完成，所以 Workfront 无法为您的组织启用这些令牌。

有关启用 Microsoft 365 旧版令牌的说明，请参阅 Microsoft 文档中的[打开或关闭旧版 Exchange Online 令牌](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off)。

有关旧版令牌的更多信息，请参阅[我可以重新打开 Exchange Online 旧版令牌吗？Microsoft 文档中的 ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on)。
