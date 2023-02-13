---
title: 查看群组中分配和使用的许可证数量
description: 作为Adobe Workfront管理员，您可以查看组及其子组中当前使用的各个许可证类型的计数。 当您需要评估是否要重新分发许可证时，此功能非常有用。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 查看群组中分配和使用的许可证数量

作为Adobe Workfront管理员，您可以查看组及其子组中当前使用的各个许可证类型的计数。 当您需要评估是否要重新分发许可证时，此功能非常有用。

如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。

>[!IMPORTANT]
>
>仅当用户的主群组是用户的主群组时，用户的许可证才会计入特定群组。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront计划</a>*</td> 
   <td> <p>团队或更高级别</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfront许可证</a>*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 查看组中使用的许可证数

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组** ![](assets/groups-icon.png).

1. 单击群组的名称。
1. 在显示的页面的右上角附近的标题区域中，查看 **使用中的许可证** 查看 **计划** 和 **工作** 当前正在使用的许可证。

   如果您正在查看顶级群组，而Workfront管理员为群组定义了每个许可证类型的最大数量，则也会显示这些数量。 例如，在以下组中，最多10个用户可以拥有计划许可证，15个用户可以拥有工作许可证：

   ![](assets/licenses-used-allocated.png)

   有关Workfront管理员如何为群组定义最大已分配许可证数的信息，请参阅部分 [设置家庭组的最大许可证计数](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) 在文章中 [管理系统中的可用许可证](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >如果您要查看的组是子组，则只能查看正在使用的许可证数量，而不能查看为该组分配的最大许可证数量。 这是因为Workfront管理员没有为子组定义最大许可证计数。
   >
   >![](assets/subgroup-used-licenses-only.png)

1. 对于组中当前使用的每种许可证类型（包括“审阅”和“请求”）的单独计数，请单击正下方的文本区域 **使用中的许可证：**

   ![](assets/click-text-to-see-more.png)

   显示的框为所有四种Workfront许可证类型提供了相同的信息：计划、工作、审核和请求。 在框的底部，您可以看到此组成员或其某个子组成员使用的许可证总数：

   ![](assets/more-license-info.png)

   对于“审阅”和“请求”许可证，“最大”列始终显示“无限制”。
