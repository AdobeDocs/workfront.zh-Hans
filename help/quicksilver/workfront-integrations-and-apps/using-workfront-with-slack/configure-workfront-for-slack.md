---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: 配置 [!DNL Adobe Workfront] Slack
description: 集成 [!DNL Adobe Workfront] 通过Slack，您可以访问和创建 [!DNL Workfront] 工作项、批准、收藏、来自Slack的最近项。
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# 配置 [!DNL Adobe Workfront for Slack]

集成 [!DNL Adobe Workfront] with [!DNL Slack] 允许您执行以下操作：

* 访问 [!DNL Workfront] 工作项、批准、收藏夹、最近的项目 [!DNL Slack].
* 订阅、批准、分配工作来源 [!DNL Slack].
* 从创建任务和问题 [!DNL Slack].
* 接收一些 [!DNL Workfront] 通知 [!DNL Slack].

根据 [!DNL Slack] 环境配置后，您可以安装和配置 [!DNL Workfront for Slack] 你自己或你 [!DNL Workfront] 管理员必须先安装和配置它，然后您才能自行配置它。

集成 [!DNL Slack] 实例 [!DNL Workfront] 用户可以使用 [!DNL Workfront] 在 [!DNL Slack] 渠道。 该集成可从任何 [!DNL Slack] 环境，包括 [!DNL Slack] 移动设备应用程序。

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

## 使用的先决条件 [!DNL Workfront] with [!DNL Slack]

* 您必须具有 [!DNL Slack] 实例。
* 您的 [!DNL Slack] 系统管理员必须允许所有 [!DNL Slack] 安装用户 [!DNL Workfront for Slack].
* 您必须具有 [!DNL Workfront] 许可证，以便能够在 [!DNL Workfront].

   >[!NOTE]
   >
   >具有任何 [!DNL Workfront] 许可证类型可访问 [!DNL Workfront] 从 [!DNL Slack]. 可从中执行的操作 [!DNL Slack] 仅限于 [!DNL Workfront] 许可和许可级别。

有关在 [!DNL Slack]，请参阅 [管理工作区的应用程序。](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## 安装 [!DNL Workfront for Slack]

每个 [!DNL Slack] 用户必须安装 [!DNL Workfront] 应用程序本身，以便使用 [!DNL Workfront] 从 [!DNL Slack].

您可以通过以下方式安装应用程序：

* [安装 [!DNL Workfront] 应用程序外部 [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [安装 [!DNL Workfront] 应用程序 [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### 安装 [!DNL Workfront] 应用程序外部 [!DNL Slack] {#install-the-workfront-app-outside-slack}

按照以下步骤运行安装过程并进行授权 [!DNL Workfront for Slack] 在 [!DNL Slack] 实例。

>[!IMPORTANT]
>
>当的 [!DNL Workfront] 如果Slack已发布，您必须重新授权应用程序才能继续使用。

1. 找到 [!DNL Adobe Workfront] 中的附加组件 [[!DNL Slack] 商店](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. 单击 **[!UICONTROL 在中打开[!DNL Slack]]**.

1. 通过指定 [!DNL Slack] URL和单击 **[!UICONTROL 继续]**.\

1. 检查 [!DNL Slack] 正在请求。 如果您同意此访问，请单击 **[!UICONTROL 允许访问]** 授权 [!DNL Workfront] 应用程序。

您现在可以访问 [!DNL Workfront] 从 [!DNL Slack]，如 [访问 [!DNL Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### 安装 [!DNL Workfront] 应用程序 [!DNL Slack] {#install-the-workfront-app-within-slack}

您可以安装 [!DNL Workfront] 应用程序 [!DNL Slack] 应用程序：

1. 导航到 [!DNL Slack] URL。

   例如： *`<YourTeamName>`.slack.com/apps*.

   或

   单击 **[!UICONTROL 添加应用程序]** 图标 [!DNL Slack] 实例。

1. 开始键入 *[!DNL Workfront]* 中。
1. 按Enter。
1. 选择 **[!DNL Workfront]** 应用程序。
1. 单击 **[!UICONTROL 设置]**.

   将显示“应用程序目录”页面。

1. 单击 **[!UICONTROL 访问应用程序网站]**.
1. 单击 **[!UICONTROL 添加到[!DNL Slack]]**.
1. 按照步骤完成安装。
1. 安装完成后，您可以访问 [!DNL Workfront] 从 [!DNL Slack]，如 [[!UICONTROL访问 [!DNL Workfront] 从 [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
