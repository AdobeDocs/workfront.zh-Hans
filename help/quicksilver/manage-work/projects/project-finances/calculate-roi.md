---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算投资回报率(ROI)
description: 投资回报率(ROI)是一个Adobe Workfront指标，它允许项目组合经理快速查看项目在原始项目计划收益和预算成本下的执行情况。
author: Lisa
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 计算投资回报率(ROI)

投资回报率(ROI)是一个Adobe Workfront指标，它允许项目组合经理快速查看项目在原始项目计划收益和预算成本下的执行情况。

## 项目投资回报率(ROI)概述

Workfront使用以下公式计算ROI：

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

以下字段会影响项目的ROI：

* **项目计划收益**：这是项目所有者在完成业务案例的项目信息区域时指定的手动条目。 这是作为项目所有者的您的项目收益的估计，如果您完成项目，可能会获得项目收益。 这是特定数量的货币，且必须为正值。\
  有关项目计划权益的更多信息，请参阅[为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)一文中的“项目信息”部分。

* **项目预算成本**：这是首次启动项目时预计的与项目关联的总成本。

  **预算成本**&#x200B;使用在业务案例的资源预算区域计算的&#x200B;**预算劳力成本**&#x200B;值，它考虑资源规划者中工作角色的预算小时数和每个工作角色的每小时成本率。\
  有关详细信息，请参阅[计算预算成本](../../../manage-work/projects/project-finances/budgeted-cost.md)。

## 找到项目投资回报率(ROI)

您可以在Workfront的以下区域查看项目的ROI值：

* 在Portfolio优化器中（如果项目与项目组合关联）

  >[!NOTE]
  >
  >所有项目ROI值的总和即为项目组合的ROI。

  有关Portfolio优化程序的信息，请参阅文章[Portfolio优化程序概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)。

* 在项目ROI字段中，将以下列表和报告添加到： 

   * 项目
   * 任务
   * 问题
   * 项目（财务数据）

  有关在Workfront中生成报表的更多信息，请参阅文章[创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
