---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: 在 [!DNL Workfront Proof]中配置拖放区域
description: 作为 [!DNL Workfront Proof] 管理员，您可以设置、查看和编辑用户的拖放区域设置。 有关拖放区域的信息，请参阅拖放区域。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# 在[!DNL Workfront Proof]中配置拖放区域

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

作为[!DNL Workfront Proof]管理员，您可以设置、查看和编辑用户的拖放区域设置。 有关拖放区域的信息，请参阅[拖放区域](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)。

1. 单击&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 帐户设置]**，然后打开&#x200B;**[!UICONTROL 拖放区域]**&#x200B;选项卡。

1. 在&#x200B;**[!UICONTROL 拖放区域详细信息]**&#x200B;部分中进行以下任何更改：

   * **[!UICONTROL Web拖放区域]**：启用或禁用拖放区域。
   * **[!UICONTROL Web拖放区域URL]**：必须输入到浏览器中的URL才能通过Dropzone提交验证。
   * **[!UICONTROL 电子邮件拖放区域]**：启用或禁用电子邮件拖放区域。

     >[!NOTE]
     >
     >不再支持通过电子邮件发送到dropzones。

   * **[!UICONTROL 拖放区域所有者]**：设置或编辑拖放区域所有者。 这是将在向Dropzone提交新内容时收到通知的人员。 要设置为拖放区域所有者，用户必须是主管、管理员、账单管理员或帐户创建者。 有关详细信息，请参阅 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[校对权限配置文件。

   * **[!UICONTROL 创建者的默认角色]**：所有提交者都将作为默认角色添加到验证。
   * **[!UICONTROL 所有创建者的电子邮件通知]**：在此处为验证创建者（提交者）设置电子邮件警报首选项。 有关可用的不同警报设置的信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)中配置电子邮件通知设置。

   * **[!UICONTROL 新版本函数]**：在Dropzone上启用和禁用New Version函数。 这允许或禁止人员通过Dropzone提交新版本的验证。
   * **[!UICONTROL 在（天）后删除草稿验证]**：指定删除草稿验证的天数。 如果将文件上传到拖放区域后未完成拖放区域提交，则验证仍处于草稿状态。
   * **[!UICONTROL 隐藏审阅人角色]**：将人员添加到拖放区域时隐藏审阅人角色字段。
   * **[!UICONTROL 激活时发送校样邮件]**：配置[!DNL Workfront Proof]以在激活校样时自动向审阅人发送校样通知电子邮件。
   * **[!UICONTROL 提交时激活验证]**：配置[!DNL Workfront Proof]以在提交时自动激活验证（无需手动激活它们）。

   * 如果验证被移出拖放区域（例如，移动到您帐户中的另一个文件夹），则拖放区域设置将不再应用于验证。 这对于电子邮件警报设置尤为重要。

1. 在&#x200B;**[!UICONTROL 拖放区域字段]**&#x200B;部分中进行任何更改，以指定在通过Dropzone提交验证时，哪些字段显示在Dropzone提交页面的[!UICONTROL 验证详细信息]部分中。
1. 在&#x200B;**[!UICONTROL 允许的域]**&#x200B;部分中，指定希望允许使用Dropzone的域。

   * 您可以单击&#x200B;**[!UICONTROL 添加域]**&#x200B;以添加域。 完成添加域详细信息后，单击&#x200B;**[!UICONTROL 保存]**。

   * 您可以&#x200B;**[!UICONTROL 编辑]**&#x200B;和&#x200B;**[!UICONTROL 删除]**&#x200B;您之前添加的任何现有域。

1. 在&#x200B;**[!UICONTROL 要通知的人员]**&#x200B;下，指定在将新验证提交到拖放区域[拖放区域](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)时，要与拖放区域所有者一起通知的人员

   * 单击&#x200B;**[!UICONTROL 添加联系人]**，输入收件人的详细信息，然后单击&#x200B;**[!UICONTROL 保存]**。

   * **[!UICONTROL 删除您之前添加的]**&#x200B;用户。
