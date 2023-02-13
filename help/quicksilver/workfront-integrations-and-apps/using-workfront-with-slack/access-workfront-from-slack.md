---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 访问 [!DNL Adobe Workfront] 从 [!DNL Slack]
description: 集成 [!DNL Adobe Workfront] with [!DNL Slack] 允许您访问 [!DNL Workfront] 从Slack，或在 [!DNL Workfront] 使用斜杠命令。 该集成可从任何 [!DNL Slack] 环境，包括 [!DNL Slack] 移动设备应用程序。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '1075'
ht-degree: 1%

---

# 访问 [!DNL Adobe Workfront] 从 [!DNL Slack]

集成 [!DNL Adobe Workfront] with [!DNL Slack] 允许您访问 [!DNL Workfront] 从 [!DNL Slack]或在中执行某些操作 [!DNL Workfront] 使用斜杠命令。 该集成可从任何 [!DNL Slack] 环境，包括 [!DNL Slack] 移动设备应用程序。

您或您的 [!DNL Slack] 管理员必须安装 [!DNL Workfront] 应用程序 [!DNL Slack] 实例 [!DNL Workfront] 从 [!DNL Slack]. 有关更多信息，请参阅 [配置Adobe Workfront以Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## 关于斜杠命令 {#about-slash-commands}

使用 [!DNL Slack]，则需在消息字段内键入消息。 当您以斜杠开头消息时，该消息将变为命令，其行为与简单消息不同。 命令会告知 [!DNL Slack] 执行操作。

您可以访问 [!DNL Workfront] 实例 [!DNL Slack] 在任意 [!DNL Slack] 渠道。

在中使用斜杠命令时，请记住以下事项 [!DNL Slack] 访问 [!DNL Workfront]:

* 斜线命令区分大小写。
* 的命令 [!DNL Workfront] 无论您在哪个渠道中键入这些内容，都只会显示给您。
* 命令应始终以开头 `/workfront` 或 `/wf`，后跟一个空格和要在中执行的操作的名称 [!DNL Workfront].

   这表示您的命令适用于 [!DNL Workfront] 应用程序。 的命令 [!DNL Workfront] 仅当您已配置 [!DNL Workfront] 应用程序 [!DNL Slack] 实例。

有关可从Slack运行的所有命令的列表，请参阅 [!DNL Workfront]，请参阅 [访问 [!DNL Workfront] 从中的斜杠命令 [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## 登录到 [!DNL Workfront] 从 [!DNL Slack] {#log-in-to-workfront-from-slack}

在Slack的消息字段中键入任意命令时，将要求您登录到 [!DNL Workfront] 第一个。\
有关 [!DNL Workfront] 命令从 [!DNL Slack]，请参阅 [访问 [!DNL Workfront] 从中的斜杠命令 [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) 章节。

登录 [!DNL Workfront] 从 [!DNL Slack]:

1. 登录到 [!DNL Slack] 实例。
1. 在任意通道中，键入以下命令之一：\
   `/workfront log in`

   或

   `/wf log in`

1. 单击 [!DNL Workfront] **[!UICONTROL 登录]** 链接。\
   此时将打开一个新选项卡，其中包含 [!DNL Workfront] 凭据。

1. 按照提示登录 [!DNL Workfront] 使用增强的身份验证、OAuth 2.0或您的安全断言标记语言(SAML)URL。

   >[!NOTE]
   >
   >* 提示您输入的主机时 [!DNL Workfront] 帐户，请使用以下格式键入： *yourCompany&#39;sDomain.my.workfront.com*. 您公司的域通常是您公司的名称。
   >* 增强的身份验证在 [!DNL Workfront] 管理员为此集成启用了此功能。



   的配置页面 [!DNL Workfront] 通知 [!DNL Slack] 打开。

1. （可选）禁用任意 [!DNL Workfront] 您不希望在 [!DNL Slack].

   有关配置的信息 [!DNL Workfront] 设置 [!DNL Slack]，请参阅 [配置设置](#configure-settings-configure-settings) 本文章节

1. 导航回您的 [!DNL Slack] 渠道。

   您已登录到 [!DNL Workfront] 从 [!DNL Slack] 实例。

## 访问 [!DNL Workfront] 从 [!DNL Slack]

* [关于斜杠命令](#about-slash-commands-about-slash-commands)
* [访问 [!DNL Workfront] 从 [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## 访问 [!DNL Workfront] 从中的斜杠命令 [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. 登录到 [!DNL Slack] 实例和登录到 [!DNL Workfront] 从 [!DNL Slack].\
   有关登录的更多信息，请参阅 [!DNL Workfront] 从 [!DNL Slack]，请参阅 [登录到 [!DNL Workfront] 从 [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. 在任意渠道中，开始在消息字段中键入以下命令：

   `/workfront help`

   或

   `/wf help`

1. 从以下命令中选择：

   * `/wf home`

      显示按钮，您可以从中访问任务、问题和批准列表。 单击其中一个按钮，将显示 [!DNL Slack].

      ![](assets/slack-home-buttons-350x80.png)

      有关管理的更多信息 [!DNL Workfront] 工作项 [!DNL Slack]，请参阅 [从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

      包括将在 [!DNL Workfront] 界面。

      将任务添加到 [!DNL Workfront].

      有关将任务添加到的详细信息 [!DNL Workfront] 从Slack中，请参阅“从 [!DNL Slack]“ ”部分 [从创建任务和问题 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

      包括将在 [!DNL Workfront] 界面。

      将问题添加到 [!DNL Workfront]

      有关将问题添加到的更多信息 [!DNL Workfront] 从 [!DNL Slack]，请参阅“从 [!DNL Slack]“ ”部分 [从创建任务和问题 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

      显示 [!DNL Workfront] 收藏。

      有关从以下位置访问收藏夹的更多信息 [!DNL Slack]，请参阅 [访问您的 [!UICONTROL 收藏夹] 列表来源 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) 部分 [从访问您的收藏夹和最近的项目 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) 文章。

   * `/wf recent`

      显示您最近在 [!DNL Workfront].

      有关从 [!DNL Slack]，请参阅 [访问您的 [!UICONTROL 最近项目] 列表来源 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] 和 [!UICONTROL 最近的项目 [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) 文章。

   * `wf tasks`

      显示任务列表。

      有关从 [!DNL Slack]，请参阅“从 [!DNL Slack]“ ”部分 [从管理您的工作和批准 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

      显示问题列表。

      有关从 [!DNL Slack]，请参阅“管理您的问题” [!DNL Slack]“ ”部分 [从管理您的工作和批准 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` 显示 [!DNL Workfront] 批准。\

      有关从 [!DNL Slack]，请参阅“从 [!DNL Slack]“ ”部分 [从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

      包括关键词。

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
      * 注释  \

         有关在中搜索的详细信息 [!DNL Slack]，请参阅 [搜索 [!DNL Adobe Workfront] 项目自Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

      将您登录到 [!DNL Workfront] 从 [!DNL Slack].

   * `/wf log out `

      将您从 [!DNL Workfront] 从 [!DNL Slack]. 您仍然登录到 [!DNL Workfront] 如果您有 [!DNL Workfront] 在另一个应用程序的另一个浏览器选项卡中打开实例。
   * `/wf settings`

      允许您配置 [!DNL Workfront] 设置 [!DNL Slack].

      有关配置的信息 [!DNL Workfront] 设置，请参阅 [配置设置](#configure-settings-configure-settings).

   * `/wf help`
显示 [!DNL Workfront].


   * `Visit Workfront Help`:打开 [!UICONTROL Slack] 部分 [!DNL Workfront] 帮助网站。


1. （可选）要删除任何命令的消息，请将鼠标悬停在包含该命令的Slack消息的右上角，然后单&#x200B;击&#x200B;**[!UICONTROL 显示消息操作]**，然后单击 **[!UICONTROL 删除消息]**.

1. （可选和视情况而定）单击 **[!UICONTROL 删除]** 确认您要删除此消息。

### 访问 [!DNL Workfront] 从 [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

您可以访问 [!DNL Workfront] 对象从链接到与您共享的对象 [!DNL Slack].

有关访问的更多信息 [!DNL Workfront] 从共享链接，请参阅 [访问 [!DNL Adobe Workfront] 对象来自 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## 配置设置 {#configure-settings}

1. 内部 [!DNL Slack] 消息字段中，键入以下命令：

   `/workfront settings`

   或

   `/wf settings`

   ![](assets/slack-configuring-settings-350x302.png)

   默认情况下，所有设置都处于启用状态。

1. 从以下选项中取消选择，以禁用Workfront设置：

   * 在 **[!UICONTROL 常规设置]** 区域，禁用 **[!UICONTROL 粘贴 [!DNL Workfront] 中的URL [!DNL Slack] 渠道、显示其他描述、截止日期或请求者名称]**&#x200B;设置 [!DNL Slack] 添加有关 [!DNL Workfront] 对象 [!UICONTROL Slack].

   * 在 **[!UICONTROL 通知设置]** 区域，禁用要停止从Workfront接收的通知。\

      有关接收的信息 [!DNL Workfront] 通知 [!DNL Slack]，请参阅 [接收 [!DNL Adobe Workfront] 通知 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## 注销 [!DNL Workfront] 从 [!DNL Slack]

1. 内部 [!DNL Slack] 消息字段中，键入以下命令：\
   `/workfront log out` 或\
   `/wf log out`\
   您会收到一条确认消息，表明您已注销 [!DNL Workfront].\
   您仍然登录到 [!DNL Workfront] 如果您有 [!DNL Workfront] 在另一个应用程序的另一个浏览器选项卡中打开实例。
