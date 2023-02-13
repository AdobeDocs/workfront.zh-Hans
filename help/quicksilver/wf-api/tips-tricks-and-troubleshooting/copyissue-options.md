---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: OPTASK copyIssue的选项配置
description: copyIssue端点预期的整数值的说明。
author: Becky
feature: Workfront API
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 93a67b3dbd59f188dad6b060ec93c3f137c981b2
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 6%

---

# OPTASK copyIssue的选项配置


copyIssue API调用的属性之一是名为的字段 `options`. 此字段应为整数。

要包括以下选项之一，请输入匹配的整数。 要包含多个选项，请输入匹配整数的和。

| 选项 | value* |
|---|---|
| 清除分配 | 2 |
| 明确进展 | 4 |
| 清除文档 | 128 |
| 清除更新 | 65536 |
| 清除权限 | 524288 |
| 清除自定义数据 | 1048576 |

*所有值均为2的幂。

示例:

* 要在复制问题时清除进度，请输入 `options` 值 `4`.

* 要清除进度和文档，请输入 `options` 值 `132`.

   清除进度= 4

   清除文档= 128

   4 + 128 = 132
