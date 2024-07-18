---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: 为 [!DNL Salesforce] 个用户配置 [!DNL Adobe Workfront] 部分
description: 在以 [!DNL Workfront] 管理员身份安装Salesforce的 [!DNL Adobe Workfront] 后，您可以将其添加到用户在Salesforce中的Opportunity和Account页面布局的新分区中，以使其对用户可用。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 1%

---

# 为[!DNL Salesforce]用户配置[!DNL Adobe Workfront]部分

需要[!UICONTROL Pro] [!DNL Workfront]计划才能使用此功能。 有关各种可用计划的详细信息，请参阅[[!DNL Workfront] 计划。](https://www.workfront.com/plans)

在以[!DNL Workfront]管理员身份安装[!DNL Salesforce]的[!DNL Adobe Workfront]后，您可以通过将其添加到用户的[!UICONTROL Opportunity]和[!UICONTROL Account]的新分区中，使其可供用户使用
[!UICONTROL Salesforce]中的页面布局。

有关安装[!DNL Workfront for Salesforce]的信息，请参阅[安装 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)。

对于同时在[!DNL Classic]和[!DNL Lightning Experience]框架中具有[!DNL Workfront]的用户，必须将[!DNL WorkfrontOpportunities]和[!DNL WorkfrontAccounts] [!UICONTROL Visualforce]页面分别添加到[!UICONTROL Opportunity]和[!UICONTROL Accounts]页面布局。

## 访问要求

您必须具有以下权限才能使用本文中所述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 先决条件

* 您必须拥有有权访问系统管理员帐户的[!DNL Salesforce]实例。
* 您必须拥有有权访问系统管理员帐户的[!DNL Workfront]实例。

## 在[!DNL Salesforce Classic]框架中配置[!DNL Workfront]部分

1. 以Workfront管理员身份登录到[!DNL Salesforce]。
1. 单击&#x200B;**[!UICONTROL 设置].**
1. 在&#x200B;**[!UICONTROL 生成]**&#x200B;部分中，展开&#x200B;**[!UICONTROL 自定义].**

1. 展开&#x200B;**[!UICONTROL Opportunities]**，然后单击&#x200B;**[!UICONTROL 页面布局]**&#x200B;以将[!DNL Workfront]部分添加到Opportunity。

   或

   展开&#x200B;**[!UICONTROL 帐户]**，然后单击&#x200B;**[!UICONTROL 页面布局]**&#x200B;以将[!DNL Workfront]部分添加到帐户
.

1. 在现有布局上单击&#x200B;**[!UICONTROL 编辑]**。

   或

   单击&#x200B;**[!UICONTROL 新建]**&#x200B;以添加新布局。

1. （可选）将&#x200B;**[!UICONTROL Section]**&#x200B;组件拖到布局中，并将其放到所需位置。\

1. （可选）为新节指定名称。

   我们建议您将此分区命名为&#x200B;**[!DNL Workfront]**。

1. （可选）为新节指定所需的&#x200B;**[!UICONTROL 布局]**&#x200B;和&#x200B;**[!UICONTROL Tab键顺序]**。

   我们建议您为[!DNL Workfront]分区选择&#x200B;**[!UICONTROL 1 — 列]**&#x200B;布局。

1. 单击&#x200B;**[!UICONTROL 确定]**。
1. 在&#x200B;**[!UICONTROL 布局]**&#x200B;区域中，单击&#x200B;**[!UICONTROL Visualforce页面].**

1. 将&#x200B;**[!UICONTROL WorkfrontOpportunities]**&#x200B;组件拖放到&#x200B;**[!UICONTROL Opportunities]**&#x200B;布局中的新分区。

   或

   将&#x200B;**[!UICONTROL WorkfrontAccounts]**&#x200B;组件拖放到&#x200B;**[!UICONTROL 帐户]**&#x200B;布局中的新分区。\

1. 单击新添加的组件右上角的&#x200B;**[!UICONTROL 属性]**&#x200B;图标。\

1. 要获得最佳显示，请为[!DNL Workfront Visualforce]页面指定以下属性：

   * **[!UICONTROL 宽度（以像素或%为单位）]**： 100%
   * **[!UICONTROL 高度（以像素为单位）]**： 600
   * 选择&#x200B;**[!UICONTROL 显示滚动条]**。

1. 单击&#x200B;**[!UICONTROL 确定]**。
1. 单击&#x200B;**[!UICONTROL 保存]**&#x200B;以保存布局。

   现在，所有已为其分配此布局的用户都可以在其[!UICONTROL 机会]或[!UICONTROL 帐户]对象上看到[!DNL Workfront]部分。

   用户在[!DNL Workfront]部分看到[!DNL Workfront]登录屏幕。 如果他们没有[!DNL Workfront]帐户，则可以折叠该部分，但不会将其从布局中删除。

## 在[!DNL Salesforce Lightning Experience]框架中配置[!DNL Workfront]部分

您可以将[!DNL Workfront]部分添加到[!DNL Salesforce] [!UICONTROL 机会]或帐户的布局中
通过访问[!UICONTROL Setup]区域或帐户在[!DNL Salesforce Lightning Experience]框架中
或[!UICONTROL 机会]对象。

* [在[!UICONTROL 设置]级别配置 [!DNL Workfront] 部分](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [在机会或帐户级别配置 [!DNL Workfront] 部分](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### 在[!UICONTROL 设置]级别配置[!DNL Workfront]部分 {#configure-the-workfront-section-at-the-setup-level}

1. 以系统管理员身份登录[!DNL Salesforce]。
1. 单击&#x200B;**[!UICONTROL 设置]**&#x200B;图标，然后单击&#x200B;**[!UICONTROL 设置]**。

1. 展开&#x200B;**[!UICONTROL 对象和字段]**，然后单击&#x200B;**[!UICONTROL 对象管理器]**。

1. 单击&#x200B;**[!UICONTROL Opportunity]**&#x200B;以自定义Opportunity的布局。

   或

   单击&#x200B;**[!UICONTROL 帐户]**&#x200B;以自定义帐户的布局。

1. 单击&#x200B;**[!UICONTROL 页面布局]**。
1. 单击现有页面布局的名称以对其进行编辑。

   或

   单击&#x200B;**[!UICONTROL 新建]**&#x200B;以创建新的页面布局。

1. 继续[在下面的机会或帐户级别](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)配置 [!DNL Workfront] 部分。

### 在机会或帐户级别配置[!DNL Workfront]部分 {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. 以系统管理员身份登录到[!DNL Salesforce]。
1. 转到&#x200B;**[!UICONTROL 机会]**&#x200B;或&#x200B;**[!UICONTROL 帐户]**。

1. 单击&#x200B;**[!UICONTROL 设置]**&#x200B;图标，然后单击&#x200B;**[!UICONTROL 编辑页面]**。\

1. 展开&#x200B;**[!UICONTROL Custom-Managed]**&#x200B;部分。
1. 将&#x200B;**[!DNL Workfront]**&#x200B;组件拖放到您的[!UICONTROL 机会]或帐户上
页面。

   我们建议对[!DNL Workfront]部分使用页面的完整宽度，而不是布局的其中一列。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   现在，所有已为其分配此布局的用户都可以在其[!UICONTROL 机会]或[!UICONTROL 帐户]对象上看到[!DNL Workfront]部分。

   >[!NOTE]
   >
   >用户在[!DNL Workfront]部分看到[!DNL Workfront]登录屏幕。 如果他们没有[!DNL Workfront]帐户，则可以折叠该部分，但不会将其从布局中删除。 用户可以使用您启用的身份验证方法登录：增强型身份验证或您的安全断言标记语言(SAML) URL。

