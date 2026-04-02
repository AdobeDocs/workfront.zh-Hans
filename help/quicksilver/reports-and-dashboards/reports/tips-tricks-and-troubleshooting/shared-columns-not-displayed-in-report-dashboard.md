---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 共享列中的数据不会显示在功能板报表中
description: 当报表置于多列功能板布局中时，不会显示共享列的数据，但会以单列布局显示。 换行符也会被覆盖。
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 1%

---

# 共享列中的数据不会显示在功能板报表中

## 问题

当报表置于多列功能板布局中时，不会显示共享列的数据，但会以单列布局显示。 换行符也会被覆盖。

## 原因

仅标记为的列

```
shortview=true
```

当仪表板布局设置左/右拆分或左/中/右拆分时，将被包含在报告的仪表板视图中。

## 解决方案

访问报表中使用的视图，并打开文本模式。 （有关详细信息，请参阅[使用文本模式编辑视图](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)。）使用以下方式标记报表中的所有列，包括在共享/合并列中使用的列

```
shortview=true
```

。之后，报表列将在功能板中正确显示。
