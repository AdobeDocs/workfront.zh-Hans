---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：任务视图的同一列中计划小时数的实际小时数
description: 在此任务视图中，每个任务在计划的小时数内显示任务上记录的实际小时数。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 查看：任务视图的同一列中计划小时数的实际小时数

在此任务视图中，每个任务在计划的小时数内显示任务上记录的实际小时数。

![actual_vs_planed_in_task_report_png](assets/actual-vs-planned-in-task-report-350x58.png)

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

## 在任务视图中查看计划小时数的实际小时数

要应用此视图，请执行以下操作：

1. 转到任务列表。
1. 从 **查看** 下拉菜单，选择 **新建视图**.

1. 在&#x200B;**列预览** ，则排除除一列之外的所有列。
1. 单击剩余列的标题，然后单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=assignments<br>column.1.displayname=<br>column.1.linkedname=direct<br>column.1.namekey=assignments<br>column.1.valuefield=assignmentsListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignmentslist<br>column.2.displayname=实际/计划小时数<br>column.2.linkedname=direct<br>column.2.namekey=actualworkrequired<br>column.2.querysort=actualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({actualWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield=actualWorkRequired<br>column.2.valueformat=compound<br>column.2.viewalias=actualworkrequired<br>column.3.aggregator.function=SUM<br>column.3.aggregator.valueexpression=SUB({actualWork}, {workRequired})<br>column.3.aggregator.valueformat=compound<br>column.3.displayname=小时差异<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.valueexpression=SUB({actualWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. 单击 **保存视图**.
