---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Portfolio优化程序得分概述
description: 您可以在Portfolio优化程序中找到Portfolio优化程序得分。 它显示在 [!UICONTROL 得分] 列。 这表示组合中每个项目的得分。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 4451b1a3-57ae-4c66-a6a1-a85bd51a1648
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 1%

---

# 概述 [!UICONTROL Portfolio优化程序] 得分

您可以在 [!UICONTROL Portfolio优化程序] 分数 [!UICONTROL Portfolio优化程序]. 它显示在 **[!UICONTROL 得分]** 列。 这表示组合中每个项目的得分。

有关查找 [!UICONTROL Portfolio优化程序]，请参阅文章 [[!UICONTROL Portfolio优化程序] 概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

有关如何 [!DNL Adobe Workfront] 使用项目得分和其他项目信息来优化 [!UICONTROL Portfolio优化程序]，请参阅 [在Portfolio优化器中优化项目](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

## 区别 [!UICONTROL 对齐分数] 和 [!UICONTROL Portfolio优化程序分数]

项目的对齐分数与项目组合优化程序分数之间存在差异。

项目的对齐分数是根据完成记分卡后获得的点数计算的。 然后，使用此分数确定组合对齐分数。 对齐分数以百分比显示。\
项目的对齐分数显示在 **[!UICONTROL 对齐方式]** 列 [!UICONTROL Portfolio优化程序] 或 [!UICONTROL 对齐方式] 字段 [!UICONTROL 业务案例摘要].

![](assets/business-case-summary-aligned-field-highlighted.png)

![](assets/project-alignment-score-portfolio-optimizer-highlighted-350x174.png)

有关生成项目对齐分数的更多信息，请参阅文章 [将记分卡应用于项目并生成对齐分数](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

的 [!UICONTROL 组合优化器] 分数是在 [!UICONTROL Portfolio优化程序] 来确定项目的优先级。 组合优化程序得分显示为一个指示器图标，并附有一个数字，它显示在 **[!UICONTROL 得分]** 列 [!UICONTROL Portfolio优化程序].

>[!NOTE]
>
>项目可在 [!UICONTROL Portfolio优化程序] 仅当其业务案例已完成时。 有关完成业务案例的更多信息，请参阅文章 [[!UICONTROL 创建业务案例] 项目](../../../manage-work/projects/define-a-business-case/create-business-case.md).

![](assets/portfolio-optimizer-project-score-highlighted-350x132.png)

每个项目的得分是根据以下类别的重要性计算的：

* [!UICONTROL 成本]
* [!UICONTROL 对齐方式]
* [!UICONTROL 净值]
* [!UICONTROL 受益风险]
* [!UICONTROL ROI]

## 计算 [!UICONTROL Portfolio优化程序] 得分

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This was edited based on this issue, per Anna: https://hub.workfront.com/issue/603d0c58000095ea0bc00ce5e2110693/overview)</p>
-->

[!DNL Workfront] 使用 [!UICONTROL Portfolio优化程序] 这是协助确定项目优先次序的排名。 组合中的值基于在项目业务案例中输入的值，并用于计算项目的得分。 得分较高的项目可被视为更重要的项目，并可优先完成这些项目，以便首先完成。

要了解项目的排名，请执行以下操作：

1. 转到 [!UICONTROL Portfolio优化程序].
1. 将鼠标悬停在排名图标上可查看项目的组合优化程序得分。

![ranking_icon_in_portfolio_optimizer_new_png](assets/ranking-icon-in-portfolio-optimizer-new-350x160.png)

计算分数的算法考虑了项目商业案例中概述的值及其所携带的权重。 它会为优化程序中的每个项目分配一个分数并将该分数标准化，以便始终有一个分数为100的项目。 这为最佳项目提供了高分。

**示例：** 例如，如果您 [!UICONTROL 高对准度] 要考虑的唯一因素是，具有最高对齐度的项目获得100分。

以下是您可以按以下标准对项目进行评分：

* [!UICONTROL 成本]
* [!UICONTROL 对齐方式]
* [!UICONTROL 值]
* [!UICONTROL 受益风险]
* [!UICONTROL ROI]

![](assets/optimizer-sliding-value-options-350x77.png)

有关如何优化项目组合中的项目的信息，请参阅 [优化 [!UICONTROL Portfolio优化程序]](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

配置面板([!UICONTROL 成本], [!UICONTROL 对齐方式], [!UICONTROL ROI], [!UICONTROL 净值], [!UICONTROL 受益风险])的权重根据您选择的值在0到100之间。

对于具有完整业务案例的每个项目，使用以下公式为每个标准生成一个分数：

```
Score Per Criteria = (Project Value For The Criteria - AVG(all the project values for this criteria)) / Standard Deviation of that value for that project
```

**示例：** 对于 [!UICONTROL 对齐分数] 对于项目A，您将具有以下功能：

```
Alignment Score = (Project A Alignment Score - AVG (of all the project Alignments)) / Standard Deviation of alignment score for that project
```

一旦你拥有了 [!UICONTROL 按标准分数] 计算后，您可以将其添加到考虑其权重的项目中，以获得每个项目的完整分数。 项目的得分使用以下公式计算：

```
Score = Cost Score * Cost Weight + Alignment Score * Alignment Weight + ROI Score * ROI Weight + Net Value Score * Net Value Weight + Risk Score * Risk Weight
```

对于项目成本和 [!UICONTROL 风险] 逻辑与其他标准的工作方式相反：如果您想要 [!UICONTROL 低成本] 对您来说，它不会增加但会降低项目的整体分数，因为 `Cost Score * Cost Weight`.

计算每个项目的得分后， [!UICONTROL 优化分数] 通过以下方式为项目定义：

1. [!UICONTROL 最小] 和 [!UICONTROL 最大值] 分数。
1. 将计算这些值之间的范围。
1. 对于每个项目， [!UICONTROL 优化分数] 使用以下公式计算：

   ```
   Optimization Score = Rounded ((Score - Minimum / Range)*100)
   ```
