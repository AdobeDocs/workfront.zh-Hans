---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：任务视图中持续时间和计划工作的基准差异
description: 此视图在任务视图 — 编辑我中显示以下内容。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2a1eef9c-016c-4a04-acda-6070fcb0e23d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---

# 查看：任务视图中持续时间和计划工作的基准差异

此视图在任务视图中显示以下内容：

* 包含基线任务信息的任务信息。
* “持续时间”和“默认基线持续时间”之间的差异。
* 计划工作与默认基准计划工作之间的差异。

>[!NOTE]
>
> 以下视图中显示的数据会将实际任务值与与默认基线任务关联的值进行比较。

 

![baseline_variance_in_a_task_view.png](assets/baseline-variance-in-a-task-view-350x38.png)

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

## 在任务视图中查看持续时间和计划工作的基线差异

1. 转到任务列表。
1. 在 **查看** 下拉菜单，选择 **新建视图**.

1. 删除视图中的所有列（第一个列除外）。
1. 选择第一列后，单击 **切换到文本模式**.
1. 复制下面的文本，并将其粘贴到视图的第一列：

   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.0.displayname=任务名称<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=compound<br>column.1.viewalias=duration<br>column.1.width=100<br>column.1.displayname=任务持续时间<br>column.2.descriptionkey=view.relatedcolumn<br>column.2.descriptionkeyargkey.0=defaultbaselinetask<br>column.2.descriptionkeyargkey.1=duration<br>column.2.linkedname=defaultBaselineTask<br>column.2.listsort=intAsInt(durationMinutes)<br>column.2.namekey=duration<br>column.2.namekeyargkey.0=defaultbaselinetask.abbr<br>column.2.namekeyargkey.1=duration.abbr<br>column.2.querysort=defaultBaselineTask:durationMinutes<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=defaultBaselineTask:durationFieldLong<br>column.2.valueformat=compound<br>column.2.viewalias=defaultBaselineTask:duration<br>column.2.width=100<br>column.2.displayname=Dflt基线任务：杜尔<br>column.2.durationunitfield=durationUnit.value<br>column.3.description=Duration Variance"column.3.linkedname=direct<br>column.3.listsort=intAsInt(durationMinutes)<br>column.3.name=持续时间差异<br>column.3.querysort=durationMinutes<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valueexpression=CONCAT(SUB({duration},{defaultBaselineTask})。{duration})/480，“天”)<br>column.3.valueformat=HTML<br>column.3.viewalias=duration<br>column.3.width=100<br>column.3.displayname=持续时间差异<br>column.4.descriptionkey=workrequired<br>column.4.linkedname=direct<br>column.4.listsort=doubleAsDouble(workRequired)<br>column.4.namekey=workrequired.abbr<br>column.4.querysort=workRequired<br>column.4.shortview=false<br>column.4.strect=0<br>column.4.valuefield=workFieldLong<br>column.4.valueformat=compound<br>column.4.viewalias=workrequired<br>column.4.width=100<br>column.4.displayname=Work Req<br>column.5.descriptionkey=view.relatedcolumn<br>column.5.descriptionkeyargkey.0=defaultbaselinetask<br>column.5.descriptionkeyargkey.1=workrequired<br>column.5.linkedname=defaultBaselineTask<br>column.5.listsort=doubleAsDouble(workRequired)<br>column.5.namekey=view.relatedcolumn<br>column.5.namekeyargkey.0=defaultbaselinetask.abbr<br>column.5.namekeyargkey.1=workrequired.abbr<br>column.5.querysort=defaultBaselineTask:workRequired<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valuefield=defaultBaselineTask:workFieldLong<br>column.5.valueformat=compound<br>column.5.viewalias=defaultBaselineTask:workrequired<br>column.5.width=100<br>column.5.displayname=Dflt基线任务：工作请求<br>column.6.descriptionkey=workrequired<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(workRequired)<br>column.6.name=工作方差<br>column.6.querysort=workRequired<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valueexpression=CONCAT(SUB({workRequired},{defaultBaselineTask})。{workRequired})/60，“小时”)<br>column.6.valueformat=HTML<br>column.6.viewalias=workrequired<br>column.6.width=100<br>column.6.displayname=Effort Variance</pre>

1. 单击 **保存视图**.\
   ![](assets/view--baseline-variance-for-duration-and-planned-work-350x78.png)
