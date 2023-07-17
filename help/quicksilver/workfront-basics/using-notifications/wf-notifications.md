---
content-type: overview;reference
navigation-topic: notifications
title: Adobe Workfront通知
description: Adobe Workfront会在您的移动设备上发送电子邮件通知、应用程序内通知和通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 4331917d133c52cf727f148b75a213853c1e5679
workflow-type: tm+mt
source-wordcount: '1317'
ht-degree: 1%

---

# [!DNL Adobe Workfront] 通知

[!DNL Adobe Workfront] 会在您的移动设备上发送电子邮件通知、应用程序内通知和通知。

## 电子邮件通知

[!DNL Workfront] 会发送大量电子邮件通知，以提醒用户有关Workfront中的活动并提供有用信息和链接。

要更改电子邮件通知的偏好设置，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>如果要从沙盒环境接收电子邮件通知，则必须在该环境中启用用户配置文件中的电子邮件。

您可以收到以下电子邮件通知 [!DNL Workfront]：

* [事件通知](#event-notifications)
* [每日摘要通知](#daily-digest-notifications)
* [已发布评论的通知](#notification-of-posted-comments)
* [自动提醒](#automatic-reminders)
* [提醒通知](#reminder-notifications)
* [讨论区通知](#boards-notifications)
* [其他 [!DNL Workfront] 电子邮件](#other-workfront-emails)

### 事件通知

事件通知在中预定义 [!DNL Workfront]. 它们通常由特定事件触发。

在事件通知由激活后 [!DNL Workfront] 管理员或组管理员，您可以通过编辑 [!UICONTROL 通知] 用户配置文件中的首选项。 您还可以选择是在事件发生时接收通知，还是接收在一封每日摘要电子邮件中摘要的事件。

取决于 [!DNL Workfront] 管理员已为配置事件通知 [!DNL Workfront] 系统（如中所述） [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md))，则您只能在设置中看到这些通知的子集。

默认状态显示创建新用户时默认为新用户启用哪些通知（每日、即时或两者）。

有关事件通知的完整列表，以及有关如何在系统级别、组级别或用户级别启用和配置这些通知的信息，请参阅 [事件通知位于 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

有关如何选择希望接收哪些事件通知的信息，请参见 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>事件通知是唯一可以配置为在每日摘要更新中发送的通知。

### 每日摘要通知

有关为每日摘要电子邮件投放启用的电子邮件通知的完整列表以及有关电子邮件通知所有类别的信息，请参阅 [事件通知](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] 不发送任何每日摘要通知 [!UICONTROL 其他] 和 [!DNL Goals] 事件类别。 您无法禁用这些类别的每日通知。

在接收每日摘要通知时，需要注意以下几点：

* 每个 [!UICONTROL 通知] 部分 **[!UICONTROL 我的设置]** 面板生成自己的每日摘要电子邮件。 您每天的每日摘要电子邮件数量可以与为每日摘要电子邮件启用的通知设置数量相同。\
   例如，如果您选择在下接收多个操作的每日摘要电子邮件 **[!UICONTROL 有关项目I的信息] 拥有，** 您会收到一封电子邮件通知，其中列出了此区域满足的所有事件。

* 每日摘要电子邮件中的通知按各种标准分组。 例如，在 **[!UICONTROL 有关我拥有的项目的信息]**，则事件按项目名称分组。

  对于 **[!UICONTROL 通信]** 类别时，通知按通信发生的对象分组。

* 每日摘要电子邮件列出某个特定区域(例如 **有关我拥有的项目的信息**)，并且是在选择交付时间之前的24小时内。
* 为每日摘要投放选择的时区与您的时区匹配，因为它是在浏览器上配置的。
* 每日摘要电子邮件在主题行中具有部分的名称以及投放日期。
* 要投放每日摘要，必须至少有一个事件触发通知。 如果未满足标记为每日摘要电子邮件的事件，则不会发送每日摘要。

### 已发布评论的通知

中的通知 [!UICONTROL 通信] 类别提醒您注意已发布在 [!UICONTROL 更新] 特定项目的流。

的每日摘要电子邮件 [!UICONTROL 通信] 已为所有可用通知选择类别。

为发生通信的对象汇总信息，并且为每个对象显示通信消息的总数。

有关配置电子邮件通知的更多信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

有关评论 [!UICONTROL 通信] 电子邮件，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

要了解有关 [!UICONTROL 通信] 电子邮件，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

有关启用每日摘要通知的更多信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### 自动提醒

自动提醒功能由以下用户启用 [!DNL Workfront] 管理员提醒您过期、延迟或接近计划完成日期的任务和问题。 对于延迟通知，在夜间发送电子邮件，直到完成任务或问题。 在管理员配置这些选项后，您将无法禁用它们。 此外，您无法更改自动提醒触发的电子邮件的内容或主题行。

它们可以发送到以下一项或多项中：

* 分配给任务或问题的用户
* 用户的直属经理
* 直属经理的经理

自动提醒电子邮件是从您电子邮件中指定的 [!DNL Workfront] 已选择管理员来处理传出电子邮件。

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

A [!DNL Workfront] 管理员（或具有权限的用户） [!UICONTROL 规划者] 访问级别和对提醒通知的管理访问权限)可以设计有关临近截止日期的提醒通知，并将其附加到项目、任务、问题和时间表。 有关如何获得所需的管理访问权限的更多信息，请参阅 [授予用户对特定区域的管理访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!IMPORTANT]
>
>如果用户收到上述任何对象的提醒通知后截止日期改变，则用户不会收到另一个提醒通知。

提醒通知是从以下电子邮件地址发送的： [!DNL Workfront] 已选择管理员来处理传出电子邮件。

有关设置和启用提醒通知的信息，请参阅 [设置提醒通知](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

### 讨论区通知

[!DNL Adobe Workfront] [!UICONTROL 讨论区] 当您添加到展示板并分配给您卡片时，会向您发送电子邮件。

您可以在讨论区首选项中选择要接收的电子邮件。 有关更多信息，请参阅 [讨论区电子邮件通知和首选项](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### 其他 [!DNL Workfront] 电子邮件

您可能会收到其他电子邮件 [!DNL Workfront] 无法配置。 以下电子邮件由自动发送 [!DNL Workfront] 当满足以下条件时：

* 恢复项目：当 [!DNL Workfront] 管理员从恢复对象 [!UICONTROL 回收] 收件箱内，系统会将电子邮件发送至 [!DNL Workfront] 管理员。
* 无法恢复：当 [!DNL Workfront] 管理员尝试从回收站恢复对象，但恢复失败，将发送电子邮件至 [!DNL Workfront] 管理员。

以下电子邮件只能在用户配置文件级别进行配置。 无法在系统级别启用或禁用它们：

* 完成个人任务：您分配给其他人的个人任务完成后，您将收到一封电子邮件。
* 添加到用户的评论：当有人对您的用户配置文件发表评论时，您将收到一封电子邮件。

## 应用程序内通知

您可在中接收通知 [!DNL Workfront] Web应用程序，在发生某些事件时。

有关应用程序内通知的更多信息，请参阅 [查看和管理应用程序内通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## 移动电子邮件应用程序中的电子邮件通知

您可以接收 [!DNL Workfront] 移动设备上移动电子邮件应用程序中的电子邮件通知。

如果您拥有 [!DNL Workfront] 安装在您手机上的移动设备应用程序，点按电子邮件中的链接会在中打开它们 [!DNL Workfront] 移动应用程序。 这包括点按以下任意操作按钮：

* [!UICONTROL 处理此项工作]
* [!UICONTROL 评论]
* [!UICONTROL 做审批决策]
* [!UICONTROL 查看所有通知]
* [!UICONTROL 添加]
* [!UICONTROL 开始]
* [!UICONTROL 查看更多详细信息]

欲知关于 [!DNL Workfront] 移动设备应用程序，请参阅 [使用 [!DNL Adobe Workfront] 移动应用程序](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
