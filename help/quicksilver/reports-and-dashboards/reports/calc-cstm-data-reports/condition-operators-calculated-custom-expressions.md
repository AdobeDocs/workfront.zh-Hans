---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 计算自定义表达式中的条件运算符
description: 在使用文本模式时，在Adobe Workfront中构建计算的自定义数据时，您可以使用条件运算符或修饰符。
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: 3e1e651662f9ff695d475ffcbdc77f0802d108f1
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 1%

---

# 计算自定义字段中的条件运算符

在使用文本模式时，在Adobe Workfront中构建计算的自定义数据时，您可以使用条件运算符或修饰符。

有关在Workfront中使用文本模式的信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

条件运算符或修饰符可通过连接语句中的现有Workfront字段并生成新字段来帮助构建条件语句。 条件运算符最常见的用法是构建“IF”语句的条件。

您可以使用Workfront中的“IF”语句来比较、设置数据字段的格式并将其字符串在一起，以用于报表和自定义数据。

您可以为以下Workfront元素构建“IF”语句：

* 视图
* 分组
* 计算的自定义字段

有关构建“IF”语句的详细信息，请参见 [“IF”语句概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

本指南中的示例说明了如何在计算的自定义字段中使用条件运算符。 当遵循报表中计算自定义字段的正确语法时，您还可以在计算自定义列或分组中使用它们。

有关报表中计算的自定义字段和计算的自定义数据之间的语法差异的信息，请参阅 [计算的自定义字段与计算的列](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

请参阅API资源管理器以查找要在计算的自定义表达式中引用的字段。 有关API Explorer的信息，请参阅 [API资源管理器](../../../wf-api/general/api-explorer.md).

您可以在Workfront中使用以下条件修饰符：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>条件运算符</th> 
   <th>条件运算符语法</th> 
   <th>条件运算符定义</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>等于 (区分大小写)</td> 
   <td>= </td> 
   <td> <p>使用此运算符指示当对帐单的第一个字段等于第二个字段时，满足条件。</p> <p>例如，在计算自定义字段中使用以下语句来构建“IF”语句，该语句将任务的计划完成日期与预计完成日期进行比较： </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>大于 </td> 
   <td>&gt; </td> 
   <td>使用此运算符指示当对帐单的第一个字段大于第二个字段时，满足条件。 <p>例如，在计算自定义字段中使用以下语句来构建“IF”语句，该语句将任务的计划完成日期与预计完成日期进行比较： </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>大于或等于 </td> 
   <td>&gt;= </td> 
   <td>使用此运算符指示当对帐单的第一个字段大于或等于第二个字段时满足条件。 <p>例如，在计算自定义字段中使用以下语句来构建“IF”语句，该语句将任务的计划完成日期与预计完成日期进行比较： </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>小于 </td> 
   <td>&lt; </td> 
   <td>使用此运算符指示当对帐单的第一个字段小于第二个字段时，满足条件。 <p>例如，在计算自定义字段中使用以下语句来构建“IF”语句，该语句将任务的计划完成日期与预计完成日期进行比较： </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>小于或等于 </td> 
   <td>&lt;= </td> 
   <td>使用此运算符指示当对帐单的第一个字段小于或等于第二个字段时满足条件。 <p>例如，在计算自定义字段中使用以下语句来构建“IF”语句，该语句将任务的计划完成日期与预计完成日期进行比较： </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>不会 </td> 
   <td>！ </td> 
   <td> <p>将此运算符添加到以上任何运算符的前面，使运算符无效。 </p> <p>例如： </p> 
    <ul> 
     <li>等于： = </li> 
     <li>不等于： ！= </li> 
    </ul> <p>将此运算符添加到以下数据表达式之前，会向表达式添加负语句： </p> 
    <ul> 
     <li>CONTAINS </li> 
     <li>位于‍ </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>有关这些数据表达式的信息以及完整列表，请参阅 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">计算数据表达式概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>或 </td> 
   <td>|| </td> 
   <td> <p>使用此运算符指示当表达式找到语句的第一个值或第二个值时满足条件。 </p> <p>例如，在计算自定义字段中使用以下语句来构建“IF”语句，该语句将处于“当前”或“计划”状态的项目标记为“活动”： </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td> 和 </td> 
   <td>&amp;&amp; </td> 
   <td> <p>使用此运算符可指示当表达式找到同时满足两个条件的项时，该条件是否满足。 </p> <p>例如，在计算自定义字段中使用以下语句来构建“IF”语句，以查找处于当前状态且条件为“存在风险”的项目并将它们标记为“需要调解”。 </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>
