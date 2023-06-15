---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 通过Adobe Admin Console删除用户
description: 您只能从Adobe Workfront Fusion中删除用户，而保留对任何其他Adobe产品配置文件的访问权限，或者也可以从Adobe Admin Console中完全删除该用户。
author: Becky
feature: Workfront Fusion
exl-id: 0d989134-46c0-4637-b465-6fbe04258b8a
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 删除用户，通过 [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>本文中的功能仅在贵组织的实例以下情况下可用： [!DNL Adobe Workfront Fusion] 已载入 [!DNL Adobe Business Platform].
>
>对于因贵组织是否已载入到以下版本而不同的过程，请参见 [!DNL Adobe Business Platform]，请参见 [基于平台的管理差异([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

您可以从中删除用户 [!DNL Adobe Workfront Fusion] 仅限，将访问权限保留给任何其他 [!DNL Adobe] 产品配置文件，或者您可以从 [!DNL Adobe Admin Console] 全部。

## 删除中的用户 [!DNL Adobe Workfront Fusion]

删除中的用户 [!DNL Adobe Workfront Fusion]，您必须通过取消激活用户 [!DNL Adobe Admin Console].

将从取消激活用户 [!DNL Adobe Admin Console] 当满足以下条件之一时：

* 用户将从产品或产品配置文件中移出，且不会分配到任何其他产品或产品配置文件。
* 将从链接到产品配置文件的组中删除用户，并且该用户不包含在链接到产品配置文件的任何其他组中。
* 用户将从产品配置文件中删除，并且未分配给其他产品配置文件。
* 在包含Workfront Fusion的组织中删除或停用用户。

  有关说明，请参阅中的“删除用户”部分 [单独管理用户](https://helpx.adobe.com/enterprise/using/manage-users-individually.html).

In [!DNL Workfront Fusion]时，停用会以下列方式之一影响用户：

* 如果用户仅在一个组织中，则该用户将被停用。
* 如果用户位于多个组织中，则会将该用户从在中修改该用户的组织中移除。 [!DNL Adobe Admin Console].
* 有关删除中的用户时的其他注意事项 [!DNL Workfront Fusion]，请参见 [在中删除用户时的注意事项 [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)
