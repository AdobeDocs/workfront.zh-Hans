---
title: 主组概述
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: 主组在用户配置文件中分配。 所有用户都必须有一个主组。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# 主组概述

主组在用户配置文件中分配。 所有用户都必须有一个主组。 一个用户可以属于多个组，但他们只能有一个主组。 有关组的详细信息，请参阅[组概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md)。

尽管系统中的任何现有组都可以指定为用户的主组，但我们建议创建和分配代表较大组织单位的新组。

建立主组时，请考虑您的组织如何划分Adobe Workfront用户。 以下是一些建议，以确定应将哪种类型的组用作主组：

* 代表部门（如IT或营销）的组
* 受不同预算控制的组
* 位于不同区域或区域的组
* 由属于同一成本中心的多个团队组成的组

>[!NOTE]
>
>如果需要将主组重新组织为组织单位，您需要>
>1. 按照[创建组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的说明创建新组。
>1. 按照[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)中的说明，将新组重新指定为用户的主组。
>

## 布局模板管理

将布局模板分配给组时，将该组作为其主组分配的所有用户都可以查看在布局模板中指定的设置。

如果将布局模板分配给主组，则它仅对分配给该主组的用户可见。

有关详细信息，请参阅[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中的[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

## 许可证管理

每个用户只能分配给一个主组，这样可以更轻松地管理许可证计数。

Workfront管理员可以选择设置主组的最大许可证计数。

设置许可证数量上限可让Workfront管理员阻止业务部门使用为其他业务部门购买的Workfront许可证。

有关详细信息，请参阅[管理系统中的可用许可证](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)。
