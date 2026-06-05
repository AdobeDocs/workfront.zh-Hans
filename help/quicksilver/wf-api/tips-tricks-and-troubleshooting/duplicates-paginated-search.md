---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 大型分页搜索期间返回的重复项
description: 大型分页搜索期间返回的重复项
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
TQID: https://experienceleague.adobe.com/1FXTHSro-rlUVHaajM1monR2Y-sxVHN6KIviogoXqRc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 111
ht-degree: 0%

---

# 大型分页搜索期间返回的重复项

## 问题

在API中针对对象执行大型分页搜索时，客户会收到重复条目和缺失记录。

## 解决方案

当未正式定义顺序时，我们依赖于Oracle数据库返回的行的顺序，这不能保证任何确定性排序。 例如，具有相同查询的两个连续调用可能会以不同的顺序返回行。 同样，在执行分页时，这些行可能会随机分配给不同的“页面”，从而导致重复。 最简单的解决方案是添加按ID排序：

```
&ID_Sort=asc
```

