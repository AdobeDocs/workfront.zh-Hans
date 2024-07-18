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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '78'
ht-degree: 3%

---


# 重命名文档或文件夹（尚未实现）

重命名外部系统中具有给定ID的文档或文件夹。

**URL**

PUT/rename

## 查询参数

| 名称  | 描述 |
|---|---|
| id | 要重命名的文档或文件夹ID |
| name  | 文档或文件夹的新名称 |


## 响应

指示成功或失败的JSON字符串，如下面的错误处理部分中所述。

**示例：** PUThttps://www.acme.com/api/rename

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
