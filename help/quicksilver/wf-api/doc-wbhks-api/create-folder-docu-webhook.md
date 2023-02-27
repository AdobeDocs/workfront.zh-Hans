---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 使用文档Web挂接创建文件夹
description: 使用文档Web挂接创建文件夹
author: Becky
feature: Workfront API
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 7%

---


# 使用文档Web挂接创建文件夹

在给定目录中创建文件夹。

## URL

POST/createFolder

## 查询参数

| **名称** | **描述** |
|---|---|
| parentId  | 应在其中创建文件夹的文件夹ID |
| name  | 新文件夹的名称 |




**响应**

新创建文件夹的元数据，由/metadata端点定义。

## 示例

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

返回

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"”,
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
