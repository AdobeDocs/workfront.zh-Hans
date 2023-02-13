---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算潜在风险成本
description: 项目的潜在风险成本考虑项目风险的潜在成本及其发生的可能性。
author: Alina
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# 计算潜在风险成本

项目的潜在风险成本考虑项目风险的潜在成本及其发生的可能性。

## 项目潜在风险成本概述

Adobe Workfront使用以下公式计算项目的潜在风险成本：

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

在审核项目的潜在风险成本时，请考虑以下事项：

* 项目的计划风险成本与潜在风险成本相同。 
* 潜在风险成本未计入项目的计划成本。 而是用于确定其净值。.

## 查找项目的潜在风险成本

您可以在Workfront的以下区域找到项目的风险及其潜在成本：

* 在项目的风险选项卡中。
* 在“业务案例摘要”中。\
   有关项目业务案例的详细信息，请参阅文章 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).
* 将“计划风险成本”字段添加到报表列时，在项目报表中。\
   有关在Workfront中构建报表的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* 在Portfolio优化程序中，当项目与Portfolio关联时，显示在“风险”列中。\
   组合中所有项目的所有潜在风险成本的总和将加总Portfolio的风险。\
   有关Portfolio优化程序的更多信息，请参阅文章 [Portfolio优化器概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

有关在项目上创建风险的详细信息，请参阅文章 [在项目中创建和编辑风险](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

有关项目业务案例的详细信息，请参阅文章 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).
