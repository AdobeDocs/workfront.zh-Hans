---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: 了解 [!DNL Workfront Proof]
description: 电子签名可增强校样的安全性并符合ISO等行业标准。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: caff2a03-cccc-4779-9dcc-3362c527dcb9
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# 了解 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

电子签名可增强校样的安全性并符合ISO等行业标准。

在帐户级别，可将此设置设为必填或非必填。 如果默认情况下它是强制的，则会在帐户中创建的所有校样上启用它，并且不能在校样级别禁用它。 如果此设置在默认情况下不是强制设置，您将能够在校样级别启用/禁用它。

有关更多信息，请参阅。

当在校样上启用电子签名设置时，电子签名框会提示对校样做出决策的任何审阅人提供其电子邮件和密码。

![Electronic_sig_required_box.png](assets/electronic-sig-required-box.png)

## 电子签名 [!UICONTROL 校样详细信息] 页面

如果审阅人通过选择 [!UICONTROL 校样详细信息] 第(1)页和 [!UICONTROL 电子签名] 弹出框将显示，要求他们输入其详细信息(2)并确认其决定(3)。

弹出窗口将显示默认消息集（如果有），并且审阅人需要输入其电子邮件和密码。

的 [!UICONTROL 电子签名] 弹出窗口将显示在校样查看器中以及 [!UICONTROL 校样详细信息] 页面。

![Electronic_Signature_-_Proof_Details.png](assets/electronic-signature---proof-details-350x146.png)

![Electronic_Signature_-_Proof_Details_2.png](assets/electronic-signature---proof-details-2-350x148.png)

如果 [!UICONTROL 单点登录] 选项，则电子邮件和密码详细信息将不会显示在 [!UICONTROL 电子签名] 做出决策时弹出。

相反，在单击 [!UICONTROL 确认] (4)此弹出窗口上的按钮将被重定向到 [!UICONTROL 单点登录] 页面。

在输入其SSO凭据后，审核者将自动重定向回 [!UICONTROL 校样详细信息] 页面(或返回 [!UICONTROL 校样查看器] 如果从此处决定)。

![Electronic_Signature_SSO_-_Proof_Details_3.png](assets/electronic-signature-sso---proof-details-3-350x146.png)

>[!NOTE]
>
> 如果该决定以电子方式签署，则 **[!UICONTROL 签名图标]** (5)于2014年12月31日的 [!UICONTROL 工作流] 部分 [!UICONTROL 校样详细信息] 页面。 如果决定不是由审阅人更改的，而是由对校样具有编辑权限的另一人更改的，则不会要求该人以电子方式签署决定，并且该决定(6)旁将没有签名图标。

![Electronic_Signature_icon.png](assets/electronic-signature-icon-350x52.png)有关单点登录的信息，请参阅 [Workfront校样中的单点登录](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

有关校样详细信息页面的信息，请参阅 [在中管理校样详细信息 [!DNL Workfront] 校样](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
