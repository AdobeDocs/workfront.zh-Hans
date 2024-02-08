---
product-area: reporting
navigation-topic: text-mode-reporting
title: 设置文本模式报表中的数字、货币和百分比值的格式
description: 可以将包括货币在内的数值配置为在Adobe Workfront的报表和列表中以各种格式显示。
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 8de9c79f6c62b74a652482ec10bf38fada8c5fc8
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 7%

---

# 设置文本模式报表中的数字、货币和百分比值的格式

<!-- Audited: 2/2024 -->

可以将包括货币在内的数值配置为在Adobe Workfront的报表和列表中以各种格式显示。

要修改数字值的格式，必须编辑 **valueformat** 行中的任意一项。

例如，如果要将“预算”列显示为$1000，则值格式行将如下所示：

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

有关使用文本模式在Workfront报表和列表中应用条件格式的详细信息，请参阅 [在文本模式下使用条件格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

您可以使用以下值来格式化数字 `valueformat` 列的行：

| 示例 | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br>或 <br><pre>整数</pre> |
| 1,234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234.56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12.34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRounded</pre> |

