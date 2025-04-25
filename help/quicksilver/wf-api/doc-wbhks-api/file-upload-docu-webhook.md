---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 通过文档Webhook上传文件
description: 通过文档Webhook上传文件
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 3%

---


# 通过文档Webhook上传文件

将文件上传到文档存储提供商的过程分为两步，需要两个单独的API端点。 Adobe Workfront通过调用/uploadInit开始上传过程。 此端点返回一个文档ID，然后在上传文档字节时将其传递到/upload。 根据基础文档存储系统的不同，可能需要创建一个长度为零的文档，然后稍后更新该文档的内容。

添加到此规范版本1.1中的文档ID和文档版本ID可用于从Workfront中检索额外信息。

**示例：**&#x200B;如果文档管理系统需要有关文档的额外信息，webhook实现代码可以使用文档ID使用Workfront的RESTful API检索该信息。 好的做法是，这些信息可能来自文档上的自定义数据字段，并且包含任务、问题或项目。

## POST方法

**URL**

POST /uploadInit

### 查询参数

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
   <td>parentId </td> 
   <td>由webhook提供程序引用的父文件夹ID。</td> 
  </tr> 
  <tr> 
   <td>文件名 </td> 
   <td>文档的名称</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfront文档ID（1.1版中添加）</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Workfront文档版本ID（在版本1.1中添加） </td> 
  </tr> 
 </tbody> 
</table>

## 响应

文件的元数据，由/metadata端点定义。 这包括提供商使用的文档ID。

**示例：**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## PUT方法

将文档的字节上载到webhook提供程序。

**URL**

PUT /upload

## 查询参数

| 名称  | 描述 |
|---|---|
| id  |  刚刚创建的文档ID。 |


**请求正文**

文档的原始内容字节。

**响应**

```
{
result: "success"
}
```

或

```
{
result: "fail"
}
```

**示例**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

响应

```
{
result:"success"
}
```
