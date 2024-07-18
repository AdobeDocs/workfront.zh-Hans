---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 通过Adobe Admin Console删除用户
description: 您只能从Adobe Workfront Fusion中删除用户，而保留对任何其他Adobe产品配置文件的访问权限，或者可以从Adobe Admin Console中完全删除该用户。
author: Becky
feature: Workfront Fusion
exl-id: 0d989134-46c0-4637-b465-6fbe04258b8a
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# 通过[!DNL Adobe Admin Console]删除用户

>[!IMPORTANT]
>
>本文中的功能仅在贵组织的[!DNL Adobe Workfront Fusion]实例已载入[!DNL Adobe Business Platform]时才可用。
>
>有关因贵组织是否已登记到[!DNL Adobe Business Platform]而不同的过程列表，请参阅[基于平台的管理差异([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md)。

您只能从[!DNL Adobe Workfront Fusion]中删除用户，而保留对任何其他[!DNL Adobe]产品配置文件的访问权限，或者您可以从[!DNL Adobe Admin Console]中完全删除该用户。

## 删除[!DNL Adobe Workfront Fusion]中的用户

若要删除[!DNL Adobe Workfront Fusion]中的用户，必须通过[!DNL Adobe Admin Console]取消激活该用户。

当满足以下任一条件时，将从[!DNL Adobe Admin Console]取消激活用户：

* 用户将从产品或产品配置文件中移出，且不会分配到任何其他产品或产品配置文件。
* 将从链接到产品配置文件的组中删除用户，但不包含在与产品配置文件链接的任何其他组中。
* 该用户将从产品配置文件中删除，并且未分配给其他产品配置文件。
* 在包括Workfront Fusion的组织中删除或停用用户。

  有关说明，请参阅[单独管理用户](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)中的“删除用户”部分。

在[!DNL Workfront Fusion]中，停用会以下列方式之一影响用户：

* 如果用户仅在一个组织中，则停用该用户。
* 如果用户位于多个组织中，则会将该用户从在[!DNL Adobe Admin Console]上修改该用户的组织中删除。
* 有关在[!DNL Workfront Fusion]中删除用户时的其他注意事项，请参阅[在 [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)中删除用户时的注意事项
