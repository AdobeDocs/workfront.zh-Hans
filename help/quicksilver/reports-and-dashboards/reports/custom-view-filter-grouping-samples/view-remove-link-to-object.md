---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：删除列中对象的链接'
description: 默认情况下，显示在视图链接中的某些对象会链接到该对象的“详细信息”(Details)页面。 例如，显示项目名称的列即是指向项目的链接；显示用户名称的列是指向用户配置文件页面的链接。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# 查看：删除列中对象的链接

默认情况下，显示在视图链接中的某些对象会链接到该对象的“详细信息”(Details)页面。 例如，显示项目名称的列即是指向项目的链接；显示用户名称的列是指向用户配置文件页面的链接。

您可以在所有视图中显示的列中使用文本模式删除此链接。

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

## 示例：从任务视图的“任务名称”列中删除指向任务的链接：

1. 转到任务列表。
1. 从 **查看** 下拉菜单中，单击 **新建视图** 创建新视图。

   或

   单击 **“编辑”图标** ![](assets/edit-icon.png)

   要编辑现有视图，请选择该视图。

1. 单击 **添加列** 添加新列。

   或

   单击包含对象链接的现有列。

1. 单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：

   <pre>displayname=任务名称<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >通过调整以下内容，您可以对其他对象使用类似的代码：
   >
   >   
   >   
   >   * 替换 **valuefield** 代码行 **valueexpression** 并在等号后保留花括号中包含的相同名称。
   >   
   >   
   >
   >   
   >   
   >   * 消除所有以>开头的行

      >   
      >     ```>   
      >     link.
      >     ```   >   
      >   
      >     
      from the original text of the column. For example, eliminate all the following lines:
      >     <pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre>
      >   
      >   
      >



1. 单击 **保存**，则 **保存视图**.
