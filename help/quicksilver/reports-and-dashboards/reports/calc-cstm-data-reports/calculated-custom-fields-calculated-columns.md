---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 计算的自定义字段与计算的列
description: 要聚合Adobe Workfront中的多个字段并在新字段中显示聚合值，您可以在自定义表单中创建计算自定义字段，或在视图中创建计算列。
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: c49b545938a78716084296ef1b4e7c0fc075ef95
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# 计算的自定义字段与计算的列

要聚合Adobe Workfront中的多个字段并在新字段中显示该聚合值，您可以创建以下内容：

* 自定义表单中的计算自定义字段\
  有关将计算的自定义字段添加到自定义表单的更多信息，请参阅部分 [将计算字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#add-a-calculated-field-to-a-custom-form) 在文章中 [将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* 视图中的计算列\
  有关在视图中使用计算的更多信息，请参阅部分 [在视图中使用文本模式](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views) 在文章中 [文本模式的常见用途概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

虽然使用文本模式来构建计算字段和计算列，但构建它们的语法不同。 请参阅上面列出的文章，了解如何构建计算字段和计算列。 有关计算数据表达式中使用的不同语法（例如计算的自定义字段和列）的信息，请参阅部分 [计算自定义字段与计算自定义列的语法](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) 本文章中。

您可以在计算字段和计算列中使用相同的计算。 但是，根据您用于这些计算的目的，您可能需要考虑构建一个报表包而不是另一个报表。

## 计算自定义字段与计算自定义列的语法

尽管使用的函数相同，但在计算自定义字段中构建表达式的语法可能与构建计算自定义列的语法不同。

例如：

* 在自定义字段中，在任务的自定义表单上，使用以下内容生成附加自定义表单的任务的父级项目的名称：

  `{project}.{name}`

* 在报表的自定义列中，您将使用以下内容在任务报表中添加“项目名称”自定义列：

  `valuefield=project:name`

  或

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >相同的语法适用于使用计算表达式的所有文本模式报表元素：视图、筛选器、分组和提示。

两种语法的区别在于：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>计算的自定义字段</strong></td>
   <td><strong>计算的自定义报表元素</strong></td> 
  </tr> 
  <tr> 
   <td> <p>使用显示在Workfront界面中的字段的名称。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>计算自定义字段中使用的字段名称示例： <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>使用对象或字段在Workfront数据库中显示的名称。 如果对象和字段是复合名称，则其名称会以小写或驼峰式大小写拼写。 </p> <p>有关数据库中显示的所有Workfront对象和字段的清单，请参阅 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API资源管理器</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>计算自定义报表元素中使用的字段名称示例： <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>用圆括号或大括号括住字段名称</td> 
   <td> <p>在中使用字段名称时，请勿将其括在方括号或圆括号中 <code>valuefield </code>行。</p> <p>在中使用字段名称时，用大括号括住字段名称 <code>valueexpression</code> 行。</p> </td> 
  </tr> 
  <tr> 
   <td>按句点分隔字段</td> 
   <td> <p>在中使用字段时，请用冒号分隔这些字段 <code>valuefield</code>行。</p> <p>在中使用字段时，按句点分隔字段 <code>valueexpression</code>行。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关必须在计算自定义列中使用的语法的更多信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 何时使用计算的自定义字段

* 当您希望对报表中的聚合结果进行分组，或者希望在图表中显示此信息时
* 当您希望聚合超出字段中计算的聚合的数据时
* 当您不关心数据的及时性时，因为数据不会更新，并且可能会随着时间的推移而发生变化

## 触发计算自定义字段更新的操作

* 在对象的主页上，单击更多图标 ![](assets/more-icon.png)，然后单击 **重新计算表达式**

* 在以下情况下批量编辑多个对象 **重新计算自定义表达式** 已启用
* 编辑自定义表单时 **更新以前的计算** 为计算的自定义字段启用

## 何时在视图中使用计算列

* 当您希望实时数据在报表上可用时。

  计算视图始终是最新的，因为计算是在运行报表或应用视图时进行的。

* 当您没有计划按汇总结果分组或在图表中使用此信息时。
* 当您不打算聚合超出列中计算的聚合范围的数据时（数据只能聚合一次）。
* 当您希望计算使用$$TODAY或$$NOW通配符包含对当前日期的引用时。

  >[!TIP]
  >
  >请勿在计算自定义字段中使用此引用，因为它们仅在编辑附加对象时重新计算。 这些类型的计算已过时。

## 计算自定义字段和列的示例

有关计算的自定义字段的示例，请参阅 [报表中计算的自定义数据](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

有关视图中计算的自定义列的示例，请参阅以下文章：

* [文本模式的常见用途概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [自定义视图、筛选器和分组示例：文章索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
