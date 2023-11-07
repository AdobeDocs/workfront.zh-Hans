---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 文档Webhook的身份验证
description: 文档Webhook的身份验证
author: Becky
feature: Workfront API
role: Developer
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 文档Webhook的身份验证

## 身份验证

Adobe Workfront文档webhook支持两种不同的身份验证形式：OAuth2和ApiKey。 在这两种情况下，Workfront在进行API调用时在标头中传递身份验证令牌。

### OAuth2

OAuth2允许Workfront代表用户向webhook提供程序发出授权的API调用。 在执行此操作之前，用户必须将其外部文档提供商帐户连接到Workfront并授予Workfront

代表他们行事的权限。 此握手过程仅针对每个用户发生一次。 以下是它的工作方式：

1. 用户开始将webhook集成连接到其帐户。 目前，可通过单击“添加文档”下拉列表>“添加服务”>自定义集成名称来完成此操作。
1. Workfront会为用户导航身份验证URL，这可能会提示用户登录到外部文档提供商。 此页面由webhook提供程序或外部文档管理系统托管。 在执行此操作时，Workfront会向身份验证URL添加“state”参数。 必须在以下步骤中，通过将相同的值附加到Workfront返回URI，将此值传递回Workfront。
1. 登录到外部系统后（或者如果用户已登录），用户将被带到“身份验证”页面，该页面解释Workfront正在请求访问权限以代表用户执行一组操作。
1. 如果用户单击“允许”按钮，浏览器将重定向到Workfront重定向URI ，并添加“code=`<code>`”到查询字符串。 根据OAuth2规范，此令牌的生命周期短。 查询字符串还必须具有以下“state=`<sent_by_workfront>`“。
1. Workfront处理此请求，并使用授权代码对令牌端点URL进行API调用。
1. 令牌端点URL返回刷新令牌和访问令牌。
1. Workfront存储这些令牌并完全为此用户预配webhook集成。
1. 从此刻起，Workfront将能够向webhook提供商发出授权的API调用。 进行这些调用时，Workfront将在HTTP请求标头中发送访问令牌，如下所示：

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. 如果访问令牌已过期，Workfront将调用令牌端点URL以检索新的访问令牌，然后尝试使用新的访问令牌再次尝试授权API调用。

### ApiKey

使用ApiKey向webhook提供程序进行授权API调用比OAuth2简单得多。 进行API调用时，Workfront只需在HTTP请求标头中传递ApiKey和Workfront用户名即可： 

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Webhook提供程序可以使用用户名来应用特定于用户的权限。 当两个系统都使用单点登录(SSO)连接到LDAP时，这种方法效果最佳。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of "username:password". See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
