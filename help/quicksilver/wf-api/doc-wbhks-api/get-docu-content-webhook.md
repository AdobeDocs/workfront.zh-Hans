---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 通过Webhook获取文档内容
description: 返回文档的原始字节
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
TQID: https://experienceleague.adobe.com/AIN65ofKDJA95iMpvNwoe3oQapmyxzDC16dpf5ehwH0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 43
ht-degree: 16%

---

# 通过Webhook获取文档内容

返回文档的原始字节

## URL

GET /download

## 查询参数

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名称 </th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>ID</p> </td> 
   <td> 文档ID</td> 
  </tr> 
 </tbody> 
</table>

## 响应

文档的原始字节。

**示例**： `https://www.acme.com/api/download?id=123456`
