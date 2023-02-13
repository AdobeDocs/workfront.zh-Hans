---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 延迟校样电子邮件
description: 当校样接近截止日期或到达截止日期时，会向收件人发送延迟校样电子邮件。 无法在校样级别禁用这些类型的电子邮件，但可以在帐户和用户个人设置级别进行配置。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!UICONTROL 延迟校样] 电子邮件

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

的 [!UICONTROL 延迟校样] 当校样接近截止日期或到达截止日期时，会向收件人发送电子邮件。 无法在校样级别禁用这些类型的电子邮件，但可以在帐户和用户个人设置级别进行配置。

* [!UICONTROL 延迟校样] 当校样到达其截止时间，且并非所有审阅或决策都已做出时，会自动向审阅人发送电子邮件。

   默认情况下，这些电子邮件处于启用状态，无法针对整个帐户进行调整，但用户可以在其“校对”默认值中禁用这些电子邮件。

* 在校样接近截止时间时，会向审阅人发送有风险的电子邮件。 默认情况下，这些规则处于禁用状态，并且可以在 [!UICONTROL 帐户设置]. 启用后，还可以在 [!UICONTROL 校对默认值].

无法自定义这些通知。

接到通知的人员包括：

* 所有者，仅在 [!UICONTROL 电子邮件] 在中选中延迟校样时的警报 [!UICONTROL 所有者校对默认值].
* 任何尚未对证据作出决定的批准者。 有关决策的信息，请参阅 [在校对查看器中对校样做出决策](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>如果在 [!UICONTROL 帐户设置]，否 [!UICONTROL 延迟校样] 即使审阅人和批准人尚未提交其意见和决定，也会发送电子邮件。 您还可以禁用 [!UICONTROL 延迟校样] 电子邮件的“校样”默认值。

请考虑以下关于校样通知的事项：

* 您的 [!DNL Workfront] 管理员或 [!DNL Workfront Proof] 管理员可以在电子邮件通知中包含贵组织的徽标，如 [品牌 [!DNL Workfront Proof] 网站](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).
* 如果您需要与同一审阅人共享多个校样，并且不希望他们收到多封电子邮件，则可以同时上载这些校样。 所有审阅人都会收到一封电子邮件，其中详细说明了所有校样，并包含每个校样的个人URL。

   >[!NOTE]
   >
   >校样的创建者将收到单独的 [!UICONTROL 制作的证明] 为创建的每个校样发送电子邮件。 有关更多信息，请参阅 [的 [!UICONTROL 制作校样] 电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md).

* 如果您或您的审阅人未收到预期的电子邮件通知，请参阅  [配置 [!DNL Workfront Proof] 电子邮件以避免垃圾邮件过滤器](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
