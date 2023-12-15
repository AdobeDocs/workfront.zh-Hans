---
content-type: overview;reference
navigation-topic: notifications
title: 通知概述
description: Adobe Workfront会在您的移动设备上发送电子邮件通知、应用程序内通知和通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 1%

---

# 通知概述

<!--Audited: 12/2023-->

[!DNL Adobe Workfront] 会在您的移动设备上发送电子邮件通知、应用程序内通知和通知。

## 电子邮件通知

[!DNL Workfront] 会发送电子邮件通知，以提醒用户有关Workfront中的活动，并提供有用的信息和链接。

要更改电子邮件通知的偏好设置，请参阅 [修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>如果您希望从沙盒环境接收电子邮件通知，则必须从该环境中的用户配置文件启用电子邮件。

您可以收到以下电子邮件通知 [!DNL Workfront]：

* [事件通知](#event-notifications)
* [每日摘要通知](#daily-digest-notifications)
* [已发布评论的通知](#notification-of-posted-comments)
* [自动提醒](#automatic-reminders)
* [提醒通知](#reminder-notifications)
* [讨论区通知](#boards-notifications)
* [其他 [!DNL Workfront] 电子邮件](#other-workfront-emails)

### 事件通知

事件通知通常由某些预定义事件触发，例如向您分配任务或获得您所做评论的回复。

在中激活事件通知后 [!DNL Workfront] 系统(按您的 [!DNL Workfront] 管理员或组管理员，您可以通过编辑 [!UICONTROL 通知] 用户配置文件中的首选项。 您还可以选择是在事件发生时接收通知，还是接收在一封每日摘要电子邮件中摘要的事件。

您可能会在设置中只看到这些通知的子集，具体取决于 [!DNL Workfront] 管理员已为配置事件通知 [!DNL Workfront] 系统。 有关更多信息，请参阅 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

默认状态显示创建新用户时默认为新用户启用哪些通知（每天、即时或同时启用两者）。

有关事件通知的完整列表，以及有关如何在系统级别、组级别或用户级别启用和配置这些通知的信息，请参阅 [事件通知可在 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

有关如何选择要接收哪些事件通知的信息，请参阅 [修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>只有事件通知可以配置为在每日摘要更新中发送。

### 每日摘要通知

每日摘要通知是一封电子邮件，其中包含您在发送电子邮件前24小时内收到的特定类型的所有通知。

有关为每日摘要电子邮件投放启用的电子邮件通知的完整列表以及有关电子邮件通知所有类别的信息，请参阅 [事件通知](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] 不发送任何每日摘要通知 [!UICONTROL 其他] 和 [!DNL Goals] 事件类别。 您无法禁用这些类别的每日通知。

接收每日摘要通知时应注意以下几点：

* 每个 [!UICONTROL 通知] 部分在您的 **[!UICONTROL 我的设置]** 面板生成自己的每日摘要电子邮件。 您每天的每日摘要电子邮件数量可以与为每日摘要电子邮件启用的通知设置数量相同。\
   例如，如果您选择在下接收多个操作的每日摘要电子邮件， **[!UICONTROL 有关“项目I”的信息] 自己的，** 您会收到一封电子邮件通知，其中列出了此区域满足的所有事件。

* 每日摘要电子邮件中的通知按各种标准进行分组。 例如，在 **[!UICONTROL 有关我拥有的项目的信息]**&#x200B;时，事件按项目名称分组。

  对于 **[!UICONTROL 通信]** 类别，则通知按通信发生的对象分组。

  >[!NOTE]
  >
  >对于“通信”类别，您可以选择仅用于即时发送的单个通知。 要在每日摘要中发送通知，您必须选择所有通知。

* 每日摘要电子邮件列出针对某个特定区域(例如 **有关我拥有的项目的信息**)，并且是在选择交付时间之前的24小时内。
* 为每日摘要投放选择的时区与您的时区匹配，因为它是在您的浏览器上配置的。
* 每日摘要电子邮件在主题行中包含分区的名称以及投放日期。
* 要投放每日摘要，必须至少有一个事件触发通知。 如果未满足标记为每日摘要电子邮件的事件，则不会发送每日摘要。

### 已发布评论的通知

中的通知 [!UICONTROL 通信] 类别提醒您注意已发布在 [!UICONTROL 更新] 特定项目的流。

的每日摘要电子邮件 [!UICONTROL 通信] 已为所有可用通知选择类别。

为发生通信的对象总结该信息，并且为每个对象显示通信消息的总数。

要回复评论或在Workfront中查看评论，请执行以下操作：

1. 单击 **[!UICONTROL 注释]** 按钮。

   此 [!UICONTROL 更新] 此时将打开对象区域，并以蓝色列出特定注释。

   打开一个回复框，您可以使用它来回复注释。

有关配置电子邮件通知（包括启用每日摘要通知）的更多信息，请参阅 [查看和修改电子邮件通知设置](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings) 在 [修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### 自动提醒

自动提醒功能由您的 [!DNL Workfront] 管理员提醒您过期、延迟或接近计划完成日期的任务和问题。 对于延迟通知，在任务或问题完成之前，每夜发送电子邮件。 管理员配置这些后，将无法禁用它们。 此外，您无法更改自动提醒触发的电子邮件的内容或主题行。

它们可以被发送至以下一类或多类人员：

* 分配给任务或问题的用户
* 用户的直属经理
* 直属经理的经理

自动提醒电子邮件发送自您的电子邮件地址 [!DNL Workfront] 已选择管理员来处理传出电子邮件。

根据激活了哪个自动提醒，自动提醒电子邮件中提供了以下类型的信息：

* 任务或问题的创建日期
* 任务或问题名称
* 任务或问题所在项目的名称
* 任务或问题的描述
* 分配给任务或问题的用户列表
* 输入任务或问题的用户的名称
* 任务或问题的优先级
* 任务或问题超期的日期

有关启用自动提醒的信息，请参阅 [设置自动提醒](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### 提醒通知

A [!DNL Workfront] 管理员(或具有 [!UICONTROL 规划者] 访问级别和对提醒通知的管理访问权限)可以设计有关临近截止时间的提醒通知，并手动将其与项目、任务、问题和时间表关联。

>[!IMPORTANT]
>
>如果用户收到上述任何对象的提醒通知后截止日期发生变化，则用户不会收到另一提醒通知。

提醒通知是从以下电子邮件地址发送的： [!DNL Workfront] 已选择管理员来处理传出电子邮件。

有关设置和启用提醒通知的信息，请参阅 [设置提醒通知](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

有关如何获得所需管理访问权限的信息，请参见 [授予用户对特定区域的管理访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

### 讨论区通知

[!DNL Adobe Workfront] [!UICONTROL 讨论区] 当您添加到展示板并分配给您卡片时，会向您发送电子邮件。 您可以在讨论区首选项中选择要接收的电子邮件。

有关更多信息，请参阅 [讨论区电子邮件通知和首选项](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### 其他 [!DNL Workfront] 电子邮件

您可能会收到其他电子邮件 [!DNL Workfront] 无法配置的属性。

以下电子邮件由自动发送 [!DNL Workfront] 当满足以下条件时：

* 恢复项目：当 [!DNL Workfront] 管理员从恢复对象 [!UICONTROL 回收] 在收件箱中，电子邮件会发送至 [!DNL Workfront] 管理员。
* 无法恢复：当 [!DNL Workfront] 管理员尝试从回收站恢复对象，恢复失败时，会向发送一封电子邮件 [!DNL Workfront] 管理员。

以下电子邮件只能在用户配置文件级别进行配置。 无法在系统级别启用或禁用它们：

* 个人任务完成：当分配给其他人的个人任务完成时，您将收到一封电子邮件。
* 添加到用户的评论：当有人对您的用户配置文件发表评论时，您将收到一封电子邮件。

## 应用程序内通知

您可以在以下位置接收通知： [!DNL Workfront] Web应用程序，在发生某些事件时。

有关应用程序内通知的更多信息，请参阅 [查看和管理应用程序内通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## 移动电子邮件应用程序中的电子邮件通知

您可以接收 [!DNL Workfront] 移动设备上的移动电子邮件应用程序中的电子邮件通知。

如果您拥有 [!DNL Workfront] 安装在您手机上的移动设备应用程序，点击电子邮件中的链接即可在以下位置打开它们： [!DNL Workfront] 移动应用程序。 这包括点按以下任一操作按钮：

* [!UICONTROL 处理此项工作]
* [!UICONTROL 注释]
* [!UICONTROL 作出批准决定]
* [!UICONTROL 查看所有通知]
* [!UICONTROL 添加]
* [!UICONTROL 开始使用]
* [!UICONTROL 查看更多详细信息]

欲知关于 [!DNL Workfront] 移动设备应用程序，请参阅 [使用 [!DNL Adobe Workfront] 移动应用程序](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
