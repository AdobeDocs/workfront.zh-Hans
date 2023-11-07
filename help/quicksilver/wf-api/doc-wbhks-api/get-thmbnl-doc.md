---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 获取文档的缩略图
description: 获取文档的缩略图
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 11%

---


# 获取文档的缩略图

返回文档的原始缩略图字节。

**URL**

GET/thumbnail

## 查询参数

| 名称  | 描述 |
|---|---|
| id  | 文档ID |
| 大小  |  缩略图的宽度。 |


## 个回应

原始缩略图字节。

**示例：**： https://www.acme.com/api/thumbnail?id=123456
