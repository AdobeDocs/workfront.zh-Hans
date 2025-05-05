---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 校对已发送电子邮件
description: 仅当验证创建者创建了验证时，才会向验证创建者发送Proof Made电子邮件。 如果某人创建了验证并使另一个人成为所有者，则只有新所有者会收到由验证组成的电子邮件。 创建者和/或所有者不会收到校样；他们只会收到“校样”电子邮件。 有关“新验证”电子邮件的更多信息，请参阅“新验证”电子邮件。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a6bfe471-2032-4b74-8316-584f923e8651
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# [!UICONTROL 校对已生成]电子邮件

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

仅当验证创建者创建了验证时，才会向验证创建者发送[!UICONTROL 校对制作]电子邮件。 如果某人已创建验证并使另一个人成为所有者，则只有新所有者也会收到[!UICONTROL 已创建验证]电子邮件。 创建者和/或所有者不会收到校样；他们只会收到[!UICONTROL 校样制作]电子邮件。 有关[!UICONTROL 新验证]电子邮件的详细信息，请参阅[[!UICONTROL 新验证]电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md)。

用户可以在个人资料设置中禁用[!UICONTROL 校对制作]电子邮件，如下所述。

>[!NOTE]
>
> 如果校对的创建者或所有者在其个人设置中默认禁用了[!UICONTROL 校对制作]电子邮件，则即使在[!UICONTROL 新校对]页面中选中了[!UICONTROL 通过电子邮件通知联系人]框，他们也不会收到任何[!UICONTROL 校对制作]或[!UICONTROL 新校对]电子邮件。

![Proof_Made_Email.png](assets/proof-made-email-350x214.png)

[!UICONTROL 校对]电子邮件包含您的个人消息（如果您包含个人消息）以及以下校对详细信息：

* 校样名称
* 证明的个人链接
* 版本号
* 验证的缩略图
* 校对进度
* 与他人共享证明的链接
* 这允许您共享原始文件的校对URL和/或下载链接。

>[!NOTE]
>
> 共享校对链接不允许您明确将审阅人添加到校对，您将只共享公共校对URL，并且收件人将获得对校对的只读访问权限。

有关详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)中共享验证。

如果不希望此链接显示在收件人的电子邮件中，则应该禁用验证上的[!UICONTROL 公共共享]设置（[!UICONTROL 下载原始文件]和[!UICONTROL 公共URL]）。

## 正在禁用[!UICONTROL 校对]电子邮件

1. 单击&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**，打开&#x200B;**[!UICONTROL 验证默认值]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL 验证就绪时电子邮件确认旁边的**&#x200B;[!UICONTROL &#x200B;禁用&#x200B;]&#x200B;**]**。

1. ![Proof_Made_-_proofing_defaults.png](assets/proof-made---proofing-defaults-350x103.png)

1. 有关更多详细说明，请参阅[在Workfront Proof中配置电子邮件通知设置](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)。
1. 如果在[!UICONTROL 帐户设置]中将电子邮件通知禁用为默认值，验证的创建者或所有者将不会收到任何[!UICONTROL 已制作验证]或[!UICONTROL 新验证]电子邮件，即使这已在他们的个人设置中启用并且已在[!UICONTROL 新验证]页面上选中[!UICONTROL 通过电子邮件通知人员]框。
