---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看和分组：显示按分组中的平均值汇总的项目实际持续时间'
description: 您可以在项目报表中添加以下列，以显示作为分组中平均值聚合的实际持续时间。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# 查看和分组：显示按分组中的平均值汇总的项目实际持续时间

您可以在项目报表中添加以下列，以显示作为分组中平均值聚合的实际持续时间。

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## 显示按分组中的平均值汇总的项目实际持续时间

要将此列添加到项目视图，请执行以下操作：

1. （推荐）为获得最佳结果并查看实际持续时间的汇总平均值，您必须将分组添加到项目列表或报表。\
   有关创建分组的更多信息，请参阅Adobe Workfront中的[分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)一文。

1. 转到现有项目视图。
1. 展开“视图”下拉菜单，然后选择&#x200B;**自定义视图**。
1. 单击&#x200B;**添加列**。
1. 单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在此列&#x200B;**区域中的**&#x200B;显示上，然后单击&#x200B;**单击以编辑文本**。

1. 删除“文本模式”框中的所有文本，然后将其替换为以下代码：
   <pre>aggregator.displayformat=compound <br>aggregator.function=AVG <br>aggregator.namekey=view.relatedcolumn <br>aggregator.namekeyargkey=actualduration <br>aggregator.valuefield=actualDurationMinutes <br>aggregator.valueformat=val <br>displayname=项目实际持续时间<br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=actualDuration <br>namication nameactualduration namicationNamouration nameargage=actualduration nameactual实际持续时间{1实际持续时间<br>querysortActual{1Actualquerysort{querysort DurationMinutes <br>textmode=true <br>valuefield=actualDurationMinutes <br>valueformat=compound#M：D <br>viewalias=actualduration</pre>

1. 单击&#x200B;**保存视图**。
