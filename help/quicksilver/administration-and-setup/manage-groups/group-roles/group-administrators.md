---
title: 组管理员
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Adobe Workfront管理员在具有许多部门的大型组织中，可能不希望管理这些部门中组织的所有部门和组。 相反，他们可以为该组中的每个部门和子组创建一个组，每个部门和子组均由组管理员管理。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 03667fbdd1b0d68b9ad2d2db4a1ed85b8136062b
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 0%

---

# 组管理员

Adobe Workfront管理员在具有许多部门的大型组织中，可能不希望管理这些部门中组织的所有部门和组。 相反，他们可以为该组中的每个部门和子组创建一个组，每个部门和子组均由组管理员管理。

群组管理员可以管理群组的需求，如用户成员资格、布局模板、自定义数据、状态和首选项。

多达14个级别的子组可以存在于一个组中。

>[!NOTE]
>
>子组上方层次结构中的所有组管理员都具有管理该子组的管理权限。

有关创建和管理群组的信息，请参阅 [创建群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) 和 [管理群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). 另请参阅 [子组概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## 指定组管理员

每个顶级组必须至少有一个组管理员。 组的Workfront管理员或管理员可以将组管理员分配给组的子组，但这不是必需的。 有关更多信息，请参阅 [创建群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

如果您是Workfront管理员，我们建议您在将用户指定为组管理员之前执行以下操作：

* 记下系统中当前的Workfront管理员数量。
* 记下系统中的组数。
* 确定是否可以更改某些Workfront管理员的访问级别，并将他们指定为组管理员。

   有关组管理员功能的详细信息，请参阅 [组管理员完成的任务](#tasks-done-by-group-administrators).

* 确定您希望群组管理员能够以其他用户身份登录，还是重置您所管理群组中用户的密码。 执行这些任务需要其他访问权限，如 [组管理员需要的访问权限](#access-needed-for-group-administrators).
* 为了更好地管理用户，请考虑将组或子组而不是用户分配给以下对象：

   * 布局模板
   * 计划
   * 周期性时间表

## 组管理员需要的访问权限 {#access-needed-for-group-administrators}

每个组管理员都需要拥有计划许可证。

我们建议群组管理员对用户具有“编辑”访问权限，以便他们能够执行以下任务：

* 以其管理的组和子组中的其他用户身份登录。
* 在用户管理的组中重置其他用户的密码。

>[!IMPORTANT]
>
>组管理员必须具有比其管理的组管理员更高的访问权限；否则，他们将无法查看或修改较低的访问级别。
>有关授予此访问权限的说明，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

对于需要将工时单配置文件分配给组和子组中用户的组管理员，我们还建议对工时单和工时进行管理访问。 有关授予此访问权限的说明，请参阅 [授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## 组管理员完成的任务 {#tasks-done-by-group-administrators}

作为组管理员，您可以执行以下任务来管理您监督的组。 其中一些与Workfront管理员所具备的能力相同。

* [管理群组成员](#manage-group-members)
* [管理组对象](#manage-group-objects)
* [管理组首选项和工具](#manage-group-preferences-and-tools)

### 管理群组成员 {#manage-group-members}

* 在您管理的组和子组中创建、编辑和删除子组。 有关说明，请参阅 [创建子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* 添加您对其拥有群组和子组编辑访问权限的任何用户。 或者，通过编辑用户档案将用户添加到组和子组。

   如果您在访问级别中启用了用户管理员（群组用户）权限，则还可以更新群组成员配置文件中的字段。

   有关更多信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   >[!NOTE]
   >
   >Workfront管理员可以覆盖群组管理员对群组成员资格所做的更改。

* 为属于您管理的组的成员的用户重置密码。 有关更多信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* 以您所管理组成员的用户身份登录。 有关更多信息，请参阅 [以其他用户身份登录](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* 查看可用于您的组及其下子组的可用许可证数量。 有关更多信息，请参阅 [管理系统中的可用许可证](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### 管理组对象 {#manage-group-objects}

* 创建组级布局模板，并将它们与您管理的组和子组相关联。 有关更多信息，请参阅 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* 创建组级工时单配置文件，将其与您管理的用户和组关联，并手动生成工时单。 有关更多信息，请参阅 [创建、编辑和分配工时单配置文件](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* 如果没有对审批流程的管理访问权限，请为您管理的组和子组创建和编辑审批流程。 有关更多信息，请参阅 [为工作项创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   有关对审批流程的管理访问权限的信息，请参阅 [授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* 创建计划，并将它们与您管理的组关联。 有关更多信息，请参阅 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* 管理分配给您管理的组的团队，而不是该团队的成员。 此外，还应根据“组”(Group)字段创建团队报表，以确定特定团队被分配到的组。 有关更多信息，请参阅 [创建团队](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* 恢复与您管理的组关联的项目，以及与项目关联的任务、问题或文档。 有关更多信息，请参阅 [恢复已删除的项目](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### 管理组首选项和工具 {#manage-group-preferences-and-tools}

* 在系统中为组解锁项目首选项、任务或问题首选项、工时单和小时首选项时，请为您管理的组编辑该首选项。 这些首选项会影响项目、任务和问题行为。 有关更多信息，请参阅以下内容：

   * [为组配置项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [为组配置任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* 为您管理的组创建和编辑组状态。 有关更多信息，请参阅 [创建或编辑群组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* 为您管理的组配置事件通知。 只有在Workfront管理员通过系统外部解锁为组配置事件通知的功能后，才能执行此操作。 有关更多信息，请参阅 [查看和配置群组的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
