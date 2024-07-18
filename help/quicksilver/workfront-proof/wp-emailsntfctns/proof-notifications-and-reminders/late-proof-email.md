---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 延迟验证电子邮件
description: 当验证接近截止日期或到达截止日期时，会向收件人发送延迟验证电子邮件。 这些类型的电子邮件无法在验证级别禁用，但可在帐户和用户个人设置级别配置。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!UICONTROL 迟到校对]电子邮件

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

当验证接近截止日期或接近截止日期时，会向收件人发送[!UICONTROL 迟验证]电子邮件。 这些类型的电子邮件无法在验证级别禁用，但可在帐户和用户个人设置级别配置。

* 当验证到达截止日期且并非所有审阅或决策都已作出时，[!UICONTROL 延迟验证]电子邮件会自动发送给审阅人。

  这些电子邮件在默认情况下处于启用状态，无法针对整个帐户进行调整，但用户可以在验证默认设置中禁用它们。

* 当验证接近截止日期时，会向审核者发送风险电子邮件。 默认情况下已禁用这些设置，可以在[!UICONTROL 帐户设置]中启用它们。 启用后，它们也可以在[!UICONTROL 校对默认值]中调整。

无法自定义这些通知。

将收到通知的用户是：

* 在[!UICONTROL 所有者的验证默认值]中，只有在[!UICONTROL 电子邮件]警报启用验证延迟时，所有者才选中。
* 尚未对证明做出决定的任何审批者。 有关决策的信息，请参阅[在验证查看者中做出校对决策](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>如果在[!UICONTROL 帐户设置]中将电子邮件通知禁用为默认值，将不会发送[!UICONTROL 迟到校对]电子邮件，即使审阅者和批准者尚未提交其评论和决定。 您还可以禁用“校对”默认值中的[!UICONTROL 迟校对]电子邮件。

有关验证通知，请考虑以下事项：

* 您的[!DNL Workfront]管理员或[!DNL Workfront Proof]管理员可以在电子邮件通知中包含您组织的徽标，如[品牌化 [!DNL Workfront Proof] 站点](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md)中所述。
* 如果您需要与同一审阅人共享多个校样，并且不希望他们收到多封电子邮件，您可以同时上传他们。 所有审阅人都会收到一封电子邮件，详细说明所有校样，并包含每个校样的个人URL。

  >[!NOTE]
  >
  >验证的创建者会收到针对所创建每个验证的单独的[!UICONTROL 校对]电子邮件。 有关详细信息，请参阅[校对[!UICONTROL 电子邮件]](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md)。

* 如果您或您的审阅人没有收到预期的电子邮件通知，请参阅[配置 [!DNL Workfront Proof] 电子邮件以避免垃圾邮件过滤器](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md)。
