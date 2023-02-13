---
product-area: reporting
navigation-topic: text-mode-reporting
title: 在文本模式报表中设置日期格式
description: 日期可配置为在Adobe Workfront的报表和列表中以多种格式显示。 要建立日期格式，必须修改列中文本模式代码的值格式行。
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 2%

---

# 在文本模式报表中设置日期格式

日期可配置为在Adobe Workfront的报表和列表中以多种格式显示。 要建立日期格式，您必须修改 `valueformat` 列中文本模式代码的行。

`valueformat= [new date format]` 例如，如果您希望将预计完成日期显示为MM/DD/YY，则代码将如下所示：

```
valueformat=atDate
valuefield=projectedCompletionDate
```

如果要将计划完成日期显示为 *Mth，DD，年*，则代码如下所示：

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

有关在Workfront报表和列表中使用文本模式应用条件格式的更多信息，请参阅 [在文本模式中使用条件格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

您可以使用以下内容设置日期格式

```
valueformat
```

 文本模式值：

| **格式** | 示例  | ***valueformat=*** |
|---|---|---|
| MM/DD/YY | 10/11/18 | `atDate` |
| MM/DD/YY时间 | 10/11/18中午12:00 | `longAtDate` |
| MM/DD/YY | 10/11/18 | `shortAtDate` |
| 马特、dd、yr | 2018年10月11日 | `mediumAtDate` |
| DW、Mth、Day、YR | 2018年10月11日星期一 | `partialAtDate` |
| DW、Mth、Day、YR时间 | 2018年10月11日，星期一中午12:00 | `fullAtDate` |
