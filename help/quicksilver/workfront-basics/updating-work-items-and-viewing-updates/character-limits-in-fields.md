---
content-type: reference
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 字段中的字符限制
description: Adobe Workfront中的某些字段会限制可包含在该字段中的字符数。 Workfront会对内容编制索引，以便以后可以搜索。 强制实施字符限制以确保Workfront系统的高质量性能。
author: Alina
feature: Get Started with Workfront
exl-id: f09dadf4-24f2-46d9-85ae-6081731d917d
source-git-commit: e2a2a8cfe402c1f9f810ca360db4912d804b0a57
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 5%

---

# 字段中的字符限制

Adobe Workfront中的某些字段会限制可包含在该字段中的字符数。 Workfront会对内容编制索引，以便以后可以搜索。 强制实施字符限制以确保Workfront系统的高质量性能。

当接近限制时，会出现一个计数器。 如果超过限制，则会突出显示多余的字符，并且您无法发布文本。 删除字符，直到您在允许的限制内。

根据您使用的字段，字符限制会有所不同。 以下显示的限制适用于使用拉丁字母（如英语）的语言。 对于包含扩展字符或双字节字符的语言，其限制可能较低。

Workfront或组管理员无法修改字段中的字符限制。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>字段类型</strong> </p> </th> 
   <th> <p><strong>字符数限制(</strong><strong>包括空间)</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>自定义表单中具有格式的文本字段</td> 
   <td>15,000</td> 
  </tr> 
  <tr> 
   <td> <p>状态更新</p> </td> 
   <td> <p>15,000</p>
   <p> 使用API时为4,000</p> </td> 
  </tr> 
  <tr> 
   <td> <p>更新</p> </td> 
   <td> <p>15,000</p> 
   <p> 使用API时为4,000</p></td> 
  </tr> 
  <tr> 
   <td> <p>描述（文档、任务、问题、项目组合、计划和项目）</p> </td> 
   <td> <p>4,000</p> </td> 
  </tr> 
  <tr> 
   <td>自定义表单中的“描述”字段</td> 
   <td>4,000</td> 
  </tr> 
  <tr> 
   <td> <p>自定义数据段落或单行文本 </p> </td> 
   <td> <p>2,000</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Report Builder中的“描述”字段</p> </td> 
   <td> <p>512</p> </td> 
  </tr> 
  <tr> 
   <td> <p>下拉菜单标签</p> </td> 
   <td> <p>255</p> </td> 
  </tr> 
  <tr> 
   <td> <p>对象名称</p> </td> 
   <td> <p>255</p> </td> 
  </tr> 
 </tbody> 
</table>
