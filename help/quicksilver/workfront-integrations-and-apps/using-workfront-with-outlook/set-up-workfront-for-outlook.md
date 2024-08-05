---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 为 [!DNL Outlook]设置 [!DNL Adobe Workfront]
description: ' [!DNL Adobe Workfront] [!DNL Outlook]加载项允许您直接从Outlook执行 [!DNL Workfront] 键任务。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: e4f722bab4c4024ca796af8413e7d6b69f6a89a7
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# 设置[!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

[!DNL Adobe Workfront] [!DNL Outlook]加载项允许您直接从Outlook中执行以下关键[!DNL Workfront]任务：

* 使用电子邮件中的信息更新现有项目、任务或问题。 有关详细信息，请参阅[从 [!DNL Outlook] 电子邮件](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md)更新现有对象。
* 根据[!DNL Outlook]中的电子邮件创建一个[!DNL Workfront]请求。 有关详细信息，请参阅[通过 [!DNL Outlook] 电子邮件](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md)创建Adobe Workfront请求。
* 在[!UICONTROL 我的工作]区域添加电子邮件作为任务。 有关详细信息，请参阅[将 [!DNL Outlook] 电子邮件作为任务添加到您的工作列表](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md)。
* 通过[!DNL Outlook]的[!DNL Workfront]加载项回复评论。 有关回复Workfront针对[!DNL Outlook]的评论的信息，请参阅[回复来自 [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md)的评论。
* 从头开始创建任务和问题，或从现有电子邮件创建任务和问题（使用拖放功能）。 有关详细信息，请参阅[将 [!DNL Outlook] 电子邮件作为任务或问题添加到项目](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md)。

在使用[!DNL Workfront for Outlook]之前，您必须将[!DNL Workfront]加载项添加到您的[!DNL Outlook]帐户。

如果您无法使用您的[!DNL Outlook]帐户安装[!DNL Workfront]加载项，请联系您的[!DNL Workfront]管理员以确保为您的组织启用[!DNL Outlook]加载项。

有关如何为您的组织启用[!DNL Outlook]集成的信息，请参阅[启用 [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md)。

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
   <td> 
   <p>新计划： [！UICONTROL Standard]</p> 
   <p>当前计划：[！UICONTROL工作]，[！UICONTROL计划]</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

您的[!DNL Workfront]管理员必须使用[!DNL Workfront]启用[!DNL Outlook for Office]，然后才能使用此集成。

## 系统要求

可以使用以下应用程序：

* Web上的&#x200B;**[!DNL Outlook]：**&#x200B;在桌面或移动设备上通过Web浏览器使用[!DNL Outlook]时，[!DNL Workfront]加载项可用。 此功能在使用[!DNL Outlook] Web App时也可用。
* **[!DNL Outlook]桌面应用程序：**&#x200B;使用[!DNL Office]包中包含的[!DNL Outlook]的[!DNL Windows]和[!DNL Mac]桌面版本时，[!DNL Workfront]加载项可用。

满足以下要求的环境支持[!DNL Outlook]的[!DNL Workfront]加载项：

* [客户端要求](#client-requirements-client-requirements)
* [邮件服务器要求](#mail-server-requirements-mail-server-requirements)

### 客户端要求 {#client-requirements}

Workfront支持[!DNL Outlook]的以下版本：

* [!DNL Outlook 2013]或更高版本（在[!DNL Windows]）
*[!DNL  Outlook 2016]或更高版本（在[!DNL Windows]）
* [!DNL Mac]上的[!DNL Outlook] ([!DNL Microsoft 365])
* [!DNL Windows]上的[!DNL Outlook] ([!DNL Microsoft 365])
* [!DNL Outlook]在Web上

您必须使用直接连接连接到[!DNL Exchange Server]或[!DNL Office 365]。

配置客户端时，用户必须选择以下帐户类型之一：

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B; &#x200B;****&#x200B;如果客户端配置为连接POP3或IMAP，则无法加载[!DNL Workfront]加载项。

### 邮件服务器要求 {#mail-server-requirements}

连接到[!DNL Office 365]或[!DNL Outlook.com]时，默认满足邮件服务器要求。 但是，如果您连接到[!DNL Exchange Server]的内部部署，则适用以下要求：

* Workfront支持所有[!DNL Exchange On-Premise]服务器
* 必须启用[!DNL Exchange Web Services] (EWS)，并且必须向Internet公开。
* 服务器必须具有有效的身份验证证书，服务器才能颁发有效的身份令牌。 [!DNL Exchange Server]的新安装包括默认的身份验证证书。

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* 若要从[[!DNL Office] 应用商店](https://store.office.com/)访问[!DNL Workfront]加载项，您的客户端访问服务器必须能够与[https://store.office.com](https://store.office.com/)通信。

有关支持的环境的更多详细信息，请参阅[[!DNL Microsoft Office 365] 主页](https://products.office.com/en-us/office-365-home)。

## 安装加载项

您可以从[Microsoft应用商店](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview)中获取适用于Outlook的Workfront加载项。

### [!DNL Outlook 365]的[!DNL Workfront] {#workfront-for-outlook-365}

1. 在[!DNL Outlook 365]中，单击Office 365界面顶部的&#x200B;**[!UICONTROL 浏览加载项]**&#x200B;图标![](assets/outlook-add-in-26x26.png)，然后单击&#x200B;**[!UICONTROL 管理加载项]**。

1. 在&#x200B;**[!UICONTROL 搜索加载项]**&#x200B;框中，搜索&#x200B;**[!DNL Workfront]**，然后按[!UICONTROL Enter]。

1. 单击&#x200B;**[!UICONTROL 添加]**。

### Web上[!DNL Outlook]的[!DNL Workfront] {#workfront-for-outlook-on-the-web}

1. 在Web浏览器中打开[!DNL Microsoft Outlook]。
1. 单击&#x200B;**[!UICONTROL 浏览]加载项**&#x200B;图标![](assets/outlook-add-in-web-version-20x20.png)。

   要查找该图标，请参阅Microsoft文档中的[在Web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon)上使用 [!DNL Outlook] 中的加载项。

1. 在&#x200B;**[!UICONTROL 搜索加载项]**&#x200B;字段中搜索&#x200B;**[!DNL Workfront]**，然后按&#x200B;**[!UICONTROL Enter]**。

1. 当它出现在列表中时，单击&#x200B;**添加**。

### [!UICONTROL Windows]或[!DNL Mac]上的[!DNL Workfront for Outlook] {#workfront-for-outlook-on-windows-or-mac}

1. 在功能区上单击&#x200B;**[!UICONTROL 主页]** > **[!UICONTROL 商店]**。

1. 在&#x200B;**[!UICONTROL 搜索]**&#x200B;字段中搜索&#x200B;**[!DNL Workfront]**，然后按&#x200B;**[!UICONTROL Enter]**。

1. 单击切换可启用&#x200B;**[!UICONTROL [!DNL Workfront]加载项]**。

## 从[!DNL Outlook]登录到[!DNL Workfront]

1. 在[!DNL Outlook]中，选择一个电子邮件，然后单击电子邮件标题中的&#x200B;**[!DNL Workfront]**&#x200B;图标。
1. 在登录页面上，单击&#x200B;**登录Workfront**。
1. 按照提示使用OAuth 2.0登录[!DNL Workfront]。<!--Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.-->

   <!--Before users can log in to the [!DNL Workfront] add-in using SAML, a [!DNL Workfront] administrator must first enable [!DNL Office 365] add-ins to authenticate using a SAML 2.0 solution. For more information, see the section [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) in the article [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).-->

   >[!NOTE]
   >
   >* 如果提示您输入[!DNL Workfront]帐户的域，请使用此格式键入该域： *您的公司&#39;sDomain.my.workfront.com*。 您公司的域通常是您公司的名称。

<!--ADDITIONAL BULLET REMOVED FROM NOTE BOX: Enhanced Authentication is not available until a Workfront administrator enables it for this integration.-->
