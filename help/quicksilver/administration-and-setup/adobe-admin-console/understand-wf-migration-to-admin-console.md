---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: 了解Workfront迁移到Adobe Admin Console
description: 本文笼统地描述了将组织移动到Adobe Admin Console的过程，以便您(Workfront管理员)能够知道会发生什么。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# 了解Workfront迁移到Adobe Admin Console

<!--DELETE ME MARCH 2026-->

>[!IMPORTANT]
>
>现在，所有Workfront组织都已登记到Adobe Admin Console。
>
>本文将在不久的将来删除。

Adobe正在改变您管理Adobe Workfront用户的方式，从而提高您和贵组织的生产效率。 作为此更改的一部分，Adobe正在将您的Workfront实例和用户迁移到Adobe Admin Console。 这是必需的迁移，不会影响任何报表、批准路径、内容或资源。 它将影响您管理用户访问权限的方式以及您的用户登录的方式。

本文笼统地描述了将组织移动到Adobe Admin Console的过程，以便您(Workfront管理员)能够知道会发生什么。

要了解如何使用Adobe Admin Console管理整个组织的Adobe权限，请参阅[在Adobe Admin Console中管理用户](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)。

## 有什么变化？

作为迁移的一部分，您的用户管理将从Workfront应用程序移至Adobe Admin Console，具有以下管理角色：

* **系统管理员**&#x200B;是具有所有管理员权限的超级用户。 他们分配所有管理角色，并管理整个组织所有产品的用户。

* **产品配置文件管理员(Workfront系统管理员)**&#x200B;管理组织中哪些用户有权访问Workfront。

* **用户将使用Adobe标识登录。**&#x200B;在Adobe将现有用户迁移到Adobe Admin Console后，用户将使用其新的Adobe身份(Adobe ID或Adobe Federated ID (SSO))登录到其Workfront实例。

* **在Workfront应用程序本身中管理所有其他功能的方式没有变化**，包括功能、用户角色、工作区、功能和行为的管理。

## 迁移历程时间线

Adobe将首先将Workfront实例迁移到Adobe Admin Console，然后使用已验证的电子邮件地址迁移所有现有用户。 如果您是系统管理员或Workfront产品配置文件管理员(Workfront系统管理员)，您将收到一封电子邮件，引导您完成迁移历程。 以下是您可以期待的时间表：

### Workfront迁移到Adobe Admin Console完成

Workfront迁移到Adobe Admin Console后，系统管理员将收到一封电子邮件。 此时，系统管理员可能需要在用户迁移开始&#x200B;**前完成一些必需的步骤**，以最大程度地减少对Workfront用户的影响。

* **如果您的Workfront用户当前使用SSO登录**，您必须在Adobe Admin Console上设置SSO，以便您的用户可以继续使用SSO登录。 如果您的Workfront用户当前未使用SSO，但希望在Adobe Admin Console上对其进行设置，则可以在迁移历程的此阶段进行设置。
* **如果您已在Adobe Admin Console中管理其他Adobe产品**，Adobe可能会征求您的同意，以自动将用户迁移到现有控制台。 单击电子邮件中的&#x200B;**开始**&#x200B;按钮以导航到同意页面。
* **如果您之前删除了请求者许可证类型**，则它将被添加到您的系统中。 不会将任何用户分配给此许可证类型，但在Workfront和Adobe Admin Console之间同步时需要此许可证。 您无需对请求者许可证类型执行任何操作。

用户管理目前没有变化。 Workfront管理员将继续管理Workfront中的用户，并且在用户迁移完成之前，用户将继续使用其Workfront ID或SSO登录。

### 计划用户迁移

系统管理员完成上一部分中概述的先决条件后，Adobe将自动计划用户迁移30天，并且还将与Workfront产品配置文件管理员(Workfront系统管理员)沟通以管理用户迁移。

Workfront产品配置文件管理员(Workfront系统管理员)将：

* 收到一封包含其计划用户迁移开始日期的电子邮件（大约在完成这些先决条件后的30天）
* 获取对指定的Workfront管理员控制台的访问权限，在该控制台中，用户可以更改其迁移日期

  >[!NOTE]
  >
  >由于迁移的复杂程度，日期更改限制在计划日期后的30天内有效。 如果您需要更晚的日期，请联系支持人员。

* 在用户迁移开始日期前1天接收提醒电子邮件

### 准备用户迁移日

作为Workfront产品配置文件管理员(Workfront系统管理员)，负责确保所有用户为迁移日期做好准备。

* 通过通知所有用户以下信息，让他们为即将迁移到Adobe Identity做好准备：

   * 在用户迁移时，他们将收到Adobe的电子邮件，通知他们对Workfront登录方式所做的更改。 将邀请用户接受首次使用Adobe身份登录的邀请，方法是使用现有Adobe ID登录，或使用同一电子邮件地址设置一个新帐户。

### 迁移日期待完成的任务

* **用户迁移将在客户托管Workfront数据中心的午夜开始。**

* **Adobe将首先自动迁移Workfront管理员。**&#x200B;将Workfront管理员迁移到Adobe身份后，将为他们分配Adobe产品配置文件管理员(Workfront系统管理员)角色。 用户在迁移之前可能拥有的现有角色将不受影响。

  >[!NOTE]
  >
  >在用户迁移期间，不会失去对产品的访问权限。 如果用户在其用户迁移期间登录，则不会产生任何影响。 但是，下次登录时，他们将必须使用其Adobe身份。



* **在迁移用户时，用户将收到Adobe的电子邮件，通知他们登录Workfront的方式发生了更改。**&#x200B;用户将被邀请接受首次使用Adobe身份进行登录的邀请，方法是使用现有Adobe ID登录，或使用同一电子邮件地址设置新的Adobe ID。

  有关如何使用Adobe ID登录Workfront的信息，请参阅[登录Adobe Experience Cloud](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud)。

### 用户迁移完成

迁移所有管理员和用户后，Adobe将通过电子邮件通知所有系统管理员和产品配置文件管理员(Workfront系统管理员)。 此时，该实例的所有Workfront用户都将使用Adobe身份登录到Workfront。 Workfront系统管理员和产品配置文件管理员(Workfront系统管理员)可以在Adobe Admin Console中管理用户访问权限。 如果客户没有在Administrator Console中使用某种形式的目录同步，则他们可能会继续在Workfront应用程序中管理对Workfront的访问。

## 获取支持

如有疑问或顾虑，请按照文章[中所述的步骤联系客户支持](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。




