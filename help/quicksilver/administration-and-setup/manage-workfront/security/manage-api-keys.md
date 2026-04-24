---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 管理API密钥
description: 为了最大程度地降低API安全漏洞，Adobe Workfront管理员可以管理用于使应用程序能够代表用户访问Workfront的API密钥。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: be11c7417023ce2f310fce3e0cf77724d101b89e
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 3%

---

# 管理 API 密钥

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->



>[!IMPORTANT]
>
>Workfront不再建议使用`/login`端点或API密钥。 请改用以下身份验证方法之一：
>
>* 使用JWT进行服务器身份验证
>* 使用OAuth2进行用户身份验证
>
>有关设置这些身份验证方法的说明，请参阅[为Workfront集成创建OAuth2应用程序](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)
>
>有关在Workfront中使用服务器身份验证的说明，请参阅[使用JWT流配置和使用您组织的自定义OAuth 2应用程序](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md)
>
>有关在Workfront中使用用户身份验证的说明，请参阅[使用授权代码流配置和使用您组织的自定义OAuth 2应用程序](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md)

为了最大程度地降低API安全漏洞，Adobe Workfront管理员可以管理用于使应用程序能够代表用户访问Workfront的API密钥。

您可以重置或删除当前管理员API密钥，将API密钥配置为过期，以及删除所有用户的API密钥。

以下是利用Workfront API的应用程序示例：

* 记录集成，例如Dropbox、Google Drive和Workfront DAM
* Workfront移动应用程序

>[!IMPORTANT]
>
>重置或删除API密钥时，必须重新配置任何利用Workfront API并通过此API密钥向Workfront进行身份验证的应用程序，才能重新获得对Workfront的访问权限。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td><p>“任一”</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p><p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## Workfront API密钥

Workfront中的每个用户都有一个唯一的API密钥。 当用户访问利用Workfront API的集成（例如Workfront移动应用程序或文档集成）时，将生成此密钥。

>[!NOTE]
>
> 在每周刷新期间，您在生产环境中生成的API密钥将会复制到预览环境中。 在每周刷新期间，您在“预览”环境中生成的任何API密钥都将由生产API密钥覆盖。

Workfront管理员还有唯一的API密钥。 当应用程序使用管理员API密钥访问Workfront时，该应用程序具有Workfront的管理员访问权限。

## 管理管理员API密钥

您可以为管理员用户帐户生成、重置或删除API密钥。

{{step-1-to-setup}}

1. 单击&#x200B;**系统>** **客户信息。**
1. （视情况而定）执行以下操作之一：

   要生成API密钥：在&#x200B;**API密钥设置**&#x200B;部分中，单击&#x200B;**生成API密钥**。

   或\
   要重置API密钥：在&#x200B;**API密钥设置**&#x200B;部分中，单击&#x200B;**重置**，然后单击&#x200B;**重置。**

   或

   要删除API密钥：在&#x200B;**API密钥设置**&#x200B;部分中，单击&#x200B;**删除**，然后单击&#x200B;**删除**。

<!--

   Remove me October 2026

## Generate an API Key for Non-Admin Users

You can generate and manage API Keys for users in roles other than Workfront administrator.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

1. (Conditional) If your organization uses Single Sign-On (SSO) access management, temporarily disable the option requiring SSO authentication.

   {{step-1-to-setup}} 
   
   1. Expand **System**, then click **Single Sign-on (SSO)**. 
   1. In the **Type** field, select the type of SSO your organization uses.
   1. With the type selected, scroll down and clear the **Enable** checkbox. 
      ![Enable SSO](assets/sysadmin-security-sso-disable-31620-350x320.png)  
   1. Click **Save**.


1. In the address bar of a browser, enter the following API call:

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=**username**&password=**password**&method=PUT

   Replace `<domain>` with your Workfront domain name, and username and password with the user's Workfront credentials.

1. (Conditional) Enable the option requiring SSO authentication if you disabled it in Step 1.

   {{step-1-to-setup}}
   
   1. Expand **System**, then click **Single Sign-on (SSO)**.
   
   1. Select your SSO method in the **Type** drop down menu.
   1. Check the checkbox requiring SSO authentication.

   -->

## 配置API密钥过期时间

您可以将API密钥配置为对系统中的所有用户过期。 当用户的API密钥过期时，用户必须向使用Workfront API访问Workfront的任何应用程序重新进行身份验证。 您可以更改API密钥的过期频率。 您还可以配置API密钥在用户密码过期时是否过期。

{{step-1-to-setup}}

1. 单击&#x200B;**系统** > **客户信息**。
1. 在&#x200B;**API密钥设置**&#x200B;区域的&#x200B;**创建**&#x200B;后&#x200B;**API密钥在**&#x200B;下拉列表中过期，请选择希望API密钥过期的时间范围。

   更改此选项时，新时间范围从您进行更改时开始。 例如，如果您将此选项从&#x200B;*1个月*&#x200B;更改为&#x200B;*6个月*，则API密钥将在您进行更改后6个月过期。

   默认情况下，API密钥每月过期。

1. 若要将API密钥配置为在用户密码过期时过期，请启用&#x200B;**在用户密码过期时删除API密钥**。

   默认情况下，不启用此选项。

   有关如何配置用户密码过期的信息，请参阅[配置系统安全首选项](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

1. 单击&#x200B;**保存**。

## 删除所有用户的API密钥

如果您担心您的Workfront系统存在特定的安全漏洞，则可以同时为所有用户删除API密钥。

>[!IMPORTANT]
>
>删除所有用户的API密钥将导致系统中所有用户的所有API密钥失效。 此操作将导致Workfront中的所有集成失败，直到您在Workfront中生成新的API密钥并更新所有集成为止。

{{step-1-to-setup}}

1. 展开&#x200B;**系统**，然后单击&#x200B;**客户信息**。

1. 在&#x200B;**API密钥设置**&#x200B;区域中，单击&#x200B;**删除所有API密钥**，然后单击&#x200B;**删除**&#x200B;**全部**。

<!--

Remove me October 2026

## Restricting API logins with an X.509 certificate

>[!IMPORTANT]
>
>The procedure described in this section applies only to organizations that have not yet been onboarded to the Adobe Business Platform. Logging in to Workfront through the Workfront API is not available if your organization has been onboarded to the Adobe Business Platform.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Administration differences between Adobe Workfront and Adobe Business Platform](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

Third-party applications can communicate with Workfront through the API. To increase the security of your Workfront site, you can configure Workfront to restrict API login requests by uploading an X.509 certificate to Workfront. Once enabled, all login requests through the API must include a client certificate in addition to username and password.

* [Obtain the X.509 certificate](#obtain-the-x-509-certificate) 
* [Upload the certificate to Workfront](#upload-the-certificate-to-workfront) 
* [Verify API login calls are restricted](#verify-api-login-calls-are-restricted)

### Obtain the X.509 certificate {#obtain-the-x-509-certificate}

Obtain a valid X.509 certificate from a trusted Certificate Authority (such as Verisign), and save it to a temporary location on your workstation. 

### Upload the certificate to Workfront {#upload-the-certificate-to-workfront}

After you have obtained the X.509 certificate from your Certificate Authority, you need to upload it to Workfront.

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  

1. Expand **System**, then click **Customer Info**.

1. In the **API Key Settings** area, select **Require X.509 Certificate for API logins**.
1. Click **Change Certificate**.
1. On your workstation, browse to and select the X.509 certificate that you previously downloaded.
1. (Optional) Click **View Details** next to the certificate name to view the following details about the certificate:

   * Subject Common Name
   * Subject Organization
   * Subject Organization Unit
   * Issuer Common Name
   * Issuer Organization
   * Issuer Organization Unit
   * Serial Number
   * Issue Date
   * Expiration Date

1. Click **Save**. 

### Verify API login calls are restricted {#verify-api-login-calls-are-restricted}

Prior to configuring your instance of Workfront to require an X.509 certificate, perform an API request to the `/login` endpoint using valid username and password parameters. You will receive a 200 response that contains a sessionID.

After making the X.509 certificate a requirement via the customer info page in your instance of Workfront, make another login attempt. This time you will receive a 500 error response with the following message: "Untrusted request. Please contact your system administrator and attach certificate."

After confirming that the X.509 certificate is required, perform the same login request with an additional parameter for apiCertificate set to the value of your certificate. If this operation was performed correctly you will receive a 200 response that contains a valid sessionID.

-->
