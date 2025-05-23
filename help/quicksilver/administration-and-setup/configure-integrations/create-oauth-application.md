---
title: 为 [!DNL Workfront] 集成创建OAuth2应用程序
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 作为 [!DNL Adobe Workfront] 管理员，您可以为 [!DNL Workfront]的实例创建OAuth2应用程序，这将允许其他应用程序访问Workfront。 然后，您的用户可以将权限授予这些其他应用程序，以访问其Workfront数据。 这样，您就可以将Workfront与您选择的应用程序（包括您自己的内部应用程序）集成。
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: 09f7e854c2df1291feb150d2169fa6ccd5cdb1d6
workflow-type: tm+mt
source-wordcount: '1981'
ht-degree: 5%

---

# 为[!DNL Workfront]集成创建OAuth2应用程序

作为[!DNL Adobe Workfront]管理员，您可以为您的[!DNL Workfront]实例创建OAuth2应用程序，这将允许其他应用程序访问[!DNL Workfront]。 然后，您的用户可以授予这些其他应用程序访问其[!DNL Workfront]数据的权限。 通过这种方法，您可以集成   包括您自己的内部应用程序在内。

创建[!UICONTROL OAuth2]应用程序时，将生成客户端ID和客户端密钥。 然后，您的用户便可以在API调用中使用客户端ID，将与您创建的应用程序集成。

>[!NOTE]
>
>在OAuth2的上下文中，“创建应用程序”是指在应用程序和服务器（如[!DNL Workfront]）之间创建此类访问链接的过程。

* 有关通过用户凭据（授权代码流）配置和使用OAuth2应用程序的说明，请参阅[使用授权代码流配置和使用您组织的自定义OAuth2应用程序](../../wf-api/api/oauth-app-code-token-flow.md)。
* 有关使用服务器身份验证（JWT流）配置和使用OAuth2应用程序的说明，请参阅[使用JWT流配置和使用您组织的自定义OAuth2应用程序](../../wf-api/api/oauth-app-jwt-flow.md)。
* 有关使用PKCE配置和使用OAuth2应用程序的说明，请参阅[使用PKCE流程配置和使用您组织的自定义OAuth2应用程序](../../wf-api/api/oauth-app-pkce-flow.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td><p>新文档： [!UICONTROL Standard]</p>
   或
   <p>当前：[!UICONTROL 计划]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> 您必须是[!DNL Workfront]管理员。 </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## OAuth2概述

假设应用程序必须从[!DNL Workfront]中提取一些特定信息。 请求信息的应用程序称为客户端。 在此示例中，客户端名称为ClientApp。 ClientApp需要访问特定用户的信息，因此必须以该用户的身份访问[!DNL Workfront]。 如果用户为ClientApp提供用户名和密码，则ClientApp可以访问用户可以访问的所有数据。 这会带来安全风险，因为ClientApp只需要一小部分特定信息。

在为ClientApp创建OAuth2应用程序时，实际上是在告知[!DNL Workfront] ClientApp允许访问[!DNL Workfront]，但前提是帐户为ClientApp所访问的用户授予了访问权限。

## 创建OAuth2应用程序

创建OAuth2应用程序时，请选择最符合集成需求的应用程序类型。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>应用程序类型</th> 
   <th>最适合</th> 
   <th>身份验证方法</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>机器对机器应用程序</p> </td> 
   <td> <p>最适合在服务器上运行的CLI、守护程序或脚本</p> <p>示例：</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>通过使用公钥/私钥对编码的 JSON Web 令牌进行身份验证。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>单页 Web 应用程序</p> </td> 
   <td> <p>最适合移动设备或单页Web应用程序</p> <p>示例：</p> 
    <ul> 
     <li> <p>[!DNL Javascript]</p> </li> 
     <li> <p>[!DNL Angular]</p> </li> 
     <li> <p>[!DNL React]</p> </li> 
     <li> <p>[!DNL Vue]</p> </li> 
    </ul> </td> 
   <td> <p>通过使用 Proof Key for Code Exchange (PKCE) 的 OAuth 2.0 授权代码流进行身份验证。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Web 应用程序</p> </td> 
   <td> <p>最适合在服务器上处理凭据和令牌的服务器端应用程序</p> <p>示例：</p> 
    <ul> 
     <li> <p>[!DNL Go]</p> </li> 
     <li> <p>[!DNL Java]</p> </li> 
     <li> <p>[!DNL ASP.Net]</p> </li> 
     <li> <p>[!DNL Node.js]</p> </li> 
     <li> <p>[!DNL PHP]</p> </li> 
    </ul> </td> 
   <td> <p>通过 OAuth 2.0 授权代码流进行身份验证。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>您一次最多可以拥有10个OAuth2应用程序。

* [使用服务器身份验证（JWT流）创建OAuth2应用程序](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [使用用户凭据创建OAuth2应用程序（授权代码流）](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [使用PKCE创建OAuth2单页Web应用程序](#create-an-oauth2-single-page-web-application-using-pkce)

### 使用服务器身份验证（JWT流）创建OAuth2应用程序 {#create-an-oauth2-application-using-server-authentication-jwt-flow}

{{step-1-to-setup}}

1. 在左侧导航面板中，单击&#x200B;**[!UICONTROL 系统]**，然后选择&#x200B;**[!UICONTROL OAuth2应用程序]**。
1. 单击&#x200B;**[!UICONTROL 创建应用集成]**。
将显示&#x200B;**新OAuth2应用程序**&#x200B;框。
1. 在&#x200B;**新OAuth2应用程序**&#x200B;框中，选择&#x200B;**[!UICONTROL 计算机到计算机应用程序]**。
1. 输入新应用程序的名称，如“[!DNL Workfront] for ClientApp”。
1. 单击&#x200B;**[!UICONTROL 创建]**。
1. 填写新应用程序的字段。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 客户端ID]</td> 
      <td> <p>此字段是自动生成的。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 客户端密码]</td> 
      <td> <p>此字段是自动生成的</p> <p><b>重要信息</b>：  <p>在关闭此页之前，将此字段的内容复制到另一个安全文件。 您将无法再次看到此密钥。</p> <p>如果丢失此密钥，请删除它并创建客户端密钥。</p> 
        <ol> 
         <li value="1"> <p>单击<b>[!UICONTROL Delete]</b>图标<img src="assets/delete.png">可删除当前客户端密钥。</p> </li> 
         <li value="2"> <p>单击<b>[!UICONTROL 添加客户端密钥]</b>以生成新的客户端密钥。</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 公钥]</td> 
      <td> <p>服务器到服务器应用程序使用公钥和私钥进行身份验证。 执行下列操作之一：</p> 
       <ul> 
        <li> <p>单击<b>[!UICONTROL Add a public key]</b>，然后输入另一个应用程序的公共密钥。</p> </li> 
        <li> <p>单击<b>[!UICONTROL 生成公钥/私钥对]</b>，然后与其他应用程序共享公钥。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名称]</td> 
      <td>该名称与您为应用程序提供的名称相同。 此字段不能为空。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 描述]</td> 
      <td>输入集成的说明。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 保存]**。

有关通过用户凭据（授权代码流）配置和使用OAuth2应用程序的说明，请参阅[使用JWT流配置和使用您组织的自定义OAuth2应用程序](../../wf-api/api/oauth-app-jwt-flow.md)。

### 使用用户凭据创建OAuth2应用程序（授权代码流） {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

>[!NOTE]
>
>如果要创建应用程序以连接到Workfront Fusion，请使用以下重定向URL之一：
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-workfront`
>* `https://app-eu.workfrontfusion.com/oauth/cb/workfront-workfront` （欧盟数据中心）
>* `https://app-az.workfrontfusion.com/oauth/cb/workfront-workfront` （Azure数据中心）

{{step-1-to-setup}}

1. 在左侧导航面板中，单击&#x200B;**[!UICONTROL 系统]**，然后选择&#x200B;**[!UICONTROL OAuth2应用程序]**。
1. 单击&#x200B;**[!UICONTROL 创建应用集成]**。

   显示&#x200B;**新OAuth2应用程序**。
1. 在&#x200B;**新OAuth2应用程序**&#x200B;框中，选择&#x200B;**[!UICONTROL Web应用程序]**。
1. 输入新OAuth2应用程序的名称，例如“[!DNL Workfront] for ClientApp”。
1. 单击&#x200B;**[!UICONTROL 创建]**。
1. 填写新应用程序的字段。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 客户端ID]</td> 
      <td> <p>此字段是自动生成的。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 客户端密码]</td> 
      <td> <p>此字段是自动生成的</p> <p><b>重要信息</b>：  <p>在关闭此页之前，将此字段的内容复制到另一个安全文件。 您将无法再次看到此密钥。</p> <p>如果丢失此密钥，请删除它并创建客户端密钥。</p> 
        <ol> 
         <li value="1"> <p>单击<b>[!UICONTROL Delete]</b>图标<img src="assets/delete.png">可删除当前客户端密钥。</p> </li> 
         <li value="2"> <p>单击<b>[!UICONTROL 添加客户端密钥]</b>以生成新的客户端密钥。</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 重定向URL]</td> 
      <td>用户使用[!DNL Workfront]进行身份验证后，会被重定向到此路径。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 刷新令牌轮换]</td> 
      <td>启用此选项可在使用刷新令牌时发出新的刷新令牌。您的应用程序必须在每次刷新后存储新的刷新令牌。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 绝对刷新令牌过期]</td> 
      <td> <p>选择刷新令牌过期前希望存在的时间。 过期后，您的用户必须再次登录该集成。 如果不希望刷新令牌过期，请选择“[!UICONTROL 无过期]”。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">不活动刷新令牌期限</td> 
      <td> <p>选择多长时间，如果用户在您的系统中未处于活动状态，则其刷新令牌将过期。 </p> <p>例如，如果非活动刷新令牌过期时间为6个月，而用户在6个月内未登录，则刷新令牌将过期，即使绝对刷新令牌过期时间可能设置为更长。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 徽标]</td> 
      <td>您可以添加徽标，使此应用程序更易于识别。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名称]</td> 
      <td>该名称与您为应用程序提供的名称相同。 此字段不能为空。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 描述]</td> 
      <td>输入集成的说明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 应用程序描述URL]</td> 
      <td>这可以是指向“关于我们”页面的链接，也可以是包含有关集成的更多信息的页面。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 保存]**。

有关通过用户凭据（授权代码流）配置和使用OAuth2应用程序的说明，请参阅[使用授权代码流配置和使用您组织的自定义OAuth2应用程序](../../wf-api/api/oauth-app-code-token-flow.md)。

### 使用PKCE创建OAuth2单页Web应用程序 {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. 在左侧导航面板中，单击&#x200B;**[!UICONTROL 系统]**，然后选择&#x200B;**[!UICONTROL OAuth2应用程序]**。
1. 单击&#x200B;**[!UICONTROL 创建应用集成]**。

   将显示&#x200B;**新OAuth2应用程序**&#x200B;框。
1. 在&#x200B;**新OAuth2应用程序**&#x200B;框中，选择&#x200B;**[!UICONTROL 单页Web应用程序]**。
1. 输入新[!UICONTROL OAuth2]应用程序的名称，例如“[!DNL Workfront] for ClientApp”。
1. 单击&#x200B;**[!UICONTROL 创建]**。
1. 填写新应用程序的字段。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 客户端ID]</td> 
      <td> <p>此字段是自动生成的。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 重定向URL]</td> 
      <td>用户通过Workfront身份验证后，会被重定向到此路径。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 每次使用令牌时都会轮换刷新令牌]</td> 
      <td>启用此选项可在使用刷新令牌时发出新的刷新令牌。您的应用程序必须在每次刷新后存储新的刷新令牌。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 绝对过期]</td> 
      <td> <p>选择刷新令牌过期前希望存在的时间。 过期后，您的用户必须再次登录该集成。 如果不希望刷新令牌过期，请选择“[!UICONTROL 无过期]”。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 非活动状态过期]</td> 
      <td> <p>选择多长时间，如果用户在您的系统中未处于活动状态，则其刷新令牌将过期。 </p> <p>例如，如果非活动刷新令牌过期时间为6个月，而用户在6个月内未登录，则刷新令牌将过期，即使绝对刷新令牌过期时间可能设置为更长。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 徽标]</td> 
      <td>您可以添加徽标，使此应用程序更易于识别。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名称]</td> 
      <td>该名称与您为应用程序提供的名称相同。 此字段不能为空。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 描述]</td> 
      <td>输入集成的说明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 开发人员姓名]</td> 
      <td>这是正在设置OAuth2应用程序的开发人员的姓名。</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL 开发人员电子邮件地址]</td> 
      <td>这是设置OAuth2应用程序的开发人员的电子邮件地址。</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL 隐私策略URL]</td> 
      <td>这是指向您的组织存储隐私策略的位置的链接。</td> 
     </tr>


   </tbody> 
   </table>

   <!-- removed this from the table, and added "Developer name" and following rows:
   [!UICONTROL App Description URL]</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.> -->

1. 单击&#x200B;**[!UICONTROL 保存]**。

## 配置并使用创建的OAuth2应用程序

进一步配置和使用创建的OAuth2应用程序需要一些技术知识，包括API调用。

* 有关通过用户凭据（授权代码流）配置和使用OAuth2应用程序的说明，请参阅[使用授权代码流配置和使用您组织的自定义OAuth2应用程序](../../wf-api/api/oauth-app-code-token-flow.md)。
* 有关使用服务器身份验证（JWT流）配置和使用OAuth2应用程序的说明，请参阅[使用JWT流配置和使用您组织的自定义OAuth2应用程序](../../wf-api/api/oauth-app-jwt-flow.md)。
* 有关使用PKCE配置和使用OAuth2应用程序的说明，请参阅[使用PKCE流程配置和使用您组织的自定义OAuth2应用程序](../../wf-api/api/oauth-app-pkce-flow.md)。

## 用于授权代码流的OAuth2进程

>[!NOTE]
>
>您的用户通过API访问[!UICONTROL OAuth2]应用程序。 本节将笼统地介绍这些功能，仅供参考。
>
>有关使用OAuth2应用程序（包括特定API调用）的特定说明，请参阅[使用授权代码流配置和使用您组织的自定义OAuth2应用程序](../../wf-api/api/oauth-app-code-token-flow.md)。

### 使用授权代码和访问令牌进行授权 {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp需要来自[!DNL Workfront]的一些信息，因此它向[!DNL Workfront] API `/authorize`终结点发送请求。 该请求包括[!UICONTROL response_type] `code`，这表示该请求应返回授权代码。
1. 这会触发[!DNL Workfront]向用户发送身份验证提示。 用户可以在提示中输入其凭据，这将授予[!DNL Workfront]与ClientApp通信的权限。 如果用户已登录[!DNL Workfront]，则可以跳过此步骤。
1. [!DNL Workfront] API向ClientApp发送授权代码。
1. ClientApp在请求中将以下信息发送到[!DNL Workfront] API `/token`   端点：

   * 在步骤3中发送到ClientApp的授权代码。 这会标识用户权限的特定实例。
   * 在[!DNL Workfront]中设置ClientApp OAuth2应用程序时生成的客户端密钥。 这允许[!DNL Workfront]知道请求来自ClientApp。

1. 如果授权代码和客户端密钥正确，[!DNL Workfront]将访问令牌发送到ClientApp。 此访问令牌直接从[!DNL Workfront]发送到ClientApp，任何其他用户或客户端应用程序无法查看、复制或使用。
1. ClientApp将访问令牌连同特定的信息请求一起发送到[!DNL Workfront]。
1. 由于访问令牌正确，[!DNL Workfront]将信息发送到ClientApp。

#### 刷新访问令牌

为安全起见，访问令牌会在较短时间后过期。 要获取新的访问令牌而无需每次都输入凭据，[!DNL OAuth2]使用刷新令牌。 刷新令牌由客户端存储。

获取刷新令牌的过程与[授权授权授权代码和访问令牌](#authorizing-with-an-authorization-code-and-access-token)一节中讨论的过程相同。 授权代码的请求包含范围`offline_access`，该范围指示请求应随授权代码一起返回请求令牌。
