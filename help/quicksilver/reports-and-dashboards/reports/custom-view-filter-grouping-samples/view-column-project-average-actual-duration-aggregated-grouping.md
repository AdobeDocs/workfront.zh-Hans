---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 查看和分组：显示按分组中的平均值合计的项目实际持续时间
description: 您可以在项目报告中添加以下列，以显示作为平均数在分组中聚合的实际持续时间。
author: Courtney
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 6%

---

# 查看和分组：显示按分组中的平均值合计的项目“实际持续时间”

<!--Audited: 11/2024-->

您可以在项目视图中添加以下列，以显示作为平均数在分组中聚合的实际持续时间。

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>投稿人或请求修改筛选器 </p>
   <p>标准或计划修改报告</p>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑报表、仪表板、日历的访问权限以修改报表</p> <p>编辑筛选器、视图、组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中的信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 显示按分组中的平均值汇总的项目“实际持续时间”

要将此列添加到项目视图，请执行以下操作：

1. 转到项目列表。
1. （必需）要查看项目实际持续时间的合计平均值，必须将分组添加到项目列表中。\
   有关创建分组的详细信息，请参阅[Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)一文。
1. 展开&#x200B;**视图**&#x200B;下拉菜单，然后选择&#x200B;**自定义视图**。
1. 单击&#x200B;**添加列**。
1. 单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 删除&#x200B;**编辑文本模式**&#x200B;框中的所有文本，并将其替换为以下代码：

   ```
   aggregator.displayformat=compound 
   aggregator.function=AVG 
   aggregator.namekey=view.relatedcolumn 
   aggregator.namekeyargkey=actualduration 
   aggregator.valuefield=actualDurationMinutes 
   aggregator.valueformat=val 
   displayname=Project Actual Duration 
   durationunitfield=durationUnit.value 
   linkedname=project 
   namekey=actualduration 
   namekeyargkey=actualduration 
   querysort=actualDurationMinutes 
   textmode=true 
   valuefield=actualDurationMinutes 
   valueformat=compound#M:D 
   viewalias=actualduration
   ```

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存视图**。
1. （可选）更新视图名称，然后单击&#x200B;**保存视图**。
