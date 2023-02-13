---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 接收 [!DNL Adobe Workfront] 通知 [!DNL Slack]
description: 接收 [!DNL Adobe Workfront] 通知 [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 6%

---

# 接收 [!DNL Adobe Workfront] 通知 [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

安装后 [!DNL Adobe Workfront for Slack]，您可以 [!DNL Workfront] 通知 [!DNL Slack].\
有关安装的信息 [!DNL Workfront for Slack]，请参阅 [配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

您可以启用选定数量 [!UICONTROL 通知] 在 [!DNL Workfront] 界面，也将在 [!DNL Slack].

电子邮件通知独立于 [!DNL Workfront] 界面通知。 您或您的 [!DNL Workfront] 管理员可以禁用电子邮件通知，但无法在 [!DNL Workfront].\
但是，您可以禁用 [!DNL Workfront] 您可能会在 [!DNL Slack]，则您只想在 [!DNL Workfront] 界面。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] 计划]</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员\

## 先决条件

在收到 [!DNL Workfront] 通知 [!DNL Slack]，您必须

* 配置 [!DNL Workfront for Slack]\
   有关配置的说明 [!DNL Workfront for Slack]，请参阅 [配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## 配置 [!DNL Workfront] 通知 [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. （视情况而定）之后 [!DNL Workfront] 已添加到 [!DNL Slack] 实例，登录 [!DNL Workfront] 从 [!DNL Slack].\
   有关登录的信息 [!DNL Workfront] 从 [!DNL Slack]，请参阅 [访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 在任意渠道中，开始在消息字段中键入以下命令之一：

   `/workfront settings`

   或

   `/wf settings`

   <img src="assets/slack-configuring-settings-350x302.png" style="width: 350;height: 302;">

1. 默认情况下，所有通知都处于启用状态。\
   禁用以下任何通知：

   * [!UICONTROL 我被指派执行新任务或问题]
   * [!UICONTROL 我的团队已分配给新任务或问题]
   * [!UICONTROL 我收到新的批准或访问请求]
   * [!UICONTROL 有人将我列入定向更新]
   * [!UICONTROL 当某人备注跟帖，向备注该跟帖的每个人发送电子邮件]
   * [!UICONTROL 我订阅的任务、问题或项目已更新]
   * [!UICONTROL 某人备注我的工作项之一]
   * [!UICONTROL 有人对我的帮助请求发表评论]

   您对 [!UICONTROL 通知] 选项将立即生效。\
   您已启用的通知将在 [!DNL Workfront] [!DNL Slack] 渠道。 在此处禁用通知时，只对 [!DNL Slack]，而不是 [!DNL Workfront] 界面。 您将继续在 [!DNL Workfront] 通知会在界面的右上角冒泡。

## 管理 [!DNL Workfront] 通知来自 [!DNL Slack]

您可以接收并响应 [!DNL Workfront] 通知来自 [!DNL Slack].

您可以对中启用的通知禁用电子邮件通知 [!DNL Slack]，以确保不会收到重复的通知。\
有关配置电子邮件通知的信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

启用或禁用 [!DNL Workfront] 通知 [!DNL Slack] 不会影响您在 [!DNL Workfront] 界面。\
通知位于 [!DNL Workfront] 无法禁用接口。

管理 [!DNL Workfront] 通知 [!DNL Slack]:

1. 登录到 [!UICONTROL Slack].
1. 登录到 [!DNL Workfront] 从 [!DNL Slack].\
   有关登录到的信息 [!DNL Workfront] 从 [!DNL Slack]，请参阅“登录到” [!DNL Workfront] 从 [!DNL Slack]“ ”部分 [访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 确保 [!DNL Workfront] 通知 [!DNL Slack] 启用。\
   有关 [!DNL Workfront] 通知可配置为也发送到 [!DNL Slack]，请参阅 [配置 [!DNL Workfront] 通知 [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. 转到 **[!DNL Workfront]** 渠道查找 [!DNL Workfront] 通知。
1. （视情况而定）执行以下任一操作：

   * 单击 **[!UICONTROL 处理它]** 接受处理任务。

      <!--   
     <img src="assets/slack-assigned-to-a-task-notification-350x198.png" alt="slack_assigned_to_a_task_notification.png" style="width: 350;height: 198;" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * （视情况而定）单击 **[!UICONTROL 回复[!DNL Workfront]]** 要回复评论，请键入您的回复，然后单击 **[!UICONTROL 回复]**.\

      ![slack_tagged_in_a_comment_notification.png](assets/slack-tagged-in-a-comment-notification.png)

   * （视情况而定）单击 **[!UICONTROL 批准]** 或 **[!UICONTROL 拒绝]** 批准或拒绝等待您批准的任务、问题或项目。\

      ![slack_approve_task_notification.png](assets/slack-approve-task-notification-350x105.png)

   * （视情况而定）单击 **[!UICONTROL 批准]**, **[!UICONTROL 更改]**&#x200B;或 **[!UICONTROL 拒绝]**、批准、批准更改或拒绝文档。

      ![slack_approve_a_document.png](assets/slack-approve-a-document-350x362.png)\
      在批准文档之前，您还可以将鼠标悬停在文档的缩略图上，然后单击放大镜图标以查看文档的更大预览。\
      仅批准的Slack [文件类型](https://api.slack.com/types/file) 可以预览。

   * （视情况而定）单击 **[!UICONTROL 授予]** 或 **[!UICONTROL 忽略]** 来授予或忽略其他用户的更多访问权限请求。

      ![](assets/slack-access-approvals-list-350x213.png)\
      您会收到一则确认消息，确认您的操作已在 [!DNL Workfront]，以获取您在通知中做出的每项决策。
