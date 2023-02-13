---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：将父任务的名称显示为全部大写
description: 您可以将此列添加到任务视图，以在所有大写字母中显示父任务的名称。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# 查看：将父任务名称显示为全部大写

您可以将此列添加到任务视图，以在所有大写字母中显示父任务的名称。

![](assets/column-task-with-all-caps-parent-350x112.png)

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 将父任务的名称显示为全部大写

要在任务视图中构建此列，请执行以下操作：

1. 转到任务列表。
1. 从 **查看** 下拉菜单，选择 **自定义视图**.\
   或\
   从 **查看** 下拉菜单，选择 **新建视图**.

1. 在&#x200B;**列预览** 区域，单击列的标题以在列表中显示任务名称。
1. 单击&#x200B;**切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码： <pre>descriptionkey=name<br>displayname=任务名称<br>textmode=true<br>valueexpression=IF({numberOfChildren}>&quot;0&quot;,UPPER({name}),{name})<br>valueformat=HTML<br>width=150<br></pre>

1. 单击 **保存视图**.
