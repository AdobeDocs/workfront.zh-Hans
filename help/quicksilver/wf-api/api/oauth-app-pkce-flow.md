---
content-type: api
navigation-topic: api-navigation-topic
title: 为OAuth 2应用程序使用PKCE流程
description: 为OAuth 2应用程序使用PKCE流程
author: Becky
feature: Workfront API
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# 使用PKCE流程配置和使用您组织的自定义OAuth 2应用程序

PKCE是一种安全授权流，可与动态刷新的应用程序（如移动应用程序）配合使用，但在所有OAuth2客户端中非常有价值。 PKCE不使用静态客户端密钥，而是使用动态生成的字符串，从而消除了泄露客户端密钥的风险。

## PKCE概述

PKCE流程具有以下步骤。 本节中的步骤仅供参考。 要执行这些步骤，请参阅本文中的其他部分。

1. 客户端创建 `code_challenge` 通过转换 `code_verifier` 使用 `S256` 加密。

1. 客户端将浏览器以及生成的指向OAuth2登录页面 `code_challenge`. 您必须注册应用程序（客户端），以便OAuth2能够接受授权请求。 注册后，您的应用程序可以将浏览器重定向到OAuth2。

1. OAuth2授权服务器将身份验证提示重定向到用户。

1. 用户使用其中一个配置的登录选项进行身份验证，并且可能会看到一个同意页面，其中列出OAuth2将授予应用程序的权限。

1. OAuth2使用重定向回您的应用程序 `authorization code`.

1. 您的应用程序发送此代码以及 `code_verifier`，重新命名为OAuth2。

1. OAuth2授权服务器转换 `code_verifier` 使用 `code_challenge_method` 根据初始授权请求检查结果， `code_challenge`. 如果两个字符串的值匹配，则服务器已验证请求是否来自同一客户端，并将发出 `access token`.

1. OAuth2返回 `access token`和（可选） `refresh token`.

1. 您的应用程序现在可以使用这些令牌代表用户调用资源服务器，例如API。

1. 资源服务器在响应请求之前验证令牌。


## 配置应用程序

在实施授权之前，您需要通过从Workfront创建应用程序集成，在OAuth2中注册应用程序。

有关创建OAuth2应用程序的说明，请参阅 [使用PKCE创建OAuth2单页Web应用程序](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) 在 [为Workfront集成创建OAuth2应用程序](../../administration-and-setup/configure-integrations/create-oauth-application.md)


## 创建用于代码交换的验证密钥

与标准的授权代码流类似，应用程序启动时会通过将用户的浏览器重定向到授权服务器的 `/authorize` 端点。 但是，在这种情况下，您还必须传递代码质询。

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
        <td role="rowheader">代码质询</td>
        <td>
          <p>代码验证器的Base64 URL编码的SHA-256哈希</p>
        </td>
      </tr>
    </tbody>
</table>


您必须在客户端应用程序中添加代码以创建代码验证器和代码质询。

PKCE生成器代码创建类似于以下内容的输出：

>[!INFO]
>
>**示例:**
>
>```
>{
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>}
>```

您的应用程序将保存 `code_verifier` 稍后发送 `code_challenge` 以及向授权服务器发出的授权请求 `/authorize` URL。

## 请求授权码

如果您使用的是默认的自定义授权服务器，则您的请求URL将类似于以下内容：

>[!INFO]
>
>**示例:**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

请注意正在传递的参数：

* `client_id` 与配置应用程序时在中创建的OAuth2应用程序的客户端ID匹配。

  有关说明，请参阅为Workfront集成创建OAuth2应用程序中的“使用PKCE创建OAuth2单页Web应用程序”。

* `response_type` 是 `code`，因为应用程序使用授权代码授予类型。

* `redirect_uri` 是用户代理所定向到的回调位置，以及 `code`. 这必须与您在创建OAuth2应用程序时指定的重定向URL之一匹配。

* `code_challenge_method` 用于生成质询的哈希方法，始终为 `S256` 适用于使用PKCE的Workfront Oauth2应用程序。

* `code_challenge` 是用于PKCE的代码质询。


## 交换令牌的代码

要交换访问令牌的授权码，请将其传递到授权服务器的 `/token` 端点以及 `code_verifier`.

>[!INFO]
>
>**示例:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> 与常规授权码流不同，此调用不需要具有客户端ID和密码的授权标头。 因此，此版本的授权代码流适用于没有后端的本机应用程序，例如移动应用程序或单页应用程序。

请注意正在传递的参数：

* `grant_type` 是 `authorization_code`，因为应用程序使用授权代码授予类型。

* `redirect_uri` 必须匹配用于获取授权代码的URI。

* `code` 是从/authorize端点收到的授权代码。

* `code_verifier` 是您的应用程序在中生成的PKCE代码验证器 [创建用于代码交换的验证密钥](#Create).

* `client_id` 标识您的客户端，并且必须匹配在OAuth2中预注册的值。


如果代码仍然有效，并且代码验证器匹配，则您的应用程序将收到一个访问令牌。

>[!INFO]
>
>**示例:**
>
>```
>{
>    "access\_token": "eyJhd\[...\]Yozv",
>    "expires\_in": 3600,
>    "token\_type": "Bearer"
>}
>```

## 验证访问令牌

当您的应用程序传递带有访问令牌的请求时，资源服务器需要验证该请求。

您可以使用类似于以下内容的API调用验证您的访问令牌：

>[!INFO]
>
>**示例:**
>
>```
>/attask/api/<api version>/proj/search \\
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
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
