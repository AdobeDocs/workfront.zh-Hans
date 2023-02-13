---
title: Adobe Workfront许可证概述
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 许可证，类型
navigation-topic: access-levels
description: 贵组织在收购Adobe Workfront时购买了一定数量的许可证。 作为Workfront管理员，在为用户分配访问级别时，您需要向每个用户分配四种类型的付费Workfront许可证之一。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7f30e2d8-f5c3-4811-b780-49a2b0d058e7
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 2%

---

# Adobe Workfront许可证概述

贵组织在收购Adobe Workfront时购买了一定数量的许可证。 作为Workfront管理员，在为用户分配访问级别时，您需要向每个用户分配四种类型的付费Workfront许可证之一。

## Workfront许可证和访问级别如何绑定在一起

这4种类型的付费Workfront许可证允许不同级别的访问Workfront。 每个访问级别都附加到其中一个许可证。

作为Workfront管理员，您无需为用户分配许可证，而是为用户分配附加到该许可证的访问权限级别。

此表和图表显示了对Workfront的主要访问级别：

| 许可证 | 关联的访问级别 |
|--- |--- |
| 计划 | 计划员系统管理员 |
| 工作 | 员工 |
| 复查 | 查看者 |
| 外部的* | 外部用户 |

>[!NOTE]
>
>外部许可证不是付费许可证。 它主要用于与不使用Workfront的协作者共享文档。 有关更多信息，请参阅 [Adobe Workfront中的内置访问级别](default-access-levels-in-workfront.md).

![](assets/licenses-and-access-levels.png)

## 许可证如何定义访问级别

附加到访问级别的许可证决定了访问级别中可用功能的总体范围。

您可以复制默认访问级别，并根据需要为用户自定义副本。 在许可证允许的复制访问级别功能范围内，您可以调整访问设置以满足用户的需求。

有关更多信息，请参阅 [访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) 和 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## 许可证计数

在为用户分配访问级别时，可用的许可证计数会减少1。

例如，如果将计划员访问权限级别分配给用户，则可用计划许可证的数量将减少1。

您可以查看分配给用户的许可证和访问级别。 有关更多信息，请参阅 [列出用户的访问级别和许可证](../../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md).

有关管理许可证的信息，请参阅 [管理系统中的可用许可证](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
