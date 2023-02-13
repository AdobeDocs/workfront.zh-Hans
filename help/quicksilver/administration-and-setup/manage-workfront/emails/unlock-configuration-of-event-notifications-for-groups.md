---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 解锁或锁定所有组的事件通知配置
description: 如果您是Adobe Workfront管理员，则可以解锁或重新锁定群组管理员为其管理的顶级群组配置事件通知的功能。 事件通知的配置包括激活或取消激活它。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# 解锁或锁定所有组的事件通知配置

如果您是Adobe Workfront管理员，则可以解锁或重新锁定群组管理员为其管理的顶级群组配置事件通知的功能。 事件通知的配置包括激活或取消激活它。

如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。

当管理员为群组配置事件通知时，该配置会影响该群组或其某个子群组为其主页群组的用户。 在用户配置文件中，这些用户看到为其主组激活的事件通知，而不是全系统激活的事件通知。 有关更多信息，请参阅 [查看和配置群组的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Workfront管理员可以解锁和重新锁定Adobe Workfront Classic和新Adobe Workfront体验中事件通知的配置。 但群组管理员只能在新的Adobe Workfront体验中为群组配置该事件通知。 使用Adobe Workfront Classic的群组管理员可以切换到新的Adobe Workfront体验，以为群组配置已解锁的事件通知，然后切换回Adobe Workfront Classic以查看生效的更改。
>* 子组从其上方的顶级组继承组级别事件通知配置。
>


## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>系统管理员</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解锁或重新锁定配置事件通知的功能

>[!IMPORTANT]
>
>当您重新锁定通知时，系统中的所有组都将完全按照您设置的方式继承通知。 这会覆盖组管理员可能为其组所做的任何更改，因此最好先与他们协商。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **电子邮件** > **通知**.

1. 确保 **事件通知** 选项卡。
1. 单击通知右侧的图标以将其切换到已解锁 ![](assets/lock-toggle-button.png) 或锁定 ![](assets/unlock-toggle-button.png) 位置。

   或

   如果要同时解锁或锁定多个通知，请选择它们，然后单击“解锁” ![](assets/unlock-icon-toolbar.png) 或锁定 ![](assets/lock-icon-locked-qs.png) 按钮。

1. 单击&#x200B;**保存**。
1. （可选）如果要为顶级组配置事件通知，而不是将此任务留给组的管理员，可以执行以下操作之一：

   * 删除 **系统事件通知** 在通知列表上方的搜索框中，搜索并选择顶级组的名称以列出其通知，然后在显示的列表中激活或取消激活已解锁的通知。
   * 单击 **群组** 在左侧菜单中，单击顶级组的名称。 单击 **事件通知** 在左侧面板中，配置已解锁的事件通知，如 [查看和配置群组的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
