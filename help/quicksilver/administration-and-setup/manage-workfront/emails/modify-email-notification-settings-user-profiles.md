---
user-type: administrator
product-area: system-administration
keywords: 修改，电子邮件，通知，设置，批量，批量编辑，配置，多个，用户
navigation-topic: emails-administration
title: 在用户配置文件中修改电子邮件通知设置
description: 如果您是Adobe Workfront管理员，或者您拥有计划员访问级别，以允许您编辑其他用户的设置，则可以一次为多个用户配置通知设置。 这包括指定用户是在发生事件时接收通知，还是在一封每日摘要电子邮件中接收通知(如Adobe Workfront通知中所述)。 有关编辑用户所需的访问级别的信息，请参阅向用户授予访问权限。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# 在用户配置文件中修改电子邮件通知设置

如果您是Adobe Workfront管理员，或者您拥有计划员访问级别，以允许您编辑其他用户的设置，则可以一次为多个用户配置通知设置。 这包括指定用户是在发生事件时接收通知，还是在一封每日摘要电子邮件中接收通知，如 [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md). 有关编辑用户所需的访问级别的信息，请参阅 [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

批量配置通知设置时，您只能更改选定用户共有的设置。

您还可以一次为一个用户配置电子邮件通知。 有关更多信息，请参阅 [激活或停用您自己的事件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
 </tbody> 
</table>

&#42;要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 批量修改多个用户的电子邮件通知设置

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **用户** ![](assets/users-icon-in-main-menu.png). 选择用户，然后单击 **编辑**.
1. 在 **编辑人员** 框，单击 **通知**.

1. 展开类别可查看与该类别相关的通知设置。

   如果至少选定了一个用户，其中通知与其他选定用户的通知不匹配，则该通知的类别复选框包含水平线 ![](assets/straight-line-instead-of-checkmark.jpg) 而不是复选标记。

1. 单击您希望用户每天或即时收到的任何通知，或清除您希望用户停止接收的任何通知。

   对于 **通信** 类别中，您只能为即时投放选择单个通知。 您必须选择要在每日摘要中发送的所有通知。

   修改通知设置时，标签 **已编辑** 将显示该通知设置，以告知您该通知设置已修改。

1. 如果您选择将通知作为每日摘要发送，请选择希望在一天中的哪个时间在 **通知** 部分 **之后的电子邮件每日摘要** 菜单。

   在您选择投放时间后， **之后的电子邮件每日摘要** 框中会显示一个橙色框，表示已编辑投放的时间。

   每日摘要包括在选定时间之前24小时满足通知标准的事件。 用户会收到每种通知类型的每日摘要电子邮件。

   根据系统中排队等待投放的电子邮件数量，每日摘要可能会在您选择的时间之后到达。 列出的时间是您在浏览器设置中指定的本地时间。
