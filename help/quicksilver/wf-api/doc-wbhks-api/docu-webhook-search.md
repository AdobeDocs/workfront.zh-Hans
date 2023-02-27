---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 通过文档Web挂接搜索
description: 通过文档Web挂接搜索
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 4%

---

# 通过文档Web挂接搜索

返回从搜索返回的文件和文件夹的元数据。 这可以作为全文搜索或常规数据库查询实现。 当用户从外部文件浏览器执行搜索时，Adobe Workfront会调用/search端点。

## URL

GET/搜索

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
   <td>查询</td> 
   <td>搜索词或短语。</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>（可选）执行搜索的文件夹ID。 注意：这是Workfront中未来功能的占位符。 当前，workfront未传递此参数。 </p> </td> 
  </tr> 
  <tr> 
   <td>最大 </td> 
   <td>要返回的最大项目数。 用于分页。</td> 
  </tr> 
  <tr> 
   <td>偏移</td> 
   <td> 页面偏移，与“max”一起使用。</td> 
  </tr> 
 </tbody> 
</table>

 

## 个回应

JSON包含与查询匹配的文件和文件夹的元数据列表。 构成“匹配”的内容由Webhook提供程序确定。 理想情况下，它应执行全文搜索。 执行基于文件名的搜索也可正常工作。

**示例:**

示例:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
