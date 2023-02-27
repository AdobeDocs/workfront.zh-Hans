---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 注册Webhook集成
description: 注册Webhook集成
author: Becky
feature: Workfront API
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 11%

---


# 注册Webhook集成

Adobe Workfront管理员可以通过导航到Workfront中的设置>文档>自定义集成，为其公司添加自定义webhook集成。 从“设置”中的“自定义集成”页面，管理员可以查看现有文档Webhook集成的列表。 在此页面中，可以添加、编辑、启用和禁用集成。

要添加集成，请单击 **添加自定义集成**.

![](assets/webhooks-integration-350x230.png)

![](assets/webhooks-integration-2-350x220.png)

## 可用字段

添加集成时，管理员将为以下字段输入值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>字段名称</th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>名称</td> 
   <td>此集成的名称。</td> 
  </tr> 
  <tr> 
   <td>基本 API URL</td> 
   <td> <p>回调API的位置。 调用外部系统时，Workfront只需将端点名称附加到此地址。 例如，如果管理员输入了基本API URL(“ https://www.mycompany.com/api/v1 ”)，则Workfront将使用以下URL获取文档的元数据：https://www.mycompany.com/api/v1/metadata?id=1234。</p> </td> 
  </tr> 
  <tr> 
   <td>请求参数</td> 
   <td> <p>要附加到每个 API 调用的查询字符串的可选值。例如，access_type=offline。 </p> </td> 
  </tr> 
  <tr> 
   <td>身份验证类型</td> 
   <td>OAuth2或ApiKey</td> 
  </tr> 
  <tr> 
   <td>身份验证 URL</td> 
   <td> <p>（仅限OAuth2）用于用户身份验证的完整URL。 Workfront将在OAuth配置过程中将用户导航到此地址。 注意：Workfront将在查询字符串中附加“state”参数。 提供程序必须通过将其附加到Workfront重定向URI，将其传递回Workfront。</p> </td> 
  </tr> 
  <tr> 
   <td>令牌端点 URL</td> 
   <td> <p>（仅限OAuth2）用于检索OAuth2令牌的完整API URL。 由Webhook提供程序或外部文档提供程序托管</p> </td> 
  </tr> 
  <tr> 
   <td>客户端 ID</td> 
   <td>（仅限OAuth2）此集成的OAuth2客户端ID</td> 
  </tr> 
  <tr> 
   <td>客户端密码</td> 
   <td> <p>（仅限OAuth2）此集成的OAuth2客户端密钥</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront 重定向 URI</td> 
   <td>（仅限OAuth2）这是只读字段，由Workfront生成。 此值用于向外部文档提供程序注册此集成。 注意：如上所述，对于身份验证URL，提供程序在执行重定向时必须将“state”参数及其值附加到查询字符串。</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>（仅限ApiKey）用于对Webhook提供程序进行授权API调用。 由Webhook提供程序颁发的API密钥。</p> </td> 
  </tr> 
 </tbody> 
</table>
