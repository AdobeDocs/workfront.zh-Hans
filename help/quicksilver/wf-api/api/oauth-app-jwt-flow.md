---
content-type: api
navigation-topic: api-navigation-topic
title: 对自定义OAuth 2应用程序使用JWT流
description: 对自定义OAuth 2应用程序使用JWT流
author: John
feature: Workfront API
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: 38e957253775f73cee7fe0c0d31bfeedb58ebf53
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# 使用JWT流程配置和使用贵组织的自定义OAuth 2应用程序

要与Workfront集成并允许您的客户端应用程序代表用户与Workfront通信，您必须：

* 创建OAuth2应用程序
* 创建公钥证书
* 创建JSON Web令牌(JWT)

## 创建OAuth2应用程序

有关创建OAuth2应用程序的说明，请参阅 [使用服务器身份验证（JWT流程）创建OAuth2应用程序](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) in [为Workfront集成创建OAuth2应用程序](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## 创建公钥证书

必须对JWT进行签名，并对base-64进行编码，以便包含在访问请求中。 JWT库提供用于执行这些任务的功能。

令牌必须使用数字签名证书的私钥进行签名。 如果这样做，您可以使用任何关联证书的私钥来签署您的JWT。

使用的算法是RS256（RSA签名与SHA-256）。 这是一种非对称算法，它使用公钥/私钥对。 身份提供者具有用于生成签名的私钥（密钥），JWT的使用者将获得用于验证签名的公钥。

要生成公钥，请执行 **one** 下面的。

* 打开MacOS/Linux终端并执行以下命令，然后上传 `certificate_pub.crt` 使用 **添加公钥** 按钮。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* 使用 **生成公共/私有密钥对** 按钮以生成RSA。

## 创建JSON Web令牌

用于服务帐户身份验证的JSON Web令牌需要一组特定声明，并且必须使用有效的数字签名证书进行签名。 我们建议您使用其中一个公开可用的库或工具来构建JWT。

下表包含有关配置JWT令牌时可能需要的字段的信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>必填. 过期参数是测量自GMT 01/01/1970以来绝对时间的必需参数。 您必须确保过期时间晚于问题时间。 此后，JWT将失效。 </p> <p>注意：我们建议您使用非常短的令牌（几分钟），以便在交换访问令牌后该令牌不久就会过期。 每次需要新的访问令牌时，都会签署和交换一个JWT。 这是一种更安全的方法。 我们建议不要使用较长的令牌来根据需要重新获取访问令牌。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">iss</td> 
   <td>必填. 颁发者是您在OAuth2应用程序详细信息中的客户ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>必填. 主题是您在设置中创建公钥的用户ID。</td> 
  </tr> 
 </tbody> 
</table>

## 交换JWT以检索访问令牌

1. 将POST请求发送到：

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. 请求正文应包含URL编码的参数，其中包含您的客户端ID、客户端密钥和JWT:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
