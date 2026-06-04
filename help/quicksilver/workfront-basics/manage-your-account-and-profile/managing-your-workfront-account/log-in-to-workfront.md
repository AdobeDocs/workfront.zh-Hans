---
product-area: user-management
navigation-topic: manage-your-workfront-account
title: 登录到 [!DNL Adobe Workfront]
description: 阅读本文以了解如何登录Workfront。
author: Courtney
feature: Get Started with Workfront
exl-id: 69297cca-6b28-47d6-a478-8ac2bc29b959
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/2YH5Y7yvmUdpuV-p5cnrVSmXBQTjix2pMyUP5o-WKpU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d8302c96-f652-4d09-896b-19a70bab02a5
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 222
ht-degree: 5%

---

# 登录 [!DNL Adobe Workfront]

<!--Audited: 2024-->

一个登录用于Workfront和所有Adobe CX Enterprise应用程序。

有关信息，请参阅[CX Enterprise界面和管理](https://experienceleague.adobe.com/zh-hans/docs/core-services/interface/experience-cloud)。

## 访问[!DNL Workfront]

登录到CX Enterprise后，您可以通过单击顶部导航区域中的组织切换器，查看您有权访问的所有[!DNL Workfront]组织和环境。 选择要使用的[!DNL Workfront]组织或环境。 如果您的组织使用[!UICONTROL 预览]和[!UICONTROL 沙盒]环境。

![查看[!DNL Workfront]组织和环境](assets/wf-org-instance-switcher-2026.png)

>[!NOTE]
>
>第一次登录到CX Enterprise时，组织将默认使用按字母顺序排列的第一个组织。 下次登录时，组织将默认为您访问的最后一个组织。

[!DNL Workfront]出现在您有权访问的CX Enterprise产品列表中。 您可以在CX Enterprise主页上的“快速访问”菜单中选择[!DNL Workfront]，或者使用产品切换器![产品切换器](assets/main-menu-icon.png)随时更改应用程序。

![选择[!DNL Workfront]以访问应用程序](assets/cx-enterprise-home-2026.png)

>[!NOTE]
>
>如果浏览器选项卡会话在您已打开Workfront的页面中过期，并且在另一个浏览器选项卡中处于活动状态Workfront会话，则您可以重新加载已过期的选项卡以重新打开Workfront页面。

<!--
>[!IMPORTANT]
>
>The procedure described on this page has been removed because it applied only to organizations that were not yet onboarded to the Adobe Admin Console. 
>
>All Workfront organizations have now been onboarded to the Adobe Admin Console.
-->

<!--DELETE ME MARCH 2026-->

<!--

{{important-not-on-aec}}

You need the following information to log in to [!DNL Adobe Workfront]:

* **A login URL:** This is your company's unique URL, which should have this format: **`yourCompanyDomain.my.workfront.com`**.\
   If you are set up for single sign-on (SSO), your URL might have been changed by your [!DNL Workfront] administrator. For more information about logging in to [!DNL Workfront] with SSO, see [Log in to [!DNL Workfront] with SSO](#log-in-to-workfront-with-sso) in this article.

   The domain name for your company is established by [!DNL Workfront]. To change your domain name, contact our Customer Support team. For information about how to contact our Customer Support team, see [Contact Customer Support](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

* **A username:** Your [!DNL Workfront] administrator sets up your user name.
* **A password:** If your system is not set up for SSO, you set up your [!DNL Workfront] password after receiving an email invitation from the [!DNL Workfront] administrator.

   For more information about logging in to [!DNL Workfront] with SSO, see [Log in to [!DNL Workfront] with SSO](#log-in-to-workfront-with-sso) in this article.

   For more information about receiving email invitations and creating a [!DNL Workfront] password, see [Receive email invitations and create a password for [!DNL Adobe Workfront]](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td> 
   <p>Contributor or higher</p>
   <p>Request or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Log in to [!DNL Workfront] without SSO

If your [!DNL Workfront] administrator did not set up [!DNL Workfront] to integrate with your SSO solution, you will need a new username and password for Workfront. For information about configuring Workfront to integrate with an SSO solution, see [Overview of single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

To log into [!DNL Workfront] using your [!DNL Workfront] username and password:

1. Open a browser window, then type in the unique URL of your company, which should have the following format: **`yourCompanyDomain.my.workfront.com`**.

   For more information about what browsers are supported for [!DNL Workfront], see [[!DNL Adobe Workfront] browser requirements](../../../workfront-basics/workfront-browser-requirements.md).

1. In the login screen, enter your username and password.

   Your username is typically the email address associated with your [!DNL Workfront] account. If you forgot your password, see [Reset your password](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

1. (Conditional) If your organization's [!DNL Workfront] login URL doesn't contain a domain, you must specify your domain in the [!UICONTROL Domain] field.
1. Click **[!UICONTROL Login]**.

## Log in to [!DNL Workfront] with SSO

If your [!DNL Workfront] administrator integrated [!DNL Workfront] with a single sign-on solution, you should contact them for the information needed for your logging in to [!DNL Workfront]. For more information about integrating Workfront with an SSO solution, see [Overview of single sign-on in [!DNL Adobe Workfront]](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

To log in to [!DNL Workfront] using your SSO username and password:

1. Open a browser window.

   For more information about what browsers are supported for [!DNL Workfront], see [[!DNL Adobe Workfront] browser requirements](../../../workfront-basics/workfront-browser-requirements.md).

1. Type the unique URL of your company.

   If your [!DNL Workfront] administrator did not change the default [!DNL Workfront] URL, it should have the following format:

   **`yourCompanyDomain.my.workfront.com`**

1. Your [!DNL Workfront] administrator can ensure that you have the correct URL.
1. On the login screen, enter your username and password.

   Your username and password are typically your network user name and password, which you use for all your applications. If you forgot your password or your user name, use the tools provided in your environment for resetting them, or contact your [!DNL Workfront] administrator.

   The look and feel of your login screen changes depending on what SSO solution you use and the way it was configured by your [!DNL Workfront] administrator.

1. Complete your login.

## Log in to the [!DNL Workfront] mobile app using company domain

1. Launch the [!DNL Workfront] mobile app, then click **Sign in with company domain**.

1. Type your organization's domain.

   This is the SAML domain if your organization is using SSO.

   >[!TIP]
   >
   >This is typically your company name. If you are unsure, contact your [!DNL Workfront] administrator
-->

<!--
1. Specify the [!DNL Workfront] URL for your company or the link to your SAML authentication portal.

   The [!DNL Workfront] URL should display in the following format:
   **`yourDomain.my.workfront.com`**

   For example:

   **`swains.my.workfront.com`**

1. If you are logging in with you SAML credentials, follow the login steps from your SAML authentication portal.

   Your [!DNL Workfront] administrator must enable SAML 2.0 authentication with the [!DNL Workfront] web application in order to log in with your SAML credentials. For information about how to enable SAML 2.0, see the section [Configure [!DNL Adobe Workfront] with SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#saml-with-workfront-web-app) in the article [Configure [!DNL Adobe Workfront] with SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md). If you cannot log in as described in this section, contact your Workfront administrator.

1. Tap **[!UICONTROL Continue in browser]**.
1. Specify the **[!UICONTROL Username]** of your [!DNL Workfront] account or SAML user.
1. Specify the **[!UICONTROL Password]** for your [!DNL Workfront] account or SAML user.
-->

<!--
1. (Conditional) If you are logging in for the first time, a page requesting permission for the [!DNL Workfront] mobile app to access your account will display. Click **Allow access** to continue.

1. You are redirected to a webpage that allows you to log in identically to the desktop site. This process varies depending on your organization's Workfront configuration, see [Log in to [!DNL Workfront] without SSO](#log-in-to-workfront-without-sso) or [Log in to [!DNL Workfront] with SSO](#log-in-to-workfront-with-sso) above for more information. 

   Once complete, you are redirected by to the mobile app and signed in.

1. Tap **[!UICONTROL Okay, got it]** or **[!UICONTROL GETTING STARTED]** to navigate through the tutorials displayed.

   These tutorials display only the first time you access the app. They display again only when you uninstall and reinstall the [!DNL Workfront] mobile app, or if you log in as another user. After closing out the tutorials, the area that displays is the one that you selected to show

## Log in to the [!DNL Workfront] mobile app using [!DNL Adobe] ID

1. Launch the [!DNL Workfront] mobile app, then click **Sign in with [!DNL Adobe] ID**.

>[!NOTE]
>
>For iOS users on IMS, you can select **Sign in with company domain** and use the domain provided by your [!DNL Workfront] administrator to log in using your [!DNL Adobe] ID.

1. Type in your email, then click **Continue**.

1. (Conditional) Select the account you would like to use to log in. Typically, this will be **Company or School Account** if your [!DNL Adobe] ID is associated with an organization. 

1. (Conditional) Select a profile to use if your account is associated with more than one organization.

1. You are now signed in. Tap **[!UICONTROL Okay, got it]** or **[!UICONTROL GETTING STARTED]** to navigate through the tutorials displayed.

   These tutorials display only the first time you access the app. They display again only when you uninstall and reinstall the [!DNL Workfront] mobile app, or if you log in as another user. After closing out the tutorials, the area that displays is the one that you selected to show
-->
