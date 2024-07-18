---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: 了解 [!DNL Workfront Proof]中的电子签名
description: 电子签名允许您增强验证的安全性并符合ISO等行业标准。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: caff2a03-cccc-4779-9dcc-3362c527dcb9
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# 了解[!DNL Workfront Proof]中的电子签名

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

电子签名允许您增强验证的安全性并符合ISO等行业标准。

在帐户级别，此设置可以是强制性的，也可以是非强制性的。 如果默认情况下是强制性的，则它将在您的帐户中创建的所有验证中启用，并且无法在验证级别禁用。 如果默认情况下不强制进行此设置，则可以在验证级别启用/禁用此设置。

有关更多信息，请参阅。

当在证明上启用电子签名设置时，电子签名框提示任何对证明做出决定的审阅者提供其电子邮件和密码。

![Electronic_sig_required_box.png](assets/electronic-sig-required-box.png)

## [!UICONTROL 证明详细信息]页面上的电子签名

如果审核者通过在[!UICONTROL 证明详细信息]页面上选择他们的决定来做出决定(1)，则会出现[!UICONTROL 电子签名]弹出框，要求他们输入详细信息(2)并确认其决定(3)。

该弹出窗口将显示默认消息集（如果有），并且要求审阅者输入其电子邮件和密码。

如果审核者决定从该级别做出决定，则[!UICONTROL 电子签名]弹出窗口将显示在验证查看者中，还将显示在[!UICONTROL 验证详细信息]页面上。

![Electronic_Signature_-_Proof_Details.png](assets/electronic-signature---proof-details-350x146.png)

![Electronic_Signature_-_Proof_Details_2.png](assets/electronic-signature---proof-details-2-350x148.png)

如果在验证上启用了[!UICONTROL 单点登录]选项，则在做出决定时，电子邮件和密码详细信息将不会显示在[!UICONTROL 电子签名]弹出窗口中。

相反，单击此弹出窗口上的[!UICONTROL 确认] (4)按钮后，审阅者将被重定向到[!UICONTROL 单点登录]页面。

输入其SSO凭据后，审核者将自动被重定向回[!UICONTROL 验证详细信息]页面（或者，如果从此处做出决定，则重定向回[!UICONTROL 验证查看者]）。

![Electronic_Signature_SSO_-_Proof_Details_3.png](assets/electronic-signature-sso---proof-details-3-350x146.png)

>[!NOTE]
>
> 如果决策是电子签名的，则&#x200B;**[!UICONTROL 签名图标]** (5)将出现在[!UICONTROL 验证详细信息]页面上的[!UICONTROL 工作流]部分中。 如果该决定不是由审阅者更改，而是由对证明具有编辑权的另一个人更改，则不会要求该人以电子方式签署该决定，并且在该决定(6)旁边不会出现签名图标。

![Electronic_Signature_icon.png](assets/electronic-signature-icon-350x52.png)有关单点登录的信息，请参阅[Workfront Proof中的单点登录](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md)。

有关校对详细信息页面的信息，请参阅[在 [!DNL Workfront] 校对](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校对详细信息。
