---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 适用于Salesforce的Adobe Workfront概述
description: 您可以为Salesforce安装 [!DNL Adobe Workfront] 以允许Salesforce用户提交 [!DNL Workfront] 请求并自动创建项目，而无需离开Salesforce。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] 概述

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>为了提供更稳定和可扩展的集成，我们正在使用Workfront自动化与集成(Fusion)转向一种现代、灵活的集成方法。 在此过渡过程中，Workfront for Salesforce集成在&#x200B;**2026年2月28日**&#x200B;后不可用。
>
>为了满足贵组织与Salesforce的集成需求，我们建议使用Workfront自动化和集成。
>
>有关Workfront自动化和集成的概述，请参阅[Adobe Workfront Fusion概述](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>有关Salesforce的Workfront自动化和集成模块的特定功能的信息，请参阅[Salesforce模块](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules)。

您可以安装[!DNL Adobe Workfront for Salesforce]以允许[!DNL Salesforce]用户提交[!DNL Workfront]请求并自动创建项目而无需离开[!DNL Salesforce]。

作为[!DNL Workfront]管理员，您可以下载和配置[!DNL Workfront for Salesforce]。 然后，您可以将其与所有其他[!DNL Salesforce]用户共享。

有关安装[!DNL Workfront for Salesforce]的详细信息，请参阅[安装 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)。

有关为所有用户配置[!DNL Workfront]中的[!DNL Salesforce]节的详细信息，请参阅[为 [!DNL Adobe Workfront] 用户配置 [!DNL Salesforce] 节](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

>[!NOTE]
>
>需要[!UICONTROL Pro] [!DNL Workfront]计划才能使用此功能。 有关各种可用计划的详细信息，请参阅[[!DNL Workfront] 计划。](https://business.adobe.com/cn/products/workfront/pricing.html)

## 访问要求

您必须具有以下权限才能使用本文中所述的功能：

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新增：标准<p>
   <p>或</p>
   <p>当前：计划</p>


</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## [!DNL Workfront for Salesforce]

使用[!DNL Workfront for Salesforce]时，您可以执行以下操作：

* 在Opportunity或Account中从[!DNL Workfront]手动创建新[!DNL Salesforce]请求。

  有关详细信息，请参阅来自[对象的 [!DNL Adobe Workfront] 提交 [!DNL Salesforce] 请求](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)。

* 当[!DNL Workfront]中满足某些条件时，在[!DNL Salesforce]中自动触发项目创建。 您的[!DNL Salesforce]系统管理员必须配置触发器以从[!DNL Salesforce]创建项目。

  有关从[!DNL Workfront]创建[!DNL Salesforce]项目的详细信息，请参阅[从 [!DNL Adobe Workfront] 对象创建 [!DNL Salesforce] 项目](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md)。

处理[!DNL Workfront]的[!DNL Salesforce]时，请考虑以下事项：

* 我们同时支持[!DNL Salesforce Classic]和[!DNL Lightning Experience]框架。
* 只能创建从[!DNL Salesforce]到[!DNL Workfront]的项。
* 您可以查看有关[!DNL Workfront]中[!DNL Salesforce]项的一些信息。 无法自定义此信息。

  有关可以从[!DNL Workfront]查看的[!DNL Salesforce]字段的列表，请参阅来自[对象的 [!DNL Adobe Workfront] 提交 [!DNL Salesforce] 请求](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)和来自[对象的 [!DNL Adobe Workfront] 创建 [!DNL Salesforce] 项目](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md)。

* 通过单击Workfront中的[!DNL Salesforce]转到Salesforce[!UICONTROL 链接，您可以直接访问链接到]的项。

  您无法在[!DNL Salesforce]中查看有关[!DNL Workfront]项的任何信息，但Workfront中有一个链接，该链接会将您转到Salesforce中的项，以便您能够在其中查看它。

  [!UICONTROL 转到Salesforce]链接显示在以下区域中：

   * 项目或问题的[!UICONTROL 详细信息]部分。
   * 项目或问题的标头。

     您的系统或组管理员必须将[!UICONTROL 集成]字段添加到您的布局模板中，才能查看项目或问题标题中的[!UICONTROL 转到Salesforce]链接。
   * 在列表中选择问题时，单击列表工具栏中的[!DNL Summary]打开摘要摘要面板图标![后问题的](assets/summary-panel-icon.png)面板。

     >[!NOTE]
     >
     >[!UICONTROL 转到Salesforce]链接对可以查看项目或问题的所有[!DNL Workfront]用户可见。 您必须拥有[!DNL Salesforce]帐户才能转到记录问题的[!DNL Salesforce]机会或帐户。

* 更新一个应用程序中一个项目的字段不会更新另一个应用程序中链接项目的任何信息。
