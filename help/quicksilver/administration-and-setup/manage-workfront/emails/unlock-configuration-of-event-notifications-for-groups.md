---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 解锁或锁定所有组的事件通知配置
description: 如果您是Adobe Workfront管理员，则可以解锁或重新锁定组管理员为其管理的顶级组配置事件通知的功能。 事件通知的配置包括激活或停用该通知。
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 解锁或锁定所有组的事件通知配置

如果您是Adobe Workfront管理员，则可以解锁或重新锁定组管理员为其管理的顶级组配置事件通知的功能。 事件通知的配置包括激活或停用该通知。

如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员也是如此（适用于任何组）。

当管理员为组配置事件通知时，该配置将影响该组或其子组之一为其主组的用户。 在其用户配置文件中，这些用户会看到为其主组激活的事件通知，而不是在系统范围内激活的事件通知。 有关详细信息，请参阅[查看和配置组](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)的事件通知。

>[!NOTE]
>
>* Workfront管理员可以在Adobe Workfront Classic和新的Adobe Workfront Experience中解锁和重新锁定事件通知的配置。 但组管理员只能在新的Adobe Workfront Experience中为组配置该事件通知。 使用Adobe Workfront Classic的组管理员可以切换到新的Adobe Workfront Experience来配置组的解锁事件通知，然后切换回Adobe Workfront Classic以查看更改的效果。
>* 子组从其上方的顶级组继承组级事件通知配置。
>

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
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>系统管理员</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 解锁或重新锁定配置事件通知的功能

>[!IMPORTANT]
>
>当您重新锁定通知时，系统中所有组都将完全按照您设置的规则继承通知。 此操作将覆盖组管理员可能已对其组进行的任何更改，因此最好先与他们协商。

{{step-1-to-setup}}

1. 单击&#x200B;**电子邮件** > **通知**。

1. 确保&#x200B;**事件通知**&#x200B;选项卡已打开。
1. 单击通知右侧的图标可将其切换到锁定的![锁定图标](assets/lock-toggle-button.png)或解锁的![解锁图标](assets/unlock-toggle-button.png)位置。

   或

   如果要一次解锁或锁定多个通知，请选择它们，然后单击列表上方工具栏中显示的“解锁![解锁”图标](assets/unlock-icon-toolbar.png)或“锁定![锁定”图标](assets/lock-icon-locked-qs.png)按钮。

1. 单击&#x200B;**保存**。
1. （可选）如果要为顶级组配置事件通知，而不是将此任务留给组管理员，可以执行以下操作之一：

   * 在通知列表上方的搜索框中删除&#x200B;**系统事件通知**，搜索并选择顶级组的名称以列出其通知，然后在显示的列表中激活或停用解锁的通知。
   * 单击左侧菜单中的&#x200B;**组**，然后单击顶级组的名称。 单击左侧面板中的&#x200B;**事件通知**，然后配置解锁的事件通知，如[查看和配置组](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)的事件通知中所述。
