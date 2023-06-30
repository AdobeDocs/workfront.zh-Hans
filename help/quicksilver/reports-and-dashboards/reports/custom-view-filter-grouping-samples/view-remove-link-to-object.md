---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：删除指向列中对象的链接'
description: 默认情况下，显示在视图链接中的某些对象将指向该对象的“详细信息”页面。 例如，显示项目名称的列是指向项目的链接；显示用户名称的列是指向用户配置文件页面的链接。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# 视图：删除列中对象的链接

默认情况下，显示在视图链接中的某些对象将指向该对象的“详细信息”页面。 例如，显示项目名称的列是指向项目的链接；显示用户名称的列是指向用户配置文件页面的链接。

您可以使用文本模式删除在所有视图中显示的列中的此链接。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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
   <td> <p>请求修改视图 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 示例：从任务视图的“任务名称”列中移除指向任务的链接：

1. 转到任务列表。
1. 从 **视图** 下拉菜单，单击 **新建视图** 以创建新视图。

   或

   单击 **“编辑”图标** ![](assets/edit-icon.png)

   要编辑现有视图，请选择该视图。

1. 单击 **添加列** 以添加新列。

   或

   单击现有列，该列带有指向对象的链接。

1. 单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在中找到的文本 **文本模式** 框中，将其替换为以下代码：
   <pre>displayname=任务名称<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >您可以通过调整以下内容，将类似的代码用于其他对象：
   >
   >* 更换 **valuefield** 代码行 **值表达式** 和将相同的名称包含在等号后的大括号中。
   >* 删除所有开头为 `link.` 从列的原始文本中。 例如，删除以下所有行：
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. 单击 **保存**，则 **保存视图**.
