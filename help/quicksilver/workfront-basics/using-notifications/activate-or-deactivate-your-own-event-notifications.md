---
product-area: setup
navigation-topic: notifications
title: 激活或停用您自己的事件通知
description: Adobe Workfront管理员会配置用户在Workfront中发生事件时收到的事件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: ea16b13b6ecb6ecea365c6c4d31ee23b7bb712c6
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# 激活或停用您自己的事件通知

您的Adobe [!DNL Workfront] 管理员可配置用户在Workfront中发生事件时接收的事件通知(如 [[!UICONTROL 配置事件] 系统中每个人的通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md))。

群组管理员还可以配置为您和家庭群组中的用户激活的事件通知。 如果 [!UICONTROL 主页组] 是一个子组，您将收到为群组上方顶级群组激活的事件通知。

您可以通过配置接收的通知来进一步自定义此通知。 您还可以选择是希望在发生事件时接收通知，还是希望在一封每日摘要电子邮件中接收通知。

有关电子邮件通知的信息，请参阅 [[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* 如果激活通知类型，然后发现您未收到该类型的通知，则可能是因为该类型不适用于您的角色。
>* 的 [!DNL Workfront] 管理员或组管理员无法配置通知 [!DNL Workfront Goals]. 有关哪些通知的更多信息，请参阅 [!DNL Workfront] 管理员可以配置，请参阅 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). 有关为配置单个通知的信息 [!DNL Workfront Goals] 继续阅读本文。
>


## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL Work]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划或许可证类型，请联系 [!DNL Workfront] 管理员。

## 查看和修改电子邮件通知设置

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击配置文件图片旁边的用户名。

1. 单击 **[!UICONTROL 更多]** 图标 ![](assets/more-icon.png) ，然后单击 **[!UICONTROL 编辑]**.

1. 在 **[!UICONTROL 编辑人员]** 框中，转到 **[!UICONTROL 通知]** 中。

1. 单击类别可查看与该类别相关的通知设置。

   ![](assets/my-profile-notifications.png)

1. 选中或取消选中右侧的复选框，以指定您是希望每天、即时还是两者都接收通知。

   您还可以使用类别的复选框来激活或停用该类别中的所有通知。

   >[!NOTE]
   >
   >如果您是项目的团队成员，您将继续收到该项目的电子邮件通知，直到您被从团队中移除为止，即使您不再具有项目访问权限。 有关从团队中删除用户的说明，请参阅 [从项目中删除用户](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   对于 **[!UICONTROL 通信]** 类别中，您只能为即时投放选择单个通知。 要在每日摘要中发送通知，必须选择所有通知。

   如果激活了给定类别的所有电子邮件通知，则类别标题中的框将显示为选中状态。 如果给定类别中的所有电子邮件通知都已停用，则取消选中该框。 如果某些通知已激活，而其他通知已停用，则“类别”复选框将显示为直线。\
   修改通知设置时，标签 **[!UICONTROL 已编辑]** 将显示该通知设置，以告知您该通知设置已修改。

1. 如果选择了任何要作为每日摘要发送的通知，请在 **[!UICONTROL 通知]** 部分 **[!UICONTROL 之后的电子邮件每日摘要]** 菜单。

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   每日摘要包括在选定时间之前24小时满足通知标准的事件。 对于每种类型的通知，您每天会收到一封摘要电子邮件。\
   根据系统中排队等待投放的电子邮件数量，每日摘要可能会在您选择的时间之后到达。 列出的时间是您在浏览器设置中指定的本地时间。

1. （视情况而定）在“预览”环境中修改电子邮件通知设置时，请启用 **[!UICONTROL 从此测试环境接收电子邮件]** 设置以接收电子邮件。 电子邮件不会从预览环境自动生成。

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. 单击 **[!UICONTROL 保存更改]**.
