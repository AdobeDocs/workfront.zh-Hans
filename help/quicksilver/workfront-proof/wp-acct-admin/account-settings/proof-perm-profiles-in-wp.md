---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 在Workfront校样中校样权限配置文件
description: 作为Workfront管理员或Workfront校样管理员，您可以向用户分配校样权限配置文件，以指定用户将对系统中的所有校样具有的校样功能。 有关配置用户校样权限配置文件的信息，请参阅在Workfront校样中配置用户的校样权限配置文件。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '1766'
ht-degree: 1%

---

# 中的校样权限配置文件 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

As a [!DNL Workfront] 管理员或 [!DNL Workfront Proof] 管理员，您可以为用户分配校样权限配置文件，以指定用户将对系统中的所有校样具有的校样功能。 有关配置用户校样权限配置文件的信息，请参阅 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>您还可以执行以下操作：
>
>* 为用户授予针对单个校样的特定角色。 有关校样角色的更多信息，请参阅 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>* 为组织中的用户创建自定义用户档案。 有关更多信息，请参阅 [在中配置自定义用户档案 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>


下表显示了每个校样权限配置文件的可用权限。

| **自有项目** |  |  |  |  | **其他用户的项目** |  |  | **管理** | **帐单** |
|---|---|---|---|---|---|---|---|---|---|
|  | **添加** | **查看** | **编辑** | **删除** | **查看** | **编辑** | **删除** | **编辑和删除** | **编辑** |
| 账单管理员 | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |
| 管理 | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |
| 监督人 | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |
| 经理 | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |   |   |   |
| 观察人 |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |
| 访客 |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style="table-layout:auto"}

请考虑以下关于角色和权限的事项：

* 分配的配置文件权限仅与您自己帐户中的用户和项目相关。 在卫星帐户中，主（中心）帐户的管理员和账单管理员可以从中心帐户级别访问和管理这些帐户的帐户设置和账单。
* 账单管理员和管理员可以删除用户。 此操作只能在帐户设置中完成。
* 当账单管理员和管理员查看其帐户中其他用户拥有的校样时，他们会以审核者的角色查看这些校样。
* 使用“只读”角色，帐单管理员和管理员可以在与其共享的文件夹或他们创建的文件夹中访问校样。

以下部分介绍了每个配置文件以及与标准中的配置文件关联的权限 [!DNL Workfront Proof] 设置：

* [帐单管理员](#billing-administrator)
* [管理员](#administrator)
* [监督人](#supervisor)
* [经理](#manager)
* [观察人](#observer)
* [访客](#visitor)
* [来宾](#guest)

## 帐单管理员 {#billing-administrator}

账单管理员有权访问 [中的帐户设置 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] 帐单页面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)，且具有以下权限：

![](assets/cleaner2.png)可以生成校样、上传文件和创建文件夹。 有关更多信息，请参阅 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [将文件和Web内容上传到 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)和 [在中创建文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)可以查看、编辑和删除自己创建的校样和文件。

![](assets/cleaner2.png)可以查看、编辑和删除组织中所有用户创建的校样和文件。

![](assets/cleaner2.png)可以删除其他用户的公共文件夹。 有关更多信息，请参阅 [在中管理文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)对帐户中创建的所有校样具有编辑权限。

![](assets/cleaner2.png)可以设置为Dropzone所有者。 有关更多信息，请参阅 [在中配置拖放区 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)可以访问帐单页面并编辑帐单详细信息。 有关更多信息，请参阅 [的 [!DNL Workfront Proof] 帐单页面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![](assets/cleaner2.png)可以访问帐户设置页面并编辑帐户详细信息。 有关更多信息，请参阅 [中的帐户设置 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)可以清空垃圾桶。 有关更多信息，请参阅 [在中还原和清空垃圾桶 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)可以添加、编辑和删除用户。

![](assets/cleaner2.png)可以创建组并添加新联系人。

![](assets/cleaner2.png)可以删除联系人。

![](assets/cleaner2.png)如果校样上没有回复，则可以编辑校样。

![](assets/no2.png)无法编辑校样回复。

![](assets/no2.png)无法删除其他用户的专用文件夹。 有关更多信息，请参阅 [在中管理文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

有关帐户设置的信息，请参阅 [中的帐户设置 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

有关帐单的信息，请参阅 [的 [!DNL Workfront Proof] 帐单页面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### 管理员 {#administrator}

管理员有权访问 [帐户设置](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)和具有以下权限：

![](assets/cleaner2.png)可以创建校样、上传文件和创建文件夹。 有关更多信息，请参阅 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [将文件和Web内容上传到 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)和 [在中创建文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)可以查看、编辑和删除其创建的校样和文件。

![](assets/cleaner2.png)可以查看、编辑和删除组织中所有用户创建的校样和文件。

![](assets/cleaner2.png)可以删除其他用户的公共文件夹。 有关更多信息，请参阅 [在中管理文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)对帐户中创建的所有校样具有编辑权限。

![](assets/cleaner2.png)可以设置为Dropzone所有者。 有关更多信息，请参阅 [在中配置拖放区 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)可以访问帐户设置页面并编辑帐户详细信息。 有关更多信息，请参阅 [中的帐户设置 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)可以清空垃圾桶。 有关更多信息，请参阅 [在中还原和清空垃圾桶 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)可以添加、编辑和删除用户。

![](assets/cleaner2.png)可以创建组并添加新联系人。

![](assets/cleaner2.png)可以删除联系人。

![](assets/cleaner2.png)如果校样上没有回复，则可以编辑校样。

![](assets/no2.png)无法编辑校样回复。

![](assets/no2.png)无法删除其他用户的专用文件夹。 有关更多信息，请参阅 [在中管理文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)无法访问帐单页面或编辑帐单详细信息。 有关更多信息，请参阅 [的 [!DNL Workfront Proof] 帐单页面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### 监督人 {#supervisor}

主管具有以下权限：

![](assets/cleaner2.png)可以创建校样、上传文件和创建文件夹。 有关更多信息，请参阅 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [将文件和Web内容上传到 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)和 [在中创建文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)可以查看、编辑和删除自己创建的校样和文件。

![](assets/cleaner2.png)可以查看、编辑和删除组织中所有用户创建的校样和文件。

![](assets/cleaner2.png)可以删除其他用户的公共文件夹。 有关更多信息，请参阅 [在中管理文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)对帐户中创建的所有校样具有编辑权限。

![](assets/cleaner2.png)可以设置为Dropzone所有者。 有关更多信息，请参阅 [在中配置拖放区 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)可以创建组并添加新联系人。

![](assets/cleaner2.png)可以删除联系人。

![](assets/cleaner2.png)如果校样上没有回复，则可以编辑校样。

![](assets/no2.png)无法编辑校样回复。

![](assets/no2.png)无法删除其他用户的专用文件夹。 有关更多信息，请参阅 [文件夹位于 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![](assets/no2.png)无法访问帐单页面或帐户设置。 有关更多信息，请参阅 [的 [!DNL Workfront Proof] 帐单页面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) 和 [中的帐户设置 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)无法添加、编辑或删除用户。

![](assets/no2.png)无法清空垃圾桶。 有关更多信息，请参阅 [在中还原和清空垃圾桶 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### 经理 {#manager}

经理具有以下权限：

![](assets/cleaner2.png)可以创建校样、上传文件和创建文件夹。 有关更多信息，请参阅 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [将文件和Web内容上传到 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)和 [在中创建文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)可以查看、编辑和删除自己创建或拥有的校样和文件。

![](assets/cleaner2.png)可以查看、审阅和批准其他用户与其明确共享的校样（对共享文件夹中所有内容的只读权限）。 有关更多信息，请参阅 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)可以创建组并添加新联系人。

![](assets/no2.png)无法查看、编辑或删除组织中其他用户创建的校样和文件。

![](assets/no2.png)无法编辑校样或回复。

![](assets/no2.png)无法删除其他用户的专用文件夹。 有关更多信息，请参阅 [在中管理文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)无法删除其他用户的公共文件夹。 有关更多信息，请参阅 [在中管理文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)无法访问帐单页面或帐户设置。 有关更多信息，请参阅 [的 [!DNL Workfront Proof] 帐单页面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) 和 [中的帐户设置 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)无法设置为Dropzone所有者。 有关更多信息，请参阅 [在中配置拖放区 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)无法清空垃圾桶。 有关更多信息，请参阅 [在中还原和清空垃圾桶 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)无法添加、编辑或删除用户。

![](assets/no2.png)无法删除联系人。

### 观察人 {#observer}

观察者具有以下权限：

![](assets/cleaner2.png)可以查看、审阅和批准其他用户与其明确共享的校样（对共享文件夹中所有内容的只读权限）。 有关更多信息，请参阅 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)可以查看与其明确共享的文件。

![](assets/cleaner2.png) 可以查看联系人和组

![](assets/no2.png)无法创建校样、上传文件和创建文件夹。 有关更多信息，请参阅 [将文件和Web内容上传到 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)无法查看、编辑或删除组织中其他用户创建的校样和文件。

![](assets/no2.png)无法编辑校样或回复。

![](assets/no2.png)无法删除组织中创建的任何项目。

![](assets/no2.png)无法访问帐单页面或帐户设置。 有关更多信息，请参阅 [的 [!DNL Workfront Proof] 帐单页面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) 和 [中的帐户设置 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)无法设置为Dropzone所有者。 有关更多信息，请参阅 [在中配置拖放区 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)无法清空垃圾桶。 有关更多信息，请参阅 [在中还原和清空垃圾桶 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)无法添加、编辑或删除用户。

![](assets/no2.png)无法创建组或添加新联系人。

![](assets/no2.png)无法删除联系人。

>[!NOTE]
>
>观察员可用的菜单和功能有限。
>
>* 观察者在其功能板中看不到标题菜单或绿色的新建菜单
>* 观察者在其“设置”中看不到以下链接：帐户设置，帐单
>


### 访客 {#visitor}

访客具有以下权限：

![](assets/cleaner2.png)可以查看、审阅和批准其他用户与其明确共享的校样（对共享文件夹中所有内容的只读权限）。 有关更多信息，请参阅 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)可以查看与其明确共享的文件。

![](assets/no2.png) 无法查看联系人和组

![](assets/no2.png)无法创建校样、上传文件和创建文件夹。 有关更多信息，请参阅 [将文件和Web内容上传到 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)无法查看、编辑或删除组织中其他用户创建的校样和文件。

![](assets/no2.png)无法编辑校样或回复。

![](assets/no2.png)无法删除组织中创建的任何项目。

![](assets/no2.png)无法访问帐单页面或帐户设置。 有关更多信息，请参阅 [的 [!DNL Workfront Proof] 帐单页面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) 和 [中的帐户设置 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)无法设置为Dropzone所有者。 有关更多信息，请参阅 [在中配置拖放区 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)无法清空垃圾桶。 有关更多信息，请参阅 [在中还原和清空垃圾桶 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)无法添加、编辑或删除用户。

![](assets/no2.png)无法创建组或添加新联系人。

![](assets/no2.png)无法删除联系人。

>[!NOTE]
>
>对访客可用的菜单和功能有限。
>
>* 访客在其功能板中看不到标题菜单或绿色的新菜单
>* 访客在其设置中看不到以下链接：帐户设置，帐单
>


### 来宾 {#guest}

来宾用户档案用于为没有自己Workfront Proof帐户的审阅人授予对校样的访问权限。 客人可以直接通过个人电子邮件通知访问与他们共享的校样。

![](assets/cleaner2.png)可以查看、审阅和批准与他们明确共享的校样。

![](assets/cleaner2.png)可以查看与其明确共享的文件。

![](assets/no2.png)无法访问功能板。

![](assets/no2.png)不能与他们共享文件夹。 有关更多信息，请参阅 [在中管理文件夹 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)无法作为作者或审核者添加到校样中。 有关更多信息，请参阅 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>来宾不是Workfront校样用户，因此他们无法在自己的功能板中看到与他们共享的所有校样。

## 编辑用户的校样权限配置文件

管理员和账单管理员可以编辑帐户中所有用户的权限配置文件。

1. 要查找要编辑的用户，请执行以下操作之一：

   * 导航到 **[!UICONTROL 帐户设置]**，然后单击 **[!UICONTROL 用户]** 选项卡。

   * 转到 **[!UICONTROL 联系人]** 页面。

1. 单击要编辑其权限的用户名称。 ![](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. 单击 **[!UICONTROL 权限配置文件]** 下拉菜单，然后选择新的权限配置文件。:

   ![Screenshot_2018-03-30_14-18-03.png](assets/screenshot-2018-03-30-14-18-03a.png)

   权限配置文件包括管理员、主管、经理和观察者。

1. 单击菜单外的任意位置进行保存。

>[!NOTE]
>
>管理员无法分配帐单管理员配置文件。 您可以在以下日志中找到配置文件更改列表：
>
>* 帐户活动日志
>* 用户的配置文件日志（仅该用户可访问）
>


有关活动日志的更多信息，请参阅 [了解 [!DNL Workfront Proof] 活动审核跟踪](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
