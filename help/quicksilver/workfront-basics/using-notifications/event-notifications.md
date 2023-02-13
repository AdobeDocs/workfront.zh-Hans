---
content-type: overview
navigation-topic: notifications
title: 事件通知
description: 事件通知是由对象（如项目、任务或问题）上各种类型的事件触发的电子邮件。 当项目中发生其他人需要了解的情况时，系统会发送这些消息。 根据事件的不同，用户会收到即时、每天或即时和每日的电子邮件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# 事件通知

事件通知是由对象（如项目、任务或问题）上各种类型的事件触发的电子邮件。 当项目中发生其他人需要了解的情况时，系统会发送这些消息。 根据事件的不同，用户会收到即时、每天或即时和每日的电子邮件通知。

>[!NOTE]
>
>事件通知是以下几种类型之一 [!DNL Adobe Workfront] 通知。 有关所有 [!DNL Workfront] 通知类型，请参阅 [[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md).

## 配置事件通知

事件通知电子邮件可以在下面列出的以下级别进行配置。 事件通知的配置包括激活或取消激活它。

* **系统级别**:A [!DNL Workfront] 管理员可以在系统级别激活和停用事件通知，如 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   默认情况下，所有组都会继承系统通知，但组管理员可能能够更改组级别的某些配置（如果允许） [!DNL Workfront] 管理员，如下面的下一个项目符号项中所述。

* **组级别**:群组管理员可以在 [!DNL Workfront] 管理员将解锁组的此功能。 如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 同样的情况也适用于 [!DNL Workfront] 管理员（适用于任何组）。 有关更多信息，请参阅 [查看和配置群组的事件通知](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

   >[!NOTE]
   >
   >此功能最初仅供群集4上的客户使用，这是分阶段推出的一部分。 此后不久，它将可用于其他群集。 此文章将随之更新。

* **用户级别**:每个用户的 [!UICONTROL 通知] 的章节。 用户可以在此处激活和停用其单个事件通知。

   [!DNL Workfront] 管理员和有权编辑其他用户的用户还可以在个人用户的配置文件中激活和停用通知。

   有关更多信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

   >[!NOTE]
   >
   >用户级通知还包括 [!DNL Workfront Goals] 通知。 但是， [!DNL Workfront] 管理员或组管理员无法为 [!DNL Workfront Goals]. 每个用户必须配置自己的 [!DNL Workfront Goals] 通知。 如果您有权编辑用户，则还可以为其他用户修改这些通知。 启用 [!DNL Workfront Goals] 有关您的配置文件或您有权编辑的其他用户的通知，请参阅 [通知：目标](../../workfront-basics/using-notifications/notifications-goals.md).

   有关哪些通知的更多信息，请参阅 [!DNL Workfront] 管理员可以配置，请参阅 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] 仅在 [!DNL Adobe Workfront] 体验。

## 事件通知内容

事件通知电子邮件包含有关所发生事件的信息，并包含指向的链接 [!DNL Workfront] 您可以在系统中查看事件的位置。 有关接收电子邮件通知的更多信息，请参阅 [[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] 管理员无法更改电子邮件通知的内容，因为这些通知的配置 [!DNL Workfront]. 但是，他们可以更改事件通知电子邮件的主题行。 有关更多信息，请参阅 [自定义事件通知的电子邮件主体](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

列出所有 [!DNL Workfront] 事件通知，以及每个事件的简要说明以及默认情况下它是活动还是非活动，请参阅 [事件通知在 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
