---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算净值
description: 项目的净价值是计算项目的收益并扣除成本后的项目总预期价值。
author: Alina
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# 计算净值

项目的净价值是计算项目的收益并扣除成本后的项目总预期价值。 

## 项目净值概览

Adobe Workfront使用以下公式计算项目的净值： 

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

以下字段可能会影响项目的净值：

* **计划收益**：这是项目所有者在完成业务案例的&#x200B;**项目信息**&#x200B;区域时指定的手动条目。\
  有关项目计划权益的更多信息，请参阅[业务案例区域概述](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)文章中的[项目信息](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info)部分。

* **预算成本**：这是首次启动项目时预计的与项目关联的总成本。

  **预算成本**&#x200B;使用在业务案例的资源预算区域计算的&#x200B;**预算劳力成本**&#x200B;值，它考虑资源规划者中工作角色的预算小时数和每个工作角色的每小时成本率。\
  预算成本影响项目的&#x200B;**净值**。 有关如何计算预算成本的更多信息，请参阅[计算预算成本](../../../manage-work/projects/project-finances/budgeted-cost.md)。

* **潜在风险成本**：这是与项目上任何风险相关的成本，这些风险在业务案例或项目的“风险”选项卡中定义。\
  有关计算项目潜在风险成本的更多信息，请参阅文章[计算潜在风险成本](../../../manage-work/projects/project-finances/potential-risk-cost.md)。

   

## 找到项目净值

您可以在Workfront的以下区域找到项目的净值：

* 在商业案例的摘要区域 \
  有关“业务案例摘要”区域的详细信息，请参阅[为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)[为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)一文中的“了解业务案例摘要”一节。

  ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* 在Portfolio优化器中（如果项目与项目组合关联）

  >[!TIP]
  >
  >所有项目净值的合计是项目组合的净值。

  有关Portfolio优化程序的详细信息，请参阅[Portfolio优化程序概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)。

* 在以下列表和报告的“项目净值”字段中：

   * 项目
   * 任务
   * 问题
   * 项目 (财务数据)

  有关创建报告的详细信息，请参阅文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
