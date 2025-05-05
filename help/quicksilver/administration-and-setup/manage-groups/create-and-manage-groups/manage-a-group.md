---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理，组，编辑，
navigation-topic: create-and-manage-groups
title: 管理组
description: 作为组管理员，您可以从“设置”的“组”区域管理组。 如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员也是如此（适用于任何组）。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1315'
ht-degree: 0%

---

# 管理组

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

作为组管理员，您可以从“设置”的“组”区域管理组。 如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员也是如此（适用于任何组）。

>[!NOTE]
>
>当您被指定为组的管理员时，您将继承其下任何子组的组管理员角色。 唯一可以管理子组的用户是上面最上层组的组管理员以及分配给该子组的任何组管理员。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>您必须是组的组管理员或系统管理员。</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 管理组的成员资格

您可以在管理的组中添加和删除用户和其他组。 您还可以将组成员指定为组的管理员，并管理组成员的用户配置文件信息。

有关说明，请参阅[查看和管理组的成员资格](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md)。

## 管理组的详细信息

您可以查看和编辑您管理的组或子组的“组详细信息”页面。 此页面包括组的说明、业务负责人和组管理员的姓名，以及允许您将组及其所有子组设为公共或私有组的选项。 此外，如果您的访问级别允许您管理自定义表单，则可以将自定义表单附加到组。

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

有关说明，请参阅[查看和管理组的详细信息](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)。

## 编辑、复制或删除组

无需离开正在查看的组的主页，即可快速编辑、复制或删除该组。

{{step-1-to-setup}}

1. 单击&#x200B;**组**。

   在显示的列表中，您可以看到您管理的组以及它们具有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 选择组，然后单击“编辑”![“编辑”图标](assets/edit-icon.png)、“复制”![“复制”图标](assets/copy-icon.png)或“删除”![“删除”图标](assets/delete.png)图标。

   如果您需要有关使用显示的框的信息，请参阅以下内容之一：

   * **编辑**：[查看和管理组的详细信息](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **复制**： [&#128279;](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group)通过复制项目[创建组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的现有组或子组创建顶级组

   * **删除**： [删除组](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## 配置组的项目、任务和问题偏好设置

如果您是组管理员，并且您的组需要与系统级别上设置的项目、任务和问题首选项设置不同的设置，则可以请求Workfront管理员解锁整个组织中所有组的首选项。 解锁后，您（和所有其他组的组管理员）可以为您管理的组配置它。

有关说明，请参阅[配置组的项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)和[配置组的任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

## 列出、添加和配置子组

您可以在管理的组下创建、查看、编辑、复制、重命名、导出和删除子组。

## 为组配置事件通知

如果Workfront管理员解锁为组织中的组配置事件通知的功能，则可以为管理的组配置这些通知。 有关说明，请参阅[查看和配置组](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)的事件通知。

## 创建和自定义组的状态

作为组管理员，您可以为所管理的顶级组创建自定义状态。 这赋予了您的组自主权，并有助于消除对数十种公司范围的自定义状态的需要。 (Workfront管理员还可以为任何组执行此操作。)

您还可以自定义顶级组的系统状态(如果Workfront管理员将系统状态配置为允许自定义)。

有关说明，请参阅[创建或编辑组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。

## 使用组的项目

在“设置”的“组”区域中，当您查看所管理组的主页时，可以对项目执行以下操作：

* 列出并处理（编辑、复制、删除和导出）与组及其子组关联并已与您共享的项目
* 为组创建新项目

有关说明，请参阅[创建和修改组的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)。

## 查看和管理组的审批流程

当您查看在组区域管理的组时，您可以查看和处理组的管理员或其子组之一具有管理访问权限的审批流程。

有关说明，请参阅[组级审批流程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md)。

## 查看和管理组的布局模板

在组区域查看您管理的组时，您可以查看和使用布局模板，组或其子组的管理员对此布局模板具有管理访问权限。

有关说明，请参阅[创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

## 查看和管理组成员的时间表

组管理员为组创建调度时，必须指定由管理员管理调度的组。 通常，这是为其创建计划的组，但如果组管理员管理多个组并指定其他组之一，则它可能是不同的组。

在查看您管理的组的主页时，如果该组被指定为管理员可以编辑调度的组，则可以从组页面查看和管理调度。

有关说明，请参阅[创建和修改组的计划](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md)。

## 查看和管理组成员的周期性工时表

在查看您管理的组的主页时，您可以管理您和组的其他管理员（或其一个子组）有权编辑的时间表配置文件。 有关说明，请参阅[创建和管理组的时间表配置文件](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)。

## 查看和管理组的子组成员

在查看您管理的组的主页时，您可以查看和管理该组子组中的所有用户。 有关说明，请参阅[查看和管理子组成员](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md)。

## 查看和管理组的团队

在组区域查看您管理的组时，您可以查看和使用与该组或其任何子组关联的团队。

有关说明，请参阅[创建和修改组的团队](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md)。

## 查看和管理组的公司

在组区域查看您管理的组时，您可以查看和使用与该组或其任何子组关联的公司。 有关说明，请参阅[创建和修改组的公司](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md)。

## 查看和管理组的项目组合和程序

当您在组区域查看您管理的组时，如果符合以下两个条件，则可以查看和使用项目组合和程序：

* 它们与您正在查看的组或其任何子组相关联
* 您有权查看这些区段，因为您已创建它们或与您共享它们

有关说明，请参阅[创建和修改组的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md)和[创建、修改和查看组的程序](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md)。

## 停用或重新激活组

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

您可以将组保持在其默认的活动状态或取消激活它。

当某个组当前未使用时，停用该组可能很有用，因为当用户搜索要与另一对象关联的组时，不再在预输入字段中看到该组。

有关使组处于非活动状态或活动状态的说明，请参阅[停用或重新激活组](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)。
