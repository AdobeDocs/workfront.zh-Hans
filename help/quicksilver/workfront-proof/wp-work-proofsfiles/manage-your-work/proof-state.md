---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 了解Workfront校样中的校样状态
description: 在 [!DNL Workfront Proof]，校样存在于不同的状态。 这些状态可决定您可以对证据采取哪些操作，例如评论或做出决策。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# 了解Workfront校样中的校样状态

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

在 [!DNL Workfront Proof]，校样存在于不同的状态。 这些状态可决定您可以对证据采取哪些操作，例如评论或做出决策。

## 了解校样状态

这四个状态如下：

* [活动](#active)
* [锁定](#locked)
* [草稿（仅限拖放区）](#draft-dropzone-only)
* [已提交（仅限Dropzone）](#submitted-dropzone-only)

### 活动 {#active}

上传到的校样 [!DNL Workfront Proof] 处理后，New Proof页面或拖放区域会显示为活动。 当校样处于活动状态时，用户可以对校样进行审阅、评论和决策。

>[!NOTE]
>
>仅当启用了提交时激活校样选项时，通过拖放区上传的校样才会显示为活动。 如果未启用选项，则必须手动激活校样。

有关Dropzone设置的更多信息，请参阅 [在中配置拖放区 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### 锁定 {#locked}

在审阅完校样后，您可以锁定校样。 锁定校样意味着不能再对校样进行评论或决策，但校样仍然可以打开。

对校样具有编辑权限的任何用户都可以解锁该校样。

有关权限的更多信息，请参阅 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>校样被锁定后，将不再发送电子邮件通知。 例如，如果校样在截止时间之前被锁定，则在到达截止时间时不会发送通知电子邮件。

### 草稿（仅限拖放区） {#draft-dropzone-only}

当您通过拖放区提交验证时，它会进入“草稿”状态，然后管理员才会激活它。 当校样位于草稿区域中时，无法对校样执行任何操作。

### 已提交（仅限Dropzone） {#submitted-dropzone-only}

在管理员激活草稿后，您的校样会在拖放区中显示为已提交。 提交后，您可以对校样执行操作。

## 查看和更改校样状态

有关查看特定状态下所有校样的列表（如查看所有活动校样或锁定校样）的信息，请参阅 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) 在文章中 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. 访问 [!DNL Workfront Proof] 功能板。

   有关更多信息，请参阅 [访问 [!DNL Workfront Proof] 从Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. 在 **[!UICONTROL 功能板]**，请单击 **[!UICONTROL 展开]** 要查看或更改状态的校样旁的箭头。

   ![](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   的 **[!UICONTROL 工作流流程]** 的上界。

   ![](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. 查看 **[!UICONTROL 州]** 在 **[!UICONTROL 工作流流程]**.

1. （可选）要更改状态，请将鼠标悬停在当前状态上 **[!UICONTROL 州]** ，然后单击下拉菜单，然后选择新状态。

   ![](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
