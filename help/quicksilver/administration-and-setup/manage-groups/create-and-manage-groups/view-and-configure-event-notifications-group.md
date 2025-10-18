---
user-type: administrator
product-area: system-administration;user-management
keywords: 视图，组，事件，通知，配置，启用，禁用
navigation-topic: create-and-manage-groups
title: 查看和配置组的事件通知
description: 作为组管理员，您可以查看为您管理的组激活的事件通知。 此外，如果Adobe Workfront管理员解锁事件通知，则可以为您管理的顶级组配置该通知。 事件通知的配置包括激活或停用该通知。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# 查看和配置组的事件通知

作为组管理员，您可以查看为您管理的组激活的事件通知。

此外，如果Adobe Workfront管理员解锁事件通知，则可以为您管理的顶级组配置该通知。 事件通知的配置包括激活或停用该通知。

Workfront管理员还可以为任何组执行此操作。

为组配置事件通知会影响用户，而该组或其子组之一是其主组。 在其用户配置文件中，这些用户会看到为其主组激活的事件通知，而不是在系统范围内激活的事件通知。

有关Workfront管理员如何解锁事件通知的信息，请参阅[解锁或锁定所有组的事件通知配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)。

有关事件的默认通知设置的信息，请参阅[事件通知类型](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr>
  <tr> 
   <td>访问级别配置</td> 
   <td>您必须是组的组管理员或系统管理员。</td>
  </tr>
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查看和配置组的事件通知

>[!TIP]
>
>如果您是Workfront管理员，并且已在“电子邮件通知”页面（“设置”>“电子邮件”>“通知”）上，您可以执行以下操作，然后跳到步骤6：在列表上方的框中删除&#x200B;**系统事件通知**，在框中开始键入组的名称，然后在组出现时单击它。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![组](assets/groups-icon.png)。

1. 单击顶级组的名称。
1. 在左侧菜单中，单击&#x200B;**事件通知**。

   在显示的列表中，左侧的&#x200B;**活动**&#x200B;列显示组的活动（蓝色）和非活动（灰色）通知。

1. 要激活或取消激活已解锁的事件通知：请单击<strong>活动</strong>列中的按钮以激活 <img src="assets/email-notification-enabled-unlocked.png">或停用 <img src="assets/email-notification-disabled-unlocked.png">它。

   >[!INFO]
   >
   >**示例：**&#x200B;您可以配置下面显示的、已为群组解锁的前两个营销群组事件通知。</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* 如果<strong>活动</strong>列中的按钮为灰色且灰显 <img src="assets/email-notification-disabled-locked.png">，已为所有用户停用事件通知，组管理员无法激活它或编辑其电子邮件主题行
   >* 如果<strong>活动</strong>列中的按钮为灰色且不暗显 <img src="assets/email-notification-disabled-unlocked.png">，已为所有用户<strong>停用事件通知，并且</strong>组管理员可以为他们的组激活该通知。
   >* 如果<strong>活动</strong>列中的按钮为蓝色且变暗 <img src="assets/email-notification-enabled-locked.png">，已为所有用户激活事件通知，组管理员无法为其组停用或编辑其电子邮件主题行。
   >* 如果<strong>活动</strong>列中的按钮为蓝色且未变暗 <img src="assets/email-notification-enabled-unlocked.png">，已为所有用户<strong>激活事件通知，并且</strong>组管理员可以为他们的组停用该通知。

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

