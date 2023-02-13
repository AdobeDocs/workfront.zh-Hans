---
content-type: overview;reference
navigation-topic: notifications
title: Adobe Workfront通知
description: Adobe Workfront会在您的移动设备上发送电子邮件通知、应用程序内通知和通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '1255'
ht-degree: 1%

---

# [!DNL Adobe Workfront] 通知

[!DNL Adobe Workfront] 在移动设备上发送电子邮件通知、应用程序内通知和通知。

## 电子邮件通知

[!DNL Workfront] 会发出大量电子邮件通知，以提醒用户Workfront中的活动，并提供有用的信息和链接。

>[!NOTE]
>
>如果要从沙盒环境接收电子邮件通知，则必须从该环境的用户配置文件中启用电子邮件。

您可以从以下地址接收电子邮件通知 [!DNL Workfront]:

* [事件通知](#event-notifications)
* [每日摘要通知](#daily-digest-notifications)
* [已发布评论的通知](#notification-of-posted-comments)
* [自动提醒](#automatic-reminders)
* [提醒通知](#reminder-notifications)
* [其他 [!DNL Workfront] 电子邮件](#other-workfront-emails)

### 事件通知

事件通知在 [!DNL Workfront]. 它们通常由某些事件触发。

在激活事件通知后 [!DNL Workfront] 管理员或组管理员，您可以通过编辑 [!UICONTROL 通知] 首选项。 您还可以选择是希望在发生事件时接收通知，还是希望接收在每日摘要电子邮件中汇总的事件。

根据 [!DNL Workfront] 管理员为 [!DNL Workfront] 系统(如 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md))，则您可能只会在设置中看到这些通知的子集。

默认状态显示在创建新用户时默认为新用户启用哪些通知（每日、即时或两者）。

有关事件通知的完整列表，以及有关如何在系统级别、组级别或用户级别启用和配置事件通知的信息，请参阅 [事件通知在 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

有关如何选择要接收的事件通知的信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>事件通知是唯一可配置为在每日摘要更新中发送的通知。

### 每日摘要通知

有关为每日摘要电子邮件投放启用了哪些电子邮件通知的完整列表，以及有关电子邮件通知所有类别的信息，请参阅 [事件通知](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] 不会为 [!UICONTROL 其他] 和 [!DNL Goals] 事件类别。 不能禁用这些类别的每日通知。

在接收每日摘要通知时，需注意以下几项事项：

* 每个 [!UICONTROL 通知] 的 **[!UICONTROL 我的设置]** 面板会生成自己的每日摘要电子邮件。 您可以每天拥有与为每日摘要电子邮件启用的通知设置相同数量的每日摘要电子邮件。\
   例如，如果您选择在 **[!UICONTROL 有关项目I的信息] 拥有，** 您会收到一封电子邮件通知，其中列出了该区域遇到的所有事件。

* 每日摘要电子邮件中的通知按各种标准分组。 例如，对于 **[!UICONTROL 有关我拥有的项目的信息]**，则事件会按项目名称分组。

   对于 **[!UICONTROL 通信]** 类别中，通知按发生通信的对象进行分组。

* 每日摘要电子邮件列出了针对某个特定区域(如 **有关我拥有的项目的信息**)，则在选定的交付时间之前的24小时内发送。
* 为每日摘要投放选择的时区与您在浏览器中配置的时区匹配。
* 每日摘要电子邮件包含主题行中部分的名称以及提交日期。
* 至少有一个事件必须触发通知才能提交每日摘要。 如果未满足标记为每日摘要电子邮件的事件，则不会发送每日摘要。

### 已发布评论的通知

中的通知 [!UICONTROL 通信] 类别会提醒您有关已在 [!UICONTROL 更新] 特定项目的流。

的每日摘要电子邮件 [!UICONTROL 通信] 类别。

该信息被汇总到发生通信的对象，并且每个对象显示通信消息的总数。

有关配置电子邮件通知的更多信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

有关注释的说明 [!UICONTROL 通信] 电子邮件，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

详细了解 [!UICONTROL 通信] 电子邮件，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

有关启用每日摘要通知的更多信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### 自动提醒

您的 [!DNL Workfront] 管理员可提醒您任务和问题已到期、延迟或接近计划完成日期。 对于延迟通知，在任务或问题完成之前，会在夜间发送电子邮件。 在管理员配置这些组件后，您将无法禁用它们。 此外，您无法更改由自动提醒触发的电子邮件的内容或主题行。

它们可以发送到以下一个或多个：

* 分配给任务或问题的用户
* 用户的直接经理
* 直接经理的经理

自动提醒电子邮件从您的 [!DNL Workfront] 管理员已选择处理传出电子邮件。

根据激活的自动提醒，自动提醒电子邮件中提供了以下类型的信息：

* 创建任务或问题的日期
* 任务或问题名称
* 任务或问题所在项目的名称
* 任务或问题的描述
* 分配给任务或问题的用户列表
* 输入任务或问题的用户的名称
* 任务或问题的优先级
* 任务或问题过期的日期

有关启用自动提醒的信息，请参阅 [设置自动提醒](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### 提醒通知

A [!DNL Workfront] 管理员(或具有 [!UICONTROL 计划员] 访问级别和对提醒通知的管理访问权限)可以设计关于接近截止时间的提醒通知，并将其附加到项目、任务、问题和时间表。 有关如何获取所需管理访问权限的详细信息，请参阅 [授予用户对特定区域的管理访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!IMPORTANT]
>
>如果截止时间在用户收到上述任何对象的提醒通知后发生更改，则用户不会再收到提醒通知。

提醒通知从电子邮件地址发送，通知中 [!DNL Workfront] 管理员已选择处理传出电子邮件。

有关设置和启用提醒通知的信息，请参阅 [设置提醒通知](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

### 其他 [!DNL Workfront] 电子邮件

您可能会从收到其他电子邮件 [!DNL Workfront] 无法配置。 以下电子邮件由 [!DNL Workfront] 当满足这些条件时：

* 恢复项目：当 [!DNL Workfront] 管理员从 [!UICONTROL 回收] 宾，则会向 [!DNL Workfront] 管理员。
* 无法还原：当 [!DNL Workfront] 管理员尝试从回收站中恢复对象，但恢复失败，则会向 [!DNL Workfront] 管理员。

以下电子邮件只能在用户配置文件级别配置。 无法在系统级别启用或禁用这些功能：

* 完成个人任务：当您分配给他人的个人任务完成后，您将收到一封电子邮件。
* 向用户添加了注释：当某人对您的用户配置文件进行评论时，您将收到一封电子邮件。

## 应用程序内通知

您可以在 [!DNL Workfront] Web应用程序，当发生某些事件时。

有关应用程序内通知的更多信息，请参阅 [查看和管理应用程序内通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## 移动电子邮件应用程序中的电子邮件通知

您可以 [!DNL Workfront] 电子邮件通知。

如果您拥有 [!DNL Workfront] 手机上安装的移动设备应用程序，点按电子邮件中的链接会在 [!DNL Workfront] 移动设备应用程序。 这包括点按以下任意操作按钮：

* [!UICONTROL 处理此项工作]
* [!UICONTROL 评论]
* [!UICONTROL 做批准决定]
* [!UICONTROL 查看所有通知]
* [!UICONTROL 添加]
* [!UICONTROL 开始]
* [!UICONTROL 查看更多详细信息]

有关 [!DNL Workfront] 移动设备应用程序，请参阅 [使用 [!DNL Adobe Workfront] 移动设备应用程序](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
