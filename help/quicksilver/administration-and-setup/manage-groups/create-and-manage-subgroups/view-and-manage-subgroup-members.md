---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 查看和管理子组成员
description: 查看由您管理的群组时，可以查看和管理该群组的子群组中的所有用户。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# 查看和管理子组成员

查看由您管理的群组时，可以查看和管理该群组的子群组中的所有用户。

如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。

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
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>在选中用户管理员（所有用户）选项的情况下编辑对用户的访问权限</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请联系您的Workfront管理员。

## 查看和管理组下子组的成员

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **群组**.

   在显示的列表中，您可以看到您管理的群组，以及这些群组拥有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击要查看或管理其子组成员的组名称。
1. 在左侧面板中，单击 **分组成员**.

   仅当组包含子组时，此左侧面板项才可用。

1. 执行以下任一操作：

   * 在列表中选择成员，然后单击“编辑” ![](assets/edit-icon.png) 以修改该人员的用户配置文件。

      有关更多信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) 或 [批量编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).

   * 选择列表中任意数量的成员，然后单击“更新” ![](assets/comment-icon.png) 向其用户配置文件添加评论。

      用户或用户会收到应用程序内通知以及包含您评论的电子邮件通知。 该评论显示在用户配置文件的更新区域中。

   * 在列表中选择任意数量的成员，然后单击“停用” ![](assets/deactivate-user.png) 或激活 ![](assets/activate-user.png).

      有关更多信息，请参阅 [停用或重新激活用户](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * 导出 ![](assets/export.png) 成员列表。
