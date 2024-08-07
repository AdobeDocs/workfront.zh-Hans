---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '视图：任务视图中工期和计划工作的基线差异'
description: 查看持续时间和计划工作的基线差异。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2a1eef9c-016c-4a04-acda-6070fcb0e23d
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# 视图：任务视图中工期和计划工时的基线差异

此视图在任务视图中显示以下内容：

* 包含基线任务信息的任务信息。
* 持续时间与默认基线持续时间之间的差异。
* 计划工作量和默认基线计划工作量之间的差异。

>[!NOTE]
>
> 以下视图中显示的数据将实际任务值与与“默认基线”任务关联的值进行比较。

 

![baseline_variance_in_a_task_view.png](assets/baseline-variance-in-a-task-view-350x38.png)

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

## 在任务视图中查看工期和计划工作的基线差异

1. 转到任务列表。
1. 在&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 移除视图中的所有列（第一个列除外）。
1. 选择第一列后，单击&#x200B;**切换到文本模式**。
1. 复制下面的文本并将其粘贴到视图的第一列：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listort=string(name)<br>column(name){name){name.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.0.displayname=任务名称<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=compound<br>column.1.viewalias=duration<br>column.1000<br>column.1.displayname=TashDuration{2 8}column.2.descriptionkey=view.relatedcolumn<br>column.2.descriptionkeyargkey.0=defaultbaselinetask<br>column.2.descriptionkeyargkey.1=duration<br>column.2.linkedname=defaultBaselinetask<br>column.2.listsort=intAsInt(durationMinutes)<br>column.2.namekey.0=duration{defaultask.0=defaultask{35 {column.2.namekeyargkey.1=duration.abbr<br>column.2.querysort=defaultBaselineTask：durationMinutes<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=defaultBaselineTask：durationFieldLong<br>column.2.valueformat=compound<br>column.2 playname=Dflt基线任务： Dur<br>列。2.durationunitfield=durationUnit.value<br>列。3.description=Duration Variance"列。3.linkedname=direct<br>列。3.listsort=intAsInt(durationMinutes)<br>列。3.name=Duration Variance<br>列。3.querysort=durationMinutes<br>列。3.short=false<br>列。3.stretage=0<br>列。3.valuevaluevalue expression=CONCAT(SUB({duration}，{defaultBaselineTask})<br><br><br><br><br>{duration})/480，" Days")<br>column.3.valueformat=HTML<br>column.3.viewalias=duration<br>column.3.width=100<br>column.3.displayname=Duration Variance<br>column.4.descriptionkey=workrequired<br>column.4.linkedname=direct<br>column.4.listsort=doubleAsDouble(workRequired)<br>column.4.namequirequired.abbr<br>column.4.querysort.abbr{work.quirequirequired.abbr.querysort=work{work1Requirequirequirequirequirequirequired{111 0}column.4.shortview=false<br>column.4.stretch=0<br>column.4.valuefield=workFieldLong<br>column.4.valueformat=compound<br>column.4.viewalias=workrequired<br>column.4.width=100<br>column.4.displayname=Wrk Req<br>column.5.descriptionkey=view.relatedcolumn<br>column.5.descriptionkeykeyarkey.0=defaultbaselinetask{1 9}column.5.descriptionkeyargkey.1=workrequired<br>column.5.linkedname=defaultBaselineTask<br>column.5.listsort=doubleAsDouble(workRequired)<br>column.5.namekeyargkey.0=defaultbaselinetask.abbr<br>column.5.namekeyargkey.1=workrequirequired.abbr<br>column.querysortBaselineTaskTaskTaskWork：work必需<br>列。5.shortview=false<br>列。5.stretch=0<br>列。5.valuefield=defaultBaselineTask：workFieldLong<br>列。5.valueformat=compound<br>列。5.viewalias=defaultBaselineTask：workrequired<br>列。5.width=100<br>列。5.displayname=Dflt基准任务：工作请求<br>列。6.descriptionkey关键字{workreq3} 4}column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(workRequired)<br>column.6.name=Effort Variance<br>column.6.querysort=workRequired<br>column.6.shortview=false<br>column.6.valueexpression=CONCAT(SUB({workRequired}，{defaultBaselineTask}。<br><br><br><br><br>{workRequired})/60，"小时")<br>column.6.valueformat=HTML<br>column.6.viewalias=workrequired<br>column.6.width=100<br>column.6.displayname=Effort Variance</pre>

1. 单击&#x200B;**保存视图**。