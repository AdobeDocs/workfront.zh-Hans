---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: OPTASK copyIssue的选项配置
description: copyIssue端点所需的整数值说明。
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
TQID: https://experienceleague.adobe.com/9cDJFoKl6zqpaAvqzpGqzflcbGZNrAWvEnUAFuqD-Rc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 122
ht-degree: 8%

---

# OPTASK copyIssue的选项配置


copyIssue API调用的属性之一是名为`options`的字段。 此字段应为整数。

要包括以下选项之一，请输入匹配的整数。 要包含多个选项，请输入匹配整数的和。

| option | 值* |
|---|---|
| 清除分配 | 2 |
| 清除进度 | 4 |
| 清除文档 | 128 |
| 清除更新 | 65536 |
| 清除权限 | 524288 |
| 清除自定义数据 | 1048576 |

*所有值均为2的幂。

示例：

* 要在复制问题时清除进度，请输入`options`值`4`。

* 要清除进度和文档，请输入`options`值`132`。

  清除进度= 4

  清除文档= 128

  4 + 128 = 132
