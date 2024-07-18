---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 注册Webhook集成
description: 注册Webhook集成
author: Becky
feature: Workfront API
role: Developer
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 11%

---


# 注册Webhook集成

Adobe Workfront管理员可以通过导航到Workfront中的设置>文档>自定义集成，为其公司添加自定义webhook集成。 在“设置”的“自定义集成”页面中，管理员可以查看现有文档Webhook集成的列表。 在此页面中，可以添加、编辑、启用和禁用集成。

要添加集成，请单击&#x200B;**添加自定义集成**。

![](assets/webhooks-integration-350x230.png)

![](assets/webhooks-integration-2-350x220.png)

## 可用字段

添加集成时，管理员将在以下字段中输入值。

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
   <td> <p>回调API的位置。 调用外部系统时，Workfront只需将端点名称附加到此地址即可。 例如，如果管理员输入基本API URL " https://www.mycompany.com/api/v1 "，Workfront将使用以下URL获取文档的元数据：https://www.mycompany.com/api/v1/metadata?id=1234。</p> </td> 
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
   <td> <p>（仅限OAuth2）用于用户身份验证的完整URL。 在OAuth配置过程中，Workfront会将用户导航到此地址。 注意：Workfront会将“state”参数附加到查询字符串中。 提供程序必须通过将它附加到Workfront重定向URI来将它传递回Workfront。</p> </td> 
  </tr> 
  <tr> 
   <td>令牌端点 URL</td> 
   <td> <p>（仅限OAuth2）用于检索OAuth2令牌的完整API URL。 它由webhook提供程序或外部文档提供程序托管</p> </td> 
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
   <td>（仅限OAuth2）这是只读字段，由Workfront生成。 此值用于将该集成注册到外部文档提供商。 注意：如上所述，对于身份验证URL，提供程序必须在执行重定向时将“state”参数及其值附加到查询字符串。</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>（仅限ApiKey）用于向webhook提供程序进行授权的API调用。 webhook提供程序发布的API密钥。</p> </td> 
  </tr> 
 </tbody> 
</table>
