---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 获取有关该服务的信息
description: 获取有关该服务的信息
author: Becky
feature: Workfront API
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 4%

---


# 获取有关该服务（尚未实施）的信息

>[!NOTE]
>
>此功能的发布日期尚未确定。

返回有关服务的信息，如特性和功能。 Adobe Workfront将使用此信息在Workfront中自定义用户界面。 例如，如果Webhook实施包含一些自定义操作，则JSON应在JSON中列出这些操作。 随后，用户将能够从Workfront中调用这些操作。

**URL**

GET/serviceInfo

## 查询参数

无. 此外，对此端点的调用不应要求进行身份验证。

## 个回应

包含有关此服务的信息的JSON

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名称</th> 
   <th>类型 </th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>字符串 </td> 
   <td>此服务实现的Webhook版本。 这是此规范顶部列出的版本号。</td> 
  </tr> 
  <tr> 
   <td>版本 </td> 
   <td>字符串 </td> 
   <td>此服务的内部版本号。 此号码由Webhook服务提供商确定，仅供参考。<br><br></td> 
  </tr> 
  <tr> 
   <td>发布者 </td> 
   <td>字符串 </td> 
   <td>提供Webhook实施的公司的名称。</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>字符串 </td> 
   <td>包含由此服务实施的API端点的列表。 这可用于确保Workfront中的用户界面反映Webhook提供商提供的功能。 列表中的每个项目都必须包含端点的名称（如“搜索”）。</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>字符串</td> 
   <td>  <p>包含由此Webhook实施的自定义操作的列表。 每个列表项都包括名称和显示名称。 显示名称将显示在Workfront的“文档操作”下拉列表中。 单击下拉列表中的项目，将通过调用/customAction端点在Webhook中调用操作。</p></td> 
  </tr> 
 </tbody> 
</table>

**示例：** `https://www.acme.com/api/serviceInfo`

返回

```
{
webhook version: “1.2”, version: “1.0”, publisher: “Acme, LLC”, availableEndpoints: [“files”, “metadata”, “search”, “download”
“thumbnail”, “uploadInit”, “upload” ], customActions [
{
name: “archive”, displayName: “Archive” 
}, 
{name: “doSomethingElse”, displayName: “Do Something” }, 
] 
}
```
