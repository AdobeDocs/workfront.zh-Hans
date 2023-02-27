---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 获取文档的缩略图
description: 获取文档的缩略图
author: Becky
feature: Workfront API
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 7%

---


# 获取文档的缩略图

返回文档的原始缩略图字节数。

**URL**

GET/缩略图

## 查询参数

| 名称  | 描述 |
|---|---|
| id  | 文档ID。 |
| 大小  |  缩略图的宽度。 |


## 个回应

原始缩略图字节。

**示例：**:https://www.acme.com/api/thumbnail?id=123456
