---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: 在中配置拖放区 [!DNL Workfront Proof]
description: As a [!DNL Workfront Proof] 管理员，您可以设置、查看和编辑用户的拖放区设置。 有关Dropzone的信息，请参阅Dropzone 。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# 在中配置拖放区 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

As a [!DNL Workfront Proof] 管理员，您可以设置、查看和编辑用户的拖放区设置。 有关Dropzone的信息，请参阅 [拖放区](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. 单击 **[!UICONTROL 设置]** > **[!UICONTROL 帐户设置]**，然后打开 **[!UICONTROL Dropzone]** 选项卡。

1. 在 **[!UICONTROL 拖放区域详细信息]** 部分：

   * **[!UICONTROL Web Dropzone]**:启用或禁用拖放区域。
   * **[!UICONTROL Web Dropzone URL]**:您必须在浏览器中输入的URL，才能通过Dropzone提交校样。
   * **[!UICONTROL 电子邮件拖放区]**:启用或禁用电子邮件拖放区。

      >[!NOTE]
      >
      >不再支持通过电子邮件发送到dropzones。

   * **[!UICONTROL Dropzone所有者]**:设置或编辑Dropzone所有者。 此人将收到有关向Dropzone提交新内容的通知。 要设置为Dropzone所有者，用户必须是主管、管理员、账单管理员或帐户创建者。 有关更多信息，请参阅 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL 创建者的默认角色]**:所有提交者都将添加到校样中，并默认使用此角色。
   * **[!UICONTROL 所有创建者的电子邮件通知]**:在此处为校样创建者（提交者）设置电子邮件警报首选项。 请参阅 [在中配置电子邮件通知设置 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) 以了解有关可用的不同警报设置的信息。

   * **[!UICONTROL 新版本函数]**:在Dropzone上启用和禁用新版本功能。 这允许用户通过拖放区提交新版本的校样。
   * **[!UICONTROL 在（天）后删除草稿校样]**:指定删除草稿校样的间隔天数。 如果在将文件上传到Dropzone后未完成Dropzone提交，则校样会保持草稿状态。
   * **[!UICONTROL 隐藏审阅人角色]**:将人员添加到拖放区时，隐藏审阅人角色字段。
   * **[!UICONTROL 在激活时发送校样消息]**:配置 [!DNL Workfront Proof] 用于在激活校样时自动向审阅人发送校样通知电子邮件。
   * **[!UICONTROL 在提交时激活校样]**:配置 [!DNL Workfront Proof] 在提交时自动激活校样（无需手动激活校样）。

   * 如果校样从Dropzone中移出（例如，移到您帐户中的其他文件夹），则Dropzone设置将不再适用于校样。 这对于电子邮件警报设置尤为重要。

1. 在 **[!UICONTROL Dropzone字段]** 部分，以指定在 [!UICONTROL 校样详细信息] 在通过拖放区提交校样时显示的区域。
1. 在 **[!UICONTROL 允许的域]** 部分，指定您希望允许使用拖放区域的域。

   * 您可以单击 **[!UICONTROL 添加域]** 添加域。 添加完域详细信息后，单击 **[!UICONTROL 保存]**.

   * 您可以 **[!UICONTROL 编辑]** 和 **[!UICONTROL 删除]** 您之前添加的任何现有域。

1. 在 **[!UICONTROL 要通知的人员]**，指定在向拖放区提交新校样时，要与拖放区所有者一起接收通知的人员 [拖放区](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * 单击 **[!UICONTROL 添加人员]**，输入收件人的详细信息，然后单击 **[!UICONTROL 保存]**.

   * **[!UICONTROL 删除]** 您之前添加的人员。
