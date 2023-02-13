---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算成本计划绩效指数(CSI)
description: 成本计划绩效指数(CSI)是一种自动计算方法，它将成本绩效指数(CPI)和计划绩效指数(SPI)组合到一个平衡成本和计划的常规量度中。
author: Alina
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# 计算成本计划绩效指数(CSI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## 成本计划绩效指数(CSI)概述

成本计划绩效指数(CSI)是一种自动计算方法，它将成本绩效指数(CPI)和计划绩效指数(SPI)组合到一个平衡成本和计划的常规量度中。 通过将这些值相乘，单个量度可以在较低预算下考虑长期计划，反之亦然。 当为了在项目中期推动进度计划而牺牲成本时，项目经理可以使用此参数来确定一般项目或任务运行状况。

>[!TIP]
>
>Adobe Workfront计算任务和项目的CSI。 Workfront不计算问题的CSI值。

仅当您的组织中存在以下信息时，您才能从此量度提供的信息中受益：

* 您的用户正在记录其完成的工作的时间。\
   这会根据小时计算CSI。
* 您的用户或职务角色具有与其关联的每小时成本费率。 

   这会根据“成本”计算CSI。

## Workfront如何计算成本计划绩效指数(CSI)

Workfront使用以下公式计算项目或任务的成本绩效指数(CSI):

```
CSI = CPI x SPI
```

有关CPI的信息，请参阅 [计算成本绩效指数(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

有关SPI的信息，请参阅文章 [计算计划性能索引(SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

CSI具有以下三个可能值：

* 1 =遵循总体计划   
* 
   >1 =预算计划组合不足
* &lt;1 =超出预算的计划组合

![](assets/csi-highlighted.png)

## 找到成本计划绩效指数(CSI)

>[!CAUTION]
>
>您必须有权在访问级别查看财务数据，并有权查看项目或任务，才能查看项目或任务的CSI值。

您可以在Workfront的以下区域找到CSI:

* 项目详细信息部分的财务区域。
* “任务详细信息”部分的财务区域。
* 项目或任务视图
* 项目或任务报告
