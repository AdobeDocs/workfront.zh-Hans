---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: IF语句概述
description: 您可以在常规编程语言中使用“IF”语句。 在Adobe Workfront中，使用“IF”语句可以比较、设置数据字段的格式和将其字符串连在一起，以便用于报告和自定义数据。 此外，通过数学方法考虑“IF”语句可以更好地理解概念，因为表达式的变量通常使用。
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# “IF”语句概述

您可以在常规编程语言中使用“IF”语句。 在Adobe Workfront中，使用“IF”语句可以比较、设置数据字段的格式和将其字符串连在一起，以便用于报告和自定义数据。 此外，通过数学方法考虑“IF”语句可以更好地理解概念，因为表达式的变量通常使用。

## Recommendations for &quot;IF&quot;语句

在创建“IF”语句之前，请考虑以下事项：

* 对于本指南，我们建议您基本了解任何一般编程语言，但我们不要求它。
* 我们需要先进地了解Workfront文本模式语法。 这有助于您了解Workfront API的术语，并了解这些特定格式中自定义数据的语法。

   有关Workfront API的信息，请参阅 [API基础知识](../../../wf-api/general/api-basics.md).

   有关使用文本模式的信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* 您可以为以下Workfront元素构建“IF”语句：

   * 视图
   * 分组
   * 计算的自定义字段

* 无法为过滤器生成“IF”语句。 这会导致Workfront中出现“Whoops”错误。
* 支持团队在构建自定义数据方面没有帮助。 在生成自定义字段或列后，如果看不到所需的结果，则可以与支持团队联系。 如需构建表达式的帮助，请联系您的客户经理以查询我们的咨询选项。
* 我们建议您首先在文本编辑器中编写这些表达式，如“崇高”或“Visual Studio Code”，因为这样可帮助您比在Workfront中更清晰地查看数据。

## “IF”语句的组件

您可以使用以下格式在Workfront中构建“IF”语句：
<pre>IF（条件，True表达式，False表达式）</pre>“IF”语句的组件包括：

* **如果**=这是“函数”的Workfront计算数据表达式。 与SUM和PROD表达式类似，它首先告知系统将函数理解为“IF”语句。 在此语句中始终对“IF”使用大写字母。\
   有关所有计算数据表达式的列表，请参阅 [计算数据表达式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **条件**=这是Workfront变量必须满足的条件，也是此等式的基础。 在等式中稍后可以指定的所有内容取决于条件。 您可以使用大量引用、比较或数学表达式来启动方程式。 一些条件示例包括：

   * 日期大于指定对象上的其他日期。
   * 状态等于指定对象上的可用状态之一。
   * 任务完成百分比小于或大于特定百分比。

* **条件运算符** =这是帮助您构建“IF”语句条件的运算符。 例如，“is equal to”或“is greater than”是条件运算符。 有关可以在语句中使用的条件运算符的列表，请参阅 [计算自定义表达式中的条件运算符](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **True****Expression**=这是“True”变量，用于告知等式在满足条件条件条件时要显示哪个指示器（true指示器）。

* **False表达式**=这是“False”变量，用于告知等式在不满足条件条件时要显示的指示器（false指示器）。

在以下示例中，原始语句格式用于为“IF”语句编写简单的数据表达式。 表达式会比较Workfront中两个不同的日期字段，后跟一个数据字符串结果为True/False:

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

在日常演讲中，这一声明将意味着：如果我对象的预计完成日期是“大于”我同一对象的计划完成日期，则在此字段中显示“非跟踪”字样。 如果没有，则显示“在跟踪”字样。

## 使用“IF”语句在自定义表单或自定义列中生成计算字段

您可以在自定义表单或自定义列的计算字段中生成“IF”语句。

在计算自定义表单中使用的语法与在计算自定义列中使用的语法有所不同。 请参阅以下示例：

* [单个“IF”语句](#single-if-statements)
* [多个“IF”语句](#multiple-if-statements)

### 单个“IF”语句 {#single-if-statements}

以下是使用“IF”语句计算的自定义字段及其相应列的示例：

* 计算的自定义字段：

构建自定义字段时，请对“IF”语句使用以下语法：

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* 计算的自定义列：

在生成自定义列时，应对值表达式行中的“IF”语句使用以下语法：

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### 多个“IF”语句 {#multiple-if-statements}

您可以将多个“IF”语句与以下语句组合在一起，以构建更复杂、更动态的表达式：

<pre>IF(Condition1,True Expression，IF(Condition2,True Expression，False Expression))</pre>请注意，现在没有第一个“IF”的false语句。 相反，我们用第二个“IF”开头替换它。

以下是使用多个“IF”语句计算自定义字段及其相应自定义列的示例：

* 计算的自定义字段：

   ```
   IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
   ```

* 计算的自定义列：

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

在此示例中，通过将两个不同的标准变量组合在一起，可以实现相同的目的。\
您可以通过在自己的环境中重建这些示例来进一步探索这些选项。

要了解这一点，最好的方法是对各种领域和情景进行试验。 此外，请熟悉API资源管理器，这会显示可使用的字段名称。 有关API资源管理器的信息，请参阅 [API Explorer](../../../wf-api/general/api-explorer.md).

有关计算数据表达式的Workfront语法的更多信息，请参阅 [计算数据表达式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
