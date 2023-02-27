---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 获取OAuth2令牌
description: 获取OAuth2令牌
author: Becky
feature: Workfront API
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 4%

---


# 获取OAuth2令牌

## 获取OAuth2令牌

返回已验证用户的OAuth2刷新令牌和访问令牌。 当用户设置文档提供程序时，将调用一次。 随后将调用以获取更新的访问令牌。

**URL**

POST/any/url

该URL是可配置的，并与自定义集成设置页面上的令牌端点URL值相对应。

### 查询参数

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>名称</th>
   <th>必填</th>
   <th>描述</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>grant_type</td>
   <td>是</td>
   <td><p>值包括“authorizationcode”或“refreshtoken”。 指定的值指示将将将这两个参数中的哪个参数传递到此API调用：代码或refresh_token。</p></td>
  </tr>
  <tr>
   <td>代码</td>
   <td>依赖</td>
   <td><p>在用户单击“授权”按钮后，发送到Adobe Workfront的授权代码。 仅当授权类型为“authorization_code”时，才需要执行此操作。 授权代码应为短时间，通常在10分钟或更短时间内过期。</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>依赖</td>
   <td><p>只有在发出后续调用以检索新的access_token时才需要执行此操作，前提是之前的access_token已过期。 发送此值时，将grant_type参数设置为“refresh_token”。</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>是</td>
   <td>在Workfront中为此自定义集成配置的客户端ID。</td>
  </tr>
  <tr>
   <td>client_secret</td>
   <td>是</td>
   <td> 在Workfront中为此自定义集成配置的客户端密钥。</td>
  </tr>
 </tbody>
</table>

 

## 个回应

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>名称</th>
   <th>类型 </th>
   <th>描述</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>access_token </td>
   <td>字符串</td>
   <td><p>用于代表用户进行授权API调用的令牌。 此设置应会过期，以防止未经授权的API调用。</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>字符串</td>
   <td><p>一个长期使用的令牌，用于通过调用此API方法来检索新的access_token。</p></td>
  </tr>
  <tr>
   <td>expires_in </td>
   <td>long</td>
   <td><p>（可选）access_token过期之前的时间（以秒为单位），通常为3,600。</p></td>
  </tr>
 </tbody>
</table>

**示例**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```

## 个回应

```
{
access_token:"ad8af5ad5ads759",
refresh_token:"9a0h5d87d808ads",
expires_id:3600
}
```
