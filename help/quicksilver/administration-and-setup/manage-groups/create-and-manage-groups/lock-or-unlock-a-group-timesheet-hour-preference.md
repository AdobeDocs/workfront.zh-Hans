---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 锁定或解锁组时间表和小时首选项
description: 如果您是组管理员，则可以在Workfront管理员在系统级别解锁您的组的时间表和小时首选项后，对其进行配置，然后锁定该首选项。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 0%

---

# 锁定或解锁组时间表和小时首选项

如果您是组管理员，则可以在Workfront管理员在系统级别解锁您的组的时间表和小时首选项后，对其进行配置，然后锁定该首选项。

锁定Adobe Workfront首选项可确保您的组及其子组中的每个人都使用该首选项的相同设置。 虽然您仍然可以重新配置已锁定的首选项，但组管理员无法对较低级别的子组执行此操作。

相反，在组级别解锁首选项可让子组管理员更灵活地管理其组处理这些项目的方式。 解锁某个首选项后，组管理员可以为这些子组重新配置该首选项。

此功能与Workfront管理员锁定或解锁系统中每个人的首选项的功能相同。

有关Workfront管理员如何锁定或解锁系统中所有组的时间表和小时首选项的信息，请参阅[配置时间表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

有关为组配置时间表和小时首选项的信息，请参阅[为组配置时间表和小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md)。

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* 为组配置解锁的首选项不会影响组下任何子组的该首选项。
>
>  但是，创建新子组时，它会继承其上方的首选项设置以及组的锁定或解锁状态。
>
>* 如果在具有锁定首选项的组下移动组，则被移动的组会继承该首选项，并且被移动的组锁定。
>* 如果在具有解锁首选项的组下移动组，则已移动的组不受该首选项的影响。
>
>  如果在移动时锁定了已移动组中的首选项，则该首选项会保持锁定状态，但组管理员现在可以将其解锁，因为已为父组解锁该首选项。

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

## 锁定或解锁组时间表和小时首选项

>[!TIP]
>
>如果您是Workfront管理员，可以绕过步骤1-4，方法是转到设置>时间表和小时数>首选项，然后在页面顶部的框中搜索组的名称。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组**。
1. 单击要锁定或解锁时间表和小时首选项的组的名称。
1. 在左侧面板中，单击&#x200B;**时间表和小时首选项**。

1. 在显示的页面上，执行以下任一操作：

   * 如果您希望组下的组管理员能够为其组配置首选项，请将其解锁![](assets/unlock-toggle-button.png)。
   * 如果您希望您下方的所有组都使用您的配置进行首选项，请确保该配置已锁定![](assets/lock-toggle-button.png)（这是默认设置）。

     >[!IMPORTANT]
     >
     >务必与管理员以及您所属组的用户进行通信，以确保以您配置锁定首选项的方式满足所有需求。 锁定后，其配置将由以下任何子组继承。 如果首选项已解锁任意时间段，则您的配置将替换较低子组中的组管理员可能已做出的配置。

1. 单击&#x200B;**保存**。
