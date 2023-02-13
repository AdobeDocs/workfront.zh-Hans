---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算投资回报(ROI)
description: 投资回报率(ROI)是Adobe Workfront的量度，它允许投资组合经理根据项目的原始计划效益和预算成本快速查看项目的执行情况。
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 计算投资回报(ROI)

投资回报率(ROI)是Adobe Workfront的量度，它允许投资组合经理根据项目的原始计划效益和预算成本快速查看项目的执行情况。

## 项目投资回报(ROI)概述

Workfront使用以下公式计算ROI:

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

以下字段会影响项目的ROI:

* **项目计划效益**:这是在完成“业务案例”的“项目信息”区域时由项目责任人指定的手动条目。 这是对作为项目所有者的您所认为的项目好处的估计，如果您完成了项目，则可能会为您带来好处。 这是特定金额的货币，必须是正值。\
   有关项目计划效益的更多信息，请参阅文章中的“项目信息”部分 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **项目预算成本**：这是在首次启动项目时估计的与项目关联的总成本。

   的 **预算成本** 使用 **预算人工成本** 值，该值在“业务案例”的“资源预算”区域中计算，并考虑在“资源计划员”中为任务职责编入预算的小时数和每个任务职责的“每小时成本”费率。\
   有关更多信息，请参阅 [计算预算成本](../../../manage-work/projects/project-finances/budgeted-cost.md).

## 找到项目投资回报(ROI)

您可以在Workfront的以下区域查看项目的ROI价值：

* 在Portfolio优化器中，如果项目与项目组合关联

   >[!NOTE]
   >
   >所有项目ROI值的总和是项目组合的ROI。

   有关Portfolio优化程序的信息，请参阅文章 [Portfolio优化器概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* 在以下列表和报表的项目ROI字段中： 

   * 项目
   * 任务
   * 问题
   * 项目（财务数据）
   有关在Workfront中构建报表的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
