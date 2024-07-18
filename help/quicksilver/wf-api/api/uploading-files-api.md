---
content-type: api
navigation-topic: api-navigation-topic
title: 通过API上传文件
description: 通过API上传文件
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 通过API上传文件

您可以使用带有API工具(例如Postman)的Workfront API或简单的cURL命令上传文件。

要上传文档，请参阅Workfront [Post行为](/help/quicksilver/wf-api/general/api-basics.md#post-behavior)中&#x200B;**上传文档**&#x200B;的说明。 您还可以将这些相同的说明用于cURL请求。

**使用API工具上载文件时，请遵循以下准则：**

* 使用API工具选项上传文件。 这些通常是请求屏幕上的&#x200B;**选择文件**&#x200B;按钮。

* 使用POSTHTTP方法发出上传文件的请求。

* 您的请求应导致响应包含其句柄的值。

* 在JSON有效负载中使用objID的句柄值、对象类型和GUID值进行后续调用。 这用于为文件创建对象，如以下示例所示：

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

您应在响应中收到对象的ID。

有关更多信息，请参阅您使用的特定API工具的帮助。
