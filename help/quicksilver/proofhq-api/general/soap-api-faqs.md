---
title: SOAP API常见问题解答
description: SOAP API常见问题解答
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# SOAP API常见问题解答

## 如何创建我的第一个文件校样？

它需要3个简单的步骤：

**步骤1**:通过向发送Post请求，将文件上传到Workfront校样  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). 我们会将文件散列返回给您 — 这非常重要！ 请注意，在此阶段，您的帐户中将看不到任何内容，您迄今所做的只是将文件发送给我们，但没有告诉我们如何处理它。

**步骤2**:如果您还没有会话ID，请使用doLogin()或getSessionID()方法获取一个会话ID。 使用前者使用用户的电子邮件地址和密码“登录”，或者使用后者方法（如果您具有用户的电子邮件地址和身份验证令牌）。

**步骤3:** 现在该创建证据了。 使用createProof()方法并至少向我们发送必填字段（当前只有5个必填字段）。 确保将Hash参数设置为在“步骤1”中返回的文件哈希，因为这样我们就可以确定在创建校样时要使用的文件。

如果您现在登录帐户，将看到校样。

## 如何创建我的第一个Web快照校样？

它需要执行两个简单的步骤：

**步骤1**:如果您还没有会话ID，请使用doLogin()或getSessionID()方法获取一个会话ID。 使用前者使用用户的电子邮件地址和密码“登录”，或者使用后者方法（如果您具有用户的电子邮件地址和身份验证令牌）。

**第2步：**现在该创建校样了。 使用createProof()方法并至少向我们发送必填字段（当前只有5个必填字段）。 确保将Hash参数设置为“web”，将SourceName参数设置为要捕获的网页的URL。

如果您现在登录帐户，将看到校样。

## 验证和版本之间有何区别？

在Workfront校样版本中，显示为单个校样。 单击Web UI中的特定版本将显示该版本的详细信息。 实际上，每个版本都是一个单独的校样，Web UI会将它们一起显示。

对于API而言，每个版本都是一个单独的校样，并且校样通过其ID链接在一起。

**createProof()** 将始终创建 **版本1** 证据。 假设在我们的示例中为此校样“100”返回了ID。

使用 **createProofVersion()** 始终以先前版本的ID发送。 如果我们想要创建 **版本2** 在证据&quot;100&quot;上，我们 **在“100”中传递ParentFileID** 参数。 这告知系统此校样应为集版本2。 方法将返回一个唯一的校样ID，例如，假设为“101”。

如果是第三个版本，即 **版本3** 是必需的，您将调用 **createProofVersion()** 这次又一次 **在“101”中传递ParentFileID** 这将确保正确创建已链接的版本列表。

## 是否需要在每次调用之前获取新的会话ID?

必须指出，每个会话ID本质上都是执行操作的用户。 

在每次调用API之前，您无需获取新的会话ID，该ID将在24小时内保持有效。 每次调用API时，过期时间都会重置。

## 什么是校样/个人URL?

**团队/公共**:每个校样版本都有一个唯一的团队（公共）URL。 如果启用，则将以只读模式打开校样。 您可以使用 [getProofURL()](http://api.proofhq.com/home/proofs/getproofurl) 方法。

**个人**:每个审阅人和校样版本的个人URL都是唯一的。 如果校样集包含3个版本，并且审阅者位于所有版本上，则审阅者将具有3个唯一的个人URL。 个人URL会打开已经由审阅人识别的校样版本，因此应该保持安全且不共享。 可通过调用 [getProofReviewers()](http://api.proofhq.com/home/proofs/getproofreviewers) 方法，然后迭代  [SOAPRecepientObject](http://api.proofhq.com/home/objects/soaprecipientobject) 和获取参数“proof_url”。

## >打开小校样时如何包含自定义参数？

通过小型校样，您可以在自己的页面中嵌入校样工具。 “referer”参数可作为小型校样的一部分包含在内，以便当用户单击小型校样中的关闭按钮时提供重定向URL。 您可以在此重定向URL中包含任意数量的自定义参数，方法是使用转义的“&amp;”字符(例如，%26。

例如，小型校样URL
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` 必须编码为 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` 以便传递自定义参数。

## 如何创建Java Web服务客户端？

[此视频](http://screencast.com/t/xsSNrqs5b) 显示如何使用Eclipse和Workfront校样WSDL定义创建Java Web服务客户端。
