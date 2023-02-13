---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: 在中管理校样角色 [!DNL Workfront Proof]
description: 校样角色允许您向受用户配置文件中配置的权限配置文件所限制的用户授予权限。 (有关权限配置文件的更多信息，请参阅 [!DNL Workfront Proof].)
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 1%

---

# 在中管理校样角色 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

校样角色允许您向受用户配置文件中配置的权限配置文件所限制的用户授予权限。 (有关权限配置文件的更多信息，请参阅 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

校样角色与帐户配置文件不同。 您的帐户配置文件与您在帐户中拥有的总体权限级别相关，并且将影响您在帐户中拥有的所有校样的权限，即使是尚未明确与您共享的校样。

有关更多信息，请参阅 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## 关于校样角色

在邀请用户查看校样时，会为用户授予以下单独校样角色：

* [只读](#read-only)
* [查看者](#reviewer)
* [审批者](#approver)
* [审核人和批准者](#reviewer-approver)
* [作者](#author)
* [审阅人](#moderator)

校样角色定义审阅人可以对该特定校样执行的操作。

例如，如果您是审阅人，系统会要求您通过添加标记和注释来查看校样。 如果您是审阅者和审批者，则系统会要求您审核校样并做出决策。

某些校样角色为审阅人提供了校样的编辑权限（即使其帐户配置文件没有），并允许他们使用一些其他功能，例如添加对注释的操作、创建新版本以及向校样添加更多审阅人。

有关更多信息，请参阅以下文章：

* [对校样注释使用操作](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [在中共享校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### 只读

{#read-only}

![cleaner.png](assets/cleaner.png) 可以查看校样

![no.png](assets/no.png) 无法添加标记

![no.png](assets/no.png) 无法添加注释

![no.png](assets/no.png) 无法作出决定

![no.png](assets/no.png) 无法删除他人的评论

![no.png](assets/no.png) 对校样没有编辑权限

>[!NOTE]
>
>如果与的用户共享文件夹 [!DNL Workfront Proof]，则会自动为文件夹中所有现有项目以及随后添加的项目授予只读权限。

有关更多信息，请参阅 [在中共享文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

### 查看者 {#reviewer}

![cleaner.png](assets/cleaner.png) 可以查看校样

![cleaner.png](assets/cleaner.png) 可以添加标记

![cleaner.png](assets/cleaner.png) 可以添加注释

![[!DNL cleaner].png](assets/cleaner.png) 如果没有回复，可以编辑自己的评论

![no.png](assets/no.png) 无法作出决定

![no.png](assets/no.png) 无法编辑或删除他人的评论

![no.png](assets/no.png) 对校样没有编辑权限

### 审批者 {#approver}

![cleaner.png](assets/cleaner.png) 可以查看校样

![cleaner.png](assets/cleaner.png) 能做决定

![no.png](assets/no.png) 无法添加标记

![no.png](assets/no.png) 无法添加注释

![no.png](assets/no.png) 无法编辑或删除他人的评论

![no.png](assets/no.png) 对校样没有编辑权限

### 审核人和批准者 {#reviewer-approver}

![cleaner.png](assets/cleaner.png) 可以查看校样

![cleaner.png](assets/cleaner.png) 可以添加标记

![cleaner.png](assets/cleaner.png) 可以添加注释

![[!DNL cleaner].png](assets/cleaner.png) 如果没有回复，可以编辑自己的评论

![cleaner.png](assets/cleaner.png) 能做决定

![no.png](assets/no.png) 无法编辑或删除他人的评论

![no.png](assets/no.png) 对校样没有编辑权限

### 作者 {#author}

![cleaner.png](assets/cleaner.png) 可以添加标记

![cleaner.png](assets/cleaner.png) 可以添加注释

![[!DNL cleaner].png](assets/cleaner.png) 如果没有回复，可以编辑自己的评论

![cleaner.png](assets/cleaner.png) 能做决定

![cleaner.png](assets/cleaner.png) 可以提交新版本

![cleaner.png](assets/cleaner.png) 可以创建校样的副本

![cleaner.png](assets/cleaner.png) 可以和别人分享证据

![cleaner.png](assets/cleaner.png) 可以对注释应用操作

![cleaner.png](assets/cleaner.png) 可以解析注释

![no.png](assets/no.png) 无法编辑或删除他人的评论

>[!NOTE]
>
>此角色只能分配给 [!DNL Workfront Proof]

### 审阅人 {#moderator}

![cleaner.png](assets/cleaner.png) 可以添加标记

![cleaner.png](assets/cleaner.png) 可以添加注释

![[!DNL cleaner].png](assets/cleaner.png) 如果没有回复，可以编辑自己的评论

![cleaner.png](assets/cleaner.png) 能做决定

![cleaner.png](assets/cleaner.png) 可以提交新版本

![cleaner.png](assets/cleaner.png) 可以添加新审阅人

![cleaner.png](assets/cleaner.png) 可以对注释应用操作

![cleaner.png](assets/cleaner.png) 可以解析注释

![cleaner.png](assets/cleaner.png) 可以删除对证明的评论和回复（由自己或他人提出）

* 删除注释线程中的第一个注释将删除整个线程
* 删除注释线程中的回复将仅删除该回复

![no.png](assets/no.png) 无法编辑他人的评论

此角色允许人员管理和审核校样评论，使他们有机会仅保留校样的相关评论并删除非相关评论。

>[!NOTE]
>
>此角色只能分配给 [!DNL Workfront Proof].

## 分配校样角色

您可以在创建新校样、创建现有校样的新版本或基于现有校样时分配校样角色。

* [新校样](#new-proofs)
* [新版本](#new-versions)
* [现有校样](#existing-proofs)

### 新校样 {#new-proofs}

可以为 [!UICONTROL 新校样] 页面(1)。

![Proof_roles_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### 新版本 {#new-versions}

创建新版本校样时，将自动显示之前版本的审阅人（与之前版本具有相同的角色）。

创建新版本(1)时，您可以编辑应用于审阅人的校样角色。

![Proof_roles_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### 现有校样 {#existing-proofs}

如果要更改人员在现有校样中的角色，可以在 [!UICONTROL 校样详细信息] 页面(1)，通过内联编辑他们在工作流部分中的角色：

![Proof_Roles_-_Proof_Details_page_2.png](assets/proof-roles---proof-details-page-2-350x131.png)

## 在校样查看器中检查角色

您可以直接从校样查看器(1)中检查审阅者的角色，并根据需要对其进行编辑(2)。

![Proof_roles_-_Proof_Viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## 默认校样角色

您可以在 [!DNL Proofing Defaults] 页面。 这意味着当您添加到校样时，将自动填充默认校样角色。 请注意，具有校样编辑权限的用户可以在校样级别更改此角色。

>[!NOTE]
>
>只有具有管理员或帐单管理员配置文件的用户才能更改其帐户中其他用户的校对默认值。

有关更多信息，请参阅 [中的个人设置 [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## 创建者和所有者

创建者和所有者对校样具有完全编辑权限。

* [创建者](#creators)
* [所有者](#owners)

### 创建者 {#creators}

校样创建者是在第一个实例中上传校样的人。 校样创建者将自动显示在校样的人员列表中（在其默认角色中）。

在 [!UICONTROL 新校样] 页面，您可以为校样创建者分配不同的校样角色（除其默认角色外）。

不能更改校样创建者或从校样中删除校样创建者。

### 所有者 {#owners}

默认情况下，创建者也是校样的所有者；但是，创建者在最初创建校样时，可以将其他人设为校样所有者(在 [!UICONTROL 新校样] 页面)。

要在New校样页面上更改所有者，请执行以下操作：

1. 单击创建者名称旁边显示的更改链接。
1. 从下拉菜单中选择新的所有者。 (2)

![Proof_roles_-_new_proof_page_change_owner_2.png](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

创建校样后，仍然可以更改所有者。 对校样具有编辑权限的任何人都可以通过 [!UICONTROL 校样详细信息] 页面（请参阅下文）。

从工作流管理的角度来看，更改校样所有者的功能特别有用。 它允许项目负责人接管校样的所有权，并赋予他们校样的编辑权限，以及在 [!UICONTROL 我的校样] 中。

要通过 [!UICONTROL 校样详细信息] 页面：

* 单击要成为所有者的人员姓名旁边的“操作”菜单
* 选择 [!UICONTROL 成为所有者] 下拉菜单中。
* 或者，您也可以单击 [!UICONTROL 所有者] 字段，然后从显示的下拉列表中选择新的“所有者”。

完成此操作后，“所有者”一词将显示在该人员姓名旁边。

>[!NOTE]
>
>只有来自同一帐户或合作伙伴帐户的用户才能成为校样的所有者。 只有符合以下条件时，合作伙伴帐户中的用户才能成为校样的所有者：
>
>* 帐户之间已设置现有的合作伙伴关系。 有关更多信息，请参阅 [合作伙伴帐户 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* 上没有自定义字段 [!UICONTROL 新校样] 页面。
>* 校样尚未分配给文件夹。
>* 尚未对校样应用标记。
>




在中临时委派校样所有权 [!DNL Workfront Proof]，请参阅 [在中指定临时校样所有者 [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
