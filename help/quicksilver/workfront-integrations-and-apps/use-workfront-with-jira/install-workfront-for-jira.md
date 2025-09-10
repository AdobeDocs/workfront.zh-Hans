---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 为 [!DNL Adobe Workfront] 安装 [!DNL Jira]
description: 您可以使用 [!DNL Adobe Workfront] for [!DNL Jira] 来集成 [!DNL Jira] 和 [!DNL Workfront] 系统。
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 064418302767ad20e176080ba9a12db548750f3c
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# 安装[!DNL Adobe Workfront for Jira]

>[!IMPORTANT]
>
>为了提供更稳定和可扩展的集成，我们正在使用Workfront自动化与集成(Fusion)转向一种现代、灵活的集成方法。 在此过渡过程中，Workfront for Jira集成在&#x200B;**2026年2月28日**&#x200B;后不可用。
>
>为了满足贵组织与Jira的集成需求，我们建议使用Workfront自动化和集成。
>
>有关Workfront自动化和集成的概述，请参阅[Adobe Workfront Fusion概述](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>有关Jira的Workfront自动化和集成模块的特定功能的信息，请参阅[Jira软件模块](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)。

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

您可以使用[!DNL Adobe Workfront for Jira]来集成[!DNL Jira]和[!DNL Workfront]系统。

安装加载项后，您可以定义在创建[!DNL Jira]工作项时自动创建[!DNL Workfront]问题的工作流。 两个应用程序中的项目会相互链接，并且其中的一些信息可以在两个系统中自动更新。

[!DNL Workfront]和[!DNL Jira]中的所有用户都可从此集成中受益。 他们只需要许可证就可以使用他们最常使用的系统，而不需要许可证就可以同时使用两个系统。

此加载项可用于[!UICONTROL 软件的]服务器[!UICONTROL 和]OnDemand[!UICONTROL &#x200B; （或]云[!DNL Jira]）版本。 此加载项不可用于[!DNL Data Center]软件的[!DNL Jira]版本。

有关[!DNL Jira]当前支持的[!DNL Workfront for Jira]版本的列表，请参阅Atlassian Marketplace上的[[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview)。

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
   <td role="rowheader">Adobe [!DNL Workfront]许可证概述</td> 
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

## 为[!DNL Workfront]安装[!DNL Jira]

为[!DNL Workfront] OnDemand安装[!DNL Jira]与在[!DNL Jira]服务器实例上安装它相同。

您必须是[!DNL Jira]管理员才能安装[!DNL Workfront]加载项。

如果您不是[!DNL Jira]管理员，则可以浏览[!DNL Workfront]加载项并请求安装它。 您的请求将发送给[!DNL Jira]管理员进行批准和安装。

有关请求在[!DNL Jira]应用程序上安装加载项的更多信息，请参阅[管理加载项的用户请求。](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

要安装[!DNL Workfront for Jira]：

1. 以[!DNL Jira]管理员身份登录[!DNL Jira]。
1. 在&#x200B;**[!DNL Workfront for Jira]**&#x200B;[[!DNL Atlassian Marketplace]&#x200B;中找到](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview)加载项。

1. 单击&#x200B;**[!UICONTROL 立即获取它]**&#x200B;以进行安装。

   安装完成后，您可以从[!DNL Workfront]登录到[!DNL Jira]并配置集成。

   有关详细信息，请参阅[配置Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

## 有关[!DNL Jira Server]安装的注意事项

>[!NOTE]
>
>这些要求不适用于[!UICONTROL 软件的]OnDemand[!UICONTROL &#x200B; (]Cloud[!DNL Jira])版本。

尽管在两个[!DNL Workfront]环境中安装[!DNL Jira]加载项类似，但在使用[!DNL Jira Server]安装时必须考虑以下事项：

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
