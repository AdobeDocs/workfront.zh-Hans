---
product-area: reporting
navigation-topic: text-mode-reporting
title: 设置文本模式报表中的数字、货币和百分比值的格式
description: 可以将包括货币在内的数值配置为在Adobe Workfront的报表和列表中以各种格式显示。
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 6%

---

# 设置文本模式报表中的数字、货币和百分比值的格式

<!-- Audited: 1/2025 -->

可以将包括货币在内的数值配置为在Adobe Workfront的报表和列表中以各种格式显示。

要修改数字值的格式，必须编辑列的&#x200B;**valueformat**&#x200B;行。

例如，如果要将“预算”列显示为$1000，则值格式行将如下所示：

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

有关使用文本模式在Workfront报表和列表中应用条件格式的详细信息，请参阅[在文本模式下使用条件格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)。

您可以使用列`valueformat`行的以下值来格式化数字：

| 示例 | `valueformat=` |
|---|---|
| 1234 | `doubleAsString`<br>或<br>`int` |
| 1,234 | `doubleAsInt` |
| $1,234 | `currencyStringCurrencyRounded` |
| 1234.56 | `doubleAsDouble` |
| $1,234.56 | `currencyStringCurrency` |
| 12% | `doubleAsPercentRounded` |
| 12.34% | `doubleAsPercent` |
| (1,234.56) | `doubleAsFinancial` |
| (1,234) | `doubleAsFinancialRounded` |

