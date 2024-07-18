---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 通过文档Webhook进行搜索
description: 通过文档Webhook进行搜索
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 3%

---

# 通过文档Webhook进行搜索

返回搜索返回的文件和文件夹的元数据。 这可以作为全文搜索或常规数据库查询来实现。 当用户从外部文件浏览器执行搜索时，Adobe Workfront会调用/search端点。

## URL

GET/search

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
   <td> <p>（可选）从中执行搜索的文件夹ID。 注意：这是Workfront中未来功能的占位符。 目前，Workfront不传递此参数。 </p> </td> 
  </tr> 
  <tr> 
   <td>最大 </td> 
   <td>要返回的最大项目数。 用于分页。</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> 页面偏移，与“max”一起使用。</td> 
  </tr> 
 </tbody> 
</table>

 

## 响应

JSON，其中包含与查询匹配的文件和文件夹的元数据列表。 构成“匹配”的内容由webhook提供程序决定。 理想情况下，应该进行全文搜索。 执行基于文件名的搜索也可正常工作。

**示例：**

示例： `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
