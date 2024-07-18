---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: “视图：任务视图同一列中计划工时的实际工时”
description: 在此任务视图中，任务中记录的实际小时数显示在每个任务的计划小时数内。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# 视图：任务视图同一列中超过计划工时的实际工时

在此任务视图中，在任务上记录的实际小时数显示为针对每个任务计划的小时数。

![actual_vs_planned_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 许可证*</td> 
   <td> <p>请求修改视图 </p>
   <p>计划修改报表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> <p><b>注释</b>

如果您仍然没有访问权限，请询问您的 Workfront 管理员是否在您的访问级别中设置了其他限制。 有关 Workfront 管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参 阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象 </a>的访问权限 。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的 Workfront 管理员。

## 在任务视图中查看计划工时之外的实际工时

要应用此视图，请执行以下操作：

1. 转到任务列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，然后单击“切换到文本模式&#x200B;**”。**
1. 将鼠标悬停在文本模式区域上，然后单击“ **单击”以编辑文本**。
1. 删除在“ **文本模式** ”框中找到的文本，并将其替换为以下代码：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string（name）<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>列.0.值字段=名称<br>列.0.值格式=HTML<br>列.0.宽度=150<br>列.1.视图别名=任务列<br>.1.显示名称=<br>列.1.链接名称=直接<br>列.1.namekey=assignments<br>列.1.valuefield=assignmentsListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignmentslist<br>column.2.displayname=实际/计划工时<br>列。2.linkedname=直接<br>列.2.namekey=actualworkRequired<br>column.2.querysort=actualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT（{actualWorkRequired}/60，' / '，{workRequired}/60）<br>column.2.valuefield=actualWorkRequired<br>column.2.valueformat=compound<br>column.2.viewalias=actualworkRequired<br>column.3.aggregator.function=SUM<br>column.3.aggregator.valueexpression=SUB（{actualWork}， {workRequired}）<br>column.3.aggregator.valueformat=compound<br>column.3.displayname=Hours Obance<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.valueexpression=SUB（{actualWork}， {workRequired}）/60<br>column.3.valueformat=customNumberAsString</pre>

1. 单击“ **保存视图**”。
