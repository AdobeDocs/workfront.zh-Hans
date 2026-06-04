---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 重命名文档或文件夹（尚未实现）
description: 重命名文档或文件夹
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
TQID: https://experienceleague.adobe.com/-HmJkcMckTK6upblNcqX5LZkdYQxoWPDeuHkFjJarh4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 81
ht-degree: 9%

---

# 重命名文档或文件夹（尚未实现）

重命名外部系统中具有给定ID的文档或文件夹。

**URL**

PUT /rename

## 查询参数

| 名称  | 描述 |
|---|---|
| ID | 要重命名的文档或文件夹ID |
| name  | 文档或文件夹的新名称 |


## 响应

指示成功或失败的JSON字符串，如下面的错误处理部分中所述。

**示例：** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

返回

```
{status: "success"
 }returns
 {
 status: "failure", error: "Folder cannot be renamed because a folder with that name already exists."
 }
```
