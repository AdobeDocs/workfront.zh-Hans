---
content-type: api
navigation-topic: api-navigation-topic
title: 通过API上传文件
description: 通过API上传文件
author: Becky
feature: Workfront API
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 通过API上传文件

您可以通过API工具(如Postman)或简单的cURL命令，使用Workfront API上传文件。

要上载文档，请参阅 **上传文档** 在Workfront [帖子行为](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWF_API%2FGeneral%2Fapi-basics.html). 您还可以对cURL请求使用相同的说明。

**使用API工具上传文件时，请遵循以下准则：**

* 使用API工具选项上传文件。 这通常是 **选择文件** 按钮。

* 使用POSTHTTP方法请求上传文件。

* 您的请求应会生成一个响应，该响应中包含其句柄的值。

* 在JSON有效负载中使用objID的句柄值、对象类型和GUID值，以进行后续调用。 这用于为文件创建对象，如以下示例中所示：

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

您应会在响应中收到对象的ID。

有关更多信息，请参阅您使用的特定API工具的帮助。
