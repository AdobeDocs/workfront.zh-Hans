---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: 了解 [!DNL Workfront Proof]中的文件夹权限
description: 如果人员有权查看文件夹中的项目，他们还可以查看文件夹本身。 但是，他们只能查看文件夹中明确与其共享的项目。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 15%

---

# 了解[!DNL Workfront Proof]中的文件夹权限

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

如果人员有权查看文件夹中的项目，他们还可以查看文件夹本身。 但是，他们只能查看文件夹中明确与其共享的项目。

## 公共文件夹

如果文件夹为公共文件夹，则帐户中的用户（不包括观察者和轻量级用户）可以在左侧边栏中看到文件夹名称。

您的权限配置文件也会影响您对公共文件夹拥有的权限：

| **配置文件/操作** | **查看文件夹中的所有项目** | **查看与他们显式共享的项目** | **添加项目** | **删除项目** | **添加子文件夹** | **删除子文件夹** | **编辑文件夹详细信息** |
|---|---|---|---|---|---|---|---|
| **创建者** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **帐单管理员** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **管理员** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **主管** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **经理** | 否 | 是 | 是 | 否 | 是 | 否 | 是 |
| **观察者** | 否 | 是 | 否 | 否 | 否 | 否 | 否 |

{style="table-layout:auto"}

如果公共文件夹归经理所有，则经理可以删除根文件夹和任何子文件夹。

有关详细信息，请参阅 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的校对权限配置文件。

## 专用文件夹

如果某个文件夹是私有文件夹，则同一帐户中的其他用户无法在左侧边栏中看到该文件夹的名称，除非该文件夹中的一个或多个项目已明确与其共享，或者他们具有“主管”、“管理员”或“账单管理员”配置文件：

| **配置文件/操作** | **查看文件夹中的所有项目** | **查看与他们显式共享的项目** | **添加项目** | **删除项目** | **添加子文件夹** | **删除子文件夹** | **编辑文件夹详细信息** |
|---|---|---|---|---|---|---|---|
| **创建者** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **帐单管理员** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **管理员** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **主管** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **经理** | 否 | 是 | 否 | 否 | 否 | 否 | 否 |
| **观察者** | 否 | 是 | 否 | 否 | 否 | 否 | 否 |

{style="table-layout:auto"}

例如，如果您希望项目经理及其团队仅查看特定文件夹，则项目经理可以设置专用文件夹，然后与特定用户共享该文件夹。

在共享专用文件夹时，您可以决定是否希望管理员能够创建、编辑和删除文件夹项目。

您可以在“新建文件夹”页面上为每个人单独设置此项，并在“文件夹详细信息”页面的“共享对象”部分中对其进行更改。 有关详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md)中创建文件夹，以及[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md)中管理文件夹及其内容。

如果与或观察者共享专用文件夹，则他们将对该文件夹中的所有项目具有只读访问权限。 有关详细信息，请参阅 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[验证权限配置文件和 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md)中的共享文件夹。

>[!NOTE]
>
>* 如果父文件夹是私有的，则所有子文件夹也是私有的。 在私有父文件夹下不能有公共子文件夹。 但是，您可以在公共父文件夹下拥有私有子文件夹。
>* 文件夹的创建者和所有者将始终具有其访问权限，并且无法移除。
>* 只有专用文件夹的创建者和所有者可以删除该文件夹。

