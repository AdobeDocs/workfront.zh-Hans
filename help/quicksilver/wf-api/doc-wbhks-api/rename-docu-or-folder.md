---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 重命名文档或文件夹（尚未实施）
description: 重命名文档或文件夹
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 6%

---


# 重命名文档或文件夹（尚未实施）

在外部系统中使用给定ID重命名文档或文件夹。

**URL**

PUT/重命名

## 查询参数

| 名称  | 描述 |
|---|---|
| id | 要重命名的文档或文件夹ID |
| name  | 文档或文件夹的新名称 |


## 个回应

指示成功或失败的JSON字符串，如下面的错误处理部分中指定。

**示例：** PUThttps://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

返回

```
{status: “success”
 }returns
 {
 status: “failure”, error: “Folder cannot be renamed because a folder with that name already exists.”
 }
```
