---
content-type: api
navigation-topic: api-navigation-topic
title: 自定义OAuth 2应用程序的授权代码流
description: 自定义OAuth 2应用程序的授权代码流
author: John
feature: Workfront API
exl-id: a1ab60c4-4255-4d80-87f1-f36d325254c2
source-git-commit: e67f397ec82858bc489313db963259ce05175428
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---


# 使用授权代码流配置和使用贵组织的自定义OAuth 2应用程序

要与Workfront集成并允许您的客户端应用程序代表用户与Workfront通信，您必须：

* 创建OAuth2应用程序
* 配置第三方应用程序
* 链接到用户的授权页面
* 设置授权代码流：用户登录到Workfront实例，并同意允许客户端应用程序代表他们连接到Workfront。 因此，您会获得一个授权代码，该代码将与访问和刷新令牌进行交换。
* 设置刷新令牌流：在此流程中，您可以使用刷新令牌在旧访问令牌过期时获取新访问令牌。

## 创建OAuth2应用程序

有关创建OAuth2应用程序的说明，请参阅 [使用用户凭据（授权代码流）创建OAuth2应用程序](../../administration-and-setup/configure-integrations/create-oauth-application.md#create3) in [为Workfront集成创建OAuth2应用程序](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## 链接到用户的授权页面

您的用户需要登录才能在其自己的帐户中授权此集成。 供他们授权的页面具有特定格式，如下所述。 使用此信息可确定应用程序授权页面的地址，并为用户提供此地址或指向此地址的链接。

* 您组织域的完整URL。 示例:

   ```
   https://myorganization.my.workfront.com
   ```


* `client_id`:这是您在Workfront中创建OAuth2应用程序时生成的客户端ID。

* `redirect_uri`:这是您在创建应用程序时输入的重定向URL。 在用户为其帐户授权应用程序后，会将用户定向到此页面。

* `response_type`:此参数必须具有值 `code`.

因此，授权页面的URL是：

```
https://<URL of your organization's domain>/integrations/oauth2/authorize?client_id=<Your ClientID>&redirect_uri=<Your redirect URL>&response_type=code
```

>[!NOTE]
>
>我们建议创建一个按钮或其他链接，供用户单击以定向到此页面。

## 配置第三方应用程序

第三方应用程序可能需要配置。 下表包含有关配置第三方应用程序时可能需要的字段的信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">授权URI</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/authorize</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code> https://myorganization.my.workfront.com/integrations/oauth2/authorize</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">令牌URL</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/api/v1/token</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>https://myorganization.my.workfront.com/integrations/oauth2/api/v1/token</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">范围</td> 
   <td>您无需指定作用域。 </td> 
  </tr> 
 </tbody> 
</table>

## 设置授权代码流

![](assets/oauth-2-authorization-code-flow-350x194.png)

要使用OAuth2登录用户，请使用以下过程：

1. 当用户打开授权页面时，它会重定向到Workfront登录页面，以便用户可以登录Workfront。 如果用户具有SSO配置，则将打开身份提供程序登录页面。

   如果用户已在同一浏览器上登录到Workfront，或者用户成功登录到Workfront，则用户将被重定向到同意屏幕：

   ![](assets/consent-screen-350x227.png)

1. 如果用户允许访问，则页面将被重定向到 `redirect_url`. 重定向必须包含以下查询参数：

* `code`:获取访问/刷新令牌所需的授权代码。
* `domain`:您组织的域。 示例：in `myorganization.my.workfront.com`，域为 `myorganization`.
* `lane`:请求的通道。 示例：in `myorganization.preview.workfront.com`，车道是 `preview`.

   >[!IMPORTANT]
   >
   >的 `code` 仅有效2分钟。 因此，您必须在该时间内获取刷新和访问令牌。

1. 当您拥有代码时，您可以通过将代码与客户端应用程序凭据一起发送到 `/integrations/oauth2/api/v1/token` 端点。

   完整的令牌请求URL为

   ```
   https://<URL of your organization's domain></span>/integrations/oauth2/api/v1/token
   ```

   **示例：**  对令牌端点的CURL调用示例：

   示例1

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Authorization: Basic **<base64(client_id:client_secret)>**' \
      --header 'Content-Type: application/json' \
      --data-raw '{
      "code": "**<code>**",
      "grant_type": "**authorization_code**",
      "redirect_uri": "**<redirect_url>**"
      }'
   ```

   示例2

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Content-Type: application/x-www-form-urlencoded' \
      --data-urlencode 'grant_type=**authorization_code**' \
      --data-urlencode 'redirect_uri=**<redirect_url>**' \
      --data-urlencode 'code=**<code>**' \
      --data-urlencode 'client_id=**<client_id>**' \
      --data-urlencode 'client_secret=**<client_secret>**'  
   ```


   >[!IMPORTANT]
   >
   > 在Workfront中注册应用程序时，会生成客户端密钥。 您应将其存储在安全位置，因为如果丢失，则无法恢复。

   当所有传递的参数均正确无误时，令牌端点会返回以下负载：

   ```
   {
      "token_type": "sessionID",
      "access_token": "string", // the value of sessionID
      "refresh_token": "string",
      "expires_in": 0,
      "wid": "string"
   }
   ```

   访问令牌与 ```sessionID```，且其过期方式与常规相同 ```sessionID```

   >[!IMPORTANT]
   >
   > 将刷新令牌存储在安全位置。 旧令牌过期后，您将需要它来获取新的刷新令牌。 Workfront不存储您的刷新令牌。

1. 现在，当您拥有访问令牌时，可以对Workfront进行API调用

   ```
   curl --request GET 'https://<workfront host>/attask/api/v14.0/proj/search \
   --header 'sessionID: <access_token>'
   ```

## 设置刷新访问令牌

![](assets/refresh-access-token-flow-350x142.png)

要刷新access_token，我们再次需要对令牌端点执行“POST”调用。 这次，我们发送不同的表单数据，如下所示：

```
curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Authorization: Basic <base64(client_id:client_secret)>' \
--header 'Content-Type: application/json' \
--data-raw '{
   "grant_type": "refresh_token",
   "refresh_token": "<refresh_token>"
}'

###### OR

curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--data-urlencode 'grant_type=refresh_token' \
--data-urlencode 'redirect_uri=<redirect_url>' \
--data-urlencode 'refresh_token=<refresh_token>' \
--data-urlencode 'client_id=<client_id>' \
--data-urlencode 'client_secret=<client_secret>'
```

它将返回以下结果：

```
{
  "token_type": "sessionID",
  "access_token": "string", // the value of sessionID
  "refresh_token": "string",
  "expires_in": 0,
  "wid": "string"
}
```

同样，访问令牌是 `sessionID` 可用于向Workfront发出API请求。
