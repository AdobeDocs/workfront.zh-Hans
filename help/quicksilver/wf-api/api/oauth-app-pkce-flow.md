---
content-type: api
navigation-topic: api-navigation-topic
title: 为OAuth 2应用程序使用PKCE流
description: 为OAuth 2应用程序使用PKCE流
author: John
feature: Workfront API
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: 03df0ad329255e86780c03bbb4541e0a0a526381
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# 使用PKCE流程配置和使用贵组织的自定义OAuth 2应用程序

PKCE是一种安全的授权流程，可与动态刷新应用程序（如移动设备应用程序）的应用程序配合使用，但在所有OAuth2客户端中都很有价值。 PKCE使用动态生成的字符串而不是静态客户端密钥，从而消除了泄露的客户端密钥的风险。

## PKCE概述

PKCE流具有以下步骤。 此部分中的步骤仅供参考。 要执行这些步骤，请参阅本文的其他章节。

1. 客户端将创建 `code_challenge` 通过 `code_verifier` 使用 `S256` 加密。

1. 客户端将浏览器引导至OAuth2登录页面以及生成的 `code_challenge`. 您必须注册您的应用程序（客户端），以便OAuth2可以接受授权请求。 注册后，您的应用程序可以将浏览器重定向到OAuth2。

1. OAuth2授权服务器将身份验证提示重定向到用户。

1. 用户使用一个配置的登录选项进行身份验证，并且可能会看到一个同意页面，其中列出了OAuth2将授予应用程序的权限。

1. OAuth2通过 `authorization code`.

1. 您的应用程序会发送此代码以及 `code_verifier`，到OAuth2。

1. OAuth2授权服务器转换 `code_verifier` 使用 `code_challenge_method` 从初始授权请求中检查结果，并根据 `code_challenge`. 如果两个字符串的值匹配，则服务器已验证请求来自同一客户端，并将发出 `access token`.

1. OAuth2会返回 `access token`，以及（可选） `refresh token`.

1. 您的应用程序现在可以使用这些令牌来调用资源服务器，如代表用户的API。

1. 资源服务器在响应请求之前会验证令牌。


## 配置应用程序

在实施授权之前，您需要先从Workfront创建应用程序集成，然后再在OAuth2中注册应用程序。

有关创建OAuth2应用程序的说明，请参阅 [使用PKCE创建OAuth2单页Web应用程序 ](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) in [为Workfront集成创建OAuth2应用程序](../../administration-and-setup/configure-integrations/create-oauth-application.md)


## 为代码交换创建校样键

与标准授权代码流类似，您的应用程序通过将用户的浏览器重定向到您授权服务器的 `/authorize` 端点。 但是，在此示例中，您还必须传递代码挑战。

您的第一步是生成代码验证器和质询。

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">代码验证器</td>
        <td>
          <p>最小长度为43个字符的随机URL安全字符串</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">代码挑战</td>
        <td>
          <p>代码验证器的SHA-256哈希由Base64 URL编码</p>
        </td>
      </tr>
    </tbody>
</table>


您必须在客户端应用程序中添加代码，以创建代码验证器和代码质询。

PKCE生成器代码创建与以下类似的输出：

>[!INFO]
>
>**示例:**
>
>```
>{
>
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>
>}
>```

您的应用程序保存 `code_verifier` 以后，并发送 `code_challenge` 以及对授权服务器的 `/authorize` URL。

## 请求授权代码

如果您使用默认的自定义授权服务器，则您的请求URL将类似于以下内容：

>[!INFO]
>
>**示例:**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

请注意正在传递的参数：

* `client_id` 与配置应用程序时在中创建的OAuth2应用程序的客户端ID匹配。

   有关说明，请参阅“创建OAuth2应用程序以进行Workfront集成”中的使用PKCE创建OAuth2单页Web应用程序。

* `response_type` is `code`，因为应用程序使用授权代码授予类型。

* `redirect_uri` 是用户代理与 `code`. 此URL必须与您在创建OAuth2应用程序时指定的重定向URL之一匹配。

* `code_challenge_method` 是用于生成挑战的哈希方法，它始终 `S256` 适用于使用PKCE的Workfront Oauth2应用程序。

* `code_challenge` 是用于PKCE的代码挑战。


## 交换令牌代码

要为访问令牌交换授权代码，请将其传递到授权服务器的 `/token` 端点以及 `code_verifier`.

>[!INFO]
>
>**示例:**
>
>```
>/token \\
>
>  --header 'accept: application/json' \\
>
>  --header 'cache-control: no-cache' \\
>
>  --header 'content-type: application/x-www-form-urlencoded' \\
>
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> 与常规的授权代码流不同，此调用不需要具有客户端ID和密钥的授权标头。 因此，此版本的授权代码流适合没有后端的本机应用程序（如移动设备应用程序或单页应用程序）。

请注意正在传递的参数：

* `grant_type` is `authorization_code`，因为应用程序使用授权代码授予类型。

* `redirect_uri` 必须匹配用于获取授权代码的URI。

* `code` 是您从/authorize端点收到的授权代码。

* `code_verifier` 是您的应用程序在中生成的PKCE代码验证器 [为代码交换创建校样键](#Create).

* `client_id` 标识您的客户端，且必须匹配OAuth2中预注册的值。


如果代码仍然有效，并且代码验证器匹配，则您的应用程序将收到访问令牌。

>[!INFO]
>
>**示例:**
>
>```
>{
>
>    "access\_token": "eyJhd\[...\]Yozv",
>
>    "expires\_in": 3600,
>
>    "token\_type": "Bearer"
>
>}
>```

## 验证访问令牌

当您的应用程序通过访问令牌传递请求时，资源服务器需要对其进行验证。

您可以通过与以下类似的API调用验证您的访问令牌：

>[!INFO]
>
>**示例:**
>
>```
>/attask/api/<api version>/proj/search \\
>
>  --header 'sessionID: <access\_token>' \\
>```

## 请求刷新令牌

要请求刷新令牌，您可以对API进行POST调用，如下所示：

>[!INFO]
>
>**示例:**
>
>```
>/token \\
>
>  --header 'accept: application/json' \\
>
>  --header 'cache-control: no-cache' \\
>
>  --header 'content-type: application/x-www-form-urlencoded' \\
>
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
