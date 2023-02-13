---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: http-modules
title: HTTP &gt;创建OAuth 2.0请求模块
description: 为了 [!DNL Adobe Workfront Fusion] 对需要OAuth 2.0授权的服务器发出HTTP(S)请求，您首先需要创建OAuth连接。 [!DNL Adobe Workfront Fusion] 确保通过此连接发起的所有调用都具有适当的授权标头，并在需要时自动刷新关联的令牌。
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2172'
ht-degree: 0%

---

# [!UICONTROL HTTP] > [!UICONTROL 发出OAuth 2.0请求] 模块

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 需要 [!DNL Adobe Workfront Fusion] 除 [!DNL Adobe Workfront] 许可证。

为了 [!DNL Adobe Workfront Fusion] 对需要OAuth 2.0授权的服务器发出HTTP(S)请求，您首先需要创建OAuth连接。 [!DNL Adobe Workfront Fusion] 确保通过此连接发起的所有调用都具有适当的授权标头，并在需要时自动刷新关联的令牌。

[!DNL Workfront Fusion] 支持以下OAuth 2.0身份验证流程：

* 授权代码流
* 隐式流量

此模块不自动支持其他流程，如资源所有者密码凭据流和客户端凭据流。

有关OAuth 2.0身份验证的更多信息，请参阅 [OAuth 2.0授权框架](https://tools.ietf.org/html/rfc6749).

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr>
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 为 [!DNL OAuth] 请求

* [在HTTP >创建OAuth 2.0请求模块中创建连接的常规说明](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [有关在HTTP >中创建与Google的连接的说明[!UICONTROL Make] OAuth 2.0请求模块](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [有关通过HTTP >发出OAuth 2.0请求模块连接到Microsoft Graph API的说明](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### 有关在 [!UICONTROL HTTP] > [!UICONTROL 发出OAuth 2.0请求] 模块

1. 在 [!DNL target] 您想要的服务 [!DNL Adobe Workfront Fusion] 进行交流。 此选项很可能在 [!UICONTROL 开发人员] 部分。

   1. 创建客户端时，请在 `[!UICONTROL Redirect URL]` 或 `[!UICONTROL Callback URL]` 字段：

      | 美洲/亚太地区 | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | 欧洲、中东和非洲 | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. 创建客户端后，给定服务会显示2个键： `[!UICONTROL Client ID]` 和 `[!UICONTROL Client Secret]`. 有些服务称为 `[!UICONTROL App Key]` 和 `[!UICONTROL App Secret]` . 将密钥和密钥保存在安全位置，以便在Workfront Fusion中创建连接时提供它们。

1. 查找 `[!UICONTROL Authorize URI]` 和 `[!UICONTROL Token URI]` （位于给定服务的API文档中）。 这些是用于 [!DNL Workfront Fusion] 与 [!DNL target] 服务。 地址用于OAuth授权。

   >[!NOTE]
   >
   >如果服务使用隐式流，则您只需 `[!UICONTROL Authorize URI]`.

   >[!INFO]
   >
   >**示例：** Yahoo地址：
   >
   >* 授权URI:
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* 令牌URI:
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. （视情况而定）如果目标服务使用作用域（访问权限），请检查服务如何分隔单个作用域，并确保在高级设置中相应地设置分隔符。 如果分隔符设置不正确， [!DNL Workfront Fusion] 无法创建连接，并且您收到无效的作用域错误。
1. 完成上述步骤后，您可以在 [!DNL Workfront Fusion]. 将OAuth 2.0 HTTP(S)请求和响应处理模块添加到您的方案中。
1. 在模块的Connection字段中，单击 **[!UICONTROL 添加]**.

1. 填写以下字段以创建连接：

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL连接名称] </td> 
      <td> <p>输入连接的名称。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL流类型]</p> </td> 
      <td> <p>选择用于获取令牌的流程。</p> 
       <ul> 
        <li><strong>[!UICONTROL授权代码]</strong>:输入 <code>[!UICONTROL Authorize URI]</code> 和 <code>[!UICONTROL Token URI]</code> 的API文档。</li> 
        <li><strong>[!UICONTROL隐式]</strong>:输入 <code>[!UICONTROL Authorize URI]</code> 的API文档。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL范围] </td> 
      <td> <p>添加单个作用域。 您可以在给定服务的开发人员(API)文档中找到此信息。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL范围分隔符] </td> 
      <td> <p>选择以上输入的范围应以分隔。 您可以在给定服务的开发人员(API)文档中找到此信息。</p> <p>警告：如果分隔符设置不正确， [!DNL Workfront Fusion] 无法创建连接，并且您收到无效的作用域错误。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客户端ID] </td> 
      <td> <p>输入客户端ID。 在要连接的服务中创建OAuth客户端时，您获取了客户端ID。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客户端密钥]</td> 
      <td> <p> 输入客户端密钥。 在要连接的服务中创建OAuth客户端时，您获取了客户端密钥。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL授权参数]</p> </td> 
      <td> <p>添加要包含在授权调用中的任何参数。 以下标准参数始终自动包含在内，无需添加。</p> <p>标准参数：</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL response_type]</strong> </p> <p> <code>code </code>适用于[!UICONTROL授权代码流]和 <code>token </code>（对于[!UICONTROL隐式流量]）</p> </li> 
        <li> <p><strong>[!UICONTROL redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">美洲/亚太地区</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">欧洲、中东和非洲 </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong> </p> <p> 您在创建帐户时收到的客户ID</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL访问令牌参数]</p> </td> 
      <td> <p>添加要包含在令牌调用中的任何参数。 以下标准参数始终自动包含在内，无需添加。</p> <p>标准参数：</p> 
       <ul> 
        <li><strong>[!UICONTROL grant_type]</strong>: <code>authorization_code</code></li> 
        <li> <p><strong>[!UICONTROL redirect_uri]:</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">美洲/亚太地区</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">欧洲、中东和非洲 </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li><strong>[!UICONTROL client_id]</strong>:您在创建帐户时收到的客户ID会自动包含在请求正文中</li> 
        <li><strong>client_secret</strong>:您在创建帐户时收到的客户端密钥会自动包含在请求正文中</li> 
        <li><strong>代码</strong>:授权请求返回的代码</li> 
       </ul> <p>注释:  <p>OAuth 2.0标准在此步骤中至少支持2种客户端身份验证方法(<code>[!UICONTROL client_secret_basic]</code> 和 <code>[!UICONTROL client_secret_post]</code>)。 [!DNL Workfront Fusion] 自动通过 <code>[!UICONTROL client_secret_post]</code> 方法。 因此，这些参数会自动包含在令牌请求正文中。 </p> <p>有关OAuth 2.0身份验证的更多信息，请参阅 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0授权框架</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL刷新令牌参数]</p> </td> 
      <td> <p>添加要包含在令牌调用中的任何参数。 以下标准参数始终自动包含在内，无需添加。</p> <p>标准参数：</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL grant_type]</strong>: <code>refresh_token</code></p> </li> 
        <li> <p><strong>[!UICONTROL refresh_token]</strong>:您连接到的服务获取的最新刷新令牌</p> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong>:您在创建帐户时收到的客户ID会自动包含在请求正文中</p> </li> 
        <li> <p><strong>[!UICONTROL client_secret]</strong>:您在创建帐户时收到的客户端密钥会自动包含在请求正文中</p> </li> 
       </ul> <p>注释:  <p>OAuth 2.0标准在此步骤中至少支持2种客户端身份验证方法(<code>[!UICONTROL client_secret_basic]</code> 和 <code>[!UICONTROL client_secret_post]</code>)。 [!DNL Workfront Fusion] 自动通过 <code>[!UICONTROL client_secret_post]</code> 方法。 因此，这些参数会自动包含在令牌请求正文中。 </p> <p>有关OAuth 2.0身份验证的更多信息，请参阅 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0授权框架</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL自定义标题]</p> </td> 
      <td> <p>指定要包含在[!UICONTROL Token]和R[!UICONTROL刷新令牌]步骤的标头中的任何其他键和值。</p> <p>注释:  <p>OAuth 2.0标准在此步骤中至少支持2种客户端身份验证方法(<code>[!UICONTROL client_secret_basic]</code> 和 <code>[!UICONTROL client_secret_post]</code>)。 [!DNL Workfront Fusion] 不自动支持 <code>[!UICONTROL client_secret_basic]</code> 方法。 如果您要连接的服务希望将客户端ID和客户端密钥合并为单个字符串，然后将base64编码到授权标头中，则应在此处添加该标头和键值。</p> <p> 有关OAuth 2.0身份验证的更多信息，请参阅 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0授权框架</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL令牌放置]</p> </td> 
      <td> <p>选择是在[!UICONTROL标头]、[!UICONTROL查询字符串]中发送令牌，还是在连接到指定的URL时同时在两者中发送令牌。</p> <p>令牌最常在请求标头中发送。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL标头令牌名称] </td> 
      <td> <p>在标头中输入授权令牌的名称。 默认: <code>[!UICONTROL Bearer]</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL查询字符串参数名称] </td> 
      <td> <p>在查询字符串中输入授权令牌的名称。 默认: <code>[!UICONTROL access_token]</code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 继续]** 保存连接设置。
1. 继续 [OAuth 2.0请求模块设置](#oauth-20-request-module-setup).

### 创建连接的说明 [!DNL Google] 在 [!UICONTROL HTTP] >[!UICONTROL 创建OAuth 2.0请求模块]

以下示例显示如何使用 [!UICONTROL HTTP] > [!UICONTROL 制作OAuth 2.0] 请求模块连接到 [!DNL Google].

1. 确保您已创建项目、配置了OAuth设置，并且已按照 [连接 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自定义OAuth客户端](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).
1. 打开 [!UICONTROL HTTP] >[!UICONTROL 发出OAuth 2.0请求] 模块。
1. 单击 **[!UICONTROL 添加]** 中。
1. 输入以下值：

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL连接名称] </td> 
      <td> <p>输入连接的名称。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL流类型]</p> </td> 
      <td> <p>[!UICONTROL授权代码]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL授权URI]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL令牌URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL范围] </td> 
      <td> <p>添加单个作用域。 有关作用域的详细信息，请参阅 <a href="https://developers.google.com/identity/protocols/oauth2/scopes">的OAuth 2.O作用域 [!DNL Google] API</a> 在 [!DNL Google] 文档。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL范围分隔符] </td> 
      <td> <p>[!UICONTROL SPACE]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客户端ID] </td> 
      <td> <p>输入 [!DNL Google] 客户端ID。 </p> <p>要创建客户端ID，请参阅 <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">创建OAuth凭据</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] to [!DNL Google Services] 使用自定义OAuth客户端</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客户端密钥]</td> 
      <td> <p>输入 [!DNL Google] 客户端密钥。 </p> <p>要创建客户端密钥，请参阅 <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">创建OAuth凭据</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] to [!DNL Google] 使用自定义OAuth客户端的服务</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL授权参数]</p> </td> 
      <td> <p>添加 <code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code>键值对。</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>注意：如果您遇到身份验证问题（例如令牌刷新），请尝试添加 <code>[!UICONTROL prompt] </code>- <code>[!UICONTROL consent] </code>键值对。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 继续]** 保存连接设置。
1. 继续 [OAuth 2.0请求模块设置](#oauth-20-request-module-setup).

### 连接到的说明 [!DNL Microsoft Graph API] 通过 [!UICONTROL HTTP] > [!UICONTROL 发出OAuth 2.0请求] 模块

有关 [!DNL Microsoft Graph API]，请参阅 [调用 [!DNL MS Graph REST API] 通过 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 发出OAuth 2.0请求] 模块](../../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## OAuth 2.0请求模块设置

当您建立 [!DNL Oauth 2].0连接，如 [为 [!DNL OAuth] 请求](#creating-a-connection-for-an-oauth-request)，继续根据需要设置模块。 所有授权令牌都会自动包含在此请求中，以及使用相同连接的任何其他请求中。

当您配置 [!UICONTROL HTTP] >[!UICONTROL 发出OAuth 2.0请求] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关设置连接的信息，请参阅 <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">为OAuth请求创建连接</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL评估所有状态为错误（2xx和3xx除外） </td> 
   <td> <p>使用此选项设置错误处理。</p> <p>有关更多信息，请参阅 <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">在中处理错误 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>输入要向发送请求的URL，如API端点、网站等。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头] </td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。 例如， <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p> 输入所需的查询键值对。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Body type]</p> </td> 
   <td> <p>HTTP Body是在HTTP事务消息中发送的数据字节（如果有任何要使用的数据字节，则紧靠标头后）。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>即使在开发人员文档未指定要发送的数据的情况下，原始主体类型通常也适用于大多数HTTP主体请求。</p> <p>在[!UICONTROL内容类型]字段中指定解析数据的形式。</p> <p>尽管选择了内容类型，数据仍以开发人员文档规定或要求的任何格式输入。</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>此主体类型用于POST数据 <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>对于 <code>[!UICONTROL application/x-www-form-urlencoded]</code>，则发送到服务器的HTTP消息正文本质上是一个查询字符串。 键和值以键值对进行编码，键值对之间用 <code>&amp;</code> 和 <code>=</code> 键和值之间。 </p> <p>对于二进制数据， <code>use [!UICONTROL multipart/form-data]</code> 中。</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>示例: </b></span></span> 
       <p>生成的HTTP请求格式示例：</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data]是用于发送文件和数据的HTTP多部分请求。 它通常用于将文件上传到服务器。</p> <p>添加要在请求中发送的字段。 每个字段必须包含键值对。</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Text]</strong> </p> <p>输入要在请求正文中发送的键和值。</p> </li> 
       <li> <p><strong>[!UICONTROL文件]</strong> </p> <p>输入键，并指定要在请求正文中发送的源文件。</p> <p>映射要从上一个模块上传的文件(例如[!UICONTROL HTTP] &gt;[!UICONTROL Get a File]或[!UICONTROL Google Drive] &gt;[!UICONTROL Download a File)]，或手动输入文件名和文件数据。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parse响应]</p> </td> 
   <td> <p>启用此选项可自动解析响应并转换JSON和XML响应，这样您就无需使用[!UICONTROL JSON] &gt; [!UICONTROL Parse JSON]或[!UICONTROL XML] &gt; [!UICONTROL Parse XML]模块。</p> <p>在使用解析后的JSON或XML内容之前，请手动运行该模块一次，以便该模块能够识别响应内容，并允许您在后续模块中映射该内容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL超时] </td> 
   <td> <p>以秒为单位输入请求超时(1-300)。 默认为40秒。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL与其他HTTP模块共享Cookie]</td> 
   <td> <p> 启用此选项，可将服务器中的Cookie与方案中的所有HTTP模块共享。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL自签名证书]</td> 
   <td> <p> 如果您希望使用自签名证书的TLS，请上传您的证书。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拒绝使用未验证（自签名）证书的连接] </td> 
   <td> <p>启用此选项可拒绝使用未验证的TLS证书的连接。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL遵循重定向]</td> 
   <td> <p> 启用此选项，可通过3xx响应来遵循URL重定向。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL按照所有重定向] </td> 
   <td> <p>启用此选项可使用所有响应代码遵循URL重定向。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL禁用与数组相同的多个查询字符串键的序列化]</p> </td> 
   <td> <p>默认情况下， [!DNL Workfront Fusion] 处理与数组相同的URL查询字符串参数键的多个值。 例如， <code>www.test.com?foo=bar&amp;foo=baz</code> 将转换为 <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. 激活此选项可禁用此功能。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL请求压缩内容]</td> 
   <td> <p> 启用此选项可请求网站的压缩版本。</p> <p>这会添加 <code>[!UICONTROL Accept-Encoding]</code> 请求压缩内容的标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL使用互相TLS]</td> 
   <td> <p>启用此选项可在HTTP请求中使用相互TLS。</p> <p>有关相互TLS的更多信息，请参阅 <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">在的HTTP模块中使用相互TLS [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
