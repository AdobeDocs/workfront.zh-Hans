---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: 安装并打开适用于XD的Adobe Workfront
description: 您可以从Adobe Workfront Marketplace安装适用于XD的Adobe插件。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d4971977-b5bd-4bb4-a1c2-44829a67d32d
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 2%

---

# 安装并打开[!DNL Adobe Workfront for XD]

您可以从Adobe Marketplace安装[!DNL Adobe Workfront for XD]插件。 插件支持以下语言：

* 英语
* 法语
* 德语
* 意大利语
* 西班牙语
* 葡萄牙语
* 日语
* 简体中文
* 繁体中文
* 韩语

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
 <!-- <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package/td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>
   <p>Standard</p>
    <p>Work or higher</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">其他产品</td> 
   <td><p>除了[!DNL Adobe Creative Cloud]许可证，您还必须具有[!DNL Workfront]许可证。</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

* 您必须先安装[!DNL Adobe XD]应用程序，然后才能安装Workfront插件。

## 为您的组织安装[!DNL Adobe Workfront for XD]插件

如果您是[!DNL Adobe Admin Console]管理员，则可以在[!DNL Creative Cloud]部署包中包含该插件。 有关详细信息，请参阅[在包中包含插件](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html)。

[在此观看视频教程](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}。

[!DNL Adobe Admin Console]管理员还可以创建仅用于分发给用户的插件包。 有关详细信息，请参阅[中的 [!DNL Adobe Workfront] 为您的用户创建[！UICONTROL [!DNL Creative Cloud]]  for [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)包

## 单独安装[!DNL Adobe Workfront for XD]插件

您可以从[!DNL Adobe Workfront for XD]中自行安装[!DNL Adobe Exchange]插件。

1. 转到Adobe Exchange上的[Adobe Workfront for XD安装页面](https://exchange.adobe.com/apps/cc/4c3566f9?pluginId=4c3566f9&workflow=share)。
1. 在出现的对话框中，单击&#x200B;**打开[!DNL Adobe Creative Cloud]桌面应用程序**。
1. 打开[!DNL Adobe XD]插件管理器后，单击&#x200B;**[!UICONTROL 安装]**。
1. 读取对话框中的信息，然后单击&#x200B;**[!UICONTROL 确定]**。
1. 有关如何打开该插件的信息，请继续阅读以下部分。

## 打开[!DNL Adobe Workfront for XD]插件

1. 打开[!DNL Adobe XD]。

1. 创建新文件或打开现有文件。

1. 单击左下角的&#x200B;**插件**&#x200B;图标。

![XD插件窗口](assets/xd-plugin-window-350x620.png)

1. 在&#x200B;**[!UICONTROL 插件面板]**&#x200B;中，找到&#x200B;**[!UICONTROL 适用于XD的Adobe Workfront]**。

1. 有关如何登录到插件的信息，请转到以下部分。

## 登录到[!DNL Adobe Workfront for XD]

1. 确保插件面板已打开，然后单击&#x200B;**[!DNL Adobe Workfront for XD]**。
1. 输入您的域，然后单击&#x200B;**[!UICONTROL 登录]**。 此时将打开一个浏览器页面。

   >[!TIP]
   >
   >* 要查找您的域，请打开浏览器，导航到您的[!DNL Workfront]实例，并复制URL的第一部分：\
   >![查找域](assets/domain-350x50.png)
   >
   >* 如果您的Workfront实例已与Experience Cloud集成，请要求您的管理员为您提供Admin Console中产品> Workfront下的Workfront域。

1. 在浏览器中输入您的[!DNL Workfront]凭据，然后单击&#x200B;**[!DNL Log in]**。 如果贵公司使用单点登录(SSO)，则会将您引导至您的SSO提供商页面以进行登录。

   >[!NOTE]
   >
   >如果您最近登录，则系统可能不会提示您输入您的[!DNL Workfront]凭据。

   按照提示登录[!DNL Workfront]。

   >[!NOTE]
   >
   >* [!DNL Workfront]使用OAuth 2.0连接到[!DNL Adobe Creative Cloud]，这是大多数基于Web的集成用于用户身份验证和授权的安全标准。
   >* 当提示您输入[帐户的]域或主机[!DNL Workfront]时，请使用此格式键入该帐户： *您的公司&#39;sDomain.my.workfront.com*。 您公司的域通常是您公司的名称。

1. 单击&#x200B;**[!UICONTROL 允许访问]**&#x200B;完成登录，然后返回[!DNL Adobe XD]查看您的工作。

### 登录错误疑难解答

尝试登录&#x200B;**时显示**“出现错误”错误


无法使用以`experience.adobe.com`开头的URL登录到插件。

![登录错误](assets/plugin-log-in-error.png) ![域](assets/incorrect-domain.png)


要解决此问题，

1. 卸载并重新安装Adobe Workfront for XD插件以清除域和错误。

1. 输入您的Workfront域。 域必须是`company-name.my.workfront.com`而不是`experience.adobe.com`。

如果您在Adobe Unified Experience上，要查找您的Workfront域，请转到
