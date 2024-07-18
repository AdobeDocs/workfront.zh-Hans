---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：解析对象详细信息时出现问题'
description: 此问题视图显示问题的解决对象的名称和完成百分比，即使没有解决任务或项目的访问权限，问题创建者也可以洞察问题的进度。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7f4c923a-01e4-4896-9f54-1f0c66d64bb5
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# 视图：解析对象详细信息时出现问题

此问题视图显示问题的解决对象的名称和完成百分比，即使没有解决任务或项目的访问权限，问题创建者也可以洞察问题的进度。

此视图使用

```
sharecol=true
```

标签组合同一列标题下的多个字段。 欲知关于

```
sharecol
```

标记，请参阅[视图：合并一个共享列](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)中多个列的信息。

![issue_custom_view_with_resolving_object_name_and_percent_complete.png](assets/issue-custom-view-350x77.png)

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

## 查看有关解析对象详细信息的问题

1. 转到问题列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：<pre>column.0.querysort=name</pre><pre>column.0.stretch=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=sourceobject<br>column.1.linkedname=direct<br>column.1.listsort=nested(referenceObject)。HTML(name)<br>column.1.namekey=sourceobject.abbr<br>column.1.1.short=false<br>column.1.stretch=0<br>column.column.column=0<br>column.column.1.column.1.referenceObject.1.referenceObject.1.reference <br>column.1.valueformat=HTML<br>column.1.viewalias=source<br>column.1.width=100<br>column.2.descriptionkey=assignedto<br>column.2.link.linkproperty.0.name=ID<br>column.2.linkproperty.0.valuefield=assignedTo：ID<br>column.2.link.0.valueformat.valueformat=int{int{link.lookup.link.view 18}column.2.link.valuefield=assignedTo：objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=assignedTo<br>column.2.listsort=nested(assignedTo)。string(name)<br>column.2.querysort=assignedTo：name<br>column.2.short=false<br>column.2.stretch=25<br>column.2 uefield=assignedTo：name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.descriptionkey=entrydate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(entryDate)<br>column.3.namekey=entrydate.abbr<br>column.3.querysort=entryDateDateDateFalse=entrateDate{false{false 35}column.3.stretch=0<br>column.3.valuefield=entryDate<br>column.3.valueformat=atDate<br>column.3.width=150<br>column.4.descriptionkey=description<br>column.4.linkedname=direct<br>column.4.listsort=string(description)<br>column.4.query.querysort=description<br>column.4.querysort=description{faly{445 {column.4.stretch=75<br>column.4.valuefield=description<br>column.4.valueformat=HTML<br>column.4.width=150<br>column.5.descriptionkey=status<br>column.5.enumclass=com.attask.common.constants.OpTaskStatusEnum<br>column.5.linkedname=direct<br>column.5.listort=string(status)<br>column(status){status){status.status.status.status.status.status{status.status {column.5.querysort=status<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.type=enum<br>column.5.valuefield=status<br>column.5.valueformat=val<br>column.5.width=150<br>column.6.displayname=Resolving Object Name<br>column.6.link=resolve6Tassalle<br>column.6.namekey.view.relatedcolumn.view.relatedcolumn.namekeyargkey.0=resolveTask<br>column.6.namekeyargkey.1=name<br>column.6.querysort=resolveTask：name<br>column.6.sharecol=true<br>column.6.textmode=true<br>column.6.valuefield=resolveTask：name<br>column.6.valueformat=HTML<br>column.7.displayname=<br>column.7.linkedname=resolveOpOpTaskTaskTaskTask{7Task7TaskTask<br>column.7 mekey=view.relatedcolumn<br>column.7.namekeyargkey.0=resolveOpTask<br>column.7.namekeyargkey.1=name<br>column.7.querysort=resolveOpTask：name<br>column.7.sharecol=true<br>column.7.valuefield=resolveOpTask：name<br>column.7.valueformat=HTML<br>column.82 column.8.linkedname=resolveProject<br>column.8.namekey=view.relatedcolumn<br>column.8.namekeyargkey.0=resolveProject<br>column.8.namekeyargkey.1=name<br>column.8.querysort=resolveProject：name<br>column.8.textmode=true<br>column.8.valuefield=resolveProject<br>column.9HTML9.displayname=解析对象完成百分比<br>列。9.textmode=true<br>列。9.valueexpression=IF(ISBLANK({resolveTask})。<br><br><br><br><br><br><br><br><br><br><br>{ID})，{resolveProject}。{percentComplete}，IF(ISBLANK({resolveProject}.{ID})，{resolveTask}。{percentComplete}，&quot;)<br>column.9.valueformat=doubleAsPercentRounded</pre>

1. 单击&#x200B;**保存视图**。
