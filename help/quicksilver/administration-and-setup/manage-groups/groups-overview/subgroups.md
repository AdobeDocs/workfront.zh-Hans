---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: 子组概述
description: 您最多可以在一个组下创建14级子组。 在任意这些级别上，可以创建不限数量的并行子组。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# 子组概述

您最多可以在一个组下创建14级子组。 在任意这些级别上，可以创建不限数量的并行子组。 有关说明，请参阅[创建子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)。

有关组的信息，请参阅[组概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md)。

## 子组会继承哪些内容？

子组继承其父组的成员资格。 因此，子组中的用户和组与属于它们共享的父组的用户和组具有相同的可见性、权限和对所有对象的访问权限。

此外，子组会自动继承其顶级组的组管理员，但您也可以分配子组的成员以充当其组管理员。

>[!TIP]
>
>有时，您可能希望使用子组将多个用户添加到现有组，以便授予他们访问所需对象的权限。
>
>例如，假设您有一组帮助台技术人员和单独的一组IT主管。 技术支持组具有对特定请求队列的权限。 您希望将IT主管添加到技术支持组，以便他们也可以拥有请求队列的权限。 如果没有子组功能，您必须手动将IT主管添加到技术支持组，这会效率低下且难以管理。 如果您将IT主管组作为子组添加到技术支持组，则只需一次更改即可更快地完成此任务。

>[!NOTE]
>
>如果将用户分别添加到子组及其父组，则从其中一个组中删除该用户不会从另一个组中删除该用户。 如果您不希望用户具有父组的访问权限，则必须从子组和父组中移除该用户。

## 公共和私有子组

对于公共组，任何具有编辑用户访问权限的用户（在组中或组外）都可以将该组添加到其他用户的配置文件中。 他们无法为专用组执行此操作。

您只能在具有多个级别的组的层次结构中的顶层父组上编辑此选项。 父组的所有子组将继承其设置。

如果在公共组下创建子组，则缺省情况下该子组也是公共的。 有关创建组并将其公开的详细信息，请参阅[创建组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)。 有关编辑用户所需访问权限的详细信息，请参阅[授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

添加到现有组的任何组都会自动成为子组，而不再是主组。 但是，子组会保留其现有用户，以及与项目、问题和任务的任何关联，以及属于新父组的所有项目、任务和问题状态。

## 子组的组管理员

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

在创建或编辑子组时，您可以将子组成员指定为子组的组管理员。 有关说明，请参阅[创建组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)一文中的[](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create)。

或者，也可以将子组的管理权留给分配给其上方的组的组管理员。 创建子组时，其上组的组管理员具有管理该子组的自动访问权限。

>[!NOTE]
>
>如果将用户添加到子组，并且该用户是该子组之上任何位置的组的组管理员，则该用户具有管理该子组的管理权限，即使未被分配为该子组的组管理员。

要了解哪些操作适用于管理Workfront系统的Adobe Workfront管理员、管理顶级组的组管理员以及管理子组的组管理员，请参阅[不同类型管理员允许的操作](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md)。
