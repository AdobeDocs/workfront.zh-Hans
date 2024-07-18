---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Portfolio优化器得分概述
description: 您可以在Portfolio优化程序中找到Portfolio优化程序分数。 它显示在每个项目的[!UICONTROL 得分]列中。 表示项目组合中每个项目的得分。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 4451b1a3-57ae-4c66-a6a1-a85bd51a1648
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# [!UICONTROL Portfolio优化器]得分概述

您可以在[!UICONTROL Portfolio优化器]中找到[!UICONTROL Portfolio优化器]分数。 它显示在每个项目的&#x200B;**[!UICONTROL 得分]**&#x200B;列中。 表示项目组合中每个项目的得分。

有关查找[!UICONTROL Portfolio优化器]的信息，请参阅文章[[!UICONTROL Portfolio优化器]概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)。

有关[!DNL Adobe Workfront]如何使用项目得分和其他项目信息在[!UICONTROL Portfolio优化器]中优化项目的信息，请参阅[在Portfolio优化器中优化项目](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md)。

## [!UICONTROL 一致性分数]与[!UICONTROL Portfolio优化器分数]之间的差异

项目一致性分数与项目组合优化器分数之间存在差异。

根据完成记分卡后获得的点数计算项目的对齐分数。 然后，将使用该得分确定项目组合匹配度分数。 一致性分数以百分比显示。\
项目的对齐分数显示在[!UICONTROL Portfolio优化程序]的&#x200B;**[!UICONTROL 对齐]**&#x200B;列或[!UICONTROL 业务案例摘要]的[!UICONTROL 对齐]字段中。

![](assets/business-case-summary-aligned-field-highlighted.png)

![](assets/project-alignment-score-portfolio-optimizer-highlighted-350x174.png)

有关生成项目对齐分数的详细信息，请参阅文章[将记分卡应用于项目并生成对齐分数](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)。

[!UICONTROL 项目组合优化器]得分是在[!UICONTROL 项目组合优化器]中自动计算的Portfolio，可根据它来确定项目的优先级。 项目组合优化程序得分显示为指示符图标，并带有数字，它显示在[!UICONTROL Portfolio优化程序]的&#x200B;**[!UICONTROL 得分]**&#x200B;列中。

>[!NOTE]
>
>只有当项目的商业案例完成时，才能在[!UICONTROL Portfolio优化器]中对其评分。 有关完成业务案例的更多信息，请参阅文章[[!UICONTROL 为项目创建业务案例]](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

![](assets/portfolio-optimizer-project-score-highlighted-350x132.png)

根据以下类别的重要性计算每个项目的得分：

* [!UICONTROL 成本]
* [!UICONTROL 对齐方式]
* [!UICONTROL 净值]
* [!UICONTROL 收益风险]
* [!UICONTROL ROI]

## 计算[!UICONTROL Portfolio优化器]得分

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This was edited based on this issue, per Anna: https://hub.workfront.com/issue/603d0c58000095ea0bc00ce5e2110693/overview)</p>
-->

[!DNL Workfront]使用[!UICONTROL Portfolio优化器]生成一个分数，该分数是帮助确定项目优先级的排名。 项目组合中的值基于在项目的业务案例中输入的值，并用于计算项目的得分。 得分较高的项目可被视为比较重要，可优先完成这些项目。

要了解项目的排名，请执行以下操作：

1. 转到[!UICONTROL Portfolio优化器]。
1. 将鼠标悬停在排名图标上，可查看项目的项目组合优化器分数。

![ranking_icon_in_portfolio_optimizer_new.png](assets/ranking-icon-in-portfolio-optimizer-new-350x160.png)

计算得分的算法考虑了项目的业务案例中概述的值及其携带的权重。 它为优化器中的每个项目提供一个分数，并将分数标准化，以便始终有一个分数为100的项目。 这样可为最佳项目给出高分。

**示例：**&#x200B;例如，如果您将[!UICONTROL 较高对齐度]作为唯一考虑的因素，则具有最高对齐度的项目将获得100分。

以下是可以为项目评分的标准：

* [!UICONTROL 成本]
* [!UICONTROL 对齐方式]
* [!UICONTROL 值]
* [!UICONTROL 收益风险]
* [!UICONTROL ROI]

![](assets/optimizer-sliding-value-options-350x77.png)

有关如何优化项目组合中的项目的信息，请参阅[在[!UICONTROL Portfolio优化器]](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md)中优化项目。

配置面板上的每个条件（[!UICONTROL 成本]、[!UICONTROL 对齐方式]、[!UICONTROL ROI]、[!UICONTROL 净值]、[!UICONTROL 收益风险]）的权重范围为0-100，具体取决于您选择的内容。

对于具有完整业务案例的每个项目，使用以下公式生成每个标准的得分：

```
Score Per Criteria = (Project Value For The Criteria - AVG(all the project values for this criteria)) / Standard Deviation of that value for that project
```

**示例：**&#x200B;对于项目A的[!UICONTROL 对齐分数]，您将具有以下内容：

```
Alignment Score = (Project A Alignment Score - AVG (of all the project Alignments)) / Standard Deviation of alignment score for that project
```

计算完所有的[!UICONTROL 每个标准得分]后，可将其添加到各个项目的积分中，并计入其权重。 使用以下公式计算项目分数：

```
Score = Cost Score * Cost Weight + Alignment Score * Alignment Weight + ROI Score * ROI Weight + Net Value Score * Net Value Weight + Risk Score * Risk Weight
```

对于项目成本和[!UICONTROL 风险]，该逻辑与其他标准的工作方式相反：如果您希望[!UICONTROL 低成本]对您很重要，它不会增加，而是会降低`Cost Score * Cost Weight`的项目整体分数。

计算每个项目的分数后，将按以下方式为项目定义[!UICONTROL 优化分数]：

1. 定义了[!UICONTROL 最小]和[!UICONTROL 最大]分数。
1. 计算这些值之间的范围。
1. 对于每个项目，[!UICONTROL 优化得分]使用以下公式计算：

   ```
   Optimization Score = Rounded ((Score - Minimum / Range)*100)
   ```
