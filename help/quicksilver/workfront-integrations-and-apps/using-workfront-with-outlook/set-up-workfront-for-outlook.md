---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 设置 [!DNL Adobe Workfront] 表示 [!DNL Outlook]
description: Adobe Workfront Fusion提供与Outlook的集成。 本文介绍了如何在您自己的工作流中开始使用此集成。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 16acba0f1981b75ca141a36d096fb6f5d37c40d1
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 0%

---

# 设置 [!DNL Adobe Workfront for Outlook]

的 [!DNL Adobe Workfront] [!DNL Outlook] 插件允许您执行以下键 [!DNL Workfront] 直接从Outlook执行任务：

* 使用电子邮件中的信息更新现有项目、任务或问题。 有关更多信息，请参阅 [从 [!DNL Outlook] 电子邮件](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* 创建 [!DNL Workfront] 根据 [!DNL Outlook]. 有关更多信息，请参阅 [通过 [!DNL Outlook] 电子邮件](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* 在 [!UICONTROL 我的工作] 的上界。 有关更多信息，请参阅 [添加 [!DNL Outlook] 电子邮件作为任务发送到您的工作列表](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* 通过回复评论 [!DNL Workfront] 插件 [!DNL Outlook]. 有关回复Workfront对 [!DNL Outlook]，请参阅 [回复来自 [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* 从头开始创建任务和问题，或从现有电子邮件创建任务和问题（使用拖放功能）。 有关更多信息，请参阅 [添加 [!DNL Outlook] 通过电子邮件将项目作为任务或问题发送给](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

您必须将 [!DNL Workfront] 的 [!DNL Outlook] 帐户 [!DNL Workfront for Outlook].

如果您无法安装 [!DNL Workfront] 插件 [!DNL Outlook] 帐户，联系 [!DNL Workfront] 管理员确保 [!DNL Outlook] 已为您的组织启用加载项。

有关如何启用 [!DNL Outlook] 贵组织的集成，请参阅 [启用 [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Work]、[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 先决条件

您的 [!DNL Workfront] 管理员必须启用 [!DNL Outlook for Office] with [!DNL Workfront] ，以便您使用此集成。

## 系统要求

以下应用程序可供使用：

* **[!DNL Outlook]在Web上：** 的 [!DNL Workfront] 使用 [!DNL Outlook] 桌面或移动设备上的Web浏览器访问。 使用 [!DNL Outlook] Web应用程序。
* **[!DNL Outlook]桌面应用程序：** 的 [!DNL Workfront] 使用 [!DNL Windows] 和 [!DNL Mac] 桌面版本 [!DNL Outlook] 包含 [!DNL Office] 包。

的 [!DNL Workfront] 插件 [!DNL Outlook] 在满足以下要求的环境中受支持：

* [客户端要求](#client-requirements-client-requirements)
* [邮件服务器要求](#mail-server-requirements-mail-server-requirements)

### 客户端要求 {#client-requirements}

我们支持以下版本的 [!DNL Outlook]:

* [!DNL Outlook 2013] 或稍后 [!DNL Windows]
*[!DNL  Outlook 2016] 或稍后 [!DNL Windows]
* [!DNL Outlook] on [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] on [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] 网上

您必须连接到 [!DNL Exchange Server] 或 [!DNL Office 365] 使用直接连接。

配置客户端时，用户必须选择以下帐户类型之一：

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;**&#x200B;**&#x200B;如果客户端配置为与POP3或IMAP连接，则 [!DNL Workfront] 加载加载项时。

### 邮件服务器要求 {#mail-server-requirements}

默认情况下，在连接到 [!DNL Office 365] 或 [!DNL Outlook.com]. 但是，如果您已连接到 [!DNL Exchange Server]，则适用以下要求：

* 我们支持 [!DNL Exchange 2016 On-Premise]
* [!DNL Exchange Web Services] (EWS)必须启用且必须显示在Internet上。
* 服务器必须具有有效的身份验证证书，才能颁发有效的身份令牌。 的新安装 [!DNL Exchange Server] 包括默认的身份验证证书。

   有关更多信息，请参阅 [中的数字证书和加密 [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) 和 [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).

* 为了访问 [!DNL Workfront] 的加载项 [[!DNL Office] 存储](https://store.office.com/)，则您的客户端访问服务器必须能够与  [https://store.office.com](https://store.office.com/).

有关受支持环境的更多详细信息，请参阅 [[!DNL Microsoft Office 365] 主页](https://products.office.com/en-us/office-365-home).

## 安装插件

有关设置 [!DNL Workfront] 插件 [!DNL Outlook]，请参阅 [[!DNL Workfront]  — 协作工作管理。](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview)

* [[!DNL Workfront] 用于 [!DNL Outlook 365]](#workfront-for-outlook-365-workfront-for-outlook-365)
* [[!DNL Workfront] 表示 [!DNL Outlook] 在Web上](#workfront-for-outlook-on-the-web-workfront-for-outlook-on-the-web)
* [[!DNL Workfront] 表示 [!DNL Outlook] on [!DNL Windows] 或 [!DNL Mac]](#workfront-for-outlook-on-windows-or-mac-workfront-for-outlook-on-windows-or-mac)

### [!DNL Workfront] 用于 [!DNL Outlook 365] {#workfront-for-outlook-365}

1. 在 [!DNL Outlook 365]，请单击 **[!UICONTROL 浏览加载项]** 图标 ![](assets/outlook-add-in-26x26.png)在Office 365界面顶部，单击 **[!UICONTROL 管理加载项]**.

1. 在 **[!UICONTROL 搜索加载项]** 框，搜索 **[!DNL Workfront]** 然后按 [!UICONTROL 输入].

1. 单击 **[!UICONTROL 添加]**.

### [!DNL Workfront] 表示 [!DNL Outlook] 在Web上 {#workfront-for-outlook-on-the-web}

1. 打开 [!DNL Microsoft Outlook] 在Web浏览器中。
1. 单击 **[!UICONTROL 浏览] 加载项** 图标 ![](assets/outlook-add-in-web-version-20x20.png).

   要找到图标，请参阅 [在中使用加载项 [!DNL Outlook] 网上](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) (在Microsoft文档中)。

1. 搜索 **[!DNL Workfront]** 在 **[!UICONTROL 搜索加载项]** 字段，然后按 **[!UICONTROL 输入]**.

1. 当列表上显示该列表时，单击 **添加**.

### [!DNL Workfront for Outlook] on [!UICONTROL Windows] 或 [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. 单击 **[!UICONTROL 主页]** > **[!UICONTROL 存储]** 在丝带上。

1. 搜索 **[!DNL Workfront]** 在 **[!UICONTROL 搜索]** 字段，然后按 **[!UICONTROL 输入]**.

1. 单击切换以启用 **[!UICONTROL [!DNL Workfront]插件]**.

## 登录到 [!DNL Workfront] 从 [!DNL Outlook]

1. 在 [!DNL Outlook]，选择电子邮件，然后单击 **[!DNL Workfront]** 图标。
1. 按照提示登录 [!DNL Workfront] 使用增强的身份验证、OAuth 2.0或您的安全断言标记语言(SAML)URL。

   在用户登录之前 [!DNL Workfront] 使用SAML( [!DNL Workfront] 管理员必须首先启用 [!DNL Office 365] 用于使用SAML 2.0解决方案进行身份验证的加载项。 有关更多信息，请参阅 [配置 [!DNL Adobe Workfront] 带有SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) 在文章中 [配置 [!DNL Adobe Workfront] 带有SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* 提示您输入的域时 [!DNL Workfront] 帐户，请使用以下格式键入： *yourCompany&#39;sDomain.my.workfront.com*. 您公司的域通常是您公司的名称。
   >* 增强的身份验证在 [!DNL Workfront] 管理员为此集成启用了此功能。


