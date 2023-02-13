---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：任务视图中每个分配的计划小时数与实际小时数
description: 此任务视图显示任务的总计划小时数、分配给每个受分派人的计划小时数、总实际小时数以及每个受分派人记录的实际小时数。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f249ff57-50c7-4aa9-a563-cb7f5562b96a
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 查看：任务视图中每个分配的计划小时数与实际小时数

此任务视图显示任务的总计划小时数、分配给每个受分派人的计划小时数、总实际小时数以及每个受分派人记录的实际小时数。

![multi_assignment_budget_vs_actual_for_tasks.png](assets/multi-assignment-budget-vs-actual-for-tasks-350x66.png)

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

## 在任务视图中查看每个分配的计划小时数与实际小时数

1. 转到任务列表。
1. 从 **查看** 下拉菜单，选择 **新建视图**.

1. 在&#x200B;**列预览** ，则排除除一列之外的所有列。
1. 单击剩余列的标题，然后单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：

   ```
   column.0.descriptionkey=name<br>column.0.isInlineEditable=false<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=workrequired<br>column.1.isInlineEditable=false<br>column.1.linkedname=direct<br>column.1.listsort=doubleAsDouble(workRequired)<br>column.1.namekey=workrequired.abbr<br>column.1.querysort=workRequired<br>column.1.section=0<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=workFieldLong<br>column.1.valueformat=compound<br>column.1.viewalias=workrequired<br>column.1.width=100<br>column.2.listdelimiter=<br>column.2.listmethod=nested(assignments).lists<br>column.2.name=Wrk Assignment(s)<br>column.2.stretch=0<br>column.2.type=iterate<br>column.2.valueexpression=CONCAT(right(CONCAT('~~~',{assignmentPercent}),3),'% (', {workRequired}/60 ,' Hours) - ',{assignedTo}.{name})<br>column.2.valueformat=HTML<br>column.2.width=300<br>column.3.descriptionkey=actualworkrequired<br>column.3.isInlineEditable=false<br>column.3.linkedname=direct<br>column.3.listsort=intAsInt(actualWorkRequired)<br>column.3.namekey=actualworkrequired.abbr<br>column.3.querysort=actualWork<br>column.3.section=0<br>column.3.shortview=false<br>column.3.stretch=100<br>column.3.valuefield=actualWorkFieldLong<br>column.3.valueformat=compound<br>column.3.viewalias=actualworkrequired<br>column.3.width=100<br>column.4.listdelimiter=<br>column.4.listmethod=nested(hours).lists<br>column.4.name=Actual Hours<br>column.4.stretch=0<br>column.4.type=iterate<br>column.4.valueexpression=CONCAT('(', {hours} ,' Hours) - ',{owner}.{name})<br>column.4.valueformat=HTML<br>column.4.width=300
   ```

1. 单击 **保存视图**.
