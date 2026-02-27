---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: 为 [!DNL Adobe Workfront] 个用户配置 [!DNL Salesforce] 部分
description: 在安装 [!DNL Adobe Workfront] 以管理员 [!DNL Workfront] 身份使用Salesforce后，您可以通过将其添加到Salesforce中Opportunity和Account页面布局的新分区中，使其对用户可用。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: 6af620284ed9c710196d8976a9f6cac1b3b36cf1
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 0%

---

# 为[!DNL Adobe Workfront]用户配置[!DNL Salesforce]部分

>[!IMPORTANT]
>
>为了提供更稳定、更可扩展的集成，我们已转为使用Workfront自动化与集成(Fusion)的现代、灵活集成方法。 在此过渡过程中，Workfront for Salesforce集成&#x200B;**不再可用**。
>
>为了满足贵组织与Salesforce的集成需求，我们建议使用Workfront自动化和集成。
>
>有关Workfront自动化和集成的概述，请参阅[Adobe Workfront Fusion概述](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>有关Salesforce的Workfront自动化和集成模块的特定功能的信息，请参阅[Salesforce模块](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules)。

<!--

After you install [!DNL Adobe Workfront] for [!DNL Salesforce] as a [!DNL Workfront] administrator, you can make it available to your users by adding it in a new section to their [!UICONTROL Opportunity] and [!UICONTROL Account]
 page layouts in [!UICONTROL Salesforce]. 

For information about installing [!DNL Workfront for Salesforce], see [Install [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

For users to have [!DNL Workfront] available in both the [!DNL Classic] and [!DNL Lightning Experience] frameworks, you must add the [!DNL WorkfrontOpportunities] and the [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] pages to the [!UICONTROL Opportunity] and [!UICONTROL Accounts] page layouts, respectively.



## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

* You must have a [!DNL Salesforce] instance with access to a system administrator account.
* You must have a [!DNL Workfront] instance with access to a system administrator account.

## Configure the [!DNL Workfront] section in the [!DNL Salesforce Classic] framework

1. Log in to [!DNL Salesforce] as a Workfront administrator.
1. Click **[!UICONTROL Setup].**
1. In the **[!UICONTROL Build]** section, expand **[!UICONTROL Customize].**

1. Expand **[!UICONTROL Opportunities]**, then click **[!UICONTROL Page Layouts]** to add the [!DNL Workfront] section to an Opportunity.

   Or

   Expand **[!UICONTROL Accounts]**, then click **[!UICONTROL Page Layouts]** to add the [!DNL Workfront] section to an Account
.

1. Click **[!UICONTROL Edit]** on an existing layout.

   Or

   Click **[!UICONTROL New]** to add a new layout. 

1. (Optional) Drag the **[!UICONTROL Section]** component to the layout and drop it in the desired position.\

1. (Optional) Specify a name for the new section.

   We recommend that you name this section **[!DNL Workfront]**.

1. (Optional) Specify the desired **[!UICONTROL Layout]** and **[!UICONTROL Tab-key Order]** for the new section.

   We recommend that you select **[!UICONTROL 1-Column]** layout for the [!DNL Workfront] section. 

1. Click **[!UICONTROL OK]**.
1. In the **[!UICONTROL Layout]** area, click **[!UICONTROL Visualforce Pages].**

1. Drag and drop the **[!UICONTROL WorkfrontOpportunities]** component to the new section in the **[!UICONTROL Opportunities]** Layout.

   Or

   Drag and drop the **[!UICONTROL WorkfrontAccounts]** component to the new section in the  **[!UICONTROL Account]** Layout.\

1. Click the **[!UICONTROL Properties]** icon in the upper right of the newly added component.\

1. To achieve an optimal display, specify the following properties for the [!DNL Workfront Visualforce] page:

   * **[!UICONTROL Width (in pixels or %)]**: 100%
   * **[!UICONTROL Height (in pixels)]**: 600
   * Select **[!UICONTROL Show scrollbars]**.

1. Click **[!UICONTROL OK]**. 
1. Click **[!UICONTROL Save]** to save your layout.

   All users who have this layout assigned to them are now able to see the [!DNL Workfront] section on their [!UICONTROL Opportunities] or [!UICONTROL Accounts] objects.

   Users see a [!DNL Workfront] login screen on the [!DNL Workfront] section. If they do not have a [!DNL Workfront] account, they can collapse the section, but not remove it from their layout. 

## Configure the [!DNL Workfront] section in the [!DNL Salesforce Lightning Experience] framework

You can add the [!DNL Workfront] section to the layout of a [!DNL Salesforce] [!UICONTROL Opportunity] or Account
 in the [!DNL Salesforce Lightning Experience] framework either by accessing the [!UICONTROL Setup] area, or from an Account
 or [!UICONTROL Opportunity] object. 

* [Configure the [!DNL Workfront] section at the [!UICONTROL Setup] level](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Configure the [!DNL Workfront] Section at the Opportunity or Account level](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Configure the [!DNL Workfront] section at the [!UICONTROL Setup] level {#configure-the-workfront-section-at-the-setup-level}

1. Log into [!DNL Salesforce] as a system administrator. 
1. Click the **[!UICONTROL Setup]** icon, then click **[!UICONTROL Setup]**.

1. Expand **[!UICONTROL Object and Fields]**, then click **[!UICONTROL Object Manager]**.

1. Click **[!UICONTROL Opportunity]** to customize the layout of an Opportunity.

   Or

   Click **[!UICONTROL Account]** to customize the layout of an Account.

1. Click **[!UICONTROL Page Layouts]**.
1. Click the name of an existing page layout to edit it.

   Or

   Click **[!UICONTROL New]** to create a new page layout.

1. Continue with [Configure the [!DNL Workfront] Section at the Opportunity or Account level](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) below.

### Configure the [!DNL Workfront] Section at the Opportunity or Account level {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Log in to [!DNL Salesforce] as a system administrator. 
1. Go to an **[!UICONTROL Opportunity]** or **[!UICONTROL Account]**.

1. Click the **[!UICONTROL Setup]** icon, then click **[!UICONTROL Edit Page]**.

1. Expand the **[!UICONTROL Custom-Managed]** section.
1. Drag and drop the **[!DNL Workfront]** component on your [!UICONTROL Opportunity] or Account
 page.

   We recommend using the full width of the page for the [!DNL Workfront] section instead of one of the columns of the layout.

1. Click **[!UICONTROL Save]**.

   All users who have this layout assigned to them are now able to see the [!DNL Workfront] section on their [!UICONTROL Opportunities] or [!UICONTROL Accounts] objects.

   >[!NOTE]
   >
   >Users see a [!DNL Workfront] login screen on the [!DNL Workfront] section. If they do not have a [!DNL Workfront] account, they can collapse the section, but not remove it from their layout. Users can log in using the authentication method you have enabled: Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.

   -->

