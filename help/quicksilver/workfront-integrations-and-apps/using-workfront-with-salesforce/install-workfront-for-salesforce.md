---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 安装 [!DNL Adobe Workfront] 表示 [!DNL Salesforce]
description: 要在应用程序在 [!DNL Salesforce] AppExchange，请参阅安装 [!DNL Workfront] (在AppExchange市场中可用之前)
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 1%

---

# 安装 [!DNL Adobe Workfront for Salesforce]

要在应用程序在 [!DNL Salesforce AppExchange]，请参阅 [安装 [!DNL Workfront for Salesforce] 在 [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

As a [!DNL Salesforce] 和 [!DNL Adobe Workfront] 管理员，您可以安装 [!DNL Workfront for Salesforce] 允许 [!DNL Salesforce] 用户提交 [!DNL Workfront] 无需离开Salesforce即可请求和自动创建项目。

了解有关通过安装 [!DNL Workfront for Salesforce]，请参阅 [[!DNL Adobe Workfront for Salesforce] 概述](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [安装和使用的先决条件 [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce-prerequisites-for-installing-and-using-workfront-for-salesforce)
* [正在安装 [!DNL Workfront for Salesforce]](#install-adobe-workfront-for-salesforce)

## 访问要求

您必须具有以下访问权限才能使用本文中描述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL计划]</p> </td> 
  </tr>  </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 安装和使用的先决条件 [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* 您必须具有 [!DNL Salesforce] 具有系统管理员帐户访问权限的实例来安装应用程序。
* 您必须具有 [!DNL Workfront] 具有系统管理员帐户访问权限的实例来配置集成。
* [!UICONTROL Salesforce] 用户必须具有 [!DNL Workfront] 帐户

   * 创建 [!DNL Workfront] 请求 [!DNL Salesforce] 或
   * 查看 [!DNL Workfront] 请求或Salesforce中的项目。

## 正在安装 [!DNL Workfrontfor Salesforce] {#installing-workfront-for-salesforce}

你必须是 [!DNL Salesforce] 和 [!DNL Workfront] 系统管理员安装和配置 [!DNL Workfront for Salesforce].

以下子部分介绍了如何安装 [!DNL Workfront] , [!DNL Salesforce] 生产环境。 您可以按照相同的步骤进行安装 [!DNL Workfront] , [!DNL Salesforce] 沙盒环境。

* [安装 [!DNL Workfront for Salesforce] 在 [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [安装 [!DNL Workfront for Salesforce] 在 [!DNL Salesforce Classic] 框架](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [安装 [!DNL Workfront for Salesforce] 在 [!DNL Salesforce Lightning Experience] 框架](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### 安装 [!DNL Workfront for Salesforce] 在 [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] 将在 [!DNL Salesforce AppExchange] 很快。

要在应用程序可用之前安装该应用程序，请执行以下操作：

1. 在生产环境中，转到

   `https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002aUZY`

   在沙盒环境中，转到

   `https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002aUZY`

1. 检查 **[!UICONTROL 是，授予对这些第三方网站的访问权限]** 框中。

   此时会显示加载屏幕，安装过程可能需要一些时间。

1. 单击 **[!UICONTROL 完成]** 安装完成后。

1. 导航到 **[!UICONTROL 设置>安全控制>远程站点设置]**.
1. （视情况而定）如果您没有看到 [!DNL Workfront] 在 **[!UICONTROL 所有远程站点]** 列表，单击 **[!UICONTROL 新建远程站点]**.

1. 指定 **[!UICONTROL 远程站点名称]**.

   例如， *[!DNL Workfront]*.

1. 指定 **[!UICONTROL 远程站点URL]**.

   例如， *yourDomain.my.workfront.com*.

1. 单击&#x200B;**[!UICONTROL 保存]**。

   的 [!DNL Workfront] 现在，您的 [!DNL Salesforce] 实例和 **[!UICONTROL WorkfrontOpportunities]** 和 **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] 已在您的环境中创建页面。

   [!DNL Salesforce] 添加 [!DNL Workfront] 部分 [!UICONTROL 机会] 或 [!UICONTROL 帐户] 页面布局。\
   有关为用户配置Workfront部分的信息，请参阅 [为Salesforce用户配置Adobe Workfront部分](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### 安装 [!DNL Workfront] 表示 [!DNL Salesforce] 在 [!DNL Salesforce Classic] 框架

1. 登录到 [!DNL Salesforce] 作为系统管理员。
1. 转到 **设置。**
1. 在 **生成** ，单击 **AppExchange市场**.

1. 在 **搜索AppExchange应用程序** 框，文字 **Workfront**.

1. 找到应用程序后，单击该应用程序，然后单击 **立即获取**.
1. 单击 **[!UICONTROL 在生产环境中安装]** 安装 [!DNL Workfront] 应用程序 [!DNL Salesforce] 生产环境。 （推荐）
1. 选择 **[!UICONTROL 我已阅读并同意了条款和条件]** 字段，以获取相关信息。
1. 单击 **[!UICONTROL 确认和安装]**.
1. 选择 **[!UICONTROL 为所有用户安装]** （推荐），然后单击 **[!UICONTROL 安装]**.

1. （视情况而定）如果询问您是否要批准第三方访问，则必须选择 **[!UICONTROL 是，授予对这些第三方网站的访问权限]**，然后单击 **[!UICONTROL 继续]**.

1. 单击 **[!UICONTROL 完成]** 安装完成后。

   的 [!DNL Workfront] 应用程序列在 **[!UICONTROL 已安装的包]**.


1. 导航到 **[!UICONTROL 设置>安全控制>远程站点设置]**.
1. （视情况而定）如果您没有看到 [!DNL Workfront] 在 **[!UICONTROL 所有远程站点]** 列表，单击 **[!UICONTROL 新建远程站点]**.\

1. 指定 **[!UICONTROL 远程站点名称]**.\
   例如， *[!DNL Workfront]*.

1. 指定 **[!UICONTROL 远程站点URL]**.\
   例如， *yourDomain.my.workfront.com*.

1. 单击&#x200B;**[!UICONTROL 保存]**。\
   的 [!DNL Workfront] 现在，您的 [!DNL Salesforce] 实例和 **[!UICONTROL WorkfrontOpportunities]** 和 **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] 已在您的环境中创建页面。\
   [!DNL Salesforce] 在您添加 [!DNL Workfront] 部分 [!UICONTROL 机会] 或 [!UICONTROL 帐户] 页面布局。\
   有关配置 [!DNL Workfront] 部分，请参阅 [配置 [!DNL Adobe Workfront] 部分 [!DNL Salesforce] 用户](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### 安装 [!DNL Workfront for Salesforce] 在 [!DNL Salesforce Lightning Experience] 框架

1. 登录到 [!DNL Salesforce] 作为系统管理员。
1. 单击 **[!UICONTROL 设置] 图标**，然后单击 **[!UICONTROL 设置]**.

1. 在 **[!UICONTROL 平台工具]** 部分，展开 **[!UICONTROL 应用程序].**

1. 单击 **[!DNL AppExchange Marketplace]**.
1. 在 **[!UICONTROL 搜索 [!DNL AppExchange] 应用程序]** 框，文字 **[!DNL Workfront]**.

1. 找到应用程序后，单击该应用程序，然后单击 **[!UICONTROL 立即获取]**.
1. 单击 **[!UICONTROL 打开登录屏幕]**.\
   您必须使用 [!DNL Workfront] 管理员帐户 [!DNL Salesforce].

1. 单击 **[!UICONTROL 允许]**.
1. 在 **[!UICONTROL 在此组织中安装]** 框，单击 **[!UICONTROL 在此处安装]** 安装 [!DNL Workfront] 在 [!DNL Salesforce] 生产环境。 （推荐）

1. 选择 **[!UICONTROL 我已阅读并同意了条款和条件]** 字段，以获取相关信息。
1. 单击 **[!UICONTROL 确认和安装]**.
1. 选择 **[!UICONTROL 为所有用户安装]** （推荐），然后单击 **[!UICONTROL 安装]**.

1. （视情况而定）如果询问您是否要批准第三方访问，则必须选择 **[!UICONTROL 是，授予对这些第三方网站的访问权限]**，然后单击 **[!UICONTROL 继续]**.

1. 单击 **[!UICONTROL 完成]** 安装完成后。

   的 [!DNL Workfront] 应用程序列在 **[!UICONTROL 已安装的包]**.

1. 导航到 **[!UICONTROL 设置].**
1. 在 **[!UICONTROL 设置]** 部分，展&#x200B;开&#x200B;**[!UICONTROL 安全性].**

1. 单击 **[!UICONTROL 远程站点设置]**.
1. （视情况而定）如果您没有看到 [!DNL Workfront] 在 **[!UICONTROL 所有远程站点]** 列表，单击 **[!UICONTROL 新建远程站点]**.

1. 指定 **[!UICONTROL 远程站点名称]**.

   例如， *[!DNL Workfront]*.

1. 指定 **[!UICONTROL 远程站点URL]**.

   例如， *yourDomain.my.workfront.com*.

1. 单击&#x200B;**[!UICONTROL 保存]**。

   的 [!DNL Workfront] 现在，您的 [!DNL Salesforce] 实例和 **[!DNL Workfront]** 组件现已添加到您的环境中。

   [!UICONTROL Salesforce] 用户可以使用 [!DNL Workfront] 添加 [!DNL Workfront] 部分 [!UICONTROL 机会] 或 [!UICONTROL 帐户] 页面布局。\
   有关配置 [!DNL Workfront] 部分，请参阅 [配置 [!DNL Adobe Workfront] 部分 [!DNL Salesforce] 用户](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
