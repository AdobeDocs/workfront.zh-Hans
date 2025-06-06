---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 疑难解答：使用Workfront for Outlook时出现outlookIdentityToken错误
description: 如果使用Workfront for Outlook时出现outlookIdentityToken错误，则必须为贵组织启用Microsoft 365旧版令牌。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 31%

---

# 疑难解答：使用Workfront for Outlook时出现outlookIdentityToken错误

>[!IMPORTANT]
>
>[Microsoft正在禁用对旧版Exchange联机令牌](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支持，Workfront Outlook加载项当前使用这些令牌进行身份验证。 Microsoft的这一更改已开始影响客户，并将在2025年10月之前继续分阶段推出。
>
>* **在Microsoft完全禁用这些令牌后，Workfront for Microsoft Outlook集成将无法再正常使用。**
>
>作为此更改的一部分，Microsoft已决定更改令牌的重新启用方式。 在&#x200B;**2025年6月30日**&#x200B;之后，管理员将无法再自行重新启用令牌 — 只有Microsoft支持部门可以授予例外。 **在2025年10月1日，将为所有租户关闭旧版令牌。 将不会授予例外。**

使用Workfront for Outlook时，您可能会看到以下错误：

```
Unexpected error
Unable to get the outlookIdentityToken
```

要解决此错误，您必须为您的组织启用 Microsoft 365 旧版令牌。因为这必须在 Microsoft 365 中完成，所以 Workfront 无法为您的组织启用这些令牌。

有关启用 Microsoft 365 旧版令牌的说明，请参阅 Microsoft 文档中的[打开或关闭旧版 Exchange Online 令牌](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off)。

有关旧版令牌的更多信息，请参阅[我可以重新打开 Exchange Online 旧版令牌吗？Microsoft 文档中的 ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on)。
