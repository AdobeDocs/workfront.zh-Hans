---
title: 组概述
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Workfront管理员可以创建与您的部门结构一致的用户组。 分组与类似，但与团队和公司不同。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# 组概述

<!-- Audited: 01/2024 -->

Workfront管理员可以创建与您的部门结构一致的用户组。 分组与类似，但与团队和公司不同。

Workfront管理员向组授予对需要工作和沟通的Workfront区域的访问权限。 然后，每个组可以将其Workfront信息（如用户、模板、自定义表单和项目）与其他部门的那些信息分开。

每个组至少需要一个组管理员。 组管理员可以使用“组”页面在一个位置管理其组。 有关详细信息，请参阅[组管理员](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)。

您最多可以在一个组下创建14级子组。 有关详细信息，请参阅[子组概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)和[创建子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)。

## 使用组来组织用户

作为Workfront管理员或组管理员，您可以将用户与组和子组关联。 如果您将组设为公用，则具有“标准”（新）或“计划”（当前）许可证的用户可以将用户与其关联。 有关组管理员和公共组的详细信息，请参阅[创建组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)。

创建用户时，我们建议您将该用户添加到相应的主组以及该用户应处理的其他组。 一个用户只能有一个主组，但可以位于多个其他组中。

成为组的一部分可让用户访问与组和子组共享的对象。 例如，如果您与某个组共享某个项目，则该组及其子组中的用户有权访问该项目。

>[!TIP]
>
>如果贵组织中的部门经常共同管理项目和这些项目上的资源，则可能不必将部门分成许多较小的组。 一些高级别的小组可能效果最好。

一个组可以有无限数量的用户。

有关创建新用户的详细信息，请参阅[添加用户](../../../administration-and-setup/add-users/add-users.md)。

## 授予组访问对象的权限

与组共享对象时，该组的所有成员（包括任何子组的成员）都可以访问该对象。 有关在Workfront中共享的详细信息，请参阅[对象权限共享概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

## 将组与对象相关联

创建或编辑以下Workfront对象之一时，可将其与组相关联：

* **项目**：您可以将单个组与项目关联，以指示项目的所有权。

  这不会隐式授予组中的每个成员对项目的权限。 要拥有项目权限，用户必须拥有与其共享的项目。

  虽然用户可以是多个组的成员，但一个项目可以有一个与其关联的组。 如果该项目已与其或其组共享，则其他组中的用户仍可处理该项目。 与项目相关的组通常是负责完成项目的组，或者是交付项目的组。

  有关将项目与组关联的说明，请参阅[管理项目概述区域中的信息](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)。

* **Portfolio、项目群或公司**：在创建或编辑项目组合、项目群或公司时，您可以为其分配单个组，以指示该组拥有它或对其负责。 通过建立这种关联，管理员和用户可轻松识别其团队正在处理的项目组合、项目和公司。

  例如，组管理员可以使用列表或报告列出组织中的所有项目组合，并在“组”列中注明哪些项目组合已分配给其组。

  >[!NOTE]
  >
  >将组分配给具有组的项目组合、项目群或公司并不自动意味着该组中的信息有权访问其数据。 您需要先手动与组共享对数据的访问权限，然后才能查看。

  有关说明，请参阅[创建项目组合](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)、[创建程序](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)和[创建和编辑公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

* **审批流程**：您可以使审批流程可用于属于特定组的项目、任务和问题。 有关详细信息，请参阅[为工作项创建批准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。
* **里程碑路径**：您可以允许特定组中的用户将里程碑路径用于其项目。 有关详细信息，请参阅[创建里程碑路径](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)。
* **布局模板**：您可以授予组的管理员修改布局模板的权限。 有关说明，请参阅[授予对布局模板的管理访问权限](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)。

* **时间表配置文件**：您可以授予组的管理员修改时间表配置文件的权限。 有关详细信息，请参阅[创建、编辑和分配时间表配置文件](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

* **计划**：您可以授予组的管理员修改计划的权限。 有关详细信息，请参阅[创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。
* **团队**：您可以将组与团队关联，以便组及其子组的管理员可以查看组区域并与这些团队合作。 有关详细信息，请参阅[创建团队](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)或[编辑团队设置](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)。
* **模板**：您可以将组分配给项目模板。 这可以帮助您简化项目创建过程，并帮助您更轻松地识别和报告哪些组拥有哪些项目模板。 有关详细信息，请参阅[编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview)一文中的[概述](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)部分。

* **最近删除和还原的项目**：您可以查看和管理最近删除的组。 有关详细信息，请参阅[查看和管理组最近删除的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md)和[查看和管理组最近恢复的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md)。
