---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 了解Workfront Proof中的验证状态
description: 在 [!DNL Workfront Proof]中，验证以不同的状态存在。 这些状态确定您可以对验证执行哪些操作，例如添加注释或做出决策。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# 了解Workfront Proof中的验证状态

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

在[!DNL Workfront Proof]中，验证以不同的状态存在。 这些状态确定您可以对验证执行哪些操作，例如添加注释或做出决策。

## 了解验证状态

这四种状态如下：

* [活动](#active)
* [锁定](#locked)
* [草稿（仅拖放区域）](#draft-dropzone-only)
* [已提交（仅拖放区域）](#submitted-dropzone-only)

### 活动 {#active}

处理通过新验证页面或拖放区域上传到[!DNL Workfront Proof]的验证后，这些验证将显示为活动。 当验证为活动时，用户可以查看、评论验证并做出决策。

>[!NOTE]
>
>仅当启用了提交时激活验证选项时，通过拖放区域上传的验证才会显示为活动。 如果未启用该选项，则必须手动激活验证。

有关拖放区域设置的详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)中配置拖放区域。

### 锁定 {#locked}

查看完验证后，您可以锁定该验证。 锁定验证意味着无法对验证做出更多评论或决定，但验证仍然可以打开。

任何对验证具有“编辑”权限的用户都可以将其解锁。

有关权限的详细信息，请参阅 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[验证权限配置文件。

>[!NOTE]
>
>锁定验证时，不再发送电子邮件通知。 例如，如果验证在截止日期之前锁定，则在到达截止日期时不会发送通知电子邮件。

### 草稿（仅拖放区域） {#draft-dropzone-only}

当您通过拖放区域提交验证时，它会在管理员激活之前进入草稿状态。 当验证位于草稿区域中时，您无法对验证执行任何操作。

### 已提交（仅拖放区域） {#submitted-dropzone-only}

管理员激活草稿后，您的验证在拖放区域显示为已提交。 提交验证后，您可以对验证执行操作。

## 查看和更改验证状态

有关查看处于特定状态的所有验证列表（如查看所有活动或锁定的验证）的信息，请参阅 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)中查看页面上的[管理项目一文中的[管理查看页面上的项目 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)。

1. 访问您的[!DNL Workfront Proof]仪表板。

   有关详细信息，请参阅[从Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)访问 [!DNL Workfront Proof] 。

1. 在&#x200B;**[!UICONTROL 仪表板]**&#x200B;上，单击要查看或更改其状态的校样旁边的&#x200B;**[!UICONTROL 展开]**&#x200B;箭头。

   ![](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   出现&#x200B;**[!UICONTROL 工作流进程]**&#x200B;部分。

   ![](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. 查看&#x200B;**[!UICONTROL 工作流进程]**&#x200B;中的&#x200B;**[!UICONTROL 状态]**。

1. （可选）要更改状态，请将鼠标悬停在当前&#x200B;**[!UICONTROL 状态]**&#x200B;上并单击下拉菜单，然后选择新状态。

   ![](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
