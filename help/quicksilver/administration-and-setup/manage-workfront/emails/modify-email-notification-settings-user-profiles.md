---
user-type: administrator
product-area: system-administration
keywords: 修改，电子邮件，通知，设置，批量，批量编辑，配置，多个，用户
navigation-topic: emails-administration
title: 修改多个用户的电子邮件通知设置
description: 本文向Workfront或组管理员提供有关如何更新其他用户的电子邮件通知的信息。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 4%

---

# 修改多个用户的电子邮件通知设置

<!-- Audited: 12/2023 -->

如果您是Adobe Workfront管理员，或者您具有允许您编辑其他用户设置的Planner访问级别，则您可以一次为多个用户配置通知设置。 这包括指定用户在事件发生时接收通知，还是在一个每日摘要电子邮件中接收通知，如[Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md)中所述。 有关编辑用户所需的访问级别的信息，请参阅[向用户授予访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

您还可以一次为一个用户配置电子邮件通知，包括您自己的配置文件。 有关详细信息，请参阅[修改您自己的电子邮件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。


## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td>“任一”</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
    <p>标准</p>
    <p>规划</p>
   </td>
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 修改多个用户的电子邮件通知设置

在批量配置通知设置时，您只能更改所选用户的常用设置。

修改通知设置时，该通知设置会显示标签&#x200B;**已编辑**，以通知您已修改该通知设置。

要修改多个用户的电子邮件通知设置：

{{step-1-to-users}}

1. 选择用户，然后单击&#x200B;**编辑**。
1. 在显示的&#x200B;**编辑人员**&#x200B;框中，单击&#x200B;**通知**。

1. 展开类别以查看与该类别相关的通知设置。

   如果至少选择一个用户的通知与其他选定用户的通知不匹配，则该通知的类别复选框包含水平线![行而不是勾号](assets/straight-line-instead-of-checkmark.jpg)，而不是勾号。


1. 单击您希望用户每天或立即接收的任何通知，或清除您希望用户停止接收的任何通知。

   >[!NOTE]
   >
   >   对于&#x200B;**通信**&#x200B;类别，您只能为即时传送选择单个通知。 您必须选择要在每日摘要中发送的所有通知。


1. 如果选择将通知作为每日摘要发送，请在&#x200B;**《电子邮件每日摘要》**&#x200B;菜单之后的&#x200B;**《通知》**&#x200B;部分顶部选择一天中的摘要发送时间。

   ![每日摘要时间](assets/daily-digest-time.png)

   每日摘要包括在所选时间前24小时符合通知标准的事件。 对于每种通知类型，用户都会收到一封每日摘要电子邮件。

   每日摘要可能在您选择的时间之后到达，具体取决于系统中排队等待发送的电子邮件数量。 列出的时间是在浏览器设置中指定的本地时间。
