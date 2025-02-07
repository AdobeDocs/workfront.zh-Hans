---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 锁定或解锁子组的项目、任务或问题偏好设置
description: 作为组管理员，您可以配置并锁定项目、任务或问题偏好设置(如果Workfront管理员在系统级别解锁了该偏好设置)。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# 锁定或解锁子组的项目、任务或问题偏好设置

作为组管理员，您可以配置并锁定项目、任务或问题偏好设置(如果Workfront管理员在系统级别解锁了该偏好设置)。

锁定已在级别配置的项目、任务或问题首选项可确保您的组及其子组中的每个人都使用该首选项的相同设置。 尽管您仍然可以重新配置您为组锁定的首选项，但组管理员无法为组重新配置它。

相反，解锁项目、任务或问题首选项可让组管理员更灵活地管理其组处理这些项目的方式。 解锁某个首选项后，组管理员可以为这些子组重新配置该首选项。

此功能与Workfront管理员锁定或解锁系统中每个人的首选项的功能相同。

有关Workfront管理员如何锁定或解锁系统中所有组的首选项的信息，请参阅[锁定或解锁系统中所有组的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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

## 锁定或解锁组项目、任务或问题偏好设置

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组**。
1. 单击要锁定或解锁项目偏好设置的组的名称。
1. 在左侧面板中，单击&#x200B;**项目首选项**&#x200B;或&#x200B;**任务和问题首选项**。

1. 在显示的页面上，针对在系统级别解锁的首选项或组上方的组执行以下任一操作：

   * 如果您希望组下的组管理员能够为其组配置首选项，请将其解锁![解锁切换](assets/unlock-toggle-button.png)。
   * 如果您希望您下方的所有组都使用您的配置进行首选项，请确保该配置已锁定![锁定切换](assets/lock-toggle-button.png)。

     >[!IMPORTANT]
     >
     >务必与管理员以及您所属组的用户进行通信，以确保以您配置锁定首选项的方式满足所有需求。 锁定后，其配置将由以下任何子组继承。 如果首选项已解锁任意时间段，则您的配置将替换较低子组中的组管理员可能已做出的配置。

1. 单击&#x200B;**保存**。
