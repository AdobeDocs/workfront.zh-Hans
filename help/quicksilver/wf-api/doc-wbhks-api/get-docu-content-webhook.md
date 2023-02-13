---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 通过Webhooks获取文档内容
description: 返回文档的原始字节
author: John
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '53'
ht-degree: 7%

---

# 通过Webhooks获取文档内容

返回文档的原始字节

## URL

GET/下载

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
   <td> <p>id</p> </td> 
   <td> 文档ID。</td> 
  </tr> 
 </tbody> 
</table>

## 个回应

文档的原始字节。

**示例：**:  [https://www.acme.com/api/download?id=123456](https://www.acme.com/api/download?id=123456)
