---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: 了解 [!DNL Workfront Proof]
description: 如果人员有权查看文件夹中的项目，则他们也可以查看文件夹本身。 但是，他们只能查看文件夹中明确与他们共享的项目。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 16%

---

# 了解 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

如果人员有权查看文件夹中的项目，则他们也可以查看文件夹本身。 但是，他们只能查看文件夹中明确与他们共享的项目。

## 公共文件夹

如果文件夹是公用的，则帐户中的用户（不包括“观察者”和“轻量级用户”）可以在左侧栏中看到文件夹名称。

您的权限配置文件还会影响您对公共文件夹拥有的权限：

| **用户档案/操作** | **查看文件夹中的所有项目** | **查看明确与他们共享的项目** | **添加项目** | **删除项目** | **添加子文件夹** | **删除子文件夹** | **编辑文件夹详细信息** |
|---|---|---|---|---|---|---|---|
| **创建者** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **帐单管理员** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **管理员** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **监督人** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **经理** | 否 | 是 | 是 | 否 | 是 | 否 | 是 |
| **观察人** | 否 | 是 | 否 | 否 | 否 | 否 | 否 |

{style="table-layout:auto"}

如果公共文件夹归经理所有，则他/她可以删除根文件夹和任何子文件夹。

有关更多信息，请参阅 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## 专用文件夹

如果文件夹是专用文件夹，则同一帐户中的其他用户将无法在左边栏中看到文件夹的名称，除非已与他们明确共享该文件夹或文件夹中的项目，或者他们具有主管、管理员或账单管理员的配置文件：

| **用户档案/操作** | **查看文件夹中的所有项目** | **查看明确与他们共享的项目** | **添加项目** | **删除项目** | **添加子文件夹** | **删除子文件夹** | **编辑文件夹详细信息** |
|---|---|---|---|---|---|---|---|
| **创建者** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **帐单管理员** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **管理员** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **监督人** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **经理** | 否 | 是 | 否 | 否 | 否 | 否 | 否 |
| **观察人** | 否 | 是 | 否 | 否 | 否 | 否 | 否 |

{style="table-layout:auto"}

例如，如果您希望项目经理及其团队仅查看特定文件夹，则项目经理可以设置一个专用文件夹，然后与特定用户共享该文件夹。

在共享专用文件夹时，您可以决定是否希望管理器能够创建、编辑和删除文件夹项目。

您可以在“新建文件夹”页面上单独为每个人员设置此设置，并在 [!UICONTROL 共享] 文件夹详细信息页面的部分。 有关更多信息，请参阅 [在中创建文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) 和 [在中管理文件夹及其内容 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

如果与或观察者共享专用文件夹，则他们将对文件夹中的所有项目具有只读访问权限。 有关更多信息，请参阅 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 和 [在中共享文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* 如果父文件夹是专用文件夹，则所有子文件夹也将是专用文件夹。 私有父文件夹下不能有公共子文件夹。 但是，您可以在公共父文件夹下有一个专用子文件夹。
>* 文件夹的创建者和所有者将始终有权访问该文件夹，并且不可删除。
>* 只有专用文件夹的创建者和所有者才能删除该文件夹。


