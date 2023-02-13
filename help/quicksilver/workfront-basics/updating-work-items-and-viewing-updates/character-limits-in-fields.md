---
content-type: reference
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 字段中的字符限制
description: Adobe Workfront中的某些字段限制可包含在该字段中的字符数。 Workfront对内容进行索引，以便以后能够进行搜索。 为了确保Workfront系统的高质量性能，强制实施字符限制。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f09dadf4-24f2-46d9-85ae-6081731d917d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 5%

---

# 字段中的字符限制

Adobe Workfront中的某些字段限制可包含在该字段中的字符数。 Workfront对内容进行索引，以便以后能够进行搜索。 为了确保Workfront系统的高质量性能，强制实施字符限制。

当接近该限制时，将显示一个计数器。 超出限制时，会突出显示超出限制的字符，并且无法发布文本。 删除字符，直到您在允许的限制内。

字符限制因所使用的字段而异。 下面显示的限制适用于使用拉丁字母的语言（如英语）。 对于包含扩展字符或双字节字符的语言，此限制可能会较低。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>字段类型</strong> </p> </th> 
   <th> <p><strong>字符限制(</strong><strong>包括空格)</strong> </p> </th> 
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
   <td> <p>描述（文档、任务、问题、项目组合、项目和项目）</p> </td> 
   <td> <p>4,000</p> </td> 
  </tr> 
  <tr> 
   <td>自定义表单中的描述字段</td> 
   <td>4,000</td> 
  </tr> 
  <tr> 
   <td> <p>自定义数据段落或单行文本 </p> </td> 
   <td> <p>2,000</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Report Builder中的描述字段</p> </td> 
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
