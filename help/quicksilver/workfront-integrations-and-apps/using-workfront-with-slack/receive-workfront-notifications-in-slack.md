---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 接收 [!DNL Adobe Workfront] 中的通知 [!DNL Slack]
description: 接收 [!DNL Adobe Workfront] 中的通知 [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 6%

---

# 接收 [!DNL Adobe Workfront] 中的通知 [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

安装之后 [!DNL Adobe Workfront for Slack]，您可以 [!DNL Workfront] 中的通知 [!DNL Slack].\
有关安装的信息 [!DNL Workfront for Slack]，请参见 [配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

您可以启用选择的数量 [!UICONTROL 通知] 中通知气泡中显示的区域 [!DNL Workfront] 界面，也将在以下位置提供： [!DNL Slack].

电子邮件通知独立于以下各项工作 [!DNL Workfront] 界面通知。 您或您的 [!DNL Workfront] 管理员可以禁用电子邮件通知，而界面通知不能在中禁用 [!DNL Workfront].\
但是，您可以禁用 [!DNL Workfront] 您可能会收到的通知 [!DNL Slack]，如果您希望仅关注 [!DNL Workfront] 界面。

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
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。\

## 先决条件

在接收之前 [!DNL Workfront] 中的通知 [!DNL Slack]，您必须

* 配置 [!DNL Workfront for Slack]\
   有关配置的说明 [!DNL Workfront for Slack]，请参见 [配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## 配置 [!DNL Workfront] 通知 [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. （视情况而定）晚于 [!DNL Workfront] 已添加到您的 [!DNL Slack] 实例，登录 [!DNL Workfront] 从 [!DNL Slack].\
   有关登录的信息 [!DNL Workfront] 从 [!DNL Slack]，请参见 [访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 从任何渠道中，开始在消息字段中键入以下命令之一：

   `/workfront settings`

   或

   `/wf settings`

1. 默认启用所有通知。\
   禁用以下任何通知：

   * [!UICONTROL 我已分配到新任务或问题]
   * [!UICONTROL 我的团队已分派到一个新任务或问题]
   * [!UICONTROL 我收到新的审批或访问请求]
   * [!UICONTROL 有人将我列入定向更新]
   * [!UICONTROL 有人评论了我所在的主题]
   * [!UICONTROL 我订阅的任务、问题或项目已更新]
   * [!UICONTROL 有人评论了我的工作项之一]
   * [!UICONTROL 某人备注我的帮助请求]

   您对 [!UICONTROL 通知] 选项立即生效。\
   您启用的通知将在 [!DNL Workfront] [!DNL Slack] 渠道。 当您在此处禁用通知时，仅对禁用通知 [!DNL Slack]，而不是对于 [!DNL Workfront] 界面。 您可继续在 [!DNL Workfront] 界面右上角的“通知”气泡。

## 管理 [!DNL Workfront] 通知来源 [!DNL Slack]

您可以接收和响应 [!DNL Workfront] 通知来源 [!DNL Slack].

您可以在中启用的通知禁用电子邮件通知 [!DNL Slack]，以确保您不会收到重复的通知。\
有关配置电子邮件通知的信息，请参阅 [修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

启用或禁用 [!DNL Workfront] 中的通知 [!DNL Slack] 不会影响您在内收到的通知 [!DNL Workfront] 界面。\
中的通知 [!DNL Workfront] 无法禁用接口。

管理您的 [!DNL Workfront] 通知 [!DNL Slack]：

1. 登录 [!UICONTROL Slack].
1. 登录 [!DNL Workfront] 从 [!DNL Slack].\
   有关登录的信息 [!DNL Workfront] 从 [!DNL Slack]，请参阅 [!DNL Workfront] 从 [!DNL Slack]中的“ ”部分 [访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 确保 [!DNL Workfront] 通知 [!DNL Slack] 已启用。\
   有关哪项的详细信息 [!DNL Workfront] 通知可以配置为也发送到 [!DNL Slack]，请参见 [配置 [!DNL Workfront] 通知 [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. 转到 **[!DNL Workfront]** 渠道查找您的 [!DNL Workfront] 通知。
1. （有条件，可选）执行以下任一操作：

   * 单击 **[!UICONTROL 处理它]** 接受以处理任务。

   * （视情况而定，可选）单击 **[!UICONTROL 回复[!DNL Workfront]]** 要回复评论，请键入您的回复，然后单击 **[!UICONTROL 回复]**.

   * （视情况而定，可选）单击 **[!UICONTROL 批准]** 或 **[!UICONTROL 拒绝]** 批准或拒绝待您审批的任务、问题或项目。

   * （视情况而定，可选）单击 **[!UICONTROL 批准]**， **[!UICONTROL 更改]**，或 **[!UICONTROL 拒绝]**，以批准、批准并更改，或拒绝文档。

     您也可以将鼠标悬停在文档的缩览图上，单击放大镜图标以查看文档的较大预览，然后再批准文档。\
      仅限已批准的Slack [文件类型](https://api.slack.com/types/file) 可以预览。

   * （视情况而定，可选）单击 **[!UICONTROL 授权]** 或 **[!UICONTROL 忽略]** 以授予或忽略来自其他用户对更多访问权限的请求。\

     您会收到一个确认消息，确认您的操作已完成 [!DNL Workfront]，适用于您在通知中做出的每个决定。
