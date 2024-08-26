---
title: 使用Adobe Workfront Planning时的许可证类型概述
description: 除了对象的权限外，您对Adobe Workfront Planning的访问权限还取决于您的许可证类型。 并非组织中的所有用户都具有相同的访问权限和权限来使用Adobe Workfront Planning。 本文介绍了用户对Adobe Workfront Planning的访问权限级别。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: f9abcd9ff4c80376bed229a1d65e0efcbfc332b0
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---


# 使用Adobe Workfront Planning时的许可证类型概述

{{planning-important-intro}}

您的Adobe Workfront许可证类型可与Adobe Workfront Planning权限配合使用，以提供以下访问权限：

* 查看、提供或管理工作区
* 查看或管理视图。

有关Workfront Planning中对象权限的信息，请参阅[Adobe Workfront Planning中的权限共享概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

有关访问Workfront Planning的信息，请参阅[访问概述](/help/quicksilver/planning/access/access-overview.md)。

## Workfront许可证类型与Workfront Planning权限之间的关系

下表描述了Adobe Workfront中用户的许可证类型与您可以根据该许可证向他们授予Adobe Workfront Planning对象的权限级别之间的关系。

向用户授予对工作区的权限也会授予他们记录类型、记录和字段的权限。

除了用户拥有的工作区权限之外，还必须向用户授予单独的视图权限，以便用户能够访问和管理视图。

| Adobe Workfront许可证类型* | Adobe Workfront Planning中允许的最高权限 |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 标准 | <p>用户可以管理工作区和视图。 他们可以创建、编辑或删除工作区、记录类型、记录、字段和视图。</p> <br> <p>系统管理员对所有工作区具有管理权限，包括他们未创建的工作区。</p> |
| 浅色或参与者 | <p>用户可以查看与其共享的工作区，以及这些工作区的记录类型、记录和字段。</p> <br> <p>用户可以查看与其共享的视图，但不能创建自己的视图。 </p><br> <p>用户无法创建、编辑或删除工作区、记录类型、记录或字段。</p> |

*Workfront Planning不适用于旧版Workfront许可证。
有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


<!--OLD 

| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

### 许可证类型和工作区权限

只有具有Standard许可证的用户才能拥有工作区的Contribute或“管理”权限。 具有所有其他许可证类型的用户都可以拥有查看与其共享的工作区的权限。

系统管理员可以查看系统中的所有工作区，甚至包括他们未创建的工作区。

>[!INFO]
>
>**示例：**
>
>参与者或轻量级许可证用户无法参与或管理工作区及其对象。
>
>共享框中有一个指示，当用户拥有较低级别的许可证时，无法向其授予参与工作区或管理工作区的权限，因为这些权限级别灰显。
>
>![](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### 许可证类型和查看权限

只有具有Standard许可证的用户才能拥有视图的管理权限。 具有所有其他许可证类型的用户均可以拥有查看与其共享的视图的权限。

>[!INFO]
>
>**示例：**
>
>参与者或轻量级许可证用户无法管理视图。 他们可以应用临时过滤器、排序或分组到他们可以访问的视图。
>
>共享框中有一个指示，当用户拥有较低级别的许可证时，无法授予用户管理视图的权限，因为这些权限级别灰显。
>
>![](assets/permissions-grayed-out-for-light-user.png)
