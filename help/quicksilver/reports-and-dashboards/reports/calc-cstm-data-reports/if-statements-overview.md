---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: IF语句概述
description: 可以在通用编程语言中使用“IF”语句。 在Adobe Workfront中，“IF”语句允许您比较、设置数据字段的格式并将其字符串在一起，以用于报表和自定义数据。 此外，从数学上考虑“IF”语句可以更好地理解概念，因为表达式变量是常用的。
author: Jenny
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# “IF”语句概述

<!-- Audited: 1/2024 -->

可以在通用编程语言中使用“IF”语句。 在Adobe Workfront中，“IF”语句允许您比较、设置数据字段的格式并将其字符串在一起，以用于报表和自定义数据。 此外，从数学上考虑“IF”语句可以更好地理解概念，因为表达式变量是常用的。

## “IF”语句的建议

在创建“IF”语句之前，请考虑以下事项：

* 对于本指南，我们建议基本了解任何通用编程语言，但我们不需要它。
* 我们需要高级了解Workfront文本模式语法。 这有助于掌握Workfront API的术语并了解这些特定格式的自定义数据的语法。

  有关Workfront API的信息，请参阅[API基础知识](../../../wf-api/general/api-basics.md)。

  有关使用文本模式的信息，请参阅[文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

* 您可以为以下Workfront元素构建“IF”语句：

   * 视图
   * 分组
   * 计算的自定义字段

* 无法为过滤器构建“IF”语句。 这会导致Workfront中出现“糟糕”错误。
* 支持团队不帮助构建自定义数据。 构建自定义字段或列且看不到所需结果后，您可以联系支持团队。 要获取构建表达式的帮助，请联系您的客户经理以查询我们的咨询选项。
* 我们建议先在文本编辑器中编写这些表达式，例如Sublime或Visual Studio Code，因为这样有助于您更清楚地查看数据，而不是显示在Workfront中。

## “IF”语句的组件

您可以使用以下格式在Workfront中构建“IF”语句：
<pre>IF（Condition，True表达式，False表达式）</pre>“IF”语句的组成部分包括：

* **IF** =这是“函数”的Workfront计算数据表达式。 与SUM和PROD表达式类似，它首先告诉系统将该函数理解为“IF”语句。 在此语句中始终使用大写字母表示“IF”。\
  有关所有计算数据表达式的列表，请参阅[计算数据表达式的概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

* **条件** =这是Workfront变量必须满足的条件，也是此方程式的基础。 之后可在方程式中指定的所有内容都取决于条件。 可以使用许多引用、比较或数学表达式来启动公式。 条件的一些示例包括：

   * 日期晚于指定对象上的另一个日期。
   * 状态等于指定对象上可用的状态之一。
   * 任务的完成百分比小于或大于某个百分比。

* **条件运算符** =此运算符可帮助您构建“IF”语句的条件。 例如，“等于”或“大于”是条件运算符。 有关可在语句中使用的条件运算符列表，请参阅计算自定义表达式中的[条件运算符](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md)。

* **True**&#x200B;**Expression** =这是“True”变量，它告知等式满足条件的条件（true指示器）后要显示的指示器。

* **False表达式** =这是“False”变量，它告知公式当不符合条件的条件（false指示符）时要显示的指示符。

在以下示例中，使用原始语句格式为“IF”语句编写简单数据表达式。 该表达式比较了Workfront中的两个不同的日期字段，然后将True/False结果作为数据字符串：

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

在日常讲话中，此语句的意思是：如果我的对象的预计完成日期大于“我的同一对象的计划完成日期”，则在此字段中显示“偏离轨道”一词。 如果没有，则显示“On Track”（正在跟踪）。

## 使用“IF”语句在自定义表单或自定义列中生成计算字段

您可以在自定义表单的计算字段中或自定义列中构建“IF”语句。

在计算自定义表单中使用的语法与计算自定义列中使用的语法有所不同。 请参阅以下示例：

* [单个“IF”语句](#single-if-statements)
* [多个“IF”语句](#multiple-if-statements)

### 单个“IF”语句 {#single-if-statements}

以下是使用“IF”语句的计算自定义字段及其对应列的示例：

* 计算的自定义字段：

构建自定义字段时，请为“IF”语句使用以下语法：

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* 计算的自定义列：

构建自定义列时，您应该对值表达式行中的“IF”语句使用以下语法：

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### 多个“IF”语句 {#multiple-if-statements}

您可以将多个“IF”语句与以下语句组合在一起，以构建更复杂且更动态的表达式：

<pre>IF(Condition1，True表达式，IF（Condition2，True表达式，False表达式）)</pre>请注意，对于第一个“IF”，现在没有错误陈述。 相反，我们用第二个“IF”的开头替换了它。

以下是使用多个“IF”语句的计算自定义字段及其对应的自定义列的示例：

* 计算的自定义字段：

  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* 计算的自定义列：

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

在此示例中，通过将两个不同的标准变量放在一起，可以实现相同的目标。\
通过在您自己的环境中重建这些示例，您可以进一步探索这些选项。

要了解这一点，最好的方法是对各种字段和场景进行实验。 此外，熟悉API Explorer，它会显示可以使用的字段名称。 有关API浏览器的信息，请参阅[API浏览器](../../../wf-api/general/api-explorer.md)。

有关计算数据表达式的Workfront语法的详细信息，请参阅[计算数据表达式概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。
