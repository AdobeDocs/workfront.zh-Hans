---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：显示列中两个字段之间的计算结果
description: 可以在列中使用文本模式来显示两个字段之间的计算。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 查看：显示列中两个字段之间的计算结果

可以在列中使用文本模式来显示两个字段之间的计算。

例如，如果要了解两个日期之间经过的周数（以天为单位），可以使用文本模式语法和数据表达式来计算此差异。\
例如，您可以计算任务的计划完成日期与实际完成日期之间的周日差，并在列中显示结果。

您可以在此计算中使用任何其他两个日期（实际开始、实际完成、预计开始、预计完成等）。\
有关计算数据表达式的更多信息，请参阅 [计算数据表达式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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

## 显示列中两个字段之间的计算结果

要将此列添加到任务视图，请执行以下操作：

1. 转到任务列表。
1. 从 **查看** 下拉菜单中，单击 **新建视图**.

1. 单击 **添加列**，则 **切换到文本模式**.

1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：
   <pre>displayname=Week Day Difference<br>textmode=true<br>valueexpression=WEEKDAYDIFF({planedCompletionDate},{actualCompletionDate})<br>valueformat=HTML</pre>

1. （可选）要聚合在分组中视图中显示的值，请按照 [分组：显示在分组中聚合多个计算值的结果](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. 单击 **保存**，则 **保存视图**.
