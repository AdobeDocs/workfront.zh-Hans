---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 删除群组
description: 您可以删除管理的群组。 如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f92eb1f5-fe98-4c7e-8ef7-8ed7134db8d4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 删除群组

您可以删除管理的群组。 如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。

有关删除子组的信息，请参阅 [管理群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md).

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

## 删除群组

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组** ![](assets/groups-icon.png).

1. 选择要删除的群组，然后单击删除图标 ![](assets/delete.png).

   >[!IMPORTANT]
   >
   >删除组或子组时，需要保留当前分配给该组或子组的用户、工作项和任何子组。 为帮助您确保保留这些对象，系统会提示您在以下步骤中将组的对象重新分配给其他组。

1. 在 **删除组** 框中，开始键入内容，然后选择要移动所删除群组的成员、工作项和子组的群组名称。

   您可以通过将鼠标悬停在正确的组上并单击信息图标来确保选择正确的组 ![](assets/info-icon.png) 显示在其旁边的。 此时会显示工具提示，其中列出了有关群组的信息，例如群组上的群组层次结构及其管理员。

1. 单击 **删除它们**.
