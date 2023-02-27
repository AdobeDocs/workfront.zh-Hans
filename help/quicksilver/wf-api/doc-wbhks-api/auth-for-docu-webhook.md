---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 文档Webhook的身份验证
description: 文档Webhook的身份验证
author: Becky
feature: Workfront API
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 文档Webhook的身份验证

## 身份验证

Adobe Workfront文档webhook支持两种不同的身份验证形式：OAuth2和ApiKey。 在这两种情况下，Workfront在进行API调用时都会在标头中传递身份验证令牌。

### OAuth2

OAuth2允许Workfront代表用户对Webhook提供程序进行授权API调用。 在执行此操作之前，用户必须将其外部文档提供程序帐户连接到Workfront并授予Workfront

有权代表他们行事。 此握手过程仅对每个用户进行一次。 其工作原理如下：

1. 用户开始将Webhook集成连接到其帐户。 目前，可通过单击“添加文档”下拉列表>“添加服务”>“自定义集成名称”来完成此操作。
1. Workfront在身份验证URL中导航用户，这可能会提示用户登录到外部文档提供程序。 此页面由Webhook提供程序或外部文档管理系统托管。 这样做时，Workfront会向身份验证URL中添加“state”参数。 此值必须通过以下步骤中的将相同的值附加到Workfront返回URI来传递回Workfront。
1. 登录到外部系统后（或用户已登录），用户将进入“身份验证”页面，该页面说明Workfront正在请求访问权限以代表用户执行一组操作。
1. 如果用户单击“允许”按钮，浏览器将重定向到Workfront重定向URI ，并添加“code=`<code>`&quot;到querystring。 根据OAuth2规范，此令牌的生命周期很短。 查询字符串还必须具有以下项： &quot;state=`<sent_by_workfront>`&quot;
1. Workfront会处理此请求，并使用授权代码对令牌端点URL进行API调用。
1. 令牌端点URL会返回刷新令牌和访问令牌。
1. Workfront存储了这些令牌，并为此用户完全配置了webhook集成。
1. 从此刻起，Workfront将能够对Webhook提供商进行授权的API调用。 进行这些调用时，Workfront将在HTTP请求标头中发送访问令牌，如下所示：

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. 如果访问令牌已过期，Workfront将调用令牌端点URL以检索新的访问令牌，然后使用新的访问令牌再次尝试授权的API调用。

### ApiKey

使用ApiKey向Webhook提供程序进行授权API调用比OAuth2简单得多。 进行API调用时，Workfront将只需在HTTP请求标头中传递ApiKey和Workfront用户名： 

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Webhook提供程序可以使用用户名来应用特定于用户的权限。 当两个系统都使用单点登录(SSO)连接到LDAP时，这种方法最有效。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of “username:password”. See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
