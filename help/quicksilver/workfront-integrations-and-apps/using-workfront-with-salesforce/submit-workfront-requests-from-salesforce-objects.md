---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 提交来自 [!DNL Adobe Workfront] 对象的 [!DNL Salesforce] 请求
description: 安装来自 [!DNL Adobe Workfront] 机会和帐户的 [!DNL Salesforce], you can submit [!DNL Workfront] 请求的 [!DNL Salesforce] 后。 经典和Lightning Experience框架中均存在此功能。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 2%

---

# 提交来自[!DNL Adobe Workfront]对象的[!DNL Salesforce]请求

>[!IMPORTANT]
>
>为了提供更稳定和可扩展的集成，我们正在使用Workfront自动化与集成(Fusion)转向一种现代、灵活的集成方法。 在此过渡过程中，Workfront for Salesforce集成在&#x200B;**2026年2月28日**&#x200B;后不可用。
>
>为了满足贵组织与Salesforce的集成需求，我们建议使用Workfront自动化和集成。
>
>有关Workfront自动化和集成的概述，请参阅[Adobe Workfront Fusion概述](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>有关Salesforce的Workfront自动化和集成模块的特定功能的信息，请参阅[Salesforce模块](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules)。

安装[!DNL Adobe Workfront for Salesforce]后，您可以提交来自[!DNL Workfront]机会和帐户的[!DNL Salesforce]请求。 此功能同时存在于[!DNL Classic]和[!DNL Lightning Experience]框架中。

## 访问要求

您必须具有以下权限才能使用本文中所述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] 计划*</p></td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] 许可证*</p></td> 
   <td> <p>[!UICONTROL 计划]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 先决条件

要提交来自[!DNL Workfront]机会或帐户的[!DNL Salesforce]请求，请确保您的环境中有以下各项：

* 您的[!DNL Workfront]管理员已安装[!DNL Workfront for Salesforce]。\
   有关安装[!DNL Workfront for Salesforce]的详细信息，请参阅[安装 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* 您的[!DNL Workfront]管理员已将[!DNL Workfront]部分添加到您的[!UICONTROL Opportunity]和[!UICONTROL Account]页面布局。\
   有关将[!DNL Workfront]分区添加到页面布局的详细信息，请参阅[为 [!DNL Adobe Workfront] 用户配置 [!DNL Salesforce] 分区](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

* 您拥有[!DNL Workfront]帐户，并且可以从您的机会或帐户中的[!DNL Workfront]部分登录到该帐户。\
   登录后，您会看到[!UICONTROL 新请求]选项卡，您可以在其中开始输入请求。

## 提交来自[!DNL Workfront]的[!DNL Salesforce]请求

1. 转到Salesforce中的机会或帐户。
1. 转到 [!DNL Workfront] 部分。
1. 在&#x200B;**[!UICONTROL 新建请求]**&#x200B;选项卡中，在&#x200B;**[!UICONTROL 选择请求类型]**&#x200B;下拉菜单中选择请求类型。

   您可以看到在Workfront中有权查看的相同请求队列。

1. 开始填写您的请求的可用字段。

   从[!DNL Salesforce]提交请求与在[!DNL Workfront] Web应用程序中提交请求相同。

   >[!NOTE]
   >
   >在[!DNL Workfront]中使用[!DNL Salesforce]插件上载文档暂时不可用。

   继续执行[创建并提交 [!DNL Adobe Workfront] 请求](../../manage-work/requests/create-requests/create-submit-requests.md)中描述的步骤。

1. 单击&#x200B;**[!UICONTROL 提交]**。

## 查看[!DNL Workfront]请求

1. 转到[!DNL Salesforce]中的机会或帐户。
1. 转到 **[!DNL Workfront]** 部分。

   >[!NOTE]
   >
   >根据[!DNL Workfront]管理员配置此部分的方式，它可能具有不同的名称。

1. 选择&#x200B;**[!UICONTROL 已提交的请求]**&#x200B;选项卡。

   您可以在此选项卡中查看您或其他人从此机会或帐户提交的所有请求。在Web应用程序中提交到此请求队列的请求不会显示在[!DNL Salesforce]的此列表中。

   >[!NOTE]
   >
   >在Web应用程序中提交到此请求队列的请求不会显示在Salesforce的此列表中。

   ![salesforce_submitted_requests.png](assets/salesforce-submitted-requests-350x58.png)

   您可以查看关于已提交请求的以下信息：

   * 请求名称（在[!UICONTROL 主题]列中）
   * 参考号
   * 请求类型
   * 状态
   * 提交日期
   * 按名称请求
   * 指定给名称\

     当此信息在[!DNL Workfront]中更新时，它也会在此列表中更新。

1. （可选）单击请求的名称以在[!DNL Workfront]中将其打开。

1. （可选）单击&#x200B;**[!UICONTROL 转到[!DNL Salesforce]]**&#x200B;以访问问题源自于Workfront以下方面的Opportunity或Account：

   * 在问题的[!UICONTROL 详细信息]部分中
   * 在列表中选择问题时，在“摘要”面板中，单击列表工具栏中的[!UICONTROL 打开摘要] ![摘要面板图标](assets/summary-panel-icon.png)。
   * 在问题标题中，当[!UICONTROL 集成]字段可用时。 您的系统或组管理员必须将[!UICONTROL 集成]字段添加到您的布局模板，才能在问题标题中查看转到Salesforce链接。 有关详细信息，请参阅[使用布局模板自定义对象标头](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

   >[!NOTE]
   >
   >[!UICONTROL 转到Salesforce]链接对可以查看问题的所有[!DNL Workfront]用户可见。 您必须拥有[!DNL Salesforce]帐户才能转到记录问题的[!DNL Salesforce]机会或帐户。
