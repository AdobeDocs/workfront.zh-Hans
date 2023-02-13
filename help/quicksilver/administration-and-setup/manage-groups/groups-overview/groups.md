---
title: 组
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Workfront管理员可以创建与您的部门结构一致的用户组。 组与团队和公司相似，但不同。 Workfront管理员授予群组访问其需要工作和通信的Workfront区域的权限。 然后，每个组都可以将其Workfront信息（如用户、模板、自定义表单和项目）与其他部门的信息分开。 每个组至少需要一个组管理员。 群组管理员可以使用群组页面在一个位置管理其群组。 您最多可以在一个组下创建14个级别的子组。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '999'
ht-degree: 0%

---

# 群组概述

Workfront管理员可以创建与您的部门结构一致的用户组。 组与团队和公司相似，但不同。

Workfront管理员授予群组访问其需要工作和通信的Workfront区域的权限。 然后，每个组都可以将其Workfront信息（如用户、模板、自定义表单和项目）与其他部门的信息分开。

每个组至少需要一个组管理员。 群组管理员可以使用群组页面在一个位置管理其群组。 有关更多信息，请参阅 [组管理员](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

您最多可以在一个组下创建14个级别的子组。 有关更多信息，请参阅 [子组概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) 和 [创建子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## 使用组组织用户

作为Workfront管理员或组管理员，您可以将用户与组和子组关联。 如果将群组设为公用群组，则具有计划员许可证的用户可以将用户与其关联。 有关群组管理员和公共群组的更多信息，请参阅 [创建群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

在创建用户时，我们建议您将该用户添加到相应的主页组以及用户应该在其中工作的其他组。 用户只能拥有一个主页组，但可以位于多个其他组中。

作为组的一部分，用户可以访问与组和子组共享的对象。 例如，如果您与某个组共享某个项目，则该组和该组的子组中的用户有权访问该项目。

>[!TIP]
>
>如果贵组织中的部门经常合作来管理项目和这些项目的资源，则可能不必将部门划分成许多较小的组。 一些高级别的小组可能效果最好。

群组可以拥有无限数量的用户。

有关创建新用户的更多信息，请参阅 [添加用户](../../../administration-and-setup/add-users/add-users.md).

## 授予对对象的组访问权限

与组共享对象时，该组的所有成员（包括任何子组的成员）都有权访问该对象。 有关在Workfront中共享的更多信息，请参阅 [对象共享权限概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## 将组与对象关联

创建或编辑以下某个Workfront对象时，可将其与组关联：

* **项目**:您可以将单个组与项目关联，以指示项目的所有权。

   这不会隐式授予组中每个成员对项目的权限。 要拥有项目权限，用户必须通过与他们共享项目来接收权限。

   虽然用户可以是多个组的成员，但一个项目可以有一个与其关联的组。 如果已与其或其组共享了项目，则来自其他组的用户仍可以处理同一项目。 与项目关联的组通常是负责完成项目的组，或交付项目的组。

   有关将项目与组关联的说明，请参阅 [在项目概述区域中管理信息](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio、项目或公司**:在创建或编辑组合、项目或公司时，您可以为其分配一个组，以指示该组拥有或负责该组。 通过建立这种关联，管理员和用户可以轻松识别其团队正在处理的项目组合、项目和公司。

   例如，群组管理员可以使用“群组”列中的列表或报表以及注释来列出组织中的所有项目组合，这些项目组合已分配给其群组。

   >[!NOTE]
   >
   >将组分配给具有组的组合、项目或公司，并不会自动表示该组中有权访问其数据的信息。 您需要先与组手动共享对数据的访问权限，然后组才能看到该数据。

   有关说明，请参阅 [创建项目组合](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [创建项目](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)和 [创建和编辑公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **审批流程**:您可以为属于特定组的项目、任务和问题提供批准流程。 有关更多信息，请参阅 [为工作项创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **里程碑路径**:您可以允许某些组中的用户在其项目中使用里程碑路径。 有关更多信息，请参阅 [创建里程碑路径](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **布局模板**:您可以为群组的管理员授予修改布局模板的权限。 有关说明，请参阅 [授予布局模板的管理访问权限](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **时间表配置文件**:您可以为组的管理员授予修改时间表配置文件的权限。 有关更多信息，请参阅 [创建、编辑和分配工时单配置文件](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **计划**:您可以为群组的管理员授予修改计划的权限。 有关更多信息，请参阅 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **团队**:您可以将组与团队关联，以便组及其子组的管理员可以从“组”区域查看和使用这些团队。 有关更多信息，请参阅 [创建团队](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) 或 [编辑团队设置](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **模板**:您可以将组分配给项目模板。 这可以帮助您简化项目创建过程，并帮助您更轻松地确定和报告哪些组拥有哪些项目模板。 有关更多信息，请参阅 [概述](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) 在文章中 [编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **最近删除和还原的项目**:您可以查看和管理最近删除的项目的群组。 有关更多信息，请参阅 [查看并管理群组最近删除的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) 和 [查看和管理组最近还原的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
