---
content-type: reference
product-area: reporting;projects
keywords: 计算、聚合、高级、视图
navigation-topic: custom-view-filter-and-grouping-samples
title: '分组：显示分组中多个计算值的聚合结果'
description: 您可以在列中使用文本模式来显示报表或列表视图中两个字段之间的计算。 每一行显示报告或列表中每个对象的计算。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# 分组：显示分组中多个计算值的聚合结果

您可以在列中使用文本模式来显示报表或列表视图中两个字段之间的计算。 每一行显示报告或列表中每个对象的计算。

例如，您可以在任务报告中在名为“工作平衡”的第三列中为每个任务显示实际小时数和计划小时数之间的差异。 有关计算数据表达式的详细信息，请参阅 [计算数据表达式概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

通过将计算添加到，您可以在一个分组的同一列中显示多个计算视图项的聚合值 `aggregator` 包含计算值的列的行。 例如，您可以汇总（显示总计）报告分组或“工作平衡”列列表中所有任务的“工作平衡”小时数。 本文介绍了如何执行此操作。

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
   <td> <p>请求修改分组 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改分组</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 显示分组中多个计算值的聚合结果

1. 转到任务报告，单击 **报表操作** > **编辑**.
1. 在 **分组** 选项卡，单击 **添加分组**，并开始键入 **项目名称** 在 **对您的报告进行分组** > **首先由** 字段，然后当它显示在列表中时将其选中。

1. 在 **列（视图）** 选项卡，单击 **添加列**，然后开始键入 **计划小时数** 在 **显示在此列中** 字段，然后当它显示在列表中时将其选中。

   >[!TIP]
   >
   >在文本模式下编辑信息之前，请始终开始使用标准界面添加尽可能多的信息。 添加最接近或包含您尝试计算的多数信息的字段。

1. 在 **此列的汇总方式** 字段，选择 **总和**，然后单击 **完成**.
1. 单击 **切换到文本模式** 在您添加的列中。
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 替换 `valuefield ` 和 `aggregator.valuefield` 在以下文本模式示例中，行高亮显示：

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
   >要获得分组中的汇总值以显示计划小时数和实际小时数字段之间的汇总差异，请将相同的公式输入到 `aggregator.valuefield` 行。 此 `aggregator.displayformat` 用于计划小时数列，将分钟转换为小时。 由于计划小时数字段用作占位符，因此无需调整此行。
   >
   >
   >此 `minutesAsHoursString` 的定义 `aggregator.displayformat` line表示无需按60除以每个字段，这在 `valueexpression` 了解结果。 在此 `aggregator.valuefield=workRequired` 变为： `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. 单击 **保存+关闭**.
