---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: workflow-examples
title: 内部审查，然后外部审查 [!DNL Workfront Proof]
description: 了解如何使用Workfront Proof在组织外部进行审阅。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c54246e9-edb8-4d98-81e1-faf7ee75f81e
source-git-commit: 692d0e903c1b92ad539eacf6d26e18e81530a8b0
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---

# 内部审查，然后外部审查 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍了独立版产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参见 [校对](../../../review-and-approve-work/proofing/proofing.md).

如果您的组织在与客户共享验证之前完成内部审查，我们建议您使用两种方法 [!DNL Workfront Proof] 要增强您的工作流，请执行以下操作：

## 客户端查看内部注释

此选项说明了客户端可以查看所有内部注释的工作流。

设计人员首先会与项目经理（以及任何其他同事）共享证明。 同事查看验证，如果批准，您可以使用共享功能与您的客户共享验证。 有关更多信息，请参阅 [在中共享验证 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

![internal_external_-_option_A.png](assets/internal-external---option-a-350x86.png)

1. **创建新验证**  — 设计人员在中创建新验证 [!DNL Workfront Proof] 并与内部评审员分享。 设计人员使项目经理成为验证的所有者。
1. **内部审查**  — 项目经理和其他同事查看证明。
1. **共享校对**  — 项目经理与客户端共享证明。
1. **新验证电子邮件**  — 客户收到新验证电子邮件，带有 [!UICONTROL 前往校对] 链接。 有关更多信息，请参阅 [新验证电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

1. **查看证据**  — 客户审核证明、添加评论并做出决定。
1. **电子邮件警报**  — 项目经理会收到电子邮件警报（具体取决于他在验证上的设置）。 有关更多信息，请参阅 [在Workfront Proof中配置电子邮件通知设置](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

1. **更改申请**  — 通过项目管理器，设计人员可了解变更请求。 可使用打印注释功能完成此操作。 有关更多信息，请参阅 [在中打印和导出注释 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md).

1. **新版本** （如果需要） — 设计人员会修改文件并将其上传到 [!DNL Workfront Proof] 作为新版本。 有关更多信息，请参阅。

您可以重复此过程，直到验证被批准。

## 客户只能看到自己的版本

此选项说明了一个工作流，其中验证过程由项目经理管理，项目经理会创建任何新版本（根据需要）并与客户端共享验证。 设计者无需参与审阅过程。)

![internal_external_-_option_B.png](assets/internal-external---option-b-350x86.png)

1. **创建新验证**  — 设计人员在中创建新验证 [!DNL Workfront Proof] 并与内部审阅人共享。 设计人员将项目经理设为证明的所有者，或者授予他以下角色 [!UICONTROL 作者] 在验证上(请参阅 [在中管理验证角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md))。

1. **内部审查**  — 项目经理和其他同事查看证明。 有关更多信息，请参阅 [在Web验证查看器中查看验证](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer) 和 [在桌面校对查看器中查看校对。](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer)

1. **新版本**  — 项目经理创建新版本（或副本）的验证并与客户端共享它。 请参阅 [复制校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) 和 [在中共享验证 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

1. **新验证电子邮件**  — 客户收到的新验证电子邮件包含 [!UICONTROL 前往校对] 链接。 有关更多信息，请参阅 [新验证电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

1. **[!UICONTROL 查看证据]**  — 客户审核证明、添加评论并做出决定。
1. 客户端只能看到已与他们明确共享的验证的版本；他们将无法看到内部版本。
1. **[!UICONTROL 电子邮件警报]**  — 项目经理会收到一封电子邮件，其中包含客户端的审阅摘要（取决于它们在验证上的设置）。
1. **更改申请**  — 通过项目管理器，设计人员可了解变更请求。 可使用打印注释功能完成此操作。 有关更多信息，请参阅 [在中打印和导出注释 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md).

1. **新版本** （如果需要） — 设计人员会修改文件并将其上传到 [!DNL Workfront Proof] 作为新版本。 有关更多信息，请参阅。

您可以重复此过程，直到验证被批准。
