---
title: 概述
description: 概述
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 1%

---

# 概述

**欢迎使用Workfront Proof API**

Workfront Proof API是使用SSL保护的简单HTTP服务。 该API旨在为您提供我们自己的应用程序中使用的所有功能。

## 支持的格式

公共接口与WSDL支持兼容SOAP 1.1。 因此，所有请求都将通过HTTPS使用XML执行。

## API版本控制

为了保持与现有客户端集成的兼容性，我们从12.1版本引入了API版本控制。 请参阅  [API更新](https://api.proofhq.com/new-updates.html)页面以了解更多信息。 如果某个方法或参数没有版本信息，则意味着您会在标准API中找到此信息，请参阅下面的“API快速入门”部分。

## API快速入门

API入口点：

`https://soap.proofhq.com/soap` （请注意HTTPS的使用）

可以在此处找到WSDL：

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**此WSDL包含到12.1版本之前的所有更改，此后我们引入了API版本控制。 有关各种WSDL版本和即将进行的更改的详细信息，请参阅API更新页面**

每个API请求都需要会话密钥。 此会话密钥用于标识执行操作的Workfront Proof用户，可通过调用doLogin()方法并传入用户的电子邮件地址和密码来获取。 在一系列API请求之前，只需要调用一次doLogin()方法。 会话密钥在短时间内保持活动状态，并在每次方法调用时续订。 *我们很快将添加对基于令牌的身份验证的支持。*

所有请求都使用以下信封、标题和正文格式：

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

