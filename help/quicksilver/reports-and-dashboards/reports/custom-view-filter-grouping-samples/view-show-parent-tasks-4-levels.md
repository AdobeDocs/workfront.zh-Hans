---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '视图：显示最深4级的父级任务'
description: 此任务视图在第一列中显示任务名称，如果存在，则在同一列表中的单独列中最多显示4个父任务。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 66b45d64-794d-4adc-b208-2ded0dc9c5dc
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 0%

---

# 视图：显示最深4级的父级任务

此任务视图在第一列中显示任务名称，如果存在，则在同一列表中的单独列中最多显示4个父任务。

![parent_tasks_4_levels_deep.png](assets/parent-tasks-4-levels-deep-350x29.png)

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

## 显示最深4级的父级任务

1. 转到任务列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：

   ```
   column.0.descriptionkey=name
   ```

   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.property.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listort=string(name)<br>column.0.name.name.abekey=name.abbr.abbr<br>column.abbr 0.querysort=name<br>column.0.shortview=false<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=parent<br>column.1.link.name=ID<br>column.1.link.property.0.valuefield.link.link.0.valueformat=int<br>.1.link.lookup=link.view<br>column.1.link.valuefield=parent：objCode<br>column.1.linkedname=parent<br>column.1.listsort=nested(parent)。string(name)<br>column.1.namekey=parent<br>column.1.querysort=parent：name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=0{parent.valuefield ：name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=Parent Parent<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=parent:parent:ID<br>column.2.link.link.lookup=link.view<br>column.link.valuefield :parent:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=parent<br>column.2.listsort=nested(parent：parent)。string(name)<br>column.2.name=Parent Parent<br>column.2.querysort=parent:parent:name<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=parent:parent:name<br>name{name{valuevaluevaluevaluefield.2.valuefield.2.valuefield format=HTML<br>column.2.width=150<br>column.3.description=Parent Parent Parent<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=parent:parent:parent：ID<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=parent:parent:obj代码<br>column.3.link.valueformat=val<br>column.3.linkedname=parent<br>column.3.listsort=nested(parent:parent:parent)。string(name)<br>column.3.name=Parent Parent Parent<br>column.3.querysort=parent:parent:parent：name<br>column.3.short view=false<br>column.3.stretch=0<br>column.3.column.3.valuefield=parent:parent:parent{name<br>parent：name{valvalvalue.valuefield.column.3 ueformat=HTML<br>column.3.width=150<br>column.4.description=Parent Parent Parent<br>column.4.link.linkproperty.0.name=ID<br>column.4.linkproperty.0.valuefield=parent:parent:parent:parent:ID<br>column.4.linkproperty.0.valueformat=int<br>column.4.link.lookup.link=link.link.view{77 8}parent:parent:objCode<br>column.4.link.valueformat=val<br>column.4.linkedname=parent<br>column.4.listsort=nested(parent:parent:parent：parent)。string(name)<br>column.4.name=Parent Parent Parent Parent<br>column.4.querysort=parent:parent:name<br>column.4.short=false<br>column.4.stretch=10<br>column.4 valuefield=parent:parent:parent:parent:name<br>column.4.valueformat=HTML<br>column.4.width=150<br><br><br><br><br>:parent::parent:</pre>

1. 单击&#x200B;**保存视图**。

   任务的名称显示在第一列中，如果任务具有任何父级，则最多有4个父级显示在剩余列中。
