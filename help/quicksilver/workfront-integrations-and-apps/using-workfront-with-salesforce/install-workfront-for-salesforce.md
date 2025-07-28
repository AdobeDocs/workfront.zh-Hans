---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 为 [!DNL Adobe Workfront] 安装 [!DNL Salesforce]
description: 要在应用程序在 [!DNL Salesforce] AppExchange中可用之前安装该应用程序，请参阅在Salesforce市场中可用之前为AppExchange安装 [!DNL Workfront] 。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '1092'
ht-degree: 1%

---

# 安装[!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>为了提供更稳定和可扩展的集成，我们正在使用Workfront自动化与集成(Fusion)转向一种现代、灵活的集成方法。 在此过渡过程中，Workfront for Salesforce集成在&#x200B;**2026年2月28日**&#x200B;后不可用。
>
>为了满足贵组织与Salesforce的集成需求，我们建议使用Workfront自动化和集成。
>
>有关Workfront自动化和集成的概述，请参阅[Adobe Workfront Fusion概述](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>有关Salesforce的Workfront自动化和集成模块的特定功能的信息，请参阅[Salesforce模块](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules)。

作为[!DNL Salesforce]和[!DNL Adobe Workfront]管理员，您可以安装[!DNL Workfront for Salesforce]以允许[!DNL Salesforce]用户提交[!DNL Workfront]请求并自动创建项目而无需离开Salesforce。

有关安装[!DNL Workfront for Salesforce]后可获取哪些内容的一般信息，请参阅[[!DNL Adobe Workfront for Salesforce] 概述](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md)。

* [安装和使用 [!DNL Workfront for Salesforce]的先决条件](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [正在安装 [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能使用本文中所述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新文档： [！UICONTROL Standard]</p><p>或</p><p>当前： [！UICONTROL计划]</p> </td> 
  </tr>  </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 安装和使用[!DNL Workfront for Salesforce]的先决条件 {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* 您必须拥有有权访问系统管理员帐户的[!DNL Salesforce]实例，才能安装应用程序。
* 您必须拥有有权访问系统管理员帐户的[!DNL Workfront]实例才能配置集成。
* [!UICONTROL Salesforce]用户必须具有[!DNL Workfront]帐户才能：

   * 从[!DNL Workfront]创建[!DNL Salesforce]请求
   * 在Salesforce中查看[!DNL Workfront]请求或项目

## 正在安装[!DNL Workfront for Salesforce]  {#installing-workfront-for-salesforce}

您必须是[!DNL Salesforce]和[!DNL Workfront]系统管理员才能安装和配置[!DNL Workfront for Salesforce]。

以下子部分介绍了如何为[!DNL Workfront]生产环境安装[!DNL Salesforce]。 您可以按照相同的步骤为[!DNL Workfront]沙盒环境安装[!DNL Salesforce]。

* [正在安装 [!DNL Workfront for Salesforce] ，使其在 [!DNL AppExchange] 市场中可用](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [正在 [!DNL Workfront for Salesforce] 框架中安装 [!DNL Salesforce Classic] ](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [正在 [!DNL Workfront for Salesforce] 框架中安装 [!DNL Salesforce Lightning Experience] ](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### 正在安装[!DNL Workfront for Salesforce]，以使其在[!DNL AppExchange]市场中可用 {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce]很快将在[!DNL Salesforce AppExchange]中可用。

在应用程序可用之前安装应用程序：

1. 在生产环境中，转到

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   在沙盒环境中，转到

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   >[!NOTE]
   >
   >您必须登录Salesforce才能访问这些页面。

1. 选中&#x200B;**[!UICONTROL 是，授予对这些第三方网站的访问权限]**&#x200B;框。

   此时将显示一个加载屏幕。 安装可能需要一些时间。

1. 安装完成后，单击&#x200B;**[!UICONTROL 完成]**。

1. 导航到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 安全性]控件** > **[!UICONTROL 远程站点设置]**。
1. （视情况而定）从列表中选择Workfront 。

   或

   如果未在[!DNL Workfront]所有远程站点&#x200B;**[!UICONTROL 列表中看到您的]** URL，请单击&#x200B;**[!UICONTROL 新建远程站点]**。

1. （视情况而定）如果添加站点，请指定&#x200B;**[!UICONTROL 远程站点名称]**。

   例如，*[!DNL Workfront]*。

1. （视情况而定）如果添加站点，请指定&#x200B;**[!UICONTROL 远程站点URL]**。

   例如，*yourDomain.my.workfront.com*。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   [!DNL Workfront]应用现已安装在您的[!DNL Salesforce]实例上，并且已在您的环境中创建&#x200B;**[!UICONTROL WorkfrontOpportunities]**&#x200B;和&#x200B;**[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce]页面。

   将[!DNL Salesforce]部分添加到其[!DNL Workfront]Opportunity[!UICONTROL 或]Account[!UICONTROL 页面布局后，]用户可以使用该应用程序。\
   有关为用户配置Workfront部分的信息，请参阅[为Salesforce用户配置Adobe Workfront部分](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

### 正在为[!DNL Workfront]框架中的[!DNL Salesforce]安装[!DNL Salesforce Classic]

1. 以系统管理员身份登录到[!DNL Salesforce]。
1. 转到&#x200B;**安装程序。**
1. 在&#x200B;**生成**&#x200B;部分中，单击&#x200B;**AppExchange Marketplace**。

1. 在&#x200B;**搜索AppExchange应用程序**&#x200B;框中，键入&#x200B;**Workfront**。

1. 找到该Workfront应用后单击该应用，然后单击&#x200B;**立即获取**。
1. 单击&#x200B;**[!UICONTROL 在生产环境中安装]**&#x200B;以在[!DNL Workfront]生产环境中安装[!DNL Salesforce]应用程序。 （推荐）
1. 阅读并同意条款和条件后，请启用&#x200B;**[!UICONTROL 我已阅读并同意条款和条件]**&#x200B;字段。
1. 单击&#x200B;**[!UICONTROL 确认并安装]**。
1. 选择&#x200B;**[!UICONTROL 为所有用户安装]** （推荐），然后单击&#x200B;**[!UICONTROL 安装]**。

1. （视情况而定）如果询问您是否要批准第三方访问权限，则必须选择&#x200B;**[!UICONTROL 是，授予对这些第三方网站的访问权限]**，然后单击&#x200B;**[!UICONTROL 继续]**。

1. 安装完成后，单击&#x200B;**[!UICONTROL 完成]**。

   [!DNL Workfront]应用列在&#x200B;**[!UICONTROL 已安装的包]**&#x200B;下。


1. 导航到&#x200B;**[!UICONTROL 设置>安全控制>远程站点设置]**。
1. （视情况而定）如果在[!DNL Workfront]所有远程站点&#x200B;**[!UICONTROL 列表中未列出您的]** URL，请单击&#x200B;**[!UICONTROL 新建远程站点]**。

1. （视情况而定）如果添加站点，请指定&#x200B;**[!UICONTROL 远程站点名称]**。
例如，*[!DNL Workfront]*。

1. （视情况而定）如果添加站点，请指定&#x200B;**[!UICONTROL 远程站点URL]**。
例如，*yourDomain.my.workfront.com*。

1. 单击&#x200B;**[!UICONTROL 保存]**。\
   [!DNL Workfront]应用现已安装在您的[!DNL Salesforce]实例上。 已在您的环境中创建&#x200B;**[!UICONTROL WorkfrontOpportunities]**&#x200B;和&#x200B;**[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce]页面。\
   在将[!DNL Salesforce]部分添加到其[!DNL Workfront]机会[!UICONTROL 或]帐户[!UICONTROL 页面布局之前，]用户尚不能使用应用程序。\
   有关为用户配置[!DNL Workfront]节的信息，请参阅[为 [!DNL Adobe Workfront] 用户配置 [!DNL Salesforce] 节](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

### 在[!DNL Workfront for Salesforce]框架中安装[!DNL Salesforce Lightning Experience]

1. 以系统管理员身份登录到[!DNL Salesforce]。
1. 单击&#x200B;**[!UICONTROL 设置]图标**，然后单击&#x200B;**[!UICONTROL 设置]**。

1. 在&#x200B;**[!UICONTROL 平台工具]**&#x200B;部分中，展开&#x200B;**[!UICONTROL 应用程序].**

1. 单击 **[!DNL AppExchange Marketplace]**。
1. 在&#x200B;**[!UICONTROL 搜索[!DNL AppExchange]应用]**&#x200B;框中，键入&#x200B;**[!DNL Workfront]**。

1. 找到该Workfront应用后单击该应用，然后单击&#x200B;**立即获取**。
1. 单击&#x200B;**[!UICONTROL 打开登录屏幕]**。\
   您必须使用[!DNL Workfront]的[!DNL Salesforce]管理员帐户登录。

1. 单击&#x200B;**[!UICONTROL 允许]**。
1. 在“**[!UICONTROL 在此组织中安装]**”框中，单击“**[!UICONTROL 在此处安装]**”以在[!DNL Workfront]生产环境中安装[!DNL Salesforce]。 （推荐）

1. 阅读并同意条款和条件后，请启用&#x200B;**[!UICONTROL 我已阅读并同意条款和条件]**&#x200B;字段。
1. 单击&#x200B;**[!UICONTROL 确认并安装]**。
1. 选择&#x200B;**[!UICONTROL 为所有用户安装]** （推荐），然后单击&#x200B;**[!UICONTROL 安装]**。

1. （视情况而定）如果询问您是否要批准第三方访问权限，则必须选择&#x200B;**[!UICONTROL 是，授予对这些第三方网站的访问权限]**，然后单击&#x200B;**[!UICONTROL 继续]**。

1. 安装完成后，单击&#x200B;**[!UICONTROL 完成]**。

   [!DNL Workfront]应用列在&#x200B;**[!UICONTROL 已安装的包]**&#x200B;下。

1. 导航到&#x200B;**[!UICONTROL 安装程序].**
1. 在&#x200B;**[!UICONTROL 设置]**&#x200B;部分中，展开&#x200B;**[!UICONTROL 安全性].**

1. 单击&#x200B;**[!UICONTROL 远程站点设置]**。
1. （视情况而定）如果在[!DNL Workfront]所有远程站点&#x200B;**[!UICONTROL 列表中未列出您的]** URL，请单击&#x200B;**[!UICONTROL 新建远程站点]**。

1. （视情况而定）如果添加站点，请指定&#x200B;**[!UICONTROL 远程站点名称]**。
例如，*[!DNL Workfront]*。

1. （视情况而定）如果添加站点，请指定&#x200B;**[!UICONTROL 远程站点URL]**。
例如，*yourDomain.my.workfront.com*。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   [!DNL Workfront]应用现已安装在您的[!DNL Salesforce]实例上，并且&#x200B;**[!DNL Workfront]**&#x200B;组件现已添加到您的环境中。

   将[!UICONTROL 部分添加到其]Opportunity[!DNL Workfront]或[!DNL Workfront]Account[!UICONTROL 页面布局后，]Salesforce[!UICONTROL 用户可以使用]应用。\
   有关为用户配置[!DNL Workfront]节的信息，请参阅[为 [!DNL Adobe Workfront] 用户配置 [!DNL Salesforce] 节](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

## 为Workfront配置权限以进行Salesforce集成

### `workfront_business`的权限

1. 导航到&#x200B;**设置** > **安全性** > **受信任的URL**。
1. 从列表中选择`workfront_business`。
1. 单击&#x200B;**编辑**。
1. 在CSP指令下，选中以下选项：

   * connect-src（脚本）
   * font-src（字体）
   * frame-src（iframe内容）
   * img-src（图像）
   * media-src（音频和视频）
   * style-src（样式表）

1. 单击&#x200B;**保存**。


### workfront_session的权限

1. 导航到&#x200B;**设置** > **安全性** > **受信任的URL**。
1. 从列表中选择`workfront_session`。
1. 单击&#x200B;**编辑**。
1. 在CSP指令下，选中以下选项：

   * connect-src（脚本）
   * font-src（字体）
   * frame-src（iframe内容）
   * img-src（图像）
   * media-src（音频和视频）
   * style-src（样式表）

1. 单击&#x200B;**保存**。

