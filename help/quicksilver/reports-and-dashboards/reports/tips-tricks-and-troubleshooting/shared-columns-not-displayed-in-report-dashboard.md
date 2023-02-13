---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 功能板报表中未显示的共享列的数据
description: 将报表置于多列功能板布局中时，共享列中的数据不会显示，但它确实会在单列布局中显示。 换行符也会被覆盖。
author: Nolan
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# 功能板报表中未显示的共享列的数据

## 问题

将报表置于多列功能板布局中时，共享列中的数据不会显示，但它确实会在单列布局中显示。 换行符也会被覆盖。

## 原因

仅标记为

```
shortview=true
```

当功能板布局设置为左/右拆分或左/中/右拆分时，报表的功能板视图中会包含这些元素。

## 解决方案

访问报表中使用的视图并打开文本模式。 (有关详细信息，请参阅 [使用文本模式编辑视图](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) 为报表中的所有列（包括共享/合并列中使用的列）设置标签

```
shortview=true
```

. 然后，报表列将在功能板中正确显示。
