---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算成本计划绩效指数(CSI)
description: 成本计划绩效指数(CSI)是一种自动计算，它将成本绩效指数(CPI)和计划绩效指数(SPI)合并为一个平衡成本和计划的一般指标。
author: Lisa
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# 计算成本计划绩效指数(CSI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## 成本计划绩效指数(CSI)概览

成本计划绩效指数(CSI)是一种自动计算，它将成本绩效指数(CPI)和计划绩效指数(SPI)合并为一个平衡成本和计划的一般指标。 通过将这些值相乘，单个量度可以以较低的预算处理较长的计划，反之亦然。 当牺牲成本以推动项目中期计划时，项目经理可以使用此项来确定一般项目或任务的运行状况。

>[!TIP]
>
>Adobe Workfront会为任务和项目计算CSI。 Workfront不会计算问题的CSI值。

仅当您的组织中存在以下项时，您才能从此指标提供的信息中获益：

* 您的用户正在记录他们完成的工作的时间。\
  这会根据小时数计算CSI。
* 您的用户或工作角色具有与其关联的每小时成本费率。 

  这将基于成本计算CSI。

## Workfront如何计算成本计划绩效指数(CSI)

Workfront使用以下公式计算项目或任务的成本绩效指数(CSI)：

`CSI = CPI x SPI`

有关CPI的信息，请参阅文章[计算成本绩效指数(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)。

有关SPI的信息，请参阅文章[计算计划绩效指数(SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)。

CSI具有以下三个可能的值：

* 1 =遵循总体规划
* \>1 =在预算计划组合下
* &lt;1 =超出预算计划组合

![](assets/csi-highlighted.png)

## 找到成本计划绩效指数(CSI)

>[!CAUTION]
>
>您必须具有在访问级别中查看财务数据的访问权限和查看项目或任务的权限，才能查看项目或任务的CSI值。

您可以在Workfront的以下区域中找到CSI：

* “项目详细信息”部分中的“财务”区域。
* “任务详细信息”部分中的“财务”区域。
* 项目或任务视图
* 项目或任务报告
