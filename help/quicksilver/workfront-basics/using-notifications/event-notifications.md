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
source-wordcount: '554'
ht-degree: 0%

---

# 事件通知

事件通知是由对象（如项目、任务或问题）上的各种类型事件触发的电子邮件。 当项目中发生其他人需要了解的情况时，将发送这些事件。 根据事件不同，用户每天都会收到关于该事件的即时电子邮件通知，或者同时收到关于该事件的即时和每日电子邮件通知。

>[!NOTE]
>
>事件通知是[!DNL Adobe Workfront]通知的几种类型之一。 有关所有[!DNL Workfront]通知类型的信息，请参阅[[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md)。

## 配置事件通知

事件通知电子邮件可以在下面列出的以下级别进行配置。 事件通知的配置包括激活或停用该通知。

* **系统级别**： [!DNL Workfront]管理员可以在系统级别激活和停用事件通知，如[为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)中所述。

  默认情况下，所有组都将继承系统通知，但如果[!DNL Workfront]管理员允许，组管理员可以更改组级别上的某些配置，如下面的下一个项目符号项中所述。

* **组级别**：组管理员可以在[!DNL Workfront]管理员为组解锁此功能后，为其管理的组配置事件通知。 如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 对于[!DNL Workfront]管理员（任何组）也是如此。 有关详细信息，请参阅[查看和配置组](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)的事件通知。

  >[!NOTE]
  >
  >此功能最初仅作为分阶段推广的一部分提供给群集4上的客户。 此后不久将可供其他集群使用。 本文将在出现这种情况时进行更新。

* **用户级别**：在系统范围内激活的所有事件通知都列在每个用户个人资料的[!UICONTROL 通知]部分中。 用户可以在该处激活和取消激活其单个事件通知。

  [!DNL Workfront]管理员和有权编辑其他用户的用户也可以在个人用户档案中激活和停用通知。

  有关详细信息，请参阅[修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

  >[!NOTE]
  >
  >用户级通知还包括[!DNL Workfront Goals]个通知。 但是，[!DNL Workfront]管理员或组管理员无法为[!DNL Workfront Goals]配置通知。 每个用户都必须在自己的配置文件中配置自己的[!DNL Workfront Goals]通知。 如果您有权限编辑用户，您还可以为其他人修改这些通知。 要为您的配置文件或您有权编辑的其他用户启用[!DNL Workfront Goals]通知，请参阅[通知：目标](../../workfront-basics/using-notifications/notifications-goals.md)。

  有关[!DNL Workfront]管理员可以配置哪些通知的更多信息，请参阅[为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。 [!DNL Workfront Goals]仅在新的[!DNL Adobe Workfront]体验中可用。

## 事件通知内容

事件通知电子邮件包含有关所发生事件的信息，并包含指向[!DNL Workfront]的链接，您可以在其中查看系统中的事件。 有关接收电子邮件通知的详细信息，请参阅[[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md)。

[!DNL Workfront]管理员无法更改电子邮件通知的内容，因为它们由[!DNL Workfront]配置。 但是，它们可以更改事件通知电子邮件的主题行。 有关详细信息，请参阅[自定义事件通知的电子邮件主题](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md)。

有关所有[!DNL Workfront]事件通知的列表，以及每个事件的简要说明，以及默认情况下是活动还是不活动，请参阅 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)中提供的[事件通知。
