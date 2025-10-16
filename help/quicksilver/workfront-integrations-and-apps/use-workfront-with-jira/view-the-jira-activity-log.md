---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 查看Jira活动日志
description: 作为 [!DNL Jira] 管理员，您可以在活动日志中查看在 [!DNL Adobe Workfront] 和 [!DNL Jira] 之间同步或创建票证期间发生的异常和错误。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: b1b55b8046aa771abb2cceda333940ccf827356a
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 查看[!UICONTROL [!DNL Jira]活动日志]

>[!IMPORTANT]
>
>为了提供更稳定和可扩展的集成，我们正在使用Workfront自动化与集成(Fusion)转向一种现代、灵活的集成方法。 在此过渡过程中，Workfront for Jira集成在&#x200B;**2026年2月28日**&#x200B;后不可用。
>
>为了满足贵组织与Jira的集成需求，我们建议使用Workfront自动化和集成。
>
>有关Workfront自动化和集成的概述，请参阅[Adobe Workfront Fusion概述](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>有关Jira的Workfront自动化和集成模块的特定功能的信息，请参阅[Jira软件模块](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)。

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

作为[!DNL Jira]管理员，您可以在[!DNL Adobe Workfront]活动日志[!DNL Jira]中查看在[!UICONTROL 和]之间同步或创建票证期间发生的异常和错误。

您在活动日志中最多可以看到500个项目，这些项目将从最新项目开始列出。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td><p>任何</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准 </p>
       <p>规划 </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira访问</td> 
   <td> <p>系统管理员访问权限</p> <p>重要信息：我们建议您在Jira和Workfront中创建单独的系统管理员帐户以专门用于此集成，而不是使用可能附加到用户的现有帐户。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在链接[!DNL Workfront]和[!DNL Jira]之间的项目之前，您必须

* 安装[!DNL Workfront for Jira]

  有关安装[!DNL Workfront for Jira]的说明，请参阅[安装 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)。

## 访问[!UICONTROL [!DNL Jira]活动日志]：

1. 以系统管理员身份登录Jira。
1. 在主&#x200B;**[!UICONTROL 菜单中单击]**&#x200B;设置[!DNL Jira]。
1. 单击&#x200B;**[!UICONTROL 插件]**，然后单击&#x200B;**[!UICONTROL 管理插件]**。

1. 展开&#x200B;**[!DNL Workfront]**&#x200B;加载项。
1. 单击&#x200B;**[!UICONTROL 配置]**。
1. 以系统管理员身份登录到[!DNL Workfront]。
1. 选择&#x200B;**[!UICONTROL 活动日志]**&#x200B;选项卡。

   查看有关创建项目或同步两个应用程序之间的字段期间发生的异常和错误的信息。

   日志包含以下字段：

   * 发生日期
   * Jira中的用户的名称
   * Jira问题编号
   * 所发生错误的简短描述。
