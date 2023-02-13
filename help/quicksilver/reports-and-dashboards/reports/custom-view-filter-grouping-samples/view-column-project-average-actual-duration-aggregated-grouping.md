---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看和分组：显示项目实际持续时间按分组中的平均值汇总
description: 您可以在项目报表中添加以下列，以将累计的实际持续时间显示为分组中的平均值。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# 查看和分组：显示项目实际持续时间按分组中的平均值汇总

您可以在项目报表中添加以下列，以将累计的实际持续时间显示为分组中的平均值。

![project_with_aggregate_actual_duration_in_grouping_view_png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## 显示项目实际持续时间按分组中的平均值汇总

要将此列添加到项目视图，请执行以下操作：

1. （推荐）要获得最佳结果并查看实际持续时间的累计平均值，您必须在项目列表或报表中添加一个分组。\
   有关创建分组的更多信息，请参阅文章 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 转到现有项目视图。
1. 展开“视图”下拉菜单，然后选择 **自定义视图**.
1. 单击 **添加列**.
1. 单击 **切换到文本模式**.
1. 将鼠标悬停在 **在此列中显示** ，然后单击 **单击以编辑文本**.

1. 删除“文本模式”框中的所有文本，并将其替换为以下代码：

   <pre>congregator.displayformat=compound <br>aggregator.function=AVG <br>regator.namekey=view.relatedcolumn <br>aggreator.namekeyargkey=actualduration <br>aggregator.valuefield=actualDurationMinutes <br>congregator.valueformat=val <br>displayname=项目实际持续时间 <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=actualduration <br>namekeyargkey=actuluration <br>querysort=actualDurationMinutes <br>textmode=true <br>valuefield=actualDurationMinutes <br>valueformat=compound#M:D <br>viewalias=actualduration</pre>

1. 单击 **保存视图**.
