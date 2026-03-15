---
content-type: reference
product-area: reporting;projects
keywords: 计算，聚合，高级，视图
navigation-topic: custom-view-filter-and-grouping-samples
title: 分组：显示分组中多个计算值的聚合结果
description: 您可以在列中使用文本模式来显示报表或列表视图中两个字段之间的计算。 每一行显示报告或列表中每个对象的计算。
author: Courtney
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 3%

---

# 分组：显示分组中多个计算值的聚合结果

<!--Audited: 10/2024-->

您可以使用列中的文本模式来显示报表或列表视图中两个字段之间的计算。 每行显示报表或列表中每个对象的计算。

例如，您可以为任务报表中的每个任务，在名为“工作平衡”的第三列中显示实际小时数与计划小时数之间的差额。 有关计算数据表达式的详细信息，请参阅[计算数据表达式概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

通过将计算添加到包含计算值的列的`aggregator`行，可以在分组中的同一列中显示多个计算视图项的聚合值。 例如，您可以汇总（显示合计）报表分组或“工作平衡”列列表中所有任务的“工作平衡”小时数。 本文介绍如何执行此操作。

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
   <p>修改过滤器的参与者或请求 </p>
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

## 显示分组中聚合多个计算值的结果

1. 转到任务报告，单击&#x200B;**报告操作** > **编辑**。
1. 在&#x200B;**分组**&#x200B;选项卡中，单击&#x200B;**添加分组**，然后在&#x200B;**分组依据**&#x200B;字段中开始输入&#x200B;**项目名称**，然后在其显示在列表时选择&#x200B;**项目>名称**。

1. 在&#x200B;**列（视图）**&#x200B;选项卡中，单击&#x200B;**添加列**，然后在&#x200B;**显示在此列**&#x200B;字段中开始键入&#x200B;**计划小时数**，然后当它显示在列表中时将其选中。

   >[!TIP]
   >
   >在文本模式下编辑信息之前，请始终使用“标准”界面开始添加尽可能多的信息。 添加与您要进行的计算最接近或包含最大信息量的字段。

1. 在“**按**&#x200B;汇总此列”字段中，选择“**和**”。
1. 在您添加的列中单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 将框中的文本替换为以下文本模式示例：

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >要获取分组中的聚合值以显示“计划小时数”和“实际小时数”字段之间的聚合差异，请将相同的等式输入到`aggregator.valuefield`行中。 用于“计划小时数”列的`aggregator.displayformat`会将分钟数转换为小时数。 由于“计划小时数”字段用作占位符，因此不需要调整此行。
   >
   >
   >`minutesAsHoursString`行的`aggregator.displayformat`定义意味着不需要像在`valueexpression`上那样将每个字段除以60以获得结果。 在此`aggregator.valuefield=workRequired`中变为： `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`。
1. 单击&#x200B;**完成**。
1. 单击&#x200B;**保存+关闭**。
