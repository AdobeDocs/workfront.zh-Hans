---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 删除文档或文件夹
description: 删除文档或文件夹
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '82'
ht-degree: 8%

---


# 删除文档或文件夹（尚未实施）

删除外部系统中具有给定ID的文档或文件夹。 删除文件夹也会删除文件夹内容。

## URL

PUT/delete

## 查询参数

| 名称  | 描述 |
|---|---|
| documentId  | 要删除的文档ID |
| folderId  |  要删除的文件夹ID |



## 个回应

指示成功或失败的JSON字符串，如下面的错误处理部分中所述。

### 示例

PUThttps://www.example.com/api/delete­­­­­­­­­­­­­­­­­­­­­­­­­­­­­id=1234
* 返回 `status: "success"`

* 返回 `status: "failure", error: "File not found"`
