---
content-type: api
navigation-topic: api-navigation-topic
title: 为自定义OAuth 2应用程序使用JWT流程
description: 为自定义OAuth 2应用程序使用JWT流程
author: Becky
feature: Workfront API
role: Developer
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# 使用JWT流配置和使用贵组织的自定义OAuth 2应用程序

要与Workfront集成并允许您的客户端应用程序代表用户与Workfront进行通信，您必须：

* 创建OAuth2应用程序
* 创建公钥证书
* 创建JSON Web令牌(JWT)

## 创建OAuth2应用程序

有关创建OAuth2应用程序的说明，请参阅[为Workfront集成创建OAuth2应用程序](../../administration-and-setup/configure-integrations/create-oauth-application.md)中的[使用服务器身份验证（JWT流）创建OAuth2应用程序](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2)

>[!NOTE]
>
>您一次最多可以拥有10个OAuth2应用程序。

## 创建公钥证书

JWT必须经过签名并进行base-64编码以包含在访问请求中。 JWT库提供了用于执行这些任务的功能。

必须使用数字签名证书的私钥对令牌进行签名。 如果这样做，您可以使用任何关联证书的私钥来签署您的JWT。

使用的算法是RS256（使用SHA-256的RSA签名）。 这是一种非对称算法，使用公钥/私钥对。 身份提供者具有用于生成签名的私钥（密钥），并且JWT的消费者获得用于验证签名的公钥。

若要生成公钥，请执行以下操作中的&#x200B;**一个**。

* 打开MacOS/Linux终端并执行以下命令，然后使用Workfront中OAuth2应用程序设置中的&#x200B;**添加公钥**&#x200B;按钮上传`certificate_pub.crt`。

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* 在Workfront中的OAuth2应用程序设置中使用&#x200B;**生成公钥/私钥对**&#x200B;按钮来生成RSA。

## 创建JSON Web令牌

用于服务帐户身份验证的JSON Web令牌需要一组特定的声明，必须使用有效的数字签名证书进行签名。 我们建议您使用其中一个公开可用的库或工具来构建JWT。

下表包含配置JWT令牌时可能需要的字段相关信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">费用</td> 
   <td> <p>必需。 到期参数是测量自01/01/1970 GMT以来的绝对时间的必需参数。 您必须确保过期时间晚于问题发生时间。 之后，JWT不再有效。 </p> <p>注意：我们建议您拥有一个生命周期非常短的令牌（几分钟），以便该令牌在转换为访问令牌后不久过期。 每次需要新的访问令牌时，都会签署和交换一个JWT。 这是一种更安全的方法。 我们不建议根据需要重复用于获取访问令牌的长效令牌。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">iss</td> 
   <td>必需。 在OAuth2应用程序详细信息中，颁发者是您的客户ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>必需。 主题是在设置中创建公钥的用户ID。</td> 
  </tr> 
 </tbody> 
</table>

## 交换JWT以检索访问令牌

1. 发送POST请求到：

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. 请求正文应包含URL编码的参数，以及您的客户端ID、客户端密钥和JWT：

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
