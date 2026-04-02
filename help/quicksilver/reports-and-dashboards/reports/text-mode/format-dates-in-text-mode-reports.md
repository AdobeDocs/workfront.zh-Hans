---
product-area: reporting
navigation-topic: text-mode-reporting
title: 设置文本模式报表中的日期格式
description: 日期可以配置为在Adobe Workfront的报表和列表中以各种格式显示。 要建立日期格式，必须修改列中文本模式代码的valueformat行。
author: Courtney
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# 设置文本模式报表中的日期格式

<!-- Audited: 1/2025 -->

日期可以配置为在Adobe Workfront的报表和列表中以各种格式显示。 要建立日期格式，必须修改列中文本模式代码的`valueformat`行。

`valueformat= [new date format]`例如，如果您希望预计完成日期显示为MM/DD/YY，则代码将如下所示：

```
valueformat=atDate
valuefield=projectedCompletionDate
```

如果要将计划完成日期显示为&#x200B;*月，DD，年*，则代码将如下所示：

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

有关使用文本模式在Workfront报表和列表中应用条件格式的详细信息，请参阅[在文本模式下使用条件格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)。

您可以使用以下`valueformat`文本模式值设置日期格式：

| **格式** | 示例  | ***valueformat=*** |
|---|---|---|
| MM/DD/YY | 10/11/18 | `atDate` |
| MM/DD/YY时间 | 10/11/18 12:00pm | `longAtDate` |
| MM/DD/YY | 10/11/18 | `shortAtDate` |
| 月、日、年 | 2018年10月11日 | `mediumAtDate` |
| DW、月、日、年 | 2018年10月11日星期一 | `partialAtDate` |
| DW、月、日、年 | 2018年10月11日，星期一中午12:00 | `fullAtDate` |
