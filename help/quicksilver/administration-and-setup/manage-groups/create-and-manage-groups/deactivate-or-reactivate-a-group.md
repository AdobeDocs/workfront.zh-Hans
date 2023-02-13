---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 停用或重新激活群组
description: 您可以停用由您管理的不再使用的群组。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# 停用或重新激活群组

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

您可以停用由您管理的不再使用的群组。

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

## 停用或重新激活群组

>[!IMPORTANT]
>
>停用群组时，下面的所有子组也会停用。
>
>如果需要重新激活其中一个插件，可以在执行以下操作之一后重新激活它们：
>
>* 将其从其父组中删除。 有关更多信息，请参阅 [从其父组中删除子组，并将其设为顶级组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) 在文章中 [管理子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* 将其移到活动组下。 有关更多信息，请参阅 [创建、移动、查看、编辑、复制、重命名、导出或删除子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) 在文章中 [管理子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>


1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，选择 **群组**.

   在显示的列表中，您可以看到您管理的群组，以及这些群组拥有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击群组的名称以打开其页面。

1. 单击“更多”菜单 ![](assets/more-icon.png) 在群组名称旁边，单击 **停用** 或 **重新激活**.

   >[!NOTE]
   >
   >如果组是已停用组的子组，则“处于活动状态”选项（“预览”中的“重新激活”选项）将不可用。 在重新激活它之前，必须将其从其父组中删除，或将其移到处于活动状态的组下，如上面的重要说明中所述。

1. （视情况而定）如果要取消激活群组，请单击 **停用** 在 **停用组** 框中。

## 非活动组的注意事项

请考虑以下有关您通过禁用部分中介绍的“是活动的”选项来停用的组的信息 [停用或重新激活群组](#View) 在本文中。

* 取消激活群组也会停用该群组下的所有子群组。 这包括您在取消激活后添加的子组。

   有关在这种情况下重新激活子组的信息，请参阅 [关于重新激活不活动父组下的子组](#about-reactivating-a-subgroup-below-an-inactive-parent-group) 在本文中。

* 当您转到“设置”中的“组”区域时，您只能在列表中看到活动组，因为“活动”是默认过滤器 ![](assets/filter-nwepng.png) 为了它。 如果要查看您管理的所有组（包括不活动的组），则可以使用“全部”筛选器。 或者，使用不活动过滤器仅列出不活动的过滤器。

   有关列表中过滤器的更多信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* 取消激活群组不会更改以下内容：

   * 组与对象的关联。 关联的对象将继续像以前一样运行，而不进行任何更改。

      例如，如果某个项目与您停用的组关联，则该项目会继续使用该组的首选项和状态，而不进行任何更改。

   * 您能够从设置的组页面中创建新对象，如批准、团队或公司。 默认情况下，新对象与不活动组关联。
   * 您作为管理员，能够在过滤器和报表中查找群组。

      您还可以在“组提前类型”字段中找到该组，您可能希望在“设置”区域中管理该组的设置。 这包括“首选项”、“事件通知”和“系统许可证”区域。

      例如，如果转到设置>项目首选项>项目，并清除其上方选项上方的提前键入字段，则仍然可以找到不活动的组并配置其项目首选项。

## 关于重新激活不活动父组下的子组 {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

取消激活群组也会停用该群组下的所有子群组。 如果需要重新激活不活动组下的其中一个子组，可以执行以下两项操作之一：

* 在活动组下移动子组。 然后，为已移动的组启用“处于活动状态”选项，如 [停用或重新激活群组](#View) 在本文中。

   有关移动组的说明，请参阅 [移动组](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* 从其父组中删除该子组（这会使该子组成为顶级组）。 然后，为已移动的组启用“处于活动状态”选项，如 [停用或重新激活群组](#View) 在本文中。

   有关从其父组中删除子组的说明，请参阅 [从其父组中删除子组，并将其设为顶级组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) 在文章中 [管理子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
