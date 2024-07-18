---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：将任务和问题详细信息合并到一个小时列表中'
description: 该小时视图结合了“任务”和“问题名称”列，以及使用sharecol标记的“任务”和“问题已计划小时数”列。 由于小时条目只能属于任务或问题，因此两个对象不能同时出现在同一列中。 视图的每一行都会填充任务或问题中的信息。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cf1137fd-c26a-4907-afe9-2373d3434631
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# 视图：以小时列表显示组合任务和问题详细信息

该小时视图结合了“任务”和“问题名称”列，以及“任务”和“问题已计划小时数”，使用

```
sharecol
```

标记之前。 由于小时条目只能属于任务或问题，因此两个对象不能同时出现在同一列中。 视图的每一行都会填充任务或问题中的信息。

要了解有关

```
sharecol
```

标记，请参阅[视图：合并一个共享列](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)中多个列的信息。\
![custom_view_hours_with_task_and_issue_information.png](assets/custom-view-hours-with-350x48.png)

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

## 在小时列表中查看组合的任务和问题详细信息

要应用此视图，请执行以下操作：

1. 转到小时列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：
   <pre>column.1.querysort=project：name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=project：name<br>column.1.valueformat=HTML<br>column.1.width=100<br>column.2.description=任务或Issue<br>column.2.link.linkproperty.0.name=ID<br>column.link：ID<br>column.link.link.link.0.valueformat.valueformat.0.valueformat=int{int}int column.2.link.lookup=link.view<br>column.2.link.valuefield=task：objCode<br>column.2.linkedname=task<br>column.2.listsort=nested(task)。string(name)<br>column.2.name=Task或Issue<br>column.2.querysort=task：name<br>column.2.sharecol=true<br>column.2.short=false<br>column.stretation =0<br>列。2.valuefield=任务：名称<br>列。2.valueformat=HTML<br>列。2.width=100<br>列。3.descriptionkey=optask<br>列。3.link.linkproperty.0.name=ID<br>列。3.link.linkproperty.0.valuefield=opTask：ID<br>列。3.link.link.0.valueformat=int<br>列。3.link.lookup.link view<br>column.3.link.valuefield=opTask：objCode<br>column.3.link.valueformat=val<br>column.3.linkedname=optask<br>column.3.listsort=nested(opTask)。string(name)<br>column.3.namekey=opTask<br>column.3.querysort=opTask：name<br>column.3.stretation=false.3.3.stretasn.3.valuefield =opTask：name<br>column.3.valueformat=HTML<br>column.3.width=1<br>column.4.valuefield=task：work<br>column.4.sharecol=true<br>column.4.linkedname=task<br>column.4.valueformat=doubleAsInt<br>column.4.namekey=view.relatedcolumn<br>column.4.querysort=task：work<br>column.true<br>column.true.namekeyargkey.0=task<br>column.4.namekeyargkey.1=work<br>column.4.displayname=计划投入<br>column.5.displayname=计划投入<br>column.5.viewalias=opTask：workrequired<br>column.5.valuefield=opTask：workRequired<br>column.5.valueformat=compound<br>column.5.querysort=opTask：op必需<br>column.5.namekeyargkey.0=opTask<br>column.5.namekeyargkey.1=workrequired<br>column.5.namekey=view.relatedcolumn<br>column.5.textmode=true<br>column.6.descriptionkey=hours<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(hours)<br>column.61}column.6.namekey=hours.abbr<br>column.namequerysort=hours =hours<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valuefield=hours<br>column.6.valueformat=doubleAsString<br>column.6.width=75<br>column.7.descriptionkey=entrydate<br>column.7.linkedname=direct<br>column.7.listsort=atAsAsAtAtDate(entDate)<br>column.7.name=entrydate.abbr<br>column.7.querysort=entryDate<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.valuefield=entryDate<br>column.7.valueformat=atDate<br>column.7.width=75<br>column.8.descriptionkey=description<br>column.8.linkedname=direct<br>column.listort=string(description)<br>column.8.name.name.name.abmekey=string br<br>column.8.querysort=description<br>column.8.shortview=false<br>column.8.stretch=0<br>column.8.valuefield=description<br>column.8.valueformat=HTML<br>column.8.width=150<br><br><br><br><br></pre>

1. 单击&#x200B;**保存视图**。
