---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '视图：显示列中两个字段之间的计算结果'
description: 您可以在列中使用文本模式来显示两个字段之间的计算。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# 视图：显示列中两个字段之间的计算结果

您可以在列中使用文本模式来显示两个字段之间的计算。

例如，如果您要了解两个日期之间经过的周天数，则可以使用文本模式语法和数据表达式来计算此差异。\
例如，您可以计算任务的计划完成日期与实际完成日期之间的工作日差异，并在列中显示结果。

您可以在此计算中使用任何其它两个日期（实际起始日期、实际完成日期、预计起始日期、预计完成日期等）。\
有关计算数据表达式的详细信息，请参阅 [计算数据表达式概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 显示列中两个字段之间的计算结果

要将此列添加到任务视图，请执行以下操作：

1. 转到任务列表。
1. 从 **视图** 下拉菜单，单击 **新建视图**.

1. 单击 **添加列**，则 **切换到文本模式**.

1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在中找到的文本 **文本模式** 框中，然后使用以下代码替换它：
   <pre>displayname=周间差异<br>textmode=true<br>valueexpression=WEEKDAYDIFF({plannedCompletionDate}，{actualCompletionDate})<br>valueformat=HTML</pre>

1. （可选）要聚合分组中视图中显示的值，请按照中所述的步骤操作 [分组：显示分组中多个计算值的聚合结果](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. 单击 **保存**，则 **保存视图**.
