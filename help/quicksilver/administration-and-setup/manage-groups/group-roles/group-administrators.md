---
title: 组管理员
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: 在具有多个部门的大型组织中，Adobe Workfront管理员可能不希望管理这些部门中的所有部门和组。 相反，他们可以为该组中的每个部门和子组创建一个组，每个组由组管理员管理。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 850e0801511177efc5189258acd9b88234cf59c9
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# 组管理员

<!-- Audited: 12/2023 -->

在具有多个部门的大型组织中，Adobe Workfront管理员可能不希望管理这些部门中的所有部门和组。 相反，他们可以为该组中的每个部门和子组创建一个组，每个组由组管理员管理。

组管理员可以管理组的需求，例如用户成员资格、布局模板、自定义数据、状态和首选项。

一个组下可以存在多达14个级别的子组。

>[!NOTE]
>
>子组之上的层级中的所有组管理员都拥有管理该子组的管理权限。

有关创建和管理组的信息，请参阅[创建组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)和[管理组](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md)。 另请参阅[子组概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)。

## 指定组管理员

每个顶级组必须至少有一个组管理员。 Workfront管理员或组管理员可以为组的子组分配组管理员，但这是不必需的。 有关详细信息，请参阅[创建组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)。

如果您是Workfront管理员，我们建议您先执行以下操作，然后再将用户指定为组管理员：

* 记下系统中当前的Workfront管理员数量。
* 记下系统中拥有的组数。
* 确定是否可更改某些Workfront管理员的访问权限级别，并将他们指定为组管理员。

  有关组管理员功能的详细信息，请参阅本文中的[组管理员完成的任务](#tasks-done-by-group-administrators)。

* 确定您是否希望组管理员能够以其他用户身份登录，或者为您管理的组中的用户重置密码。 执行这些任务需要其他访问权限，如下文[组管理员所需访问权限](#access-needed-for-group-administrators)中所述。
* 为了更好地管理用户，请考虑将组或子组而不是用户分配给以下对象：

   * 布局模板
   * 计划
   * 周期性时间表

## 组管理员所需的访问权限 {#access-needed-for-group-administrators}

要求每个组管理员拥有

* 当前定价和打包模型中的计划许可证
* 新的定价和包装模式中的标准许可证

我们建议组管理员具有用户的“编辑”权限，以便他们能够执行以下任务：

* 以其他用户身份登录他们管理的组和子组。
* 重置他们管理的组中的其他用户的密码。

>[!IMPORTANT]
>
>组管理员必须比他们管理的组管理员拥有更高的访问权限；否则，他们将无法查看或修改较低的访问级别。
>有关授予此访问权限的说明，请参阅[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

对于需要为其组和子组中的用户分配时间表配置文件的组管理员，我们还建议对时间表和小时数的管理访问权限。 有关授予此访问权限的说明，请参阅[授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

## 组管理员完成的任务 {#tasks-done-by-group-administrators}

作为组管理员，您可以执行以下概述的任务来管理您监督的组。 其中一些功能与Workfront管理员获得的功能相同。

>[!NOTE]
>
>在新的定价和包装模型中，您必须拥有高级计划或更高版本才能执行以下操作：
>
> * 创建组事件通知
> * 配置组项目首选项
> * 配置组任务和问题首选项
> * 解锁子组首选项的配置
> * 组时间表和小时首选项
> * 解锁时间表和小时首选项

### 管理组成员 {#manage-group-members}

* 创建、编辑和删除您管理的组和子组中的子组。 有关说明，请参阅[创建子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)。
* 添加您对您的组和子组具有“编辑”权限的任何用户。 或者，通过编辑用户配置文件将用户添加到组和子组。

  如果您在访问级别中启用了用户管理员（组用户）权限，则还可以更新组成员配置文件中的字段。

  有关详细信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

  >[!NOTE]
  >
  >Workfront管理员可以覆盖组管理员对组成员资格所做的更改。

* 重置作为您管理的组成员的用户的密码。 有关详细信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。
* 以您管理组成员的用户身份登录。 有关详细信息，请参阅[以其他用户身份登录](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)。
* 查看您的组及其下方的子组可用的许可证数量。 有关详细信息，请参阅[管理系统中的可用许可证](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)。

### 管理组对象 {#manage-group-objects}

* 创建组级布局模板，并将其与您管理的组和子组相关联。 有关详细信息，请参阅[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。
* 创建组级时间表配置文件，将其与您管理的用户和组相关联，并手动生成时间表。 有关详细信息，请参阅[创建、编辑和分配时间表配置文件](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。
* 如果没有对审批流程的管理访问权限，请为您管理的组和子组创建和编辑审批流程。 有关详细信息，请参阅[为工作项创建批准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

  有关对审批流程的管理访问权限的信息，请参阅[授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* 创建时间表并将其与您管理的组相关联。 有关详细信息，请参阅[创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。
* 管理分配给您管理的组的团队，但不成为团队成员。 此外，根据“组”字段创建团队报告，以确定某个团队被分配到哪个组。 有关详细信息，请参阅[创建团队](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)。
* 恢复与您管理的组关联的项目，以及与项目关联的任何任务、问题或文档。 有关详细信息，请参阅[还原已删除的项](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

### 管理组首选项和工具 {#manage-group-preferences-and-tools}

* 当为系统中的组解锁项目首选项、任务或问题首选项、或时间表和小时首选项时，请编辑您管理组的该首选项。 这些首选项影响项目、任务和问题行为。 有关更多信息，请参阅以下内容：

   * [配置组的项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [配置组的任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* 创建和编辑您管理的组的组状态。 有关详细信息，请参阅[创建或编辑组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。
* 为您管理的组配置事件通知。 只有在Workfront管理员解锁通过系统为组配置事件通知的功能后，您才能执行此操作。 有关详细信息，请参阅[查看和配置组](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)的事件通知。
