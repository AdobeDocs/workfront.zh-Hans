---
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: 常见问题解答 — 创建和共享校样和文件
description: 校样是可在校样查看器中查看的静态、音频或视频文件。 添加到校样的审阅人拥有一套工具可供他们对校样进行评论和决策。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb0eb160-4bcf-4bc1-ad13-df19f692bef6
source-git-commit: d5ffd576fcedf9b10dce5e5d5bd9245dd7f67ef8
workflow-type: tm+mt
source-wordcount: '1365'
ht-degree: 0%

---

# 常见问题解答 — 创建和共享校样和文件

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

## 什么是证据？

### 回答

校样是可在校样查看器中查看的静态、音频或视频文件。 添加到校样的审阅人拥有一套工具可供他们对校样进行评论和决策。

## 支持哪些文件类型？

### 回答

可以使用静态、音频和视频文件创建校样。 无法上传大于4GB的文件。 [!DNL Workfront] 支持150多种文件类型(请参阅 [支持的校对文件类型和大小限制概述](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md) )。

## 校样和文件之间有何区别？

### 回答

将文件上传到 [!DNL Workfront Proof]，则系统会将文件存储在 [!DNL Workfront Proof] 帐户。 当你分享它时， [!DNL Workfront Proof] 向收件人发送电子邮件，以便他们单击该链接来下载文件。 您可以共享所需的任何文件类型。

从上传到的文件创建校样时 [!DNL Workfront Proof]，则可以使文件在校样查看器中可供查看。 审阅人会收到一封包含校样链接的电子邮件。 当他们打开校样时，会看到校样图像，并可以添加评论并据此做出决策。 您可以使用支持的文件类型列表中的文件创建校样。 您还可以使用网站和其他Web内容的URL创建校样。

有关支持的文件类型的完整列表，请参阅 [支持的校对文件类型和大小限制概述](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

## 如何创建证明？

### 回答

您可以从静态文件、音频文件、视频文件和URL创建校样（请参阅）。

要在帐户中创建校样，您需要是具有权限配置文件的用户(请参阅 [[!UICONTROL 校样权限配置文件] in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md))。

如果同时上传多个文件，则可以创建多个校样，然后使用一封电子邮件将这些校样发送给同一组审阅人。 如果贵组织具有 [!UICONTROL 企业] 或 [!UICONTROL 无限制] 帐户，您可以将文件合并到单个校样中(请参阅 [创建多页校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md))。

## 什么是校样角色和电子邮件警报？

### 回答

校样角色定义审阅人需要对校样执行的操作。 在创建校样时，您可以为审阅人使用不同的角色选项，具体取决于您是否希望审阅人能够进行评论、做出决策等。 有关更多信息，请参阅 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

电子邮件警报会根据校样的进度更新审阅人（它们与新校样和延迟校样通知不同）。 您可以根据每个审阅人对校样的角色，为不同的审阅人选择不同的选项。 有关更多信息，请参阅 [使用创建高级校样 [!UICONTROL 自动化工作流]](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 我可以从多个文件创建校样吗？

### 回答

将多个文件合并到单个校样中是 [!UICONTROL 企业] 和 [!UICONTROL 无限制] 版本计划。 此选项仅适用于静态文件，而不适用于视频文件。 有关更多信息，请参阅  [创建多页校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## 我是否可以从URL创建校样？

### 回答

可以，您可以从网站和其他Web内容创建校样。 添加URL以创建校样时，您可以指定是希望进行静态校样还是进行交互式校样：

* 在交互式校样中，审阅人可以像往常一样导航和与网站或其他Web内容（如带有流视频或音频的广告）进行交互， [!DNL Flash] 广告、HTML动画和交互式横幅中的元素。 有关更多信息，请参阅 [在ZIP文件中为交互式内容创建校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).
* 对于静态校样， [!DNL Workfront] 为您指定的页面和子页面设置屏幕截图。 超链接在校样中处于活动状态，因此您可以测试它们是否指向正确的目标。 有关更多信息，请参阅 [为网站或其他Web内容创建静态校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-static-proof-website-other-web-content.md).

如果用空格分隔多个URL，则可以一次添加它们。 请注意，组合仅在 [!UICONTROL 企业] 和 [!UICONTROL 无限制] 版本计划。

## 没有登录名的人员能否在我的帐户中创建验证？

### 回答

您需要登录凭据才能直接在 [!DNL Workfront Proof] 帐户。

## 分享证据意味着什么？

### 回答

通过共享校样，审阅人可以访问校样，以便添加注释和标记并据此做出决策。 来宾审阅人从收到的电子邮件通知中访问校样。 具有自己的审阅人 [!DNL Workfront Proof] 帐户可以访问校样 [!UICONTROL 功能板].

## 如何共享证据？

### 回答

创建校样时，可以在 [!UICONTROL 工作流] 部分 [!UICONTROL 新校样] 页面。 证据准备好后， [!DNL Workfront Proof] 向审阅者发送一封电子邮件，其中包含指向校样的链接。

如果您对校样拥有足够的权限，则可以使用校样查看器， [!UICONTROL 功能板]，或任何用于将审阅者添加到现有校样的列表视图(请参阅 [在中共享校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) and [Manage Items on the [!UICONTROL Views] 页面 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

添加审阅人是共享校样的最常用方式。 如果您想要探索其他可用选项，请参阅：

* [在中共享校样链接 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof-links.md)
* [在中共享公共URL [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md)
* [在中订阅校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)
* [在中创建小校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/create-mini-proof.md)

## 您是否必须是用户才能查看校样？

### 回答

否. 来宾审阅人(没有 [!DNL Workfront Proof] 登录凭据)可以从收到的校样电子邮件通知中访问校样。 您可以与所需数量的客人共享校样。

可以限制用户通过 [!DNL Workfront Proof] 登录凭据。 这为校样添加了另一个安全层。 为了增强安全性， [!UICONTROL 企业] 和 [!UICONTROL 无限制] 计划可以为组织中创建的所有校样配置此要求。

有关要求登录的更多信息，请参阅 [中的验证安全性 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/proof-security-in-workfront-proof.md).

如果贵组织要求审阅人以电子方式签署校样，则需要登录 [!DNL Workfront Proof]，则用户只能与注册用户共享校样。 此选项在 [!UICONTROL 企业] 和 [!UICONTROL 无限制] 版本计划。 有关更多信息，请参阅 [了解 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md).

## 我可以为审阅人设置截止日期吗？

### 回答

在创建校样时，您可以为新校样或新校样版本设置截止日期。 在 [!UICONTROL 工作流] 部分 [!UICONTROL 新校样] 页面。 如果您使用 [!UICONTROL 自动化工作流]，则可以为审阅的每个阶段设置不同的截止日期。

您还可以使用 [!UICONTROL 校样详细信息] 页面。 有关更多信息，请参阅 [在中管理校样详细信息 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

## 如何创建验证的新版本？

### 回答

审阅人通常要求对校样的评论进行更改，并希望看到校样的新版本。 您可以创建校样的新版本。 [!DNL Workfront Proof] 会记住校样在以前版本中的设置。 如果需要执行添加或删除校样审阅人之类的操作，您仍可以编辑这些设置。

您必须将每个版本与需要查看的特定审阅人共享。 例如，如果您只与审阅人共享版本3，则该人员将看不到版本1和2。 您帐户中的主管和管理员会监督帐户中的所有项目，以便他们能够查看和编辑校样的所有版本。

有关更多信息，请参阅。

## 我能否使用 [!DNL Workfront Proof]?

### 回答

是. 如果您希望与他人共享某些内容，但您不需要他们将其视为校样（或者它是不受支持的文件类型） [!DNL Workfront Proof])，您可以将其作为文件上传到 [!DNL Workfront Proof] 帐户。 与校样一样，您可以将文件整理到文件夹、标记文件中，并在共享文件时向通知电子邮件添加自定义消息。 有关更多信息，请参阅 [将文件和Web内容上传到 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

当您的收件人收到有关您共享的文件的电子邮件通知时，他们可以通过单击通知中的链接下载该文件。

[!DNL Workfront Proof] 用户在将文件保存到其帐户中后，可以将其转换为校样。

<!--Is there a limit-->
