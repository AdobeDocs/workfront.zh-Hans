---
user-type: administrator
product-area: system-administration;user-management
keywords: 视图，组，事件，通知，配置，启用，禁用
navigation-topic: create-and-manage-groups
title: 查看和配置群组的事件通知
description: 作为群组管理员，您可以查看为您管理的群组激活的事件通知。 此外，如果Adobe Workfront管理员解锁事件通知，您可以为您管理的顶级组配置该通知。 事件通知的配置包括激活或取消激活它。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: 306d6493ff0413d5814f4aed8ab44fb897f3568d
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# 查看和配置群组的事件通知

作为群组管理员，您可以查看为您管理的群组激活的事件通知。

此外，如果Adobe Workfront管理员解锁事件通知，您可以为您管理的顶级组配置该通知。 事件通知的配置包括激活或取消激活它。

Workfront管理员还可以为任何组执行此操作。

为组配置事件通知会影响该组或其某个子组为其“主组”的用户。 在用户配置文件中，这些用户看到为其主组激活的事件通知，而不是全系统激活的事件通知。

有关Workfront管理员如何解锁事件通知的信息，请参阅 [解锁或锁定所有组的事件通知配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

有关事件默认通知设置的信息，请参阅 [事件通知在Adobe Workfront中可用](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront计划</a>*</td> 
   <td> <p>专业或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfront许可证</a>*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 查看和配置组的事件通知

1. （视情况而定）如果您是Workfront管理员，并且已经在“电子邮件通知”页面（设置>电子邮件>通知）上，则可以执行以下操作，然后跳到步骤6:删除 **系统事件通知** 在列表上方的框中，开始在框中键入群组的名称，然后在出现时单击该名称。
1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组** ![](assets/groups-icon.png).

1. 单击顶级群组的名称。
1. 在左侧菜单中，单击 **事件通知**.

   在显示的列表中， **活动** 左侧的列显示组的哪些通知处于活动状态（蓝色）和非活动状态（灰色）。

1. 要激活或停用已解锁的事件通知，请执行以下操作：单击 <strong>活动</strong> 列激活 <img src="assets/email-notification-enabled-unlocked.png"> 或停用 <img src="assets/email-notification-disabled-unlocked.png"> 它。

   >[!INFO]
   >
   >**示例：** 您可以配置下面显示的前两个已为群组解锁的营销群组事件通知。</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* 如果 <strong>活动</strong> 列灰暗 <img src="assets/email-notification-disabled-locked.png">，则对于所有用户和群组管理员都无法激活或编辑其电子邮件主题行的事件通知将被停用
   >* 如果 <strong>活动</strong> 列为灰色且不灰显 <img src="assets/email-notification-disabled-unlocked.png">，则事件通知为 <strong>已停用</strong> 群组管理员可以为其群组激活它。
   >* 如果 <strong>活动</strong> 列为蓝色且灰显 <img src="assets/email-notification-enabled-locked.png">，则会激活事件通知，以便所有用户和群组管理员都无法将其停用或编辑其群组的电子邮件主题行。
   >* 如果 <strong>活动</strong> 列为蓝色且不灰显 <img src="assets/email-notification-enabled-unlocked.png">，则事件通知为 <strong>已激活</strong> 群组管理员可以为其群组停用该功能。


<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

