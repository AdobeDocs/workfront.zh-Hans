---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 安装 [!DNL Adobe Workfront] 对象 [!DNL Salesforce]
description: 在应用程序在中可用之前进行安装 [!DNL Salesforce] AppExchange，请参阅安装 [!DNL Workfront] 在Salesforce在AppExchange市场中可用之前提供。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 1%

---

# 安装 [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>在应用程序在中可用之前进行安装 [!DNL Salesforce AppExchange]，请参见 [安装 [!DNL Workfront for Salesforce] 使其在中可用之前 [!DNL AppExchange] 市场](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

作为 [!DNL Salesforce] 和 [!DNL Adobe Workfront] 管理员，您可以安装 [!DNL Workfront for Salesforce] 允许您的 [!DNL Salesforce] 要提交的用户 [!DNL Workfront] 请求并自动创建项目，而无需离开Salesforce。

大致了解安装后可获得的好处 [!DNL Workfront for Salesforce]，请参见 [[!DNL Adobe Workfront for Salesforce] 概述](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [安装和使用的先决条件 [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [安装 [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

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

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 安装和使用的先决条件 [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* 您必须拥有 [!DNL Salesforce] 具有系统管理员帐户访问权限的实例以安装应用程序。
* 您必须拥有 [!DNL Workfront] 具有系统管理员帐户访问权限的实例以配置集成。
* [!UICONTROL Salesforce] 用户必须具有 [!DNL Workfront] 帐户以便能够：

   * 创建 [!DNL Workfront] 请求自 [!DNL Salesforce]
   * 视图 [!DNL Workfront] Salesforce中的请求或项目

## 安装 [!DNL Workfront for Salesforce] {#installing-workfront-for-salesforce}

您必须是 [!DNL Salesforce] 和 [!DNL Workfront] 要安装和配置的系统管理员 [!DNL Workfront for Salesforce].

以下子部分介绍了如何安装 [!DNL Workfront] 您的 [!DNL Salesforce] 生产环境。 您可以按照相同的步骤进行安装 [!DNL Workfront] 您的 [!DNL Salesforce] 沙盒环境。

* [安装 [!DNL Workfront for Salesforce] 使其在中可用之前 [!DNL AppExchange] 市场](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [安装 [!DNL Workfront for Salesforce] 在 [!DNL Salesforce Classic] 框架](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [安装 [!DNL Workfront for Salesforce] 在 [!DNL Salesforce Lightning Experience] 框架](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### 安装 [!DNL Workfront for Salesforce] 使其在中可用之前 [!DNL AppExchange] 市场 {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] 将在 [!DNL Salesforce AppExchange] 很快。

在应用程序可用之前安装应用程序：

1. 在生产环境中，转到

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   在沙盒环境中，转到

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   >[!NOTE]
   >
   >您必须登录Salesforce才能访问这些页面。

1. 查看 **[!UICONTROL 是，授予对这些第三方网站的访问权限]** 盒子。

   此时将显示一个加载屏幕。 安装可能需要一些时间。

1. 单击 **[!UICONTROL 完成]** 安装完成时。

1. 导航到 **[!UICONTROL 设置]** > **[!UICONTROL 安全性] 控件** > **[!UICONTROL 远程站点设置]**.
1. （视情况而定）从列表中选择Workfront 。

   或

   如果您没有看到 [!DNL Workfront] URL列在 **[!UICONTROL 所有远程站点]** 列表，单击 **[!UICONTROL 新建远程站点]**.

1. （视情况而定）如果添加站点，请指定 **[!UICONTROL 远程站点名称]**.

   例如， *[!DNL Workfront]*.

1. （视情况而定）如果添加站点，请指定 **[!UICONTROL 远程站点URL]**.

   例如， *yourDomain.my.workfront.com*.

1. 单击&#x200B;**[!UICONTROL 保存]**。

   此 [!DNL Workfront] 应用程序现已安装在您的 [!DNL Salesforce] 实例和 **[!UICONTROL WorkfrontOpportunities]** 和 **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] 已在您的环境中创建页面。

   [!DNL Salesforce] 添加应用程序后，用户可以使用该应用程序。 [!DNL Workfront] 部分到其 [!UICONTROL 机会] 或 [!UICONTROL 帐户] 页面布局。\
   有关为用户配置Workfront部分的信息，请参阅 [为Salesforce用户配置Adobe Workfront部分](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### 安装 [!DNL Workfront] 对象 [!DNL Salesforce] 在 [!DNL Salesforce Classic] 框架

1. 登录 [!DNL Salesforce] 作为系统管理员。
1. 转到 **设置。**
1. 在 **生成** 部分，单击 **AppExchange市场**.

1. 在 **搜索AppExchange应用程序** 框，键入 **Workfront**.

1. 找到Workfront应用程序后，单击该应用程序，然后单击 **立即获取**.
1. 单击 **[!UICONTROL 在生产环境中安装]** 安装 [!DNL Workfront] 应用程序在您的 [!DNL Salesforce] 生产环境。 （推荐）
1. 阅读并同意条款和条件后，启用 **[!UICONTROL 我已阅读并同意相关条款和条件]** 字段。
1. 单击 **[!UICONTROL 确认并安装]**.
1. 选择 **[!UICONTROL 为所有用户安装]** （推荐），然后单击 **[!UICONTROL 安装]**.

1. （视情况而定）如果系统询问您是否要批准第三方访问，则必须选择 **[!UICONTROL 是，授予对这些第三方网站的访问权限]**，然后单击 **[!UICONTROL 继续]**.

1. 单击 **[!UICONTROL 完成]** 安装完成时。

   此 [!DNL Workfront] 应用程序列在 **[!UICONTROL 已安装的包]**.


1. 导航到 **[!UICONTROL “设置”>“安全控制”>“远程站点设置”]**.
1. （视情况而定）如果您没有看到 [!DNL Workfront] URL列在 **[!UICONTROL 所有远程站点]** 列表，单击 **[!UICONTROL 新建远程站点]**.

1. （视情况而定）如果添加站点，请指定 **[!UICONTROL 远程站点名称]**.
例如， *[!DNL Workfront]*.

1. （视情况而定）如果添加站点，请指定 **[!UICONTROL 远程站点URL]**.
例如， *yourDomain.my.workfront.com*.

1. 单击&#x200B;**[!UICONTROL 保存]**。\
   此 [!DNL Workfront] 应用程序现已安装在您的 [!DNL Salesforce] 实例。 此 **[!UICONTROL WorkfrontOpportunities]** 和 **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] 已在您的环境中创建页面。\
   [!DNL Salesforce] 在添加之前，用户尚不能使用应用程序。 [!DNL Workfront] 部分到其 [!UICONTROL 机会] 或 [!UICONTROL 帐户] 页面布局。\
   有关配置 [!DNL Workfront] 部分，有关用户，请参阅 [配置 [!DNL Adobe Workfront] 部分 [!DNL Salesforce] 用户](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### 安装 [!DNL Workfront for Salesforce] 在 [!DNL Salesforce Lightning Experience] 框架

1. 登录 [!DNL Salesforce] 作为系统管理员。
1. 单击 **[!UICONTROL 设置] 图标**，然后单击 **[!UICONTROL 设置]**.

1. 在 **[!UICONTROL 平台工具]** 部分，展开 **[!UICONTROL 应用程序].**

1. 单击 **[!DNL AppExchange Marketplace]**。
1. 在 **[!UICONTROL Search [!DNL AppExchange] 应用程序]** 框，键入 **[!DNL Workfront]**.

1. 找到Workfront应用程序后，单击该应用程序，然后单击 **立即获取**.
1. 单击 **[!UICONTROL 打开“登录”屏幕]**.\
   您必须使用您的 [!DNL Workfront] 管理员帐户 [!DNL Salesforce].

1. 单击 **[!UICONTROL 允许]**.
1. 在 **[!UICONTROL 在此组织中安装]** 框中，单击 **[!UICONTROL 在此处安装]** 安装 [!DNL Workfront] 在您的 [!DNL Salesforce] 生产环境。 （推荐）

1. 阅读并同意条款和条件后，启用 **[!UICONTROL 我已阅读并同意相关条款和条件]** 字段。
1. 单击 **[!UICONTROL 确认并安装]**.
1. 选择 **[!UICONTROL 为所有用户安装]** （推荐），然后单击 **[!UICONTROL 安装]**.

1. （视情况而定）如果系统询问您是否要批准第三方访问，则必须选择 **[!UICONTROL 是，授予对这些第三方网站的访问权限]**，然后单击 **[!UICONTROL 继续]**.

1. 单击 **[!UICONTROL 完成]** 安装完成时。

   此 [!DNL Workfront] 应用程序列在 **[!UICONTROL 已安装的包]**.

1. 导航到 **[!UICONTROL 设置].**
1. 在 **[!UICONTROL 设置]** 部分，展开 **[!UICONTROL 安全性].**

1. 单击 **[!UICONTROL 远程站点设置]**.
1. （视情况而定）如果您没有看到 [!DNL Workfront] URL列在 **[!UICONTROL 所有远程站点]** 列表，单击 **[!UICONTROL 新建远程站点]**.

1. （视情况而定）如果添加站点，请指定 **[!UICONTROL 远程站点名称]**.
例如， *[!DNL Workfront]*.

1. （视情况而定）如果添加站点，请指定 **[!UICONTROL 远程站点URL]**.
例如， *yourDomain.my.workfront.com*.

1. 单击&#x200B;**[!UICONTROL 保存]**。

   此 [!DNL Workfront] 应用程序现已安装在您的 [!DNL Salesforce] 实例，以及 **[!DNL Workfront]** 组件现已添加到环境中。

   [!UICONTROL Salesforce] 用户可以使用 [!DNL Workfront] 添加后应用程序 [!DNL Workfront] 部分到其 [!UICONTROL 机会] 或 [!UICONTROL 帐户] 页面布局。\
   有关配置 [!DNL Workfront] 部分，有关用户，请参阅 [配置 [!DNL Adobe Workfront] 部分 [!DNL Salesforce] 用户](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
