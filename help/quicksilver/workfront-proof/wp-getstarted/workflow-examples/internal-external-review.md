---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: workflow-examples
title: 在 [!DNL Workfront Proof]中进行内部审核，然后再进行外部审核
description: 了解如何使用Workfront Proof在组织外部进行审核。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c54246e9-edb8-4d98-81e1-faf7ee75f81e
source-git-commit: 153951e3bba91d67bcfe5fbf22c0970743f0dc6e
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# 在[!DNL Workfront Proof]中进行内部审查，然后再进行外部审查

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

如果贵组织在与客户共享校样之前完成内部审查，我们建议您两种使用[!DNL Workfront Proof]来增强工作流程的方法：

## 客户端查看内部注释

此选项说明了客户端可以查看所有内部注释的工作流。

设计人员首先会与项目经理（以及任何其他同事）共享证明。 同事查看验证，如果批准，您可以使用共享功能与您的客户共享验证。 有关详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)中共享校对。

![internal_external_-_option_A.png](assets/internal_external_-_option_A.png)

1. **创建新校对** — 设计者在[!DNL Workfront Proof]中创建新校对并将其共享给内部审阅者。 设计人员使项目经理成为验证的所有者。
1. **内部审核** — 项目经理和其他同事审核证明。
1. **共享验证** — 项目经理与客户端共享验证。
1. **新验证电子邮件** — 客户端将收到包含[!UICONTROL 转到验证]链接的新验证电子邮件。 有关详细信息，请参阅[新验证电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md)。

1. **审阅校样** — 客户端审阅校样、添加评论并做出决定。
1. **电子邮件警报** — 项目经理会收到电子邮件警报（取决于他在验证上的设置）。 有关详细信息，请参阅[在Workfront Proof中配置电子邮件通知设置](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)。

1. **更改请求** — 项目经理通知设计人员有关更改请求的信息。 可使用打印注释功能完成此操作。 有关详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md)中打印和导出注释。

1. **新版本**（如果需要） — 设计器将修改文件并将其作为新版本上载到[!DNL Workfront Proof]。 有关更多信息，请参阅。

您可以重复此过程，直到验证被批准。

## 客户只能看到自己的版本

此选项说明了一个工作流，其中验证过程由项目经理管理，项目经理会创建任何新版本（根据需要）并与客户端共享验证。 设计者无需参与审阅过程。)

![internal_external_-_option_B.png](assets/internal_external_-_option_B.png)

1. **创建新校对** — 设计人员在[!DNL Workfront Proof]中创建新校对并与内部审阅人共享。 设计者使项目经理成为校对的所有者，或者赋予他在校对上[!UICONTROL 作者]的角色（请参阅 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)中的管理校对角色）。

1. **内部审核** — 项目经理和其他同事审核证明。 有关详细信息，请参阅[在Web验证查看器中查看验证](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer)和[在桌面验证查看器中查看验证。](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer)

1. **新版本** — 项目管理器将创建一个新版本（或副本）的验证并与客户端共享。 请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md)中复制校样，以及[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)中共享校样。

1. **新验证电子邮件** — 客户端收到带有[!UICONTROL 前往验证]链接的新验证电子邮件。 有关详细信息，请参阅[新验证电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md)。

1. **[!UICONTROL 审阅校样]** — 客户端审阅校样、添加评论并做出决定。
1. 客户端只能看到已与他们明确共享的验证的版本；他们将无法看到内部版本。
1. **[!UICONTROL 电子邮件警报]** — 项目经理会收到一封电子邮件，其中包含客户审核的摘要（取决于他们在验证上的设置）。
1. **更改请求** — 项目经理通知设计人员有关更改请求的信息。 可使用打印注释功能完成此操作。 有关详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md)中打印和导出注释。

1. **新版本**（如果需要） — 设计器将修改文件并将其作为新版本上载到[!DNL Workfront Proof]。 有关更多信息，请参阅。

您可以重复此过程，直到验证被批准。
