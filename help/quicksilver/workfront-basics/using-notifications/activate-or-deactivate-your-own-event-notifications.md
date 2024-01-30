---
product-area: setup
navigation-topic: notifications
keywords: 修改，电子邮件，通知，设置
title: 修改您自己的电子邮件通知
description: 本文介绍了如何在用户配置文件中管理电子邮件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# 修改您自己的电子邮件通知

<!-- Audited: 1/2024 -->

您的Adobe [!DNL Workfront] 管理员配置用户在Workfront中发生事件时收到的电子邮件通知（如中所述） [[!UICONTROL 配置事件] 系统中的每个人的通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md))。

您的组管理员还可以配置为您和您的中的用户激活哪些通知 [!UICONTROL 主组]. 如果您的 [!UICONTROL 主组] 是一个子组，您将收到为组上方的顶层组激活的通知。

您可以通过配置接收哪些通知来进一步自定义此设置。 您还可以选择要在事件发生时接收通知，还是要在一封每日摘要电子邮件中接收通知。

有关电子邮件通知的更多信息，请参阅 [[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* 如果您激活了通知类型，然后发现您没有收到该类型的通知，则可能是因为该类型不适用于您的职责。
>* 此 [!DNL Workfront] 管理员或组管理员无法配置通知 [!DNL Workfront Goals]. 有关哪些通知的更多信息， [!DNL Workfront] 管理员可以配置，请参见 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). 有关配置单个通知的信息 [!DNL Workfront Goals] 请继续阅读本文。
>

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证</strong></td> 
   <td>  <p>新增：</p> 
   <ul><li>参与者或更高</li></ul>
   <p>当前：</p>
   <ul><li>请求或更高版本</li></ul>
   </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 查看和修改电子邮件通知设置

{{step1-click-profile-pic}}

1. 单击 **[!UICONTROL 更多]** 图标 ![](assets/more-icon.png) ，然后单击 **[!UICONTROL 编辑]**.

1. 在 **[!UICONTROL 编辑人员]** 框，转到 **[!UICONTROL 通知]** 部分。

1. 单击某个类别可查看与该类别相关的通知设置。

   ![](assets/my-profile-notifications.png)

1. 选中或取消选中右侧的复选框，以指定您希望每天接收还是不接收通知，即时接收通知，或两者都接收。

   您还可以使用类别对应的复选框来激活或停用该类别中的所有通知。

   >[!NOTE]
   >
   >如果您是项目的团队成员，则将继续收到该项目的电子邮件通知，直到您从团队中删除为止，即使您不再具有对该项目的访问权限。 有关从团队中删除用户的说明，请参阅 [从项目中删除用户](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   对于 **[!UICONTROL 通信]** 类别中，您可以选择仅用于即时发送的单个通知。 要在每日摘要中发送通知，您必须选择所有通知。

   如果激活了给定类别的所有电子邮件通知，则类别标题中的框显示为选中状态。 如果给定类别中的所有电子邮件通知都已停用，则该框处于未选中状态。 如果激活了某些通知，而取消激活了其他通知，则类别复选框将以直线显示。\
   修改通知设置时，标签 **[!UICONTROL 已编辑]** ，通知您该通知设置已被修改。

1. 如果您选择了任何要作为每日摘要发送的通知，请在 **[!UICONTROL 通知]** 中的部分 **[!UICONTROL 在以下时间后发送电子邮件每日摘要：]** 菜单。

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   每日摘要包括在所选时间之前24小时满足通知标准的事件。 对于每种类型的通知，您都会收到一封每日摘要电子邮件。\
   每日摘要可能会在您选择的时间之后到达，具体取决于系统中排队等待发送的电子邮件数量。 列出的时间是您在浏览器设置中指定的本地时间。

1. （有条件和可选）在预览环境中修改电子邮件通知设置时，启用 **[!UICONTROL 接收来自此测试环境的电子邮件]** 设置为接收电子邮件。 不会从预览环境自动生成电子邮件。

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. 单击 **[!UICONTROL 保存更改]**.
