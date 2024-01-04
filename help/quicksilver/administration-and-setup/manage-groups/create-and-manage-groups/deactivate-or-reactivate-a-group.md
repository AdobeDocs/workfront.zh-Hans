---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 停用或重新激活组
description: 您可以停用您管理的不再使用的组。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 停用或重新激活组

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

您可以停用您管理的不再使用的组。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系Workfront管理员。

## 停用或重新激活组

>[!IMPORTANT]
>
>取消激活组时，也将取消激活该组下的任何子组。
>
>如果您需要重新激活其中一个，可以在执行以下操作之一之后重新激活：
>
>* 将其从父组中移除。 有关更多信息，请参阅部分 [从父组中移除子组，并将其设为顶级组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) 在文章中 [管理子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* 将其移动到活动组下。 有关更多信息，请参阅部分 [创建、移动、查看、编辑、复制、重命名、导出或删除子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) 在文章中 [管理子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，选择 **组**.

   在显示的列表中，您可以看到您管理的组以及它们具有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击组的名称以打开其页面。

1. 单击更多菜单 ![](assets/more-icon.png) 单击组名旁边的，然后单击 **取消激活** 或 **重新激活**.

   >[!NOTE]
   >
   >如果组是已停用组的子组，则处于活动状态选项（预览中的重新激活选项）不可用。 在重新激活它之前，必须将其从父组中移除，或将其移动到活动组下，如上面的重要说明中所述。

1. （视情况而定）如果要停用组，请单击 **取消激活** 在 **停用组** 框。

## 有关不活动组的注意事项

对于通过禁用一节中说明的“处于活动状态”选项而取消激活的组，请考虑以下事项 [停用或重新激活组](#View) 本文章中。

* 停用组也会停用其下的所有子组。 这包括在停用子组后添加的子组。

  有关在此情况下重新激活子组的信息，请参阅 [关于重新激活非活动父组下的子组](#about-reactivating-a-subgroup-below-an-inactive-parent-group) 本文章中。

* 当您转到“设置”中的“组”区域时，您只能在列表中看到活动组，因为“活动”是默认筛选器 ![](assets/filter-nwepng.png) 为了它。 如果要查看您管理的所有组（包括非活动组），可以使用“全部”筛选器。 或者使用非活动筛选器仅列出非活动筛选器。

  有关列表中过滤器的更多信息，请参阅 [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* 停用组不会更改以下内容：

   * 组与对象的关联。 关联的对象将继续像以前一样工作，不会发生任何更改。

     例如，如果项目与您取消激活的组相关联，则项目将继续使用组的首选项和状态，而不做任何更改。

   * 您可以在“设置”中从组的页面内创建新对象，如批准、团队或公司。 默认情况下，新对象与非活动组相关联。
   * 作为管理员，您能够在过滤器和报表中查找组。

     您还可以在组预输入字段中找到该组，您可能希望在该字段的“设置”区域中管理组的设置。 这包括“首选项”、“事件通知”和“系统许可证”区域。

     例如，如果您转到设置>项目偏好设置>项目，并清除其中选项上方的前进键入字段，则仍可找到不活动的组并配置其项目偏好设置。

## 关于重新激活非活动父组下的子组 {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

停用组也会停用其下的所有子组。 如果需要重新激活非活动组下的某个子组，可以执行以下两项操作之一：

* 将子组移动到活动组下方。 然后为移动的组启用处于活动状态选项，如一节中所述 [停用或重新激活组](#View) 本文章中。

  有关移动组的说明，请参见 [移动组](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* 从父组中移除子组（使子组成为顶级组）。 然后为移动的组启用处于活动状态选项，如一节中所述 [停用或重新激活组](#View) 本文章中。

  有关从父组中删除子组的说明，请参阅部分 [从父组中移除子组，并将其设为顶级组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) 在文章中 [管理子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
