---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 共享列中的数据不会显示在功能板报表中
description: 当报表置于多列功能板布局中时，不会显示共享列的数据，但会以单列布局显示。 换行符也会被覆盖。
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OEFlwkdPf98g4-rC1tzaTmmEwb5-BXHx-j8XGrRR8sE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 162
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

访问报表中使用的视图，并打开文本模式。 （有关详细信息，请参阅[使用文本模式编辑视图](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)。） 为报表中的所有列（包括共享/合并列中使用的列）添加标签，并使用

```
shortview=true
```

. 之后，报表列将在功能板中正确显示。
