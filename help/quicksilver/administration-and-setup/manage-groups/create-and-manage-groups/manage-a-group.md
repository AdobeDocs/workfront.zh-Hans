---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理，组，编辑，
navigation-topic: create-and-manage-groups
title: 管理群组
description: 作为组管理员，您可以从“设置”的“组”区域管理您管理的组。 如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '1321'
ht-degree: 0%

---

# 管理群组

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

作为组管理员，您可以从“设置”的“组”区域管理您管理的组。 如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。

>[!NOTE]
>
>将您分配为群组的管理员后，您将继承该群组下所有子群组的群组管理员角色。 只能管理子组的用户是其上方顶级组的组管理员，以及分配给该子组的任何组管理员。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 管理群组成员关系

您可以向您管理的群组中添加用户和其他群组，并将其删除。 您还可以将群组成员分配为群组的管理员，并管理群组成员的用户配置文件信息。

有关说明，请参阅 [查看和管理群组成员关系](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## 管理群组的详细信息

您可以查看和编辑您管理的组或子组的“组详细信息”页。 本页包括对群组的描述、业务负责人和群组管理员的姓名，以及允许您将群组及其所有子群组设为公用或私有的选项。 此外，如果您的访问级别允许您管理自定义表单，则可以将自定义表单附加到群组。

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

有关说明，请参阅 [查看和管理群组的详细信息](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## 编辑、复制或删除群组

无需离开您正在查看的组的主页，即可快速编辑、复制或删除

<!--
DRAFTED IN FLARE:
or deactivate

-->

组。

<!--
DRAFTED IN FLARE:
Make this change when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **群组**.

   在显示的列表中，您可以看到您管理的群组，以及这些群组拥有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 选择群组，然后单击“编辑” ![](assets/edit-icon.png)，复制 ![](assets/copy-icon.png)，或删除 ![](assets/delete.png) 图标。

   如果您需要有关使用显示的框的信息，请参阅以下内容之一：

   * **编辑**: [查看和管理群组的详细信息](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **复制**: [通过复制现有组或子组创建顶级组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) 在文章中 [创建群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **删除**: [删除群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## 为组配置项目、任务和问题首选项

如果您是组管理员，并且您的组需要与在系统级别设置的项目、任务和问题首选项设置不同的设置，则可以请求Workfront管理员解锁整个组织中所有组的首选项。 解锁后，您（以及所有其他组的组管理员）可以为您管理的组配置它。

有关说明，请参阅 [为组配置项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 和  [为组配置任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## 列出、添加和配置子组

您可以在您管理的群组下创建、查看、编辑、复制、重命名、导出和删除子群组。

## 为组配置事件通知

如果Workfront管理员解锁了为组织中的组配置事件通知的功能，则可以为您管理的组配置这些通知。 有关说明，请参阅 [查看和配置群组的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## 为群组创建和自定义状态

作为群组管理员，您可以为您管理的顶级群组创建自定义状态。 这可让您的群组拥有自主权，并有助于消除对公司范围内数十种自定义状态的需求。 (对于任何组，Workfront管理员也可以执行此操作。)

如果Workfront管理员已将顶级组配置为允许自定义，则还可以为其自定义系统状态。

有关说明，请参阅 [创建或编辑群组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## 使用组的项目

在“设置”的“组”区域中，当您查看所管理组的主页时，可以对项目执行以下操作：

* 列出并处理（编辑、复制、删除和导出）与组及其子组关联且已与您共享的项目
* 为组创建新项目

有关说明，请参阅 [创建和修改组的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## 查看和管理群组的批准流程

在“组”(Groups)区域中查看您管理的组时，您可以查看和处理组管理员或其某个子组具有管理访问权限的审批流程。

有关说明，请参阅 [组级别的审批流程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## 查看和管理组的布局模板

在“组”区域中查看由您管理的组时，您可以查看和使用布局模板，该组或其某个子组的管理员对其具有管理访问权限。

有关说明，请参阅 [创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 查看和管理组成员的计划

为组创建计划的组管理员必须指定管理员将管理计划的组。 通常，这是为其创建计划的组，但如果组管理员管理多个组并指定其他组之一，则它可能是另一个组。

在查看您管理的组的主页时，如果该组被指定为管理员可以编辑计划的组，则可以从该组的页面查看和管理计划。

有关说明，请参阅 [创建和修改组的计划](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## 查看和管理组成员的时间表配置文件

在查看您管理的组的主页时，可以管理您和其他管理的组（或组的一个子组）拥有编辑权限的时间表配置文件。 有关说明，请参阅 [创建和管理组的时间表配置文件](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## 查看和管理组的子组成员

在查看您管理的组的主页时，可以查看和管理该组的子组中的所有用户。 有关说明，请参阅 [查看和管理子组成员](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## 查看和管理群组的团队

在“组”区域中查看由您管理的组时，可以查看与该组或其任何子组关联的团队并与之合作。

有关说明，请参阅 [创建和修改组的团队](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## 查看和管理群组的公司

在“组”区域中查看由您管理的组时，可以查看与该组或其任何子组关联的公司并与之合作。 有关说明，请参阅 [创建和修改群组的公司](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## 查看和管理组的项目组合和项目

当您在“组”区域中查看由您管理的组时，如果满足以下条件，则可以查看和使用项目组合和项目：

* 它们与您正在查看的组或其任何子组相关联
* 您之所以有权查看这些组件，是因为您创建了这些组件，或者已与您共享这些组件

有关说明，请参阅 [创建和修改组的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) 和 [创建、修改和查看组的程序](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## 停用或重新激活群组

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

您可以将组保持为默认活动状态或将其停用。

当组当前未使用时，停用该组会很有用，因为当用户在搜索要与另一个对象关联的组时，他们不再在“提前键入”字段中看到该组。

有关将组设为非活动或活动的说明，请参阅 [停用或重新激活群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
