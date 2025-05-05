---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 在 [!DNL Slack]中接收 [!DNL Adobe Workfront] 通知
description: 在 [!DNL Slack]中接收 [!DNL Adobe Workfront] 通知
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---

# 在[!DNL Slack]中接收[!DNL Adobe Workfront]通知

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

安装[!DNL Adobe Workfront for Slack]后，您可以在[!DNL Slack]中接收[!DNL Workfront]通知。\
有关安装[!DNL Workfront for Slack]的信息，请参阅[配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

您可以启用显示在[!DNL Workfront]界面的通知泡泡中的[!UICONTROL 通知]的选定数量，以便在[!DNL Slack]中传送。

电子邮件通知独立于[!DNL Workfront]界面通知工作。 您或您的[!DNL Workfront]管理员可以禁用电子邮件通知，而无法在[!DNL Workfront]中禁用界面通知。\
但是，如果您希望仅关注[!DNL Workfront]界面中的通知，则可以禁用[!DNL Slack]中可能收到的[!DNL Workfront]通知。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront]计划]</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。\

## 先决条件

在[!DNL Slack]中接收[!DNL Workfront]通知之前，您必须

* 配置[!DNL Workfront for Slack]\
   有关配置[!DNL Workfront for Slack]的说明，请参阅[配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 为[!DNL Slack]配置[!DNL Workfront]通知 {#configure-workfront-notifications-for-slack}

1. （视情况而定）将[!DNL Workfront]添加到您的[!DNL Slack]实例后，从[!DNL Slack]登录到[!DNL Workfront]。\
   有关从[!DNL Slack]登录[!DNL Workfront]的信息，请参阅[从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)访问 [!DNL Adobe Workfront] 。

1. 从任何渠道中，开始在消息字段中键入以下命令之一：

   `/workfront settings`

   或

   `/wf settings`

1. 默认启用所有通知。\
   禁用以下任何通知：

   * [!UICONTROL 我已分配到新任务或问题]
   * [!UICONTROL 我的团队已分派至新任务或问题]
   * [!UICONTROL 我收到新的审批或访问请求]
   * [!UICONTROL 有人将我包含在定向更新中]
   * [!UICONTROL 某人备注我所在的线程]
   * [!UICONTROL 我订阅的任务、问题或项目已更新]
   * [!UICONTROL 某人备注我的工作项之一]
   * [!UICONTROL 某人备注我的帮助请求]

   您对[!UICONTROL 通知]选项所做的更改会立即生效。\
   您启用的通知将在[!DNL Workfront] [!DNL Slack]渠道中传递。 当您在此处禁用通知时，仅对[!DNL Slack]禁用通知，而不会对[!DNL Workfront]界面禁用通知。 您将继续在界面右上角的[!DNL Workfront]通知气泡中收到它们。

## 管理来自[!DNL Slack]的[!DNL Workfront]通知

您可以接收和响应来自[!DNL Slack]的[!DNL Workfront]通知。

您可以禁用在[!DNL Slack]中启用的通知的电子邮件通知，以确保不会收到重复的通知。\
有关配置电子邮件通知的信息，请参阅[修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

在[!DNL Slack]中启用或禁用[!DNL Workfront]通知不会影响您在[!DNL Workfront]界面中收到的通知。\
无法禁用[!DNL Workfront]界面中的通知。

要管理[!DNL Slack]的[!DNL Workfront]通知，请执行以下操作：

1. 登录到[!UICONTROL Slack]。
1. 从[!DNL Slack]登录到[!DNL Workfront]。\
   有关从[!DNL Slack]登录到[!DNL Workfront]的信息，请参阅[访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的“从[!DNL Slack]登录到[!DNL Workfront]”部分。

1. 确保已启用[!DNL Slack]的[!DNL Workfront]通知。\
   有关哪些[!DNL Workfront]通知可以配置为也发送到[!DNL Slack]的更多信息，请参阅[为 [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack)配置 [!DNL Workfront] 通知。

1. 转到&#x200B;**[!DNL Workfront]**&#x200B;频道以查找您的[!DNL Workfront]通知。
1. （有条件，可选）执行以下任一操作：

   * 单击&#x200B;**[!UICONTROL 处理它]**&#x200B;接受处理任务。

   * （有条件，可选）单击&#x200B;**[!UICONTROL 在[!DNL Workfront]]**&#x200B;中回复以回复评论，键入您的回复，然后单击&#x200B;**[!UICONTROL 回复]**。

   * （有条件，可选）单击&#x200B;**[!UICONTROL 批准]**&#x200B;或&#x200B;**[!UICONTROL 拒绝]**&#x200B;以批准或拒绝待您批准的任务、问题或项目。

   * （有条件，可选）单击&#x200B;**[!UICONTROL 批准]**、**[!UICONTROL 更改]**&#x200B;或&#x200B;**[!UICONTROL 拒绝]**，以批准、批准更改或拒绝文档。

     您也可以将鼠标悬停在文档的缩览图上，单击放大镜图标以查看文档的较大预览，然后再批准文档。\
      只能预览已批准的Slack [文件类型](https://api.slack.com/types/file)。

   * （有条件且可选）单击&#x200B;**[!UICONTROL 授予]**&#x200B;或&#x200B;**[!UICONTROL 忽略]**&#x200B;以授予或忽略来自其他用户的更多访问权限请求。\

     对于您在通知中作出的每个决定，您都会收到一个确认信息，表明您的操作已在[!DNL Workfront]中完成。
