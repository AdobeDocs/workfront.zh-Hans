---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: 配置 [!DNL Adobe Workfront] 部分 [!DNL Salesforce] 用户
description: 安装后 [!DNL Adobe Workfront] 用于Salesforce as a [!DNL Workfront] 管理员，您可以通过在Salesforce中的“机会和帐户”页面布局的新部分中添加它，使其对用户可用。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 1%

---

# 配置 [!DNL Adobe Workfront] 部分 [!DNL Salesforce] 用户

A [!UICONTROL Pro] [!DNL Workfront] 使用此功能需要计划。 有关各种可用计划的更多信息，请参阅 [[!DNL Workfront] 计划。](https://www.workfront.com/plans)

安装后 [!DNL Adobe Workfront] 表示 [!DNL Salesforce] as a [!DNL Workfront] 管理员，您可以通过在用户的新部分中将其添加到 [!UICONTROL 机会] 和 [!UICONTROL 帐户]
页面布局 [!UICONTROL Salesforce].

有关安装的信息 [!DNL Workfront for Salesforce]，请参阅 [安装 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

对于用户， [!DNL Workfront] 在 [!DNL Classic] 和 [!DNL Lightning Experience] 框架中，您必须 [!DNL WorkfrontOpportunities] 和 [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] 页面 [!UICONTROL 机会] 和 [!UICONTROL 帐户] 页面布局。

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
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 先决条件

* 您必须具有 [!DNL Salesforce] 具有系统管理员帐户访问权限的实例。
* 您必须具有 [!DNL Workfront] 具有系统管理员帐户访问权限的实例。

## 配置 [!DNL Workfront] 部分 [!DNL Salesforce Classic] 框架

1. 登录到 [!DNL Salesforce] 作为Workfront管理员。
1. 单击 **[!UICONTROL 设置].**
1. 在 **[!UICONTROL 生成]** 部分，展开 **[!UICONTROL 自定义].**

1. 展开 **[!UICONTROL 机会]**，然后单击 **[!UICONTROL 页面布局]** 添加 [!DNL Workfront] 部分到Opportunity。

   或

   展开 **[!UICONTROL 帐户]**，然后单击 **[!UICONTROL 页面布局]** 添加 [!DNL Workfront] 部分添加到帐户。

1. 单击 **[!UICONTROL 编辑]** 在现有布局中。

   或

   单击 **[!UICONTROL 新建]** 以添加新布局。

1. （可选）将 **[!UICONTROL 区域]** 组件，并将其放置到所需位置。\

1. （可选）为新部分指定名称。

   我们建议您将此部分命名为 **[!DNL Workfront]**.

1. （可选）指定所需的 **[!UICONTROL 布局]** 和 **[!UICONTROL Tab键顺序]** ，以查看新章节。

   我们建议您选择 **[!UICONTROL 1列]** 布局 [!DNL Workfront] 中。

1. 单击 **[!UICONTROL 确定]**.
1. 在 **[!UICONTROL 布局]** 区域，单击 **[!UICONTROL 可视化强制页面].**

1. 拖放 **[!UICONTROL WorkfrontOpportunities]** 组件添加到 **[!UICONTROL 机会]** 布局。

   或

   拖放 **[!UICONTROL WorkfrontAccounts]** 组件添加到  **[!UICONTROL 帐户]** 布局。\

1. 单击 **[!UICONTROL 属性]** 图标。\

1. 要获得最佳显示，请为 [!DNL Workfront Visualforce] 页面：

   * **[!UICONTROL 宽度（以像素或%为单位）]**:100%
   * **[!UICONTROL 高度（像素）]**:600
   * 选择 **[!UICONTROL 显示滚动条]**.

1. 单击 **[!UICONTROL 确定]**.
1. 单击 **[!UICONTROL 保存]** 以保存布局。

   现在，所有已分配此布局的用户都能够查看 [!DNL Workfront] 部分 [!UICONTROL 机会] 或 [!UICONTROL 帐户] 对象。

   用户会看到 [!DNL Workfront] 登录屏幕 [!DNL Workfront] 中。 如果他们没有 [!DNL Workfront] 帐户，则他们可以折叠部分，但不能将其从布局中删除。

## 配置 [!DNL Workfront] 部分 [!DNL Salesforce Lightning Experience] 框架

您可以将 [!DNL Workfront] 的版面 [!DNL Salesforce] [!UICONTROL 机会] 或 [!DNL Salesforce Lightning Experience] 框架 [!UICONTROL 设置] 区域，或帐户或 [!UICONTROL 机会] 对象。

* [配置 [!DNL Workfront] 部分 [!UICONTROL 设置] 级别](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [配置 [!DNL Workfront] Opportunity或Account级别的部分](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### 配置 [!DNL Workfront] 部分 [!UICONTROL 设置] 级别 {#configure-the-workfront-section-at-the-setup-level}

1. 登录 [!DNL Salesforce] 作为系统管理员。
1. 单击 **[!UICONTROL 设置]** 图标，然后单击 **[!UICONTROL 设置]**.

1. 展开 **[!UICONTROL 对象和字段]**，然后单击 **[!UICONTROL 对象管理器]**.

1. 单击 **[!UICONTROL 机会]** 自定义Opportunity的布局。

   或

   单击 **[!UICONTROL 帐户]** 自定义帐户的布局。

1. 单击 **[!UICONTROL 页面布局]**.
1. 单击现有页面布局的名称以对其进行编辑。

   或

   单击 **[!UICONTROL 新建]** 创建新页面布局。

1. 继续 [配置 [!DNL Workfront] Opportunity或Account级别的部分](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) 下。

### 配置 [!DNL Workfront] Opportunity或Account级别的部分 {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. 登录到 [!DNL Salesforce] 作为系统管理员。
1. 转到 **[!UICONTROL 机会]** 或 **[!UICONTROL 帐户]**.

1. 单击 **[!UICONTROL 设置]** 图标，然后单击 **[!UICONTROL 编辑页面]**.\

1. 展开 **[!UICONTROL 自定义管理]** 中。
1. 拖放 **[!DNL Workfront]** 组件 [!UICONTROL 机会] 或帐户页面。

   我们建议将页面的全宽度用于 [!DNL Workfront] 部分而不是布局的列之一。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   现在，所有已分配此布局的用户都能够查看 [!DNL Workfront] 部分 [!UICONTROL 机会] 或 [!UICONTROL 帐户] 对象。

   >[!NOTE]
   >
   >用户会看到 [!DNL Workfront] 登录屏幕 [!DNL Workfront] 中。 如果他们没有 [!DNL Workfront] 帐户，则他们可以折叠部分，但不能将其从布局中删除。 用户可以使用您已启用的身份验证方法登录：增强的身份验证或您的安全断言标记语言(SAML)URL。

