---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 列出文件或文件夹的元数据
description: 列出文件或文件夹的元数据
author: Becky
feature: Workfront API
role: Developer
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
TQID: https://experienceleague.adobe.com/nZv42xMbDRJbkwR-lFKI6dAbeszSzGWAwn--qkKhVVM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 101
ht-degree: 6%

---

# 获取文件夹内容的项目列表

列出给定文件夹的文件和文件夹的元数据。

**URL**

获取/files

## 查询参数

| 名称  | 描述 |
|---|---|
| parentId  | 文件夹ID。 要获取根目录的元数据，请使用值“/”。 |
| max  | 要返回的最大项目数。 用于分页。 |
| offset  |  页面偏移，与“max”一起使用。 |


## 响应

包含文件和文件夹列表的JSON。 每个项的元数据与/metadata端点返回的元数据相同。

**示例：** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ",
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ",
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
