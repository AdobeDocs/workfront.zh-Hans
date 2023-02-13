---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 创建和管理组的时间表配置文件
description: 在“组”区域中查看您管理的组时，可以查看和处理该组管理员或其某个子组具有管理访问权限的时间表配置文件。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 创建和管理组的时间表配置文件

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

在“组”区域中查看您管理的组时，可以查看和处理该组管理员或其某个子组具有管理访问权限的时间表配置文件。

如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是组的组管理员。</p>  <p>您还必须具有对工时单的管理访问权限。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">授予用户对特定区域的管理访问权限</a>.</p>  <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建和编辑组级别的工时单配置文件

您可以创建和编辑工时单配置文件，以在您管理的组中使用。 有关说明，请参阅 [创建、编辑和分配工时单配置文件](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## 删除组级别的工时单配置文件

您可以删除由您管理的组正在使用的时间表配置文件。 有关说明，请参阅 [删除工时单配置文件](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## 手动生成组工时单

要启用对工时单配置文件进行分组以反映在当前组工时单中的更改，必须先删除现有工时单，然后手动生成新工时单。 有关说明，请参阅 [从工时单和工时区手动生成工时单](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) in [手动生成工时单](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

有关删除组工时单的信息，请参阅 [删除Adobe Workfront中的工时单](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## 导出组级别的工时单配置文件

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).
1. 单击 **群组**.

   在显示的列表中，您可以看到您管理的群组，以及这些群组拥有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击要导出工时单配置文件的组名称。
1. 单击 **时间表配置文件**.
1. 单击 **导出** 导出组的时间表配置文件列表。
