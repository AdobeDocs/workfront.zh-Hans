---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 获取文件或文件夹的元数据
description: 获取文件或文件夹的元数据
author: Becky
feature: Workfront API
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 6%

---


# 获取文件或文件夹的元数据

返回指定文件或文件夹的元数据。

**URL**

GET/metadata?id=[文档或文件夹ID]

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
   <td>id</td> 
   <td>文件或文件夹的ID，由Webhook提供程序引用。 这与Adobe Workfront的文档ID不同。 要获取根目录的元数据，请使用值“/”。
   <p>注意：此ID的最大长度为255个字符。</p></td> 
  </tr> 
 </tbody> 
</table>

 

## 个回应

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名称 </th> 
   <th>类型 </th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>字符串 </td> 
   <td>文档或文件夹的名称</td> 
  </tr> 
  <tr> 
   <td>一种 </td> 
   <td>字符串 </td> 
   <td>指定此项目是否为文件或文件夹（“file”或“folder”）</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>字符串 </td> 
   <td>文件或文件夹的ID。</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>字符串 </td> 
   <td> <p>用户在浏览器窗口中查看文档时使用的URL路径。 该URL可由文档提供程序或本机外部存储提供程序托管。</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>字符串 </td> 
   <td> <p>用户在浏览器窗口中下载文档时使用的URL路径。 该URL可由文档提供程序或本机外部存储提供程序托管。</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>字符串 </td> 
   <td>文件的MIME类型。 (可选)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>字符串 </td> 
   <td>上次修改此文件时（格式化的RFC 3339时间戳）</td> 
  </tr> 
  <tr> 
   <td>大小</td> 
   <td>长</td> 
   <td> 文件的大小（以字节为单位）。 (可选)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>布尔值</td> 
   <td> 指示此文件或文件夹是否对经过身份验证的用户是只读的。(可选) </td> 
  </tr> 
 </tbody> 
</table>

**示例：** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title:"My Document",<br>kind:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"20140605T17:39:45.251Z”，<br>大小："32554694"<br>}</pre>

>[!NOTE]
>
>错误处理应在所有API调用中保持一致。 有关详细信息，请参阅下面的“错误处理”部分。
