---
product-area: reporting
navigation-topic: text-mode-reporting
title: 在文本模式报表中设置数字、货币和百分比值的格式
description: 数值（包括货币）可配置为在Adobe Workfront的报表和列表中以各种格式显示。
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 7%

---

# 在文本模式报表中设置数字、货币和百分比值的格式

数值（包括货币）可配置为在Adobe Workfront的报表和列表中以各种格式显示。

要修改数值的格式，您必须编辑 **valueformat** 行。

例如，如果您想将“预算”列显示为$1000，则值格式行将如下所示：

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

有关在Workfront报表和列表中使用文本模式应用条件格式的更多信息，请参阅 [在文本模式中使用条件格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

您可以使用 `valueformat` 列行：

| 示例 | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br>或 <br><pre>int</pre> |
| 1,234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234.56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12.34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRounded</pre> |
