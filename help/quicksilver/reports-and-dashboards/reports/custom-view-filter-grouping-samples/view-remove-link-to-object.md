---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：删除列中对象的链接'
description: 默认情况下，显示在视图链接中的某些对象将指向对象的“详细信息”页面。 例如，显示项目名称的列是指向项目的链接；显示用户名称的列是指向用户配置文件页面的链接。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# 视图：删除列中对象的链接

默认情况下，显示在视图链接中的某些对象将指向对象的“详细信息”页面。 例如，显示项目名称的列是指向项目的链接；显示用户名称的列是指向用户配置文件页面的链接。

您可以使用在所有视图中显示的列中的文本模式删除此链接。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求修改视图 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 示例：从任务视图的“任务名称”列中移除指向任务的链接：

1. 转到任务列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，单击&#x200B;**新建视图**&#x200B;以创建新视图。

   或

   单击&#x200B;**编辑图标** ![](assets/edit-icon.png)

   要编辑现有视图，请选择该视图。

1. 单击&#x200B;**添加列**&#x200B;以添加新列。

   或

   单击现有列，该列带有指向对象的链接。

1. 单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：
   <pre>displayname=任务名称<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >您可以通过调整以下内容，对其他对象使用类似的代码：
   >
   >* 将代码的&#x200B;**valuefield**&#x200B;行替换为&#x200B;**valueexpression**，并在等号后面保留大括号中包含的相同名称。
   >* 从列的原始文本中删除所有以`link.`开头的行。 例如，消除以下所有行：
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. 单击&#x200B;**保存**，然后单击&#x200B;**保存视图**。
