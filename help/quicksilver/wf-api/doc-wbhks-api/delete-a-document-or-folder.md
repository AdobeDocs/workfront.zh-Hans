---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 删除文档或文件夹
description: 删除文档或文件夹
author: John
feature: Workfront API
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: 9de8ee7fad2a3cb67c4fc6bfdff4d6ce50f15afd
workflow-type: tm+mt
source-wordcount: '82'
ht-degree: 6%

---


# 删除文档或文件夹（尚未实施）

删除外部系统中具有给定ID的文档或文件夹。 删除文件夹也会删除文件夹内容。

## URL

PUT/删除

## 查询参数

| 名称  | 描述 |
|---|---|
| documentId  | 要删除的文档ID |
| folderId  |  要删除的文件夹ID |



## 个回应

指示成功或失败的JSON字符串，如下面的错误处理部分中指定。

### 示例

PUThttps://www.example.com/api/deleteid=1234
* 返回 `status: “success”`

* 返回 `status: “failure”, error: “File not found”`
