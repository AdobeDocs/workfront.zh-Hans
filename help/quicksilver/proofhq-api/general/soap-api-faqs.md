---
title: SOAP API常见问题解答
description: SOAP API常见问题解答
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 79b6370ec3283922a16435e8eb8069f7f9560c55
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# SOAP API常见问题解答

## 如何创建第一个文件校对？

它需要3个简单的步骤：

**步骤1**：通过Post请求将文件发送到，以将文件上传到Workfront Proof  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php)。 我们将返回文件哈希 — 这非常重要！ 请注意，在此阶段，您不会看到帐户中的任何内容，您迄今为止所做的一切只是向我们发送文件，但未告知我们应如何处理该文件。

**步骤2**：如果还没有会话ID，请使用doLogin()或getSessionID()方法获取一个。 使用前者可使用用户的电子邮件地址和密码“登录”，如果您拥有用户的电子邮件地址和身份验证令牌，则使用后者进行登录。

**步骤3：**&#x200B;现在可以创建校对。 使用createProof()方法向我们发送至少必填字段（当前只有5个必填字段）。 请确保将哈希参数设置为在“步骤1”中返回的文件哈希，因为这将允许我们确定在创建验证时使用的文件。

如果您现在登录到您的帐户，您将看到证明。

## 如何创建我的第一个Web快照校对？

它需要2个简单的步骤：

**步骤1**：如果还没有会话ID，请使用doLogin()或getSessionID()方法获取一个。 使用前者可使用用户的电子邮件地址和密码“登录”，如果您拥有用户的电子邮件地址和身份验证令牌，则使用后者进行登录。

**步骤2：**现在可以创建校对。 使用createProof()方法向我们发送至少必填字段（当前只有5个必填字段）。 确保将Hash参数设置为“web”，并将SourceName参数设置为要捕获的网页的URL。

如果您现在登录到您的帐户，您将看到证明。

## 验证和版本之间有何区别？

在Workfront Proof中，版本显示为单个校对。 单击Web UI中的特定版本将显示该版本的详细信息。 实际上，每个版本都是一个单独的验证，Web UI会一起显示这些验证。

从API的角度来看，每个版本都是一个单独的验证，并且验证通过其ID链接在一起。

**createProof()**&#x200B;将始终创建&#x200B;**版本1**&#x200B;的校对。 例如，假设为此校对返回的ID为“100”。

使用&#x200B;**createProofVersion()**&#x200B;时，始终发送早期版本的ID。 如果要在校对“100”上创建&#x200B;**版本2**，我们&#x200B;**为ParentFileID**&#x200B;参数传入“100”。 这会告知系统，此验证应为集合的版本2。 方法将返回唯一的校对ID，例如，假设这是“101”。

如果需要第三个版本，即&#x200B;**版本3**，您将再次调用&#x200B;**createProofVersion()**，这次为ParentFileID **传递“101”，这将确保正确创建版本的链接列表。**

## 我是否需要在每次调用之前获取新的会话ID？

需要指出的是，每个会话ID本质上都是一个执行操作的用户。 

您无需在每次调用API之前获取新的会话ID，会话ID将在24小时内保持有效。 每次调用API时，到期时间都会重置。

## 什么是校对/个人URL？

**团队/公共**：每个校对版本都有一个唯一的团队（公共）URL。 如果启用，它将以只读模式打开验证。 您可以使用[getProofURL()](https://api.proofhq.com/home/proofs/getproofurl.html)方法获取团队URL。

**个人**：每个审阅人和验证版本的个人URL都是唯一的。 如果验证集包含3个版本，并且查看者位于所有版本，则查看者将具有3个唯一的个人URL。 个人URL会打开验证版本，其中已识别审阅人，因此应保持安全且不予共享。 通过调用[getProofReviewers()](https://api.proofhq.com/home/proofs/getproofreviewers.html)方法，然后对每个方法进行迭代，可以获得个人URL  [SOAPRecepientObject](https://api.proofhq.com/home/objects/soaprecipientobject.html)，正在获取参数“proof_url”。

## >在打开小型验证时如何包含自定义参数？

通过小型校对，可将校对工具嵌入到您自己的页面中。 “referer”参数可以包含在miniproof中，以便在用户单击miniproof中的关闭按钮时提供重定向URL。 通过使用转义的“&amp;”字符（例如%26）附加任意数量的自定义参数，您可以将这些参数包含在此重定向URL中。

例如，miniproof URL
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=`必须编码为 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=`以便传递自定义参数。


