---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 从 [!DNL Slack]访问 [!DNL Adobe Workfront]
description: 将 [!DNL Adobe Workfront] 与 [!DNL Slack] 集成允许您从Slack访问 [!DNL Workfront] ，或使用斜杠命令在 [!DNL Workfront] 中执行某些操作。 可以从任何 [!DNL Slack] 环境（包括 [!DNL Slack] 移动应用程序）使用该集成。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 1%

---

# 从[!DNL Slack]访问[!DNL Adobe Workfront]

将[!DNL Adobe Workfront]与[!DNL Slack]集成允许您从[!DNL Slack]访问[!DNL Workfront]，或使用斜杠命令在[!DNL Workfront]中执行某些操作。 可以从任何[!DNL Slack]环境（包括[!DNL Slack]移动应用）使用该集成。

您或您的[!DNL Slack]管理员必须在您的[!DNL Slack]实例中安装[!DNL Workfront]应用，然后才能从[!DNL Slack]使用[!DNL Workfront]。 有关详细信息，请参阅[为Slack配置Adobe Workfront](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 关于斜杠命令 {#about-slash-commands}

使用[!DNL Slack]时，在消息字段中键入消息。 当以斜杠启动消息时，它会变成一个命令，其行为与简单消息不同。 该命令告知[!DNL Slack]执行操作。

您可以通过在任何[!DNL Slack]通道中键入斜杠命令从[!DNL Slack]访问[!DNL Workfront]实例。

在[!DNL Slack]中使用斜杠命令访问[!DNL Workfront]时，请记住以下事项：

* 斜杠命令区分大小写。
* [!DNL Workfront]的命令只对您可见，无论您输入的是哪个渠道。
* 该命令应始终以`/workfront`或`/wf`开头，后跟一个空格和要在[!DNL Workfront]中执行的操作的名称。

  这表示您的命令适用于[!DNL Workfront]应用程序。 只有当您已使用[!DNL Slack]实例配置了[!DNL Workfront]应用时，[!DNL Workfront]的命令才有效。

有关可从[!DNL Workfront]的Slack运行的所有命令的列表，请参阅 [!DNL Slack][&#128279;](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack)中的Access [!DNL Workfront] slash命令。

## 从[!DNL Slack]登录到[!DNL Workfront] {#log-in-to-workfront-from-slack}

当您在Slack的消息字段中键入任何命令时，将要求您先登录[!DNL Workfront]。\
有关来自[!DNL Slack]的[!DNL Workfront]命令的完整列表，请参阅本文中 [!DNL Slack][&#128279;](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack)部分的Access [!DNL Workfront] from a slash命令。

要从[!DNL Slack]登录到[!DNL Workfront]，请执行以下操作：

1. 登录到您的[!DNL Slack]实例。
1. 在任意通道中，键入以下命令之一：\
   `/workfront log in`

   或

   `/wf log in`

1. 单击响应中显示的[!DNL Workfront] **[!UICONTROL 登录]**&#x200B;链接。\
   将打开一个新选项卡，其中包含[!DNL Workfront]凭据的字段。

1. 按照提示使用增强型身份验证、OAuth 2.0或您的安全断言标记语言(SAML) URL登录[!DNL Workfront]。

   >[!NOTE]
   >
   >* 当提示您输入[!DNL Workfront]帐户的主机时，请使用此格式键入该主机： *您的公司&#39;sDomain.my.workfront.com*。 您公司的域通常是您公司的名称。
   >* 在[!DNL Workfront]管理员为此集成启用增强身份验证之前，该身份验证不可用。


   [!DNL Slack]中[!DNL Workfront]通知的配置页面打开。

1. （可选）禁用您不希望在[!DNL Slack]中接收的任何[!DNL Workfront]通知。

   有关为[!DNL Slack]配置[!DNL Workfront]设置的信息，请参阅本文中的[配置设置](#configure-settings-configure-settings)部分

1. 导航回您的[!DNL Slack]频道。

   您从[!DNL Slack]实例登录到[!DNL Workfront]。

## 从[!DNL Slack]访问[!DNL Workfront]

* [关于斜杠命令](#about-slash-commands-about-slash-commands)
* [从 [!DNL Slack]中的共享链接访问 [!DNL Workfront] ](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## 从[!DNL Slack]中的斜杠命令访问[!DNL Workfront] {#access-workfront-from-a-slash-command-in-slack}

1. 从[!DNL Slack]登录到[!DNL Slack]实例并登录到[!DNL Workfront]。\
   有关从[!DNL Slack]登录到[!DNL Workfront]的详细信息，请参阅[从 [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)登录到 [!DNL Workfront] 

1. 从任何渠道中，开始在消息字段中键入以下命令：

   `/workfront help`

   或

   `/wf help`

1. 从以下命令中选择：

   * `/wf home`

     显示按钮，从中可访问任务、问题和审批的列表。 单击其中一个按钮将显示[!DNL Slack]中每个列表的前20项。

     有关从[!DNL Slack]管理[!DNL Workfront]工作项的更多信息，请参阅[从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md)管理您的工作和批准。

   * `/wf add task <TaskName>`

     包括任务在[!DNL Workfront]界面中显示的名称。

     向[!DNL Workfront]添加任务。

     有关从Slack将任务添加到[!DNL Workfront]的更多信息，请参阅[从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md)创建任务和问题中的“从[!DNL Slack]创建任务”部分。

   * `/wf add issue <Issue Name>`

     包括问题名称，该名称将显示在[!DNL Workfront]界面中。

     向[!DNL Workfront]添加问题

     有关从[!DNL Slack]向[!DNL Workfront]添加问题的更多信息，请参阅[从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md)创建任务和问题[!DNL Slack]中的“创建问题”部分。

   * `/wf favorites`

     显示[!DNL Workfront]收藏夹列表。

     有关从[!DNL Slack]访问收藏夹的详细信息，请参阅[从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md)访问收藏夹和最新项目一文中的[从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites)访问您的[!UICONTROL 收藏夹]列表。

   * `/wf recent`

     显示[!DNL Workfront]中最近访问项目的列表。

     有关从[!DNL Slack]访问您最近项目的详细信息，请参阅[从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] 访问您的[!UICONTROL 最近项目]列表和从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md)访问最近项目。

   * `wf tasks`

     显示任务列表。

     有关从[!DNL Slack]管理任务的更多信息，请参阅[从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md)管理您的工作和审批中的“从[!DNL Slack]管理您的任务”部分。

   * `/wf issues`

     显示问题列表。

     有关从[!DNL Slack]管理您的问题的更多信息，请参阅[从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md)管理您的工作和审批中的“从[!DNL Slack]管理您的问题”部分。

   * `/wf approvals`显示您的[!DNL Workfront]审批。\

     有关从[!DNL Slack]管理您的审批的更多信息，请参阅[从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md)管理您的工作和审批中的“从[!DNL Slack]管理您的审批”部分。

   * `/wf search <keyword>`

     Include关键字。

     搜索特定关键词。 您可以搜索以下类型的对象：

      * 项目
      * 任务
      * 问题
      * 报告
      * 人员
      * 模板
      * 文档
      * 项目组合
      * 项目群
      * 仪表板
      * 公司
      * 注释\

        有关在[!DNL Slack]中搜索的详细信息，请参阅[从Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md)中搜索 [!DNL Adobe Workfront] 项。
   * `/wf log in`

     将您从[!DNL Slack]登录到[!DNL Workfront]。

   * `/wf log out `

     将您从[!DNL Slack]注销[!DNL Workfront]。 如果您在另一个应用程序的另一个浏览器选项卡中打开了单独的[!DNL Workfront]实例，则您仍会登录到[!DNL Workfront]。
   * `/wf settings`

     授予您在[!DNL Slack]中配置[!DNL Workfront]设置的权限。

     有关在Slack中配置[!DNL Workfront]设置的信息，请参阅[配置设置](#configure-settings-configure-settings)。

   * `/wf help`
显示[!DNL Workfront]的完整命令列表。


   * `Visit Workfront Help`：在新的Slack标签页中打开[!DNL Workfront]帮助网站上的[!UICONTROL 浏览器标签]部分。


1. （可选）要删除任何命令的消息，请将鼠标悬停在包含该命令的Slack消息的右上角，单击&#x200B;**[!UICONTROL 显示消息操作]**，然后单击&#x200B;**[!UICONTROL 删除消息]**。

1. （可选且有条件）单击&#x200B;**[!UICONTROL 删除]**&#x200B;以确认要删除此消息。

### 从[!DNL Slack]中的共享链接访问[!DNL Workfront] {#access-workfront-from-a-shared-link-in-slack}

您可以通过链接访问[!DNL Workfront]对象，这些链接指向在[!DNL Slack]中与您共享的对象。

有关从共享链接访问[!DNL Workfront]的详细信息，请参阅 [!DNL Slack][&#128279;](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md)中的从共享链接访问 [!DNL Adobe Workfront] 对象。

## 配置设置 {#configure-settings}

1. 在[!DNL Slack]消息字段中键入以下命令：

   `/workfront settings`

   或

   `/wf settings`

   默认启用所有设置。

1. 从以下选项中取消选择，以禁用Workfront设置：

   * 在&#x200B;**[!UICONTROL 常规设置]**&#x200B;区域中，禁用&#x200B;**[!UICONTROL 在[!DNL Slack]渠道中粘贴[!DNL Workfront] URL时，显示其他描述、截止日期或请求者姓名]**&#x200B;设置(如果您不希望[!DNL Slack]在共享[!UICONTROL Slack]中对象的URL时添加有关[!DNL Workfront]对象的其他信息)。

   * 在&#x200B;**[!UICONTROL 通知设置]**&#x200B;区域，禁用要停止从Workfront接收的通知。\

     有关在[!DNL Slack]中接收[!DNL Workfront]通知的信息，请参阅 [!DNL Slack][&#128279;](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md)中的接收 [!DNL Adobe Workfront] 通知。

## 从[!DNL Slack]注销[!DNL Workfront]

1. 在[!DNL Slack]消息字段中键入以下命令：\
   `/workfront log out`或\
   `/wf log out`\
   您会收到一个确认信息，表明您已从[!DNL Workfront]中注销。\
   如果您在另一个应用程序的另一个浏览器选项卡中打开了单独的[!DNL Workfront]实例，则您仍会登录到[!DNL Workfront]。
