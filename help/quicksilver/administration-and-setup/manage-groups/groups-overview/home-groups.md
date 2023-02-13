---
title: 主页组概述
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: 在用户的配置文件中分配了“主页组”。 所有用户都需要拥有主页组。 一个用户可以属于多个组，但只能拥有一个主页组。 虽然系统中的任何现有组都可以分配为用户的主组，但我们建议创建和分配代表较大组织单位的新组。 在建立主组时，请考虑您的组织如何划分Adobe Workfront用户。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 主页组概述

在用户的配置文件中分配了“主页组”。 所有用户都需要拥有主页组。 一个用户可以属于多个组，但只能拥有一个主页组。 有关群组的更多信息，请参阅 [群组概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

虽然系统中的任何现有组都可以分配为用户的主组，但我们建议创建和分配代表较大组织单位的新组。

在建立主组时，请考虑您的组织如何划分Adobe Workfront用户。 以下是一些建议，用于确定应将哪种类型的组用作主页组：

* 代表部门的组，如IT或营销
* 受不同预算管理的组
* 位于不同区域或区域的组
* 由属于同一成本中心的多个团队组成的组

>[!NOTE]
>
>如果需要将家庭组重组为组织单位，则需要>
>1. 创建新组，如 [创建群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).
>1. 将新组重新指派为用户的主组，如 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>


## 布局模板管理

将布局模板分配给组后，所有将该组分配为其主页组的用户都可以查看布局模板中指定的设置。

如果将布局模板分配给主页组，则仅对分配给该主页组的用户可见。

有关更多信息，请参阅 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) in [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## 许可证管理

每个用户只能分配到一个主组，这样便于管理许可证计数。

Workfront管理员可以选择为主组设置最大许可证计数。

通过设置最大许可证计数，Workfront管理员可以阻止业务部门使用为其他业务部门购买的Workfront许可证。

有关更多信息，请参阅 [管理系统中的可用许可证](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
