---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 执行自定义操作
description: 执行自定义操作
author: Becky
feature: Workfront API
role: Developer
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 2%

---


# 执行自定义操作（尚未实施）

此端点允许Adobe Workfront用户（或自动工作流事件）在外部系统中执行操作。 /customAction端点接受“name”参数，该参数允许webhook提供程序实现多个自定义操作。

webhook提供程序通过在customActions下的/serviceInfo响应中包含操作来向Workfront注册自定义操作。 在设置>文档>自定义集成下设置或刷新webhook提供程序时，Workfront会加载此列表。

用户可以通过选择“文档操作”下的部分来触发自定义操作

**URL**

GET/customAction

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
   <td> <p>name</p> </td> 
   <td> <p>指定要执行的操作类型的标识符。 此值对应于/serviceInfo终结点返回的customAction值之一。</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>正在对其执行操作的Workfront文档ID。</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> 正在对其执行操作的Workfront文档版本ID。</td> 
  </tr> 
 </tbody> 
</table>

 

## 响应

指示成功或失败的JSON字符串，如下面的错误处理部分中所述。 出现故障时（即状态=“故障”），Workfront将向用户显示提供的错误消息。

**示例：**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

响应

```
{
status: "success"
}
```
