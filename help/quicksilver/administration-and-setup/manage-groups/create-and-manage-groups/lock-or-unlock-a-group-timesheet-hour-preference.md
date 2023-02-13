---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 锁定或解锁组时间表和小时首选项
description: 如果您是组管理员，则可以在Workfront管理员在系统级别解锁组后，配置并锁定组的时间表和小时首选项。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# 锁定或解锁组时间表和小时首选项

如果您是组管理员，则可以在Workfront管理员在系统级别解锁组后，配置并锁定组的时间表和小时首选项。

锁定Adobe Workfront首选项可确保组及其子组中的每个人都使用该首选项的相同设置。 虽然您仍可以重新配置您锁定的首选项，但组管理员无法为较低的子组重新配置。

相反，通过在组级别解锁首选项，子组管理员可以更灵活地管理其组处理这些项目的方式。 解锁首选项后，组管理员可以为这些子组重新配置该首选项。

这与Workfront管理员必须锁定或解锁系统中每个人的首选项的功能平行。

有关Workfront管理员如何锁定或解锁系统中所有组的时间表和小时首选项的信息，请参阅 [配置工时单和工时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

有关为组配置时间表和小时首选项的信息，请参阅 [为组配置工时单和小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* 为组配置已解锁首选项不会影响该组下任何子组的该首选项。
>
>  但是，当创建新子组时，它会继承该组的首选项设置以及该组上方的锁定或解锁状态。
>
>* 如果在具有锁定首选项的组下移动组，则被移动的组会继承该首选项，并且会为被移动的组锁定该首选项。
>* 如果在具有已解锁首选项的组下移动组，则移动的组不受该首选项的影响。
>
>  如果移动时已锁定移动组中的首选项，则该首选项将保持锁定状态，但组管理员现在可以解锁，因为已为父组解锁该首选项。

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

## 锁定或解锁组时间表和小时首选项

>[!TIP]
>
>如果您是Workfront管理员，则可以绕过步骤1-4，方法是转到“设置”>“时间表和小时数”>“首选项”，然后在页面顶部的框中搜索组名称。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组**.
1. 单击要锁定或解锁工时单和工时首选项的组名称。
1. 在左侧面板中，单击 **工时单和工时首选项**.

1. 在显示的页面上，执行以下任一操作：

   * 如果您希望群组下的群组管理员能够为其群组配置首选项，请解锁该首选项 ![](assets/unlock-toggle-button.png).
   * 如果您希望下面的所有组都使用您的配置作为首选项，请确保已锁定该配置 ![](assets/lock-toggle-button.png) （这是默认设置）。

      >[!IMPORTANT]
      >
      >请务必与您下面组中的管理员和用户通信，以确保通过配置锁定首选项的方式满足所有需求。 锁定后，其配置将由下面的任何子组继承。 如果该首选项已在任意时间段内解锁，则您的配置将替换下级子组中的组管理员可能已解锁的组。

1. 单击&#x200B;**保存**。
