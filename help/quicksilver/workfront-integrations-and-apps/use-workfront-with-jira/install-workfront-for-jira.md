---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 为 [!DNL Jira]安装 [!DNL Adobe Workfront]
description: 您可以使用 [!DNL Adobe Workfront] for [!DNL Jira] 来集成 [!DNL Jira] 和 [!DNL Workfront] 系统。
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 安装[!DNL Adobe Workfront for Jira]

您可以使用[!DNL Adobe Workfront for Jira]来集成[!DNL Jira]和[!DNL Workfront]系统。

安装加载项后，您可以定义在创建[!DNL Workfront]工作项时自动创建[!DNL Jira]问题的工作流。 两个应用程序中的项目会相互链接，并且其中的一些信息可以在两个系统中自动更新。

[!DNL Workfront]和[!DNL Jira]中的所有用户都可从此集成中受益。 他们只需要许可证就可以使用他们最常使用的系统，而不需要许可证就可以同时使用两个系统。

此加载项可用于[!DNL Jira]软件的[!UICONTROL 服务器]和[!UICONTROL OnDemand] （或[!UICONTROL 云]）版本。 此加载项不可用于[!DNL Jira]软件的[!DNL Data Center]版本。

有关[!DNL Workfront for Jira]当前支持的[!DNL Jira]版本的列表，请参阅Atlassian Marketplace上的[[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> 
   <p>新建：任何</p>
   <p>当前： [!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe[!DNL Workfront]许可证概述</td> 
   <td> 
   <p>新增：标准</p>
   <p>当前： [!UICONTROL 计划]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 访问</td> 
   <td> <p>系统管理员访问权限</p> <p>重要提示：建议您在[!DNL Jira]和[!DNL Workfront]中创建单独的系统管理员帐户以专门用于此集成，而不是使用可能附加到用户的现有帐户。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td><p>您必须是[!DNL Workfront]管理员。</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为[!DNL Jira]安装[!DNL Workfront]

为[!DNL Jira] OnDemand安装[!DNL Workfront]与在[!DNL Jira]服务器实例上安装它相同。

您必须是[!DNL Jira]管理员才能安装[!DNL Workfront]加载项。

如果您不是[!DNL Jira]管理员，则可以浏览[!DNL Workfront]加载项并请求安装它。 您的请求将发送给[!DNL Jira]管理员进行批准和安装。

有关请求在[!DNL Jira]应用程序上安装加载项的更多信息，请参阅[管理加载项的用户请求。](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

要安装[!DNL Workfront for Jira]：

1. 以[!DNL Jira]管理员身份登录[!DNL Jira]。
1. 在[[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview)中找到&#x200B;**[!DNL Workfront for Jira]**&#x200B;加载项。

1. 单击&#x200B;**[!UICONTROL 立即获取它]**&#x200B;以进行安装。

   安装完成后，您可以从[!DNL Jira]登录到[!DNL Workfront]并配置集成。

   有关详细信息，请参阅[配置Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

## 有关[!DNL Jira Server]安装的注意事项

>[!NOTE]
>
>这些要求不适用于[!DNL Jira]软件的[!UICONTROL OnDemand] ([!UICONTROL Cloud])版本。

尽管在两个[!DNL Jira]环境中安装[!DNL Workfront]加载项类似，但在使用[!DNL Jira Server]安装时必须考虑以下事项：

* 在[!DNL Jira]中配置加载项时，在&#x200B;**[!DNL JIRA Base URL]**&#x200B;字段中指定的地址可能与您在专用服务器上用于访问[!DNL Jira]的URL不同。 **[!DNL JIRA Base URL]**&#x200B;必须是一个可公开访问的地址，该地址使用NAT或反向代理协议连接到您的专用服务器，因此[!DNL Workfront]可以访问该地址以向您的服务器发出请求。

* 您必须使用SSL加密来保护[!DNL Jira]和[!DNL Workfront]之间的通信。 启用SSL时，必须从证书颁发机构获得完整的SSL证书栈栈。 我们不支持自签名证书。
* 您必须确保可从公司服务器访问[!DNL jira.workfront.com]域。 它充当介于[!DNL Workfront]和[!DNL Jira]之间的中间件环境，是加载项运行所必需的。

  您还必须将以下静态IP地址添加到防火墙上的允许列表中，以便进行出站和入站连接。

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  有关将防火墙配置为具有[!DNL Workfront]的最佳功能的详细信息，请参阅[配置防火墙](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。
