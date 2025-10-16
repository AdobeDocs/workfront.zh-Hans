---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 视图：通过缩进任务显示任务中的父子关系
description: 您可以维护导出任务列表中的父子关系的区别，方法是：向任务列表添加自定义视图，并确保在导出列表之前选择此视图。
author: Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---

# 视图：通过缩进任务显示任务中的父子关系

<!--Audited: 11/2024-->

您可以维护导出任务列表中的父子关系的区别，方法是：向任务列表添加自定义视图，并确保在导出列表之前选择此视图。

![父子缩进](assets/parent-child-indented-custom-view-350x94.png)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>修改视图的参与者或请求 </p>
   <p>用于修改报告的标准或计划</p>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


+++

## 通过缩进任务显示任务中的父子关系

1. 转到包含要导出的任务列表的项目。
1. 单击&#x200B;**视图**&#x200B;下拉菜单，然后选择&#x200B;**新建视图**。
1. 在&#x200B;**任务名称**&#x200B;列标题中单击。
1. 选择右上角的&#x200B;**切换到文本模式**。
1. 单击&#x200B;**编辑文本模式**&#x200B;并删除所有现有文本。
1. 粘贴以下文本：


   ```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
   ```

1. 单击&#x200B;**完成** > **保存视图**。
