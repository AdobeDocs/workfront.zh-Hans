---
title: 使用Adobe Workfront Planning时的许可证类型概述
description: 除了对象的权限外，您对Adobe Workfront Planning的访问权限还取决于您的许可证类型。 并非组织中的所有用户都具有相同的访问权限和权限来使用Adobe Workfront Planning。 本文介绍了用户对Adobe Workfront Planning的访问权限级别。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---


# 使用Adobe Workfront Planning时的许可证类型概述

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

您的Adobe Workfront许可证类型可与Adobe Workfront Planning权限配合使用，以提供以下访问权限：

* 查看、参与或管理工作区或记录类型
* 查看或管理视图。

有关Workfront Planning中对象权限的信息，请参阅[Adobe Workfront Planning中的权限共享概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

有关访问Workfront Planning的信息，请参阅[Adobe Planning访问概述](/help/quicksilver/planning/access/access-overview.md)。

## Workfront许可证类型与Workfront Planning权限之间的关系

下表描述了Adobe Workfront中用户的许可证类型与您可以根据该许可证向他们授予Adobe Workfront Planning对象的权限级别之间的关系。

向用户授予对工作区的权限也会授予他们记录类型、记录和字段的权限。

除了用户拥有的工作区权限之外，还必须向用户授予单独的视图权限，以便用户能够访问和管理视图。

使用记录类型权限时，请考虑以下事项：

* 用户自动从工作区继承记录类型权限。
* 当用户具有工作区的管理权限时，他们对记录类型的访问权限不能减少到仅此而已。
* 用户对于记录类型的权限不能超过其对于该记录类型所属的工作区的权限。
* 删除用户对记录类型的权限不会删除他们对工作区中所有记录类型的查看访问权限，因为这不会删除他们对工作区的权限。

| Adobe Workfront许可证类型* | Adobe Workfront Planning中允许的最高权限 |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 标准 | <p>用户可以管理工作区、记录类型和视图。 他们可以创建、编辑或删除工作区、记录类型、记录、字段和视图。</p> <br> <p>系统管理员对所有工作区具有管理权限，包括他们未创建的工作区。</p> |
| 浅色或参与者 | <p>用户可以查看与其共享的工作区，以及这些工作区的记录类型、记录和字段。</p> <br> <p>用户可以查看与其共享的视图，但不能创建自己的视图。 </p><br> <p>用户无法创建、编辑或删除工作区、记录类型、记录或字段。</p> |

*Workfront Planning不适用于旧版Workfront许可证。
有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


### 许可证类型以及工作区和记录类型的权限

只有具有Standard许可证的用户才能对工作区和记录类型具有Contribute或Manage权限。 工作区和记录类型的Contribute和Manage权限也会传输到记录和字段。

具有所有其他许可证类型的用户均可以拥有对共享给他们的工作区和记录类型及其记录和字段的查看权限。

系统管理员可以查看系统中的所有工作区，包括他们未创建的工作区。

>[!INFO]
>
>**示例：**
>
>参与者或轻量级许可证用户无法参与或管理工作区及其对象。
>
>共享框中有一个指示，当用户拥有较低级别的许可证时，无法向其授予参与工作区或管理工作区的权限，因为这些权限级别灰显。
>
>![参与者用户在工作区中的权限灰显](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### 许可证类型和视图权限

只有具有Standard许可证的用户才能拥有视图的管理权限。 具有所有其他许可证类型的用户均可以拥有查看与其共享的视图的权限。

>[!INFO]
>
>**示例：**
>
>参与者或轻量级许可证用户无法管理视图。 他们可以应用临时过滤器、排序或分组到他们可以访问的视图。
>
>共享框中有一个指示，当用户拥有较低级别的许可证时，无法授予用户管理视图的权限，因为这些权限级别灰显。
>
>![权限在视图共享上对于轻量级用户呈灰显状态](assets/permissions-grayed-out-for-light-user.png)
