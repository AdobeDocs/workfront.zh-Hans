---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 视图：显示列中两个字段之间的计算结果
description: 您可以在列中使用文本模式来显示两个字段之间的计算。
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# 视图：显示列中两个字段之间的计算结果

<!--Audited: 11/2024-->

您可以在列中使用文本模式来显示两个字段之间的计算。

例如，如果您要了解两个日期之间经过的周天数，则可以使用文本模式语法和数据表达式来计算此差异。\
例如，您可以计算任务的计划完成日期与实际完成日期之间的工作日差异，并在列中显示结果。

您可以在此计算中使用任何其它两个日期（实际起始日期、实际完成日期、预计起始日期、预计完成日期等）。\
有关计算数据表达式的详细信息，请参阅[计算数据表达式的概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>修改过滤器的参与者或请求 </p>
   <p>用于修改报告的标准或计划</p>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 显示列中两个字段之间的计算结果

要将此列添加到任务视图，请执行以下操作：

1. 转到任务列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，单击&#x200B;**新建视图**。

1. 单击&#x200B;**添加列**，然后单击&#x200B;**切换到文本模式** > **编辑文本模式**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：

   ```
   displayname=Week Day Difference
   textmode=true
   valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})
   valueformat=HTML
   ```

1. （可选）要聚合分组中视图中显示的值，请按照[分组中描述的步骤操作：显示聚合分组](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md)中多个计算值的结果。
1. 单击&#x200B;**完成**，然后单击&#x200B;**保存视图**。
