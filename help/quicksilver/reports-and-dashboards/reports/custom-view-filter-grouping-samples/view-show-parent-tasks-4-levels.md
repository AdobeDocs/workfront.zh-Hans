---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：显示最多4级深度的父任务
description: 此任务视图在第一列中显示任务名称，并在同一列表中的单独列中显示（如果存在）最多4个父任务。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 66b45d64-794d-4adc-b208-2ded0dc9c5dc
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---

# 查看：显示最多4层的父任务

此任务视图在第一列中显示任务名称，并在同一列表中的单独列中显示（如果存在）最多4个父任务。

![parent_tasks_4_levels_deep.png](assets/parent-tasks-4-levels-deep-350x29.png)

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

## 显示最多4个级别的父任务深度

1. 转到任务列表。
1. 从 **查看** 下拉菜单，选择 **新建视图**.

1. 在&#x200B;**列预览** ，则排除除一列之外的所有列。
1. 单击剩余列的标题，然后单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：

   ```
   column.0.descriptionkey=name
   ```

   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=parent<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=parent:ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=parent:objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=parent<br>column.1.listsort=nested(parent)。string(name)<br>column.1.namekey=parent<br>column.1.querysort=parent:name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=parent.name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=父项<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=parent:parent:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=parent:parent:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=parent<br>column.2.listsort=nested(parent:parent)。string(name)<br>column.2.name=父项<br>column.2.querysort=parent:parent:name<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=parent:parent:name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.description=父父项<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=parent:parent:parent:ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=parent:parent:parent:objCode<br>column.3.link.valueformat=val<br>column.3.linkedname=parent<br>column.3.listsort=nested(parent):parent:parent)。string(name)<br>column.3.name=父级父级<br>column.3.querysort=parent:parent:父项：name<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=parent:parent:父项：name<br>column.3.valueformat=HTML<br>column.3.width=150<br>column.4.description=父父项父项<br>column.4.link.linkproperty.0.name=ID<br>column.4.link.linkproperty.0.valuefield=parent:parent:父项:parent:ID<br>column.4.link.linkproperty.0.valueformat=int<br>column.4.link.lookup=link.view<br>column.4.link.valuefield=parent:parent:父项:parent:objCode<br>column.4.link.valueformat=val<br>column.4.linkedname=parent<br>column.4.listsort=nested(parent):parent:parent:parent)。string(name)<br>column.4.name=父父级父级<br>column.4.querysort=parent:parent:父项:parent:name<br>column.4.shortview=false<br>column.4.stretch=100<br>column.4.valuefield=parent:parent:父项:parent:name<br>column.4.valueformat=HTML<br>column.4.width=150</pre>

1. 单击 **保存视图**.

   任务的名称显示在第一列中，如果任务有任何父项，则最多有4个父项显示在其余的列中。
