---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 在API中对查询结果排序
description: 在API中对查询结果排序
author: John
feature: Workfront API
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# 在API中对查询结果排序

如果在API调用中附加以下内容，则可以按任意字段对结果进行排序：

```
&entryDate_Sort=asc
```

例如，如果要按任务“计划起始日期”排序，请删除 `entryDate` 用 `plannedCompletionDate`.

这适用于Adobe Workfront中的大多数字段。
