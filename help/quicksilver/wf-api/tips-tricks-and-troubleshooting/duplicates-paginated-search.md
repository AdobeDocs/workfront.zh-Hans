---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 在大型分页搜索期间返回的重复项
description: 在大型分页搜索期间返回的重复项
author: John
feature: Workfront API
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# 在大型分页搜索期间返回的重复项

## 问题

在API中对对象执行大量分页搜索时，客户会收到重复条目和缺失记录。

## 解决方案

当顺序未正式定义时，我们依赖Oracle数据库返回的行的顺序，这不能保证任何确定性排序。 例如，具有相同查询的两个连续调用可能会以不同的顺序返回行。 同样，在执行分页时，行可能会随机被分配到不同的“页面”，从而导致重复。 最简单的解决方案可以是按ID添加排序：

```
&ID_Sort=asc
```

