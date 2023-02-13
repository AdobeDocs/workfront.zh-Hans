---
title: 概述
description: 概述
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 1%

---

# 概述

**欢迎使用Workfront Proof API**

Workfront校样API是一项简单的HTTP服务，使用SSL进行保护。 API旨在为您提供我们自己的应用程序中使用的所有功能。

## 支持的格式

公共接口符合SOAP 1.1与WSDL支持的规范。 因此，所有请求都使用XML通过HTTPS执行。

## API版本控制

为了保持与现有客户端集成的兼容性，我们从12.1版本中引入了API版本控制。 请参阅  [API更新](http://api.proofhq.com/new-updates) 页面以了解更多信息。 如果方法或参数没有版本信息，则意味着您将在我们的标准API中找到该内容，请参阅下面的“API快速入门”部分。

## API快速入门

API入口点：

`https://soap.proofhq.com/soap` （请注意使用HTTPS）

可以在以下位置找到WSDL:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**在12.1版本之前，此WSDL包含所有更改，在此版本之后，我们引入了API版本控制。 有关各种WSDL版本和即将进行的更改的详细信息，请参阅API更新页面**

每个API请求都需要一个会话密钥。 此会话密钥标识执行操作的Workfront校样用户，并通过调用doLogin()方法并传递用户的电子邮件地址和密码来获取该用户。 只需在API请求序列之前调用一次doLogin()方法。 会话键会保持短时间活动状态，并在每次方法调用时续订。 *我们很快将添加对基于令牌的身份验证的支持。*

所有请求都使用以下信封、标题和正文格式：

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
	   ... API function and data inserted here ...
	</soapenv:Body>
	</soapenv:Envelope>
```

## 常见问题解答

有关常见问题集合，请访问 [此](http://api.proofhq.com/faqs) 页面。
