---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: 子组概述
description: 您最多可以在一个组下创建14个级别的子组。 在这些级别中的任一级别上，您可以创建无限数量的并行子组。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# 子组概述

您最多可以在一个组下创建14个级别的子组。 在这些级别中的任一级别上，您可以创建无限数量的并行子组。 有关说明，请参阅 [创建子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

有关群组的信息，请参阅 [群组概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## 子组将继承什么？

子组将继承其父组的成员资格。 因此，子组中的用户和组与其共享的父组所属的用户和组具有相同的可见性、权限和对所有对象的访问权限。

此外，子组会自动继承其顶级组的组管理员，但您也可以分配子组的成员以充当其组管理员。

>[!TIP]
>
>有时，您可能希望使用子组向现有组添加多个用户，以便他们有权访问所需的对象。
>
>例如，假定您拥有一组帮助台技术人员和一组单独的IT主管。 帮助台组有权访问特定请求队列。 您希望将IT控制器添加到帮助台组，以便他们也有权使用请求队列。 如果没有子组功能，您必须手动将IT控制器添加到帮助台组，这可能效率低下且难以管理。 如果将IT控制器组作为子组添加到帮助台组，则只需一次更改即可更快地完成此任务。

>[!NOTE]
>
>如果将某个用户分别添加到子组及其父组，则从一个组中删除该用户时，不会从另一个组中删除该用户。 如果您不希望用户具有允许父组访问的权限，则必须同时从子组和父组中删除该用户。

## 公共和私人子组

对于公共群组，任何具有编辑用户访问权限的用户（群组内或群组外）都可以将群组添加到其他用户的配置文件中。 他们不能为私人组执行此操作。

您只能在具有多个级别的组层次结构中的顶层父组上编辑此选项。 父组的所有子组将继承其设置。

如果在公共的组下创建子组，则默认情况下，该子组也是公共的。 有关创建群组并将其公开的更多信息，请参阅 [创建群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 有关编辑用户所需访问权限的更多信息，请参阅 [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

添加到现有组的任何组都会自动变成子组，不再是主组。 但是，除了属于新父组的所有项目、任务和发布状态之外，子组还会保留其现有用户以及与项目、问题和任务的任何关联。

## 子组的组管理员

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

在创建或编辑子组时，可以将子组成员指定为组管理员。 有关说明，请参阅 [](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) 在文章中 [创建群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

或者，也可以将子组的管理保留给分配给其上方组的组管理员。 在创建子组时，组管理员对其上的组具有管理子组的自动访问权限。

>[!NOTE]
>
>如果将用户添加到子组，并且该用户是子组上方任何位置的组的组管理员，则该用户具有管理子组的管理权限，即使未被指派为该子组的组管理员。

要了解哪些操作可供管理Workfront系统的Adobe Workfront管理员、管理顶级群组的群组管理员以及管理子群组的群组管理员使用，请参阅 [允许对不同类型管理员执行的操作](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
