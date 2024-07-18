---
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: 常见问题解答 — 创建和共享验证和文件
description: 校样是一个静态、音频或视频文件，可在校样查看器中查看。 添加到验证的查看者拥有一组可用于对验证进行评论和决策的工具。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb0eb160-4bcf-4bc1-ad13-df19f692bef6
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '1369'
ht-degree: 1%

---

# 常见问题解答 — 创建和共享验证和文件

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

## 什么是证据？

### 答案

校样是一个静态、音频或视频文件，可在校样查看器中查看。 添加到验证的查看者拥有一组可用于对验证进行评论和决策的工具。

## 支持哪些文件类型？

### 答案

可以从静态、音频和视频文件创建校样。 您无法上载大于4GB的文件。 [!DNL Workfront]支持150多种文件类型（有关完整列表，请参阅[支持的校对文件类型和大小限制概述](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md)）。

## 证明和文件有何区别？

### 答案

将文件上传到[!DNL Workfront Proof]时，系统会将文件存储在您的[!DNL Workfront Proof]帐户中。 当您共享时，[!DNL Workfront Proof]会向收件人发送一封电子邮件，其中包含他们可以单击以下载文件的链接。 您可以共享任何所需的文件类型。

当您从已上载到[!DNL Workfront Proof]的文件创建验证时，可以使文件在验证查看器中可供查看。 查看者会收到一封电子邮件，其中包含指向验证的链接。 当他们打开验证时，他们会看到验证图像，并可以对它添加评论和做出决策。 您可以从支持的文件类型列表中使用文件创建校样。 您还可以使用URL为网站和其他Web内容创建验证。

有关支持的文件类型的完整列表，请参阅[支持的校对文件类型和大小限制概述](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md)。

## 如何创建验证？

### 答案

您可以从静态文件、音频文件、视频文件和URL创建验证（请参阅）。

要在帐户中创建验证，您需要是具有正确权限配置文件的用户（请参阅 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[[!UICONTROL 验证权限配置文件]）。

如果同时上载多个文件，您将创建多个校样，这些校样可以使用一封电子邮件发送给同一审阅人组。 如果您的组织具有[!UICONTROL Enterprise]或[!UICONTROL Unlimited]帐户，您可以将文件合并到单个验证中（请参阅[创建多页验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)）。

## 什么是验证角色和电子邮件警报？

### 答案

验证角色定义查看者需要对验证执行的操作。 在创建验证时，您可以为审阅人使用不同的角色选项，具体取决于您是否希望审阅人能够做出评论、决策等。 有关详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)中管理校对角色。

电子邮件警报会根据验证进度更新审阅人（它们不同于新验证和延迟验证通知）。 您可以根据每位审阅人在校样中的角色，为不同的审阅人选择不同的选项。 有关详细信息，请参阅[使用[!UICONTROL 自动化工作流]](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)创建高级校对。

## 我是否可以从多个文件创建验证？

### 答案

将多个文件合并为单个校对是[!UICONTROL Enterprise]和[!UICONTROL Unlimited]版本计划上提供的功能。 此选项仅适用于静态文件，不适用于视频文件。 有关详细信息，请参阅[创建多页校对](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)。

## 我能否从URL创建验证？

### 答案

是，您可以从网站和其他网络内容创建验证。 添加URL以创建验证时，您可以指定是需要静态验证还是交互式验证：

* 在交互式验证中，查看者可以像平常一样导航和交互网站或其他网络内容，例如带有流视频或音频的广告、广告中的[!DNL Flash]元素、HTML动画和交互式横幅。 有关详细信息，请参阅[在ZIP文件中为交互式内容创建验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md)。
* 对于静态校对，[!DNL Workfront]会获取您指定的页面和子页面的一组屏幕截图。 超链接在验证中处于活动状态，因此您可以测试它们是否指向正确的目标。 有关详细信息，请参阅[为网站或其他Web内容创建静态校对](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-static-proof-website-other-web-content.md)。

如果使用空格分隔多个URL，则可以一次添加多个URL。 请注意，组合仅适用于[!UICONTROL Enterprise]和[!UICONTROL Unlimited]版本计划。

## 没有登录凭据的用户能否在我的帐户中创建验证？

### 答案

您需要登录凭据才能直接在[!DNL Workfront Proof]帐户中创建验证。

## 共享证明意味着什么？

### 答案

共享校样可为审阅人提供对其的访问权限，以便他们可以添加评论和标记并对其做出决策。 来宾审阅人可从他们收到的电子邮件通知中访问校样。 拥有自己[!DNL Workfront Proof]帐户的审阅者可以访问[!UICONTROL 仪表板]上的验证。

## 如何共享证明？

### 答案

创建校对时，您可以在[!UICONTROL 新校对]页面的[!UICONTROL 工作流]部分中添加审阅人。 当校对准备就绪时，[!DNL Workfront Proof]向审阅人发送一封包含校对链接的电子邮件。

如果您对校对拥有足够的权限，则可以使用校对查看器、您的[!UICONTROL 仪表板]或任何列表视图将审阅者添加到现有校对(请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) and [Manage Items on the [!UICONTROL Views] 中共享校对 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)中的页面。

添加审阅人是共享验证的最常见方式。 如果您想探索其他可用选项，请参阅：

* [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof-links.md)中共享校对链接
* [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md)中共享公共URL
* [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)中订阅校对
* [在 [!DNL Workfront Proof]中创建迷你校对](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/create-mini-proof.md)

## 您必须是用户才能查看验证吗？

### 答案

不可以。来宾审阅者（没有[!DNL Workfront Proof]登录凭据的人员）可以从他们收到的验证电子邮件通知中访问验证。 您可以与所需数量的来宾共享证明。

可以将共享验证限制到具有[!DNL Workfront Proof]登录凭据的用户。 这会为验证添加另一个安全层。 为了增强安全性，具有[!UICONTROL Enterprise]和[!UICONTROL Unlimited]计划的组织的系统管理员可以为组织中创建的所有验证配置此要求。

有关要求登录的详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/proof-security-in-workfront-proof.md)中验证安全性。

如果您的组织要求审阅人以电子方式签署验证，这需要登录到[!DNL Workfront Proof]，则用户只能与注册用户共享验证。 这适用于[!UICONTROL Enterprise]和[!UICONTROL Unlimited]版本计划。 有关详细信息，请参阅[了解 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)中的电子签名。

## 我可以设置审阅人的截止日期吗？

### 答案

在创建验证时，您可以为新验证或新验证版本设置截止时间。 请在[!UICONTROL 新校对]页面的[!UICONTROL 工作流]部分执行此操作。 如果您使用[!UICONTROL 自动工作流]，则可以为审阅的每个阶段设置不同的截止日期。

您还可以使用[!UICONTROL 验证详细信息]页面设置或更新现有验证的截止日期。 有关详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校对详细信息。

## 如何创建新版本的验证？

### 答案

查看者通常请求更改其对验证评论的内容，并希望查看该验证的新版本。 您可以创建新版本的验证。 [!DNL Workfront Proof]记住以前版本中的校对设置。 如果需要执行添加或删除校样审阅者等操作，您仍然可以编辑这些设置。

您必须将每个版本与需要查看该版本的特定审阅人共享。 例如，如果仅与审阅人共享版本3，则此人看不到版本1和2。 您帐户中的主管和管理员负责监督帐户中的所有项目，以便他们可以查看和编辑证明的所有版本。

有关更多信息，请参阅。

## 我可以使用[!DNL Workfront Proof]共享文件吗？

### 答案

可以。如果您希望与其他人共享某些内容，但您不需要他们以证明的形式查看它（或如果它是[!DNL Workfront Proof]不支持的文件类型），则可以将其作为文件上传到您的[!DNL Workfront Proof]帐户。 与验证一样，您可以在共享文件时将文件整理到文件夹中、标记文件以及向通知电子邮件添加自定义消息。 有关详细信息，请参阅[将文件和Web内容上载到 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)。

当您的收件人收到有关您正在共享文件的电子邮件通知时，他们可以通过单击通知中的链接下载该文件。

[!DNL Workfront Proof]用户可以将文件保存到其帐户中后转换为验证。

<!--Is there a limit-->
