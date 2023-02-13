---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 通过文档Webhooks上传文件
description: 通过文档Webhooks上传文件
author: John
feature: Workfront API
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: b117eb11e4e9325e6249687448d3de98a11e5e00
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 3%

---


# 通过文档Webhooks上传文件

将文件上传到文档存储提供程序是一个两步流程，需要两个单独的API端点。 Adobe Workfront通过调用/uploadInit开始上传过程。 此端点会返回一个文档ID，在上传文档字节时，该ID会被传递到/upload。 根据基础文档存储系统，可能需要创建一个零长度文档，然后稍后更新文档的内容。

添加到此规范的1.1版中，文档ID和文档版本ID可用于从Workfront中检索其他信息。

**示例：** 如果文档管理系统需要有关文档的额外信息，则Webhook实施代码可以使用文档ID来使用Workfront的RESTful API检索该信息。 作为一种好的做法，此信息可能来自文档上的自定义数据字段，其中包含任务、问题或项目。

## POST方法

**URL**

POST/uploadInit

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
   <td>Webhook提供程序引用的父文件夹ID。</td> 
  </tr> 
  <tr> 
   <td>文件名 </td> 
   <td>文档的名称</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfront文档ID（在版本1.1中添加）</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Workfront文档版本ID（在版本1.1中添加） </td> 
  </tr> 
 </tbody> 
</table>

## 个回应

文件的元数据，由/metadata端点定义。 这包括提供商使用的文档ID。

**示例:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## PUT方法

将文档的字节上载到Webhook提供程序。

**URL**

PUT/上载

## 查询参数

| 名称  | 描述 |
|---|---|
| id  |  刚刚创建的文档ID。 |


**请求正文**

文档的原始内容字节。

**响应**

```
{
result: “success”
}
```

或

```
{
result: “fail”
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
