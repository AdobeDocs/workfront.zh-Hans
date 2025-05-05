---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: '为Slack配置 [!DNL Adobe Workfront] '
description: 将 [!DNL Adobe Workfront] 与Slack集成允许您从Slack访问和创建 [!DNL Workfront] 工作项、批准、收藏夹、最近项目。
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 配置[!DNL Adobe Workfront for Slack]

将[!DNL Adobe Workfront]与[!DNL Slack]集成允许您执行以下操作：

* 从[!DNL Slack]访问您的[!DNL Workfront]工作项、批准、收藏夹和最近项。
* 从[!DNL Slack]订阅、批准、分配工作。
* 从[!DNL Slack]创建任务和问题。
* 在[!DNL Slack]中接收一些[!DNL Workfront]通知。

您可以自行安装和配置[!DNL Workfront for Slack]，具体取决于[!DNL Slack]环境的配置方式，或者[!DNL Workfront]管理员必须先安装和配置它，然后才能自行配置。

当您将[!DNL Slack]实例与[!DNL Workfront]集成时，用户可以在其[!DNL Slack]渠道中协作时使用[!DNL Workfront]。 可以从任何[!DNL Slack]环境（包括[!DNL Slack]移动应用）使用该集成。

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

## 将[!DNL Workfront]与[!DNL Slack]一起使用的先决条件

* 您必须具有[!DNL Slack]实例。
* 您的[!DNL Slack]系统管理员必须允许所有[!DNL Slack]用户安装[!DNL Workfront for Slack]。
* 您必须拥有[!DNL Workfront]许可证才能使用[!DNL Workfront]中的集成功能。

  >[!NOTE]
  >
  >具有任何[!DNL Workfront]许可证类型的用户可以从[!DNL Slack]访问[!DNL Workfront]。 您可以从[!DNL Slack]执行的操作仅限于[!DNL Workfront]许可证和权限级别。

有关在[!DNL Slack]中管理应用的详细信息，请参阅[为您的Workspace管理应用。](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## 安装[!DNL Workfront for Slack]

每个[!DNL Slack]用户必须自行安装[!DNL Workfront]应用，才能使用来自[!DNL Slack]的[!DNL Workfront]。

您可以通过以下方式安装应用程序：

* [在 [!DNL Slack]外部安装 [!DNL Workfront] 应用程序](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [在 [!DNL Slack]中安装 [!DNL Workfront] 应用程序](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### 在[!DNL Slack]外部安装[!DNL Workfront]应用 {#install-the-workfront-app-outside-slack}

按照以下步骤运行安装过程并授权[!DNL Slack]实例上的[!DNL Workfront for Slack]。

>[!IMPORTANT]
>
>发布Slack的新版本[!DNL Workfront]后，您必须重新授权应用程序才能继续使用它。

1. 在[[!DNL Slack] 存储](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info)中找到[!DNL Adobe Workfront]加载项。

1. 单击&#x200B;**[!UICONTROL 在[!DNL Slack]]**&#x200B;中打开。

1. 通过指定您的[!DNL Slack] URL并单击&#x200B;**[!UICONTROL 继续]**&#x200B;登录到工作区。\

1. 检查[!DNL Slack]请求的访问。 如果您同意此访问权限，请单击&#x200B;**[!UICONTROL 允许访问]**&#x200B;以授权[!DNL Workfront]应用程序。

您现在可以从[!DNL Slack]访问[!DNL Workfront]，如[从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] 访问 [!DNL Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中所述。

### 在[!DNL Slack]中安装[!DNL Workfront]应用 {#install-the-workfront-app-within-slack}

您可以直接从[!DNL Slack]应用程序安装[!DNL Workfront]应用程序：

1. 导航到您的[!DNL Slack] URL。

   例如： *`<YourTeamName>`.slack.com/apps*。

   或

   单击[!DNL Slack]实例中的&#x200B;**[!UICONTROL 添加应用程序]**&#x200B;图标。

1. 开始在搜索字段中键入&#x200B;*[!DNL Workfront]*。
1. 按Enter。
1. 选择&#x200B;**[!DNL Workfront]**&#x200B;应用。
1. 单击&#x200B;**[!UICONTROL 设置]**。

   此时将显示“应用程序目录”页面。

1. 单击&#x200B;**[!UICONTROL 访问应用网站]**。
1. 单击&#x200B;**[!UICONTROL 添加到[!DNL Slack]]**。
1. 按照步骤完成安装。
1. 安装完成后，您可以从[!DNL Slack]访问[!DNL Workfront]，如 [!DNL Slack]&rbrack;[&#128279;](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in Access [!DNL Adobe Workfront] 的&lbrack;[[!UICONTROL 访问 [!DNL Workfront] 中所述。 [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)
