---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算净值
description: 项目净值是在计算项目效益和消除成本后项目的预计总价值。
author: Alina
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# 计算净值

项目净值是在计算项目效益和消除成本后项目的预计总价值。 

## 项目净值概述

Adobe Workfront使用以下公式计算项目的净值： 

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

以下字段可能会影响项目的净值：

* **计划福利**:这是项目所有者在完成 **项目信息** “商业案例”区域。\
   有关项目计划效益的详细信息，请参阅 [项目信息](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) 文章章节 [业务案例领域概述](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **预算成本**：这是在首次启动项目时估计的与项目关联的总成本。

   的 **预算成本** 使用 **预算人工成本** 值，该值在“业务案例”的“资源预算”区域中计算，并考虑在“资源计划员”中为任务职责编入预算的小时数和每个任务职责的“每小时成本”费率。\
   预算成本影响 **净值** 的项目。 有关如何计算预算成本的详细信息，请参阅 [计算预算成本](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **潜在风险成本**:这是与项目中任何风险（如“业务案例”或项目的“风险”选项卡中所定义）相关的成本。\
   有关计算项目潜在风险成本的详细信息，请参阅文章 [计算潜在风险成本](../../../manage-work/projects/project-finances/potential-risk-cost.md).

    

## 找到项目净值

您可以在Workfront的以下区域中找到项目的净值：

* 在业务案例摘要区域中 \
   有关“业务案例摘要”区域的详细信息，请参阅文章中的“了解业务案例摘要”部分 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md) [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

   ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* 在Portfolio优化器中，如果项目与项目组合关联

   >[!TIP]
   >
   >所有项目净值的合计是项目组合的净值。

   有关Portfolio优化程序的更多信息，请参阅 [Portfolio优化器概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* 在以下列表和报表的项目净值字段中：

   * 项目
   * 任务
   * 问题
   * 项目 (财务数据)
   有关创建报表的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
