---
content-type: overview
navigation-topic: notifications
title: 事件通知
description: 事件通知是由对象（如项目、任务或问题）上的各种类型事件触发的电子邮件。 当项目中发生其他人需要了解的情况时，将发送这些事件。 根据事件不同，用户每天都会收到关于该事件的即时电子邮件通知，或者同时收到关于该事件的即时和每日电子邮件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# 事件通知

事件通知是由对象（如项目、任务或问题）上的各种类型事件触发的电子邮件。 当项目中发生其他人需要了解的情况时，将发送这些事件。 根据事件不同，用户每天都会收到关于该事件的即时电子邮件通知，或者同时收到关于该事件的即时和每日电子邮件通知。

>[!NOTE]
>
>事件通知是以下几种类型之一 [!DNL Adobe Workfront] 通知。 有关所有的信息 [!DNL Workfront] 通知类型，请参阅 [[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md).

## 配置事件通知

事件通知电子邮件可以在下面列出的以下级别进行配置。 事件通知的配置包括激活或停用该通知。

* **系统级别**：A [!DNL Workfront] 管理员可以在系统级别激活和停用事件通知，如中所述 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  默认情况下，所有组都会继承系统通知，但如果允许，组管理员可以更改组级别上的某些配置。 [!DNL Workfront] 管理员，如下面的下一个项目符号项目中所述。

* **组级别**：组管理员可以为他们管理的组配置事件通知。 [!DNL Workfront] 管理员为组解锁此功能。 如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 同样的情况也适用于 [!DNL Workfront] 管理员（适用于任何组）。 有关更多信息，请参阅 [查看和配置组的事件通知](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

  >[!NOTE]
  >
  >此功能最初仅作为分阶段推广的一部分提供给群集4上的客户。 此后不久将可供其他集群使用。 本文将在出现这种情况时进行更新。

* **用户级别**：在系统范围内激活的所有事件通知都列在每个用户的 [!UICONTROL 通知] 部分。 用户可以在该处激活和取消激活其单个事件通知。

  [!DNL Workfront] 管理员和有权编辑其他用户的用户也可以在个人用户的配置文件中激活和取消激活通知。

  有关更多信息，请参阅 [修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >用户级通知还包括 [!DNL Workfront Goals] 通知。 但是， [!DNL Workfront] 管理员或组管理员无法配置通知 [!DNL Workfront Goals]. 每个用户必须配置自己的库 [!DNL Workfront Goals] 通知中。 如果您有权限编辑用户，您还可以为其他人修改这些通知。 用于启用 [!DNL Workfront Goals] 有关您的配置文件或您有权编辑的其他用户的通知，请参阅 [通知：目标](../../workfront-basics/using-notifications/notifications-goals.md).

  有关哪些通知的更多信息， [!DNL Workfront] 管理员可以配置，请参见 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] 仅在新的 [!DNL Adobe Workfront] 体验。

## 事件通知内容

事件通知电子邮件包含有关所发生事件的信息，并包含指向的链接 [!DNL Workfront] 您可以在其中查看系统中的事件。 有关接收电子邮件通知的更多信息，请参阅 [[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] 管理员无法更改电子邮件通知的内容，因为它们是由配置的 [!DNL Workfront]. 但是，它们可以更改事件通知电子邮件的主题行。 有关更多信息，请参阅 [自定义事件通知的电子邮件主题](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

对于列表，所有 [!DNL Workfront] 事件通知，以及每个事件的简要说明，以及默认情况下事件是处于活动状态还是处于不活动状态，请参阅 [事件通知可在 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
