---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 在API中对查询结果进行排序
description: 在API中对查询结果进行排序
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 5936982217adc6cfcaf9e400bfff67a1496d3a78
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# 在API中对查询结果进行排序

如果将以下内容附加到API调用，则可以按任何字段对结果进行排序：

```
&entryDate_Sort=asc
```

例如，如果要按任务计划完成日期排序，请删除`entryDate`并将其替换为`plannedCompletionDate`。

```
&plannedCompletionDate_Sort=asc
```

这适用于Adobe Workfront中的大多数字段。
