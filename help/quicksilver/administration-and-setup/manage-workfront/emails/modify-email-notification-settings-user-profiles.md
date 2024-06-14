---
user-type: administrator
product-area: system-administration
keywords: 修改，电子邮件，通知，设置，批量，批量编辑，配置，多个，用户
navigation-topic: emails-administration
title: 修改多个用户的电子邮件通知设置
description: 本文为Workfront或组管理员提供有关如何更新其他用户的电子邮件通知的信息。
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# 修改多个用户的电子邮件通知设置

<!-- Audited: 12/2023 -->

如果您是Adobe Workfront管理员或者您具有允许您编辑其他用户设置的“规划者”访问级别，则可以一次为多个用户配置通知设置。 这包括指定用户是在发生事件时接收通知，还是在一封每日摘要电子邮件中接收通知，如中所述 [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md). 有关编辑用户所需的访问级别的信息，请参阅 [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

您还可以一次为一个用户配置电子邮件通知，包括您自己的配置文件。 有关更多信息，请参阅 [修改您自己的电子邮件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


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
   <td> <p>新计划：标准 </p>
 <p>或</p> 
<p>当前计划：计划 </p> 
</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 修改多个用户的电子邮件通知设置

批量配置通知设置时，只能更改选定用户的共同设置。

修改通知设置时，标签 **已编辑** ，通知您该通知设置已被修改。

要修改多个用户的电子邮件通知设置，请执行以下操作：

{{step-1-to-users}}

1. 选择用户，然后单击 **编辑**.
1. 在 **编辑人员** 框中，单击 **通知**.

1. 展开类别可查看与该类别相关的通知设置。

   如果至少选择一个用户的通知与其他选定用户的通知不匹配，则该通知的类别复选框包含水平线 ![](assets/straight-line-instead-of-checkmark.jpg) 而不是复选标记。


1. 单击您希望用户每天或即时接收的任何通知，或清除您希望用户停止接收的任何通知。

   >[!NOTE]
   >
   >   对于 **通信** 类别中，您可以选择仅用于即时发送的单个通知。 您必须选择所有要在每日摘要中发送的通知。


1. 如果您选择了通知作为每日摘要发送，请在顶部选择一天中您希望摘要发送的时间 **通知** 中的部分 **在以下时间后发送电子邮件每日摘要：** 菜单。

   ![](assets/daily-digest-time.png)

   每日摘要包括在所选时间之前24小时满足通知标准的事件。 用户会收到一封每种通知类型的每日摘要电子邮件。

   每日摘要可能会在您选择的时间之后到达，具体取决于系统中排队等待发送的电子邮件数量。 列出的时间是您在浏览器设置中指定的本地时间。
