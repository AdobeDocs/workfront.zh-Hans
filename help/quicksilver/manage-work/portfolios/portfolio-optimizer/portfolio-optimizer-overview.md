---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Portfolio优化器概述
description: 的 [!UICONTROL Portfolio优化程序] 是用于项目评估和比较的工具。 审核和比较分配给项目组合的项目业务案例值的过程，是项目组合经理如何对项目进行优先级排序并为组织生成最大价值的过程。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: 4440fc50e988da6e446fd9a3195ae94f978b4b74
workflow-type: tm+mt
source-wordcount: '1654'
ht-degree: 0%

---

# [!UICONTROL Portfolio优化程序] 概述

的 [!UICONTROL Portfolio优化程序] 是用于项目评估和比较的工具。 审查和比较的过程 [!UICONTROL 商业案例] 分配给项目组合的项目值是项目组合经理如何对项目进行优先级排序，并为组织生成最大价值。

的目的 [!UICONTROL 组合优化器] 是提供一个界面，通过该界面，组合经理、指导委员会或产品管理办公室可以查看有关每个项目的业务案例的摘要信息。 然后，可以根据战略价值和目标或项目的总体得分确定项目的优先级。

的 [!UICONTROL Portfolio优化程序] 仅当您完成了以下先决条件时，才能提供协助：


* 的 [!UICONTROL 商业案例] 已经完成了项目。 有关信息，请参阅章节中的文章 [定义业务案例](../../projects/define-a-business-case/define-business-case.md).
* 在“项目详细信息”部分的“项目概述”区域中为要审核的项目定义了项目组合
* 您为要审核的项目指明了项目预算和计划福利。 “固定成本”和“固定收入”是可选的，但会添加额外价值。 有关信息，请参阅 [项目财务字段](../../projects/project-finances/project-finances-overview-1.md).


有关查找 [!UICONTROL Portfolio优化程序]，请参阅 [找到 [!UICONTROL Portfolio优化程序]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## 财务 [!UICONTROL Portfolio优化程序]

* [金融领域 [!UICONTROL Portfolio优化程序]](#the-financial-areas-in-the-portfolio-optimizer)
* [中的财务字段 [!UICONTROL Portfolio优化程序]](#the-financial-fields-in-the-portfolio-optimizer)

在使用 [!UICONTROL Portfolio优化程序].

在中处理财务时，请考虑以下事项 [!UICONTROL Portfolio优化程序]:

* 每个项目在其 [!UICONTROL 商业案例] 将根据 [!UICONTROL Portfolio优化程序]. 例如，低成本或高校准项目的得分较高。

   有关计算项目的组合优化程序分数的更多信息，请参阅文章 [概述 [!UICONTROL Portfolio优化程序] 得分](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* 本集团于财务 [!UICONTROL Portfolio优化程序] 使用 [!UICONTROL 预算成本] 在 [!UICONTROL 商业案例] 的项目。
* 您可以在 [!UICONTROL Portfolio优化程序]，并考虑到所有与他们有关的信息。 例如，这包括财务数据、与记分卡的一致性、ROI。

### 金融领域 [!UICONTROL Portfolio优化程序] {#the-financial-areas-in-the-portfolio-optimizer}

您可以在 [!UICONTROL Portfolio优化程序]:

* **[!UICONTROL Portfolio标题]**:此区域显示从组合中的所有项目收集的财务信息。 它显示在Portfolio对象的每个选项卡中。
* **[!UICONTROL Portfolio选定项目的财务]**:此区域显示从 [!UICONTROL Portfolio优化程序]. 您可以添加或删除项目，并通过查看此区域中的信息了解这将如何影响项目组合的财务状况。
* **[!UICONTROL 项目财务]**:此区域显示 [!UICONTROL Portfolio优化程序].

### 中的财务字段 [!UICONTROL Portfolio优化程序] {#the-financial-fields-in-the-portfolio-optimizer}

以下财务字段显示在 [!UICONTROL Portfolio优化程序]:

* [Portfolio标题](#portfolio-header)
* [Portfolio选定项目的资金](#portfolio-finances-for-selected-projects)

#### Portfolio标题 {#portfolio-header}

![](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] 使用状态仅等同于的项目信息计算组合标题中的财务字段 [!UICONTROL 已批准] 或 [!UICONTROL 当前].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>字段名称</strong> </th> 
   <th><strong>描述</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL On Time]</td> 
   <td> <p>组合中被视为[!UICONTROL On Time]的项目的百分比。 此图标可在Portfolio内的任意选项卡中显示。</p> <p>项目时，项目被视为[!UICONTROL On Time] <strong>[!UICONTROL条件]</strong> is <strong>[!Uicontrol On Target]</strong>. <br>有关[!UICONTROL项目条件]的更多信息，请参阅文章 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">项目条件和条件类型概述</a>.</p> <p>的 <strong>[!UICONTROL On Time]</strong> 百分比使用以下公式计算：</p> <p><em>[!UICONTROL On Time Approved Percentage] = [!UICONTROL On Time]项目数/ [!UICONTROL Current]或[!UICONTROL Approved]状态中的项目总数</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL On Budget]</td> 
   <td> <p>组合中被视为[!UICONTROL On Budget]的项目的百分比。 此图标可在[!UICONTROLPortfolio]内的任意选项卡中显示。</p> <p>项目包括 <strong>[!UICONTROL On Budget]</strong> 未超过预定预算时。 <br>有关项目预算的详细信息，请参阅文章 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">“项目财务”区域中的[!UICONTROL管理]信息</a>.</p> <p>[!UICONTROL On Budget]百分比使用以下公式计算：</p> <p><em>[！预算Portfolio百分比的UICONTROL] = [！预算上的UICONTROL]项目数/项目总数 </em><em>在[!UICONTROL Current]或[!UICONTROL Approved]状态中</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI（针对产品组合）</td> 
   <td> <p>组合的[!UICONTROL投资回报](ROI)是考虑[!UICONTROLPortfolio]的[!UICONTROL优势]总额和项目的[!UICONTROL预算成本]总额来计算的。 此图标可在Portfolio内的任意选项卡中显示。</p> <p>PortfolioROI值使用以下公式计算：</p> <p><em>PortfolioROI =（[!UICONTROL总收益] - [!UICONTROL总预算成本]）/ [!UICONTROL总成本] x 100</em> </p> <p>有关如何计算项目ROI的更多信息，请参阅文章 <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">计算投资回报(ROI)</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aligned]或[!UICONTROL Alignment Score] </td> 
   <td> <p>在完成项目的[!UICONTROL Business Case]中的[!UICONTROL Scorecard]后计算的所有[!UICONTROL项目协调分数]值的平均值。 每个项目的对齐分数列在[!UICONTROL Alignment]的[!UICONTROL Optimizer]列中。 此图标可在组合中的任意选项卡中显示。</p> <p>有关为项目生成对齐分数的更多信息，请参阅文章 <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">将记分卡应用于项目并生成对齐分数</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL净值]</td> 
   <td> <p>组合中所有项目的所有[!UICONTROL净值]的总和。 此图标可在组合中的任意选项卡中显示。</p> <p>有关如何为项目计算[!UICONTROL Net Value]的更多信息，请参阅文章 <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">计算净值</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Portfolio选定项目的资金 {#portfolio-finances-for-selected-projects}

![](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>字段名称</strong> </th> 
   <th> <p><strong>描述</strong> </p> <p> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL项目数]</td> 
   <td> <p>组合中活动项目的总数。 在项目组合中被视为活动的项目可以处于以下任何状态：</p> 
    <ul> 
     <li>[!UICONTROL当前]</li> 
     <li>[!UICONTROL Planning]</li> 
     <li>[!UICONTROL Approved]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL预算]</td> 
   <td>您可以手动更新此字段以指示整个组合的总预算。 此预算用于项目组合中的所有项目。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retained]</td> 
   <td> <p>组合内所有项目的所有[!UICONTROL预算成本]之后的剩余预算已从组合预算中减去。</p> <p>[!UICONTROL剩余Portfolio预算]使用以下公式计算：</p> <p><em>[!UICONTROL剩余Portfolio预算] = [!UICONTROL总Portfolio预算] — 所有Portfolio项目的[!UICONTROL预算成本]合计</em> </p> <p>组合中所有项目的总[!UICONTROL预算成本]在预算字段下的指标栏中显示。 </p> <p>有关跟踪项目成本的更多信息，请参阅文章<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL总成本]</td> 
   <td> <p>[!UICONTROLPortfolio优化器]中显示的所有项目的成本总和。 每个项目的成本与项目的[!UICONTROL预算成本]相同，它显示在[!UICONTROL业务案例汇总]中。 </p> <p>有关[!UICONTROL Business Case]中项目的财务字段的详细信息，请参阅文章中的“了解业务案例中的财务字段”一节 <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">为项目创建业务案例 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL风险] </td> 
   <td> <p>组合中所有项目的所有[!UICONTROL潜在风险成本]的总和。 每个项目的[!UICONTROL潜在风险成本]列在[!UICONTROLPortfolio优化程序]的[!UICONTROL风险]列中。 </p> <p>有关计算项目风险的详细信息，请参阅文章 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">计算潜在风险成本 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL优势]</td> 
   <td> <p>组合中所有项目的所有[!UICONTROL计划福利]值的总和。 每个项目的“计划福利”值列在[!UICONTROL Optimizer]的[!UICONTROL Benefit]列中。 </p> <p>有关项目[!UICONTROL计划效益]的更多信息，请参阅文章 <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">项目计划效益概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL风险对净值]指标</td> 
   <td> <p>衡量[!UICONTROL潜在风险]值时，会考虑组合中所有项目提供的[!UICONTROL净值]。 要在产品组合中实现最高效率，您希望看到[!UICONTROL Risk]指标较低，[!UICONTROL Net Value]指标较高。 </p> <p>有关计算[!UICONTROL净值]风险的详细信息，请参阅文章 <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">计算组合中的风险对净值</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自定义 [!UICONTROL Portfolio优化程序]

您只能自定义 [!UICONTROL Portfolio优化程序] 使用设置更改列表中的信息。

以下图标和选项适用于 [!UICONTROL Portfolio优化程序]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Portfolio优化器中的图标</td> 
   <td>名称</td> 
   <td>功能</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL设置项目优先级]</td> 
   <td>当您要根据项目优先级保存项目顺序时，请使用此图标。 </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[!UICONTROL优化产品组合]</td> 
   <td>使用此图标可根据项目的以下财务值优化项目组合：
    <ul>
     <li>[!UICONTROL成本]</li>
     <li>[!UICONTROL Alignment]</li>
     <li>[!UICONTROL值]</li>
     <li>[!UICONTROL Risk to Beent]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>有关优化产品组合的更多信息，请参阅文章 <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">在[!UICONTROLPortfolio优化器]中优化项目 </a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>[!UICONTROL撤消]/ [!UICONTROL重做]图标</td> 
   <td>在保存之前，使用这些图标可取消或重做您对[!UICONTROLPortfolio优化器]所做的更改。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[!UICONTROL Show]/ [!UICONTROL Hide unchecked]项目</td> 
   <td>使用这些图标可显示或隐藏您未选中的项目组合中的项目。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL导出] </td> 
   <td> <p>使用此图标可导出[!UICONTROL Project Optimizer]的[!UICONTROL Project Hiresidence]区域中的Portfolio。 您可以将其导出为以下格式：</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[!UICONTROL制表符]分隔</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL首选项]</td> 
   <td> <p>使用此图标可修改[!UICONTROLPortfolio优化程序]列中显示的项目字段，或根据您在[!UICONTROL优化程序]中显示的项目状态，修改这些项目。 </p> <p>提示：  
     <ul> 
      <li> <p>并非全部 [!DNL Workfront] 可在列中添加标准字段。 </p> </li> 
     </ul> 
     <ul> 
      <li> <p>您只能在项目组合中的任何项目中添加值不为零的自定义字段。</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
