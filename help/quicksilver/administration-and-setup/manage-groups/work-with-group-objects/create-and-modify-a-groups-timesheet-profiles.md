---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 创建和管理组的周期性工时表
description: 当您查看在组区域管理的组时，可以查看和使用组或其子组的管理员具有管理访问权限的时间表配置文件。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 创建和管理组的周期性工时表

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

当您查看在组区域管理的组时，可以查看和使用组或其子组的管理员具有管理访问权限的时间表配置文件。

如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员也是如此（适用于任何组）。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是组的组管理员。</p>  <p>您还必须对时间表具有管理访问权限。 有关详细信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">授予用户对特定区域的管理访问权限</a>。</p>  <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 创建和编辑组级时间表配置文件

您可以创建和编辑要在您管理的组中使用的时间表配置文件。 有关说明，请参阅[创建、编辑和分配时间表配置文件](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

## 删除组级别周期性工时表

您可以删除您管理的组正在使用的时间表配置文件。 有关说明，请参阅[删除时间表配置文件](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md)。

## 手动生成组时间表

要使您对组时间表配置文件所做的更改能够反映在当前组时间表中，您必须首先删除现有时间表，然后手动生成新时间表。 有关说明，请参阅[手动生成时间表](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)中的[从时间表和小时区域](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually)手动生成时间表。

有关删除组时间表的信息，请参阅[删除Adobe Workfront中的时间表](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md)。

## 导出组级别周期性工时表

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。
1. 单击&#x200B;**组**。

   在显示的列表中，您可以看到您管理的组以及它们具有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击包含要导出的时间表配置文件的组的名称。
1. 单击&#x200B;**周期性工时表**。
1. 单击&#x200B;**导出**&#x200B;以导出组的时间表配置文件列表。
