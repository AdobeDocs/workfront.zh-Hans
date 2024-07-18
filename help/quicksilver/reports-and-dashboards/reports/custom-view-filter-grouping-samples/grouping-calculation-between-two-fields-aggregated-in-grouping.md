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

例如，您可以在任务报告中在名为“工作平衡”的第三列中为每个任务显示实际小时数和计划小时数之间的差异。 有关计算数据表达式的详细信息，请参阅[计算数据表达式的概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

通过将计算添加到包含计算值的列的`aggregator`行，可以在分组中在同一列中显示多个计算视图项的聚合值。 例如，您可以汇总（显示总计）报告分组或“工作平衡”列列表中所有任务的“工作平衡”小时数。 本文介绍了如何执行此操作。

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

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 显示分组中多个计算值的聚合结果

1. 转到任务报告，单击&#x200B;**报告操作** > **编辑**。
1. 在&#x200B;**分组**&#x200B;选项卡中，单击&#x200B;**添加分组**，然后在&#x200B;**对您的报告进行分组** > **按**&#x200B;排序的字段开始键入&#x200B;**项目名称**，然后当它显示在列表中时将其选中。

1. 在&#x200B;**列（视图）**&#x200B;选项卡中，单击&#x200B;**添加列**，然后在&#x200B;**显示在此列**&#x200B;字段中开始键入&#x200B;**计划小时数**，然后当它显示在列表中时将其选中。

   >[!TIP]
   >
   >在文本模式下编辑信息之前，请始终开始使用标准界面添加尽可能多的信息。 添加最接近或包含您尝试计算的多数信息的字段。

1. 在&#x200B;**按**&#x200B;汇总此列，选择&#x200B;**总和**，然后单击&#x200B;**完成**。
1. 在您添加的列中单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 将`valuefield `和`aggregator.valuefield`行替换为以下文本模式示例中高亮显示的行：

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
   >要获得分组中的聚合值以显示计划小时数和实际小时数字段之间的聚合差异，请在`aggregator.valuefield`行中输入相同的等式。 用于计划小时数列的`aggregator.displayformat`将分钟转换为小时。 由于计划小时数字段用作占位符，因此无需调整此行。
   >
   >
   >`aggregator.displayformat`行的`minutesAsHoursString`定义意味着不需要像在`valueexpression`上那样将每个字段除以60以获得结果。 在此`aggregator.valuefield=workRequired`中变为： `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`。

1. 单击&#x200B;**保存+关闭**。
