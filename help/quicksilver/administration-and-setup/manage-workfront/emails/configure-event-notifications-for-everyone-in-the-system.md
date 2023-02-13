---
title: 为系统中的每个人配置事件通知
description: 事件通知会在发生特定事件时触发发送给用户的电子邮件。 作为Adobe Workfront管理员或具有计划员访问权限级别的用户，您可以为系统中的所有用户配置事件通知。 事件通知的配置包括激活或取消激活它。
author: Caroline, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 为系统中的每个人配置事件通知

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

事件通知会在发生特定事件时触发发送给用户的电子邮件。 作为Adobe Workfront管理员或具有计划员访问权限级别的用户，您可以为系统中的所有用户配置事件通知。 事件通知的配置包括激活或取消激活它。

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

根据您启用的事件以及用户在其个人资料中保持启用状态，用户在发生事件时会收到即时、每天或即时和每日电子邮件通知。

您首先必须在Workfront实例的“设置”区域中指定希望所有用户接收的通知。 在“设置”区域中激活通知后，该通知会在其配置文件页面中显示为每个用户的激活状态。

在“设置”区域中激活通知并在用户配置文件页面中显示通知后，具有计划许可证的个人用户或其他用户也可以在用户配置文件中配置激活的通知，以控制特定用户收到的通知以及接收通知的频率。 有关更多信息，请参阅 [激活或停用您自己的事件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

有关可激活和取消激活的所有事件通知的列表，请参阅 [事件通知在Adobe Workfront中可用](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

有关解锁事件通知以便群组管理员为其群组配置该通知的信息，请参阅 [解锁或锁定所有组的事件通知配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) 和 [查看和配置群组的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>计划员或更高级别，具有提醒通知的管理访问权限</p> <p>有关授予计划用户管理访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 为所有用户配置事件通知

必须先在Workfront的“设置”区域中启用通知，用户才能在其配置文件中启用或禁用通知。

>[!TIP]
>
>您无法从“设置”区域激活Workfront目标的通知。 用户只能在其配置文件中激活这些通知。 具有计划许可证的用户可以为其他用户激活它们。 有关为用户启用Workfront Target通知的信息，请参阅 [通知：目标](../../../workfront-basics/using-notifications/notifications-goals.md).

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **电子邮件** > **通知**.

1. 确保 **事件通知** 选项卡。
1. 单击事件名称左侧的开关以将其打开或关闭。

   要查看事件的默认通知状态，请参阅 [事件通知](../../../workfront-basics/using-notifications/event-notifications.md).

1. （可选）单击事件通知的名称以自定义电子邮件通知的主题行。

   有关自定义电子邮件通知主题行的更多信息，请参阅 [自定义事件通知的电子邮件主体](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. （可选）如果要解锁电子邮件通知的配置，以便群组管理员可以为其群组单独配置该配置，请单击按钮 ![](assets/lock-toggle-button.png) 到通知的右侧，以将其切换到解锁位置 ![](assets/unlock-toggle-button.png).

   >[!NOTE]
   >
   >此功能最初仅供群集4上的客户使用，这是分阶段推出的一部分。 此后不久，它将可用于其他群集。 此文章将随之更新。

   有关更多信息，请参阅 [解锁或锁定所有组的事件通知配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).
