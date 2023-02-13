---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 计算自定义字段与计算列
description: 要在Adobe Workfront中聚合多个字段并在新字段中显示该聚合值，您可以执行以下操作 — 编辑我。
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# 计算自定义字段与计算列

要在Adobe Workfront中聚合多个字段并在新字段中显示该聚合值，您可以执行以下操作：

* 自定义表单中的计算自定义字段\
   有关将计算的自定义字段添加到自定义表单的更多信息，请参阅部分 [向自定义表单中添加计算字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#creating-calculated-custom-fields) 在文章中 [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* 视图中的计算列\
   有关在视图中使用计算的详细信息，请参阅部分 [在视图中使用文本模式](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#using-text-mode-in-views) 在文章中 [文本模式常见用法概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

尽管使用文本模式来生成计算字段和计算列，但生成这些字段的语法却有所不同。 请参阅上面列出的文章，了解如何生成计算字段和计算列。 有关计算数据表达式（如计算自定义字段和列）中使用的不同语法的信息，请参阅部分 [计算自定义字段与计算自定义列的语法](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns-syntax) 在本文中。

您可以在两个计算字段和计算列中使用相同的计算。 但是，根据您用于这些计算的目的，您可能需要考虑构建一个计算器，而不是另一个计算器。

## 计算自定义字段与计算自定义列的语法

尽管您使用的函数相同，但在计算自定义字段中构建表达式的语法可能与在构建计算自定义列时所用的语法不同。

例如：

* 在自定义字段中，对于任务的自定义表单，您可以使用以下方法生成附加了自定义表单的任务的父项目的名称：

   ```
   {project}.{name}
   ```

* 在报表的自定义列中，您可以使用以下方法在任务报表中添加项目名称自定义列：

   ```
   valuefield=project:name
   ```

   或

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >相同的语法适用于使用计算表达式的所有文本模式报表元素：视图、过滤器、分组、提示。

这两种语法的区别是：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>计算的自定义字段</td> 
   <td>计算的自定义报表元素</td> 
  </tr> 
  <tr> 
   <td> <p>使用字段在Workfront界面中显示的名称。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>在计算的自定义字段中使用的字段名称示例： <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>使用对象或字段在Workfront数据库中显示的名称。 对象和字段的名称以小写或驼峰式拼写（如果它们是复合名称）。 </p> <p>有关数据库中显示的所有Workfront对象和字段的清单，请参阅 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>计算自定义报表元素中使用的字段名称示例： <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>用圆括号或大括号括住字段名称</td> 
   <td> <p>在 <code>valuefield </code>行。</p> <p>在 <code>valueexpression</code> 行。</p> </td> 
  </tr> 
  <tr> 
   <td>按句点分隔字段</td> 
   <td> <p>在 <code>valuefield </code>行</p> <p>在 <code>valueexpression </code>行。 </p> </td> 
  </tr> 
 </tbody> 
</table>

有关在计算自定义列中必须使用的语法的更多信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 何时使用计算的自定义字段

* 当您想要在报表中对聚合结果进行分组或希望在图表中显示此信息时
* 当您想要聚合超出在字段中计算的聚合的数据时
* 当您不担心数据的及时性时，由于数据不会更新，并且可能会随时间而改变

## 触发计算自定义字段更新的操作

* 在对象的主页上，单击更多图标 ![](assets/more-icon.png)，然后单击 **重新计算表达式**

* 在 **重新计算自定义表达式** 已启用
* 编辑自定义表单时 **更新以前的计算** 为计算的自定义字段启用

## 何时在视图中使用计算列

* 您希望实时数据在报表中可用时。

   计算视图始终是全新的，因为计算是在运行报表或应用视图时进行的。

* 当您没有计划按汇总结果进行分组，或在图表中使用此信息时。
* 当您不打算聚合除列中计算的聚合之外的数据时（数据只能聚合一次）。
* 当您希望计算时，使用$$TODAY或$$NOW通配符包含对当前日期的引用。

   >[!TIP]
   >
   >请勿在计算的自定义字段中使用此引用，因为只有在编辑附加的对象时，这些引用才会重新计算。 这些类型的计算已过时。

## 计算自定义字段和列的示例

有关计算自定义字段的示例，请参阅 [报表中的计算自定义数据](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

有关视图中计算自定义列的示例，请参阅以下文章：

* [文本模式常见用法概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [自定义视图、过滤器和分组示例](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
