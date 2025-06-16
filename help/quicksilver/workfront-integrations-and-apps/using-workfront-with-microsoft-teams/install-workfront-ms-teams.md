---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-microsoft-teams
title: '为Microsoft Teams安装 [!DNL Adobe Workfront] '
description: ' [!DNL Adobe Workfront for Microsoft Teams] 应用允许您在不离开 [!DNL Microsoft Teams] 聊天频道的情况下在 [!DNL Workfront] 中执行基本操作。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: a8d4e48c-1ccc-4e6e-a0a0-9b68748590c0
source-git-commit: 940cbfb34f12eacd5ba698f60fb7a3e67eb62b22
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---

# 为Microsoft Teams安装[!DNL Adobe Workfront]

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>由于[Microsoft将过渡到“新团队”客户端](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability)，因此Classic Teams客户端在2025年7月1日后将不再可用。 要继续使用Microsoft Teams和Workfront等集成应用程序，客户必须在此日期之前过渡到新团队客户端。
>
>更新的Workfront集成现已可用，并与新团队体验完全兼容。 在大多数情况下，用户完成过渡后，Workfront会自动显示。 如果不包含，则可以从Microsoft Teams App Store手动安装集成。


[!DNL Adobe Workfront for Microsoft Teams]应用允许您在不离开[!DNL Microsoft Teams]聊天渠道的情况下在[!DNL Workfront]中执行基本操作。

>[!NOTE]
>
>[!DNL Microsoft Teams]不再支持[!DNL Internet Explorer]。 要使用[!DNL Adobe Workfront for Microsoft Teams integration]，您必须使用[!DNL Internet Explorer]以外的Web浏览器。


## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td><p>新增：标准</p>
    <p>当前： [!UICONTROL 工作]，[!UICONTROL 计划]</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

您必须是[!DNL Microsoft Teams]中的团队所有者才能为[!DNL Microsoft Teams]安装[!DNL Workfront]。

## 安装[!DNL Workfront for Microsoft Teams]

作为[!DNL Microsoft Teams]中的团队所有者，您可以通过[!DNL Microsoft]应用商店或[!DNL Workfront]提供的文件为每个团队安装[!DNL Workfront for Microsoft Teams]应用程序。

### 从[!DNL Microsoft]存储区安装[!DNL Workfront for Microsoft Teams]

1. 以团队所有者的身份登录到[!DNL Microsoft Teams]。
1. 选择要为其安装[!DNL Workfront for Microsoft Teams]应用程序的团队。
1. 对于要为其安装Workfront for Microsoft Teams集成的团队，单击&#x200B;**[!UICONTROL 更多]**&#x200B;图标
1. 单击&#x200B;**[!UICONTROL 应用]**&#x200B;选项卡。
1. 在&#x200B;**[!UICONTROL 搜索应用及更多]**&#x200B;框中，键入&#x200B;*[!DNL Workfront]*。
1. 单击&#x200B;**添加**。
1. 在打开的对话框中单击&#x200B;**添加**。
1. 在选择渠道部分中，选择要将Workfront应用程序添加到的团队，然后单击&#x200B;**转到**。

   ![选择团队](assets/select-a-team.png)
1. 单击&#x200B;**登录** Workfront以访问适用于Microsoft Teams的Workfront。

   有关登录到[!DNL Workfront]的信息，请参阅本文中的[从Microsoft Teams登录到Workfront](#log-in-to-workfront-from-microsoft-teams)部分。

### 从专用文件安装[!DNL Workfront for Microsoft Teams]

如果您的组织限制了对从[!DNL Microsoft]应用商店下载应用的访问，则必须联系我们的支持团队并请求[!DNL Workfront for Microsoft Teams]应用的专用文件以安装应用。

有关联系我们的支持团队的信息，请参阅[联系客户支持](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。

要从专用文件安装[!DNL Workfront for Microsoft Teams]，请执行以下操作：

1. 在计算机上保存您从[!DNL Workfront]收到的专用文件。
1. 以[!DNL Microsoft]团队所有者的身份登录到[!DNL Microsoft Teams]。
1. 单击要为其安装[!DNL Workfront for Microsoft Teams]的团队的&#x200B;**[!UICONTROL 更多]**&#x200B;图标。

1. 单击&#x200B;**[!UICONTROL 管理团队]**。
1. 选择应用程序选项卡，然后单击屏幕左上角的上传应用程序。
1. 浏览您保存在计算机上的专用文件，然后按照安装步骤安装[!DNL Workfront for Microsoft Teams]。
1. 安装完成后，您选择的团队的“常规”渠道中会显示安装成功的通知。 团队的所有成员都可以看到此通知。

## 从[!DNL Microsoft]团队登录到[!DNL Workfront]

作为[!DNL Microsoft Teams]团队所有者，您必须先为团队安装[!DNL Workfront for Microsoft Teams]应用，您或团队中的任何人都可以登录[!DNL Workfront from Microsoft Teams]。

当您从[!DNL Microsoft Teams]登录到[!DNL Workfront]时，您可以在[!DNL Workfront]机器人频道中接收[!DNL Workfront]通知，或者您可以从[!DNL Microsoft Teams]在[!DNL Workfront]中执行某些操作。

有关安装[!DNL Workfront]应用的信息，请参阅本文中的[安装 [!DNL Workfront for Microsoft Teams]](#install-workfront-for-microsoft-teams)部分。

有关从[!DNL Microsoft Teams]访问[!DNL Workfront]以执行某些操作的信息，请参阅[从 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/access-workfront-from-ms-teams.md)访问 [!DNL Adobe Workfront] 。

要从[!DNL Microsoft Teams]登录到[!DNL Workfront]，请执行以下操作：

1. 转到已安装[!DNL Workfront for Microsoft Teams]应用程序的团队的&#x200B;**[!UICONTROL 常规]**&#x200B;渠道，然后单击&#x200B;**[!UICONTROL 登录到Workfront]**。

   [!DNL Workfront]机器人聊天频道已添加到您的[!DNL Microsoft Teams]聊天频道。

1. 转到[!DNL Microsoft Teams]中的[!DNL Workfront]机器人聊天频道，然后在&#x200B;**[!UICONTROL 中键入&#x200B;*[!UICONTROL 登录]*在此处键入您的问题]**&#x200B;或&#x200B;**键入消息**&#x200B;字段。

   或

   单击&#x200B;**[!UICONTROL 登录]**。

   此时将打开一个新的浏览器选项卡。

1. 按照提示使用增强型身份验证、OAuth 2.0或您的安全断言标记语言(SAML) URL登录[!DNL Workfront]。

   >[!NOTE]
   >
   >* 当系统提示您输入[!DNL Workfront]帐户的域时，请使用此格式键入该域： *您的公司&#39;sDomain.my.workfront.com*。 您公司的域通常是您公司的名称。
   >* 在[!DNL Workfront]管理员为此集成启用增强身份验证之前，该身份验证不可用。
   >* 适用于Microsoft Teams的Workfront与Workfront沙盒环境不兼容。


1. 关闭您用来登录的浏览器选项卡并返回[!DNL Microsoft Teams]。

   [!DNL Workfront]机器人聊天渠道中会显示通知，以确认您已成功登录[!DNL Workfront]。
