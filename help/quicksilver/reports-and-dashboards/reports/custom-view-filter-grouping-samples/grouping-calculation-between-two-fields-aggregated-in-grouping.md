---
content-type: reference
product-area: reporting;projects
keywords: 计算，聚合，高级，视图
navigation-topic: custom-view-filter-and-grouping-samples
title: “分组：显示在分组中聚合多个计算值的结果
description: 您可以在列中使用文本模式来在报表或列表视图的两个字段之间显示计算。 每一行显示报表或列表中每个对象的计算。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 分组：显示在分组中聚合多个计算值的结果

您可以在列中使用文本模式来在报表或列表视图的两个字段之间显示计算。 每一行显示报表或列表中每个对象的计算。

例如，您可以在名为“工作余额”的第三列中显示任务报表中每项任务的实际小时数与计划小时数之间的差异。 有关计算数据表达式的更多信息，请参阅 [计算数据表达式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

您可以通过向 `aggregator` 包含计算值的列的行。 例如，您可以汇总（显示总和）报表分组或工作平衡列列表中所有任务的工作平衡小时数。 本文介绍了如何执行此操作。

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

## 显示在分组中聚合多个计算值的结果

1. 转到任务报告，单击 **报表操作** > **编辑**.
1. 在 **分组** ，单击 **添加分组**，然后开始键入 **项目名称** 在 **对报表进行分组** > **首先由** 字段，然后在其列表中显示时将其选中。

1. 在 **列（视图）** ，单击 **添加列**，然后开始键入 **计划小时数** 在 **在此列中显示** 字段，然后在其列表中显示时将其选中。

   >[!TIP]
   >
   >在文本模式下编辑信息之前，请始终先使用标准界面添加尽可能多的信息。 添加最接近或包含最多信息的字段，以便进行您尝试的计算。

1. 在 **按以下方式汇总此列** 字段，选择 **总和**，然后单击 **完成**.
1. 单击 **切换到文本模式** 在添加的列中。
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 替换 `valuefield ` 和 `aggregator.valuefield` 在以下文本模式中突出显示线条的线条示例：

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
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") viewalias=workrequired displayname=Work Balance
   ```

   >[!TIP]
   >
   >为了在分组中获取汇总值以显示“计划小时数”和“实际小时数”字段之间的汇总差异，请在 `aggregator.valuefield` 行。 的 `aggregator.displayformat` 用于“计划小时数”列将分钟数转换为小时数。 由于“计划时数”字段用作占位符，因此无需调整此行。
   >
   >
   >的 `minutesAsHoursString` 定义 `aggregator.displayformat` 折线表示无需按在 `valueexpression` 来获取结果。 在此 `aggregator.valuefield=workRequired` 变为： `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. 单击 **保存并关闭**.
