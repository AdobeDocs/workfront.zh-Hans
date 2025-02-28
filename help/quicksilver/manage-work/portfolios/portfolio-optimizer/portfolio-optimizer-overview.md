---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Portfolio Optimizer概述
description: '[!UICONTROL Portfolio优化器]是用于项目评估和比较的工具。 审查和比较分配至项目组合的项目业务案例值的流程是项目组合经理如何确定项目的优先级并为组织生成最大价值的流程。'
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: c53e7d2229032c59710a8f955de53cfbd7fc6df4
workflow-type: tm+mt
source-wordcount: '1647'
ht-degree: 0%

---

# [!UICONTROL Portfolio Optimizer]概述

<!-- Audited: 01/2024 -->

[!UICONTROL Portfolio优化器]是用于项目评估和比较的工具。 审查和比较分配给项目组合的项目的[!UICONTROL 业务案例]值的过程是项目组合经理如何排列项目的优先顺序并为组织生成最大值的过程。

具有项目的![Portfolio优化器](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

[!UICONTROL 项目组合优化器]的目的是提供一个界面，项目组合经理、指导委员会或产品管理办公室可以通过该界面查看有关每个项目的业务案例的摘要信息。 然后，可根据战略价值和目标，或根据其总体得分，确定项目的优先次序。

[!UICONTROL Portfolio Optimizer]只有在您已完成以下先决条件时才可以协助您：

* 项目中的[!UICONTROL 业务案例]已完成。 有关信息，请参阅[定义业务案例：文章索引](../../projects/define-a-business-case/define-business-case.md)中的文章。
* 在要审阅的项目的“项目详细信息”部分的“项目概述”区域中定义项目组合。
* 您已为要审阅的项目指明了项目预算和计划收益。 固定成本和固定收入是可选的，但可增加其他值。 有关信息，请参阅[项目财务字段](../../projects/project-finances/project-finances-overview-1.md)。

有关查找[!UICONTROL Portfolio优化器]的信息，请参阅[查找[!UICONTROL Portfolio优化器]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md)。

## [!UICONTROL Portfolio Optimizer]中的财务

在使用[!UICONTROL Portfolio Optimizer]时，您可以在项目周期内的任何时间查看项目组合的财务状态。

在[!UICONTROL Portfolio Optimizer]中处理财务时，请考虑以下事项：

* 根据项目在[!UICONTROL Portfolio优化器]中匹配的标准，当项目的[!UICONTROL 业务案例]完成时，每个项目都会获得一个分数。 例如，低成本或高一致性项目会获得较高的得分。

  有关计算项目的项目组合优化器分数的详细信息，请参阅[Portfolio优化器分数[!UICONTROL 概述]](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md)。

* [!UICONTROL Portfolio优化器]的财务计算使用项目的[!UICONTROL 业务案例]中的[!UICONTROL 预算成本]。
* 您可以在[!UICONTROL Portfolio Optimizer]中手动设置项目的优先级，并会考虑有关这些项目的所有信息。 这包括财务数据、与记分卡的一致性以及ROI等。

### [!UICONTROL Portfolio Optimizer]中的财务区域 {#the-financial-areas-in-the-portfolio-optimizer}

您可以在[!UICONTROL Portfolio Optimizer]的以下区域中查看财务信息：

* **[!UICONTROL Portfolio标题]**：此区域显示从项目组合中的所有项目收集的财务信息。 它显示在Portfolio对象的每个选项卡上。
* **[!UICONTROL Portfolio选定项目的财务信息]**：此区域显示从[!UICONTROL Portfolio Optimizer]中选择的项目收集的财务信息。 您可以通过查看此区域中的信息，添加或删除项目并了解这将如何影响项目组合的财务。
* **[!UICONTROL 项目财务]**：此区域显示[!UICONTROL Portfolio优化器]中列出的每个项目的财务信息。

### [!UICONTROL Portfolio Optimizer]中的财务字段 {#the-financial-fields-in-the-portfolio-optimizer}

以下财务字段显示在[!UICONTROL Portfolio优化器]中：

* [Portfolio标题](#portfolio-header)
* [Portfolio为选定项目财务](#portfolio-finances-for-selected-projects)

#### Portfolio标题 {#portfolio-header}

![Portfolio标头](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront]使用来自项目的信息计算项目组合标题中的财务字段，这些项目的状态仅等于[!UICONTROL 已批准]或[!UICONTROL 当前]。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>字段的名称</strong> </th> 
   <th><strong>描述</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL On Time]</td> 
   <td> <p>项目组合中被认为是[！UICONTROL按时]的项目所占的百分比。 这可以从项目组合内的任何选项卡中看到。</p> <p>如果项目<strong>[！UICONTROL条件]</strong>是<strong>[！UICONTROL On Target]</strong>，则项目被视为[！UICONTROL On Time]。 <br>有关[！UICONTROL项目条件的更多信息，请参阅文章<a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">项目条件和条件类型概述</a>。</p> <p>使用以下公式计算<strong>[！UICONTROL On Time]</strong>百分比：</p> <p><em>[！UICONTROL On Time Portfolio Percentage] = [！UICONTROL On Time]项目数/处于[！UICONTROL Current]或[！UICONTROL Approved]状态的项目总数</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL On Budget]</td> 
   <td> <p>项目组合中被认为是[！UICONTROL按预算]的项目的百分比。 这可以从[！UICONTROL项目组合]中的任何选项卡中看到。</p> <p>当项目未超出其预定义的预算时，项目为<strong>[！UICONTROL On Budget]</strong>。 <br>有关项目预算的详细信息，请参阅项目财务区域</a>中的文章<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">[！UICONTROL Manage]信息。</p> <p>使用以下公式计算[！UICONTROL On Budget]百分比：</p> <p><em>[！UICONTROL On Budget Portfolio Percentage] = [！UICONTROL On Budget]项目数/ [！UICONTROL Current]或[！UICONTROL Approved]状态下的项目总数</em><em></em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI（针对项目组合）</td> 
   <td> <p>项目组合的[！UICONTROL投资回报率] (ROI)的计算方法是：考虑[！UICONTROL Portfolio]的[！UICONTROL收益]合计和项目的[！UICONTROL预算成本]合计。 这可以从项目组合内的任何选项卡中看到。</p> <p>Portfolio ROI值使用以下公式计算：</p> <p><em>Portfolio ROI = （[！UICONTROL总收益] - [！UICONTROL总预算成本]）/[！UICONTROL总成本] * 100</em> </p> <p>有关如何计算项目ROI的更多信息，请参阅文章<a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">计算投资回报率(ROI)</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Aligned]或[！UICONTROL Alignment Score] </td> 
   <td> <p>所有[！UICONTROL项目对齐分数]值的平均值，该值是在完成项目[！UICONTROL Business Case]中的[！UICONTROL Scorecard]之后计算的。 每个项目的对齐方式得分都列在[！UICONTROL Portfolio Optimizer]的[！UICONTROL Alignment]列中。 这可以从项目组合内的任何选项卡中看到。</p> <p>有关为项目生成一致性分数的详细信息，请参阅文章<a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">将记分卡应用于项目并生成一致性分数</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL净值]</td> 
   <td> <p>项目组合中所有项目的所有[！UICONTROL净值]的总和。 这可以从项目组合内的任何选项卡中看到。</p> <p>有关如何为项目计算[！UICONTROL净值]的详细信息，请参阅文章<a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">计算净值</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Portfolio为选定项目财务 {#portfolio-finances-for-selected-projects}

![Portfolio财务](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>字段的名称</strong> </th> 
   <th><strong>描述</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL项目数]</td> 
   <td> <p>项目组合中的活动项目总数。 项目组合中被视为活动的项目可以处于以下任意状态：</p> 
    <ul> 
     <li>[！UICONTROL当前版本]</li> 
     <li>[！UICONTROL规划]</li> 
     <li>[！UICONTROL已批准]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL预算]</td> 
   <td>您可以手动更新此字段以指示整个项目组合的总预算。 此预算用于项目组合内的所有项目。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL剩余]</td> 
   <td> <p>项目组合内所有项目的[！UICONTROL总成本]之后的剩余预算已从项目组合预算中减去。</p> <p>使用以下公式计算[！UICONTROL Portfolio剩余预算]：</p> <p><em>[！UICONTROL Portfolio剩余预算] = [！UICONTROL Portfolio总预算] — 所有Portfolio项目的总[！UICONTROL预算成本]</em> </p> <p>项目组合预算是Portfolio Optimizer的“预算”字段中的一个手动条目。 </p> <p>有关跟踪项目成本的更多信息，请参阅<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL总成本]</td> 
   <td> <p>在[！UICONTROL Portfolio Optimizer]中显示的所有项目的成本总和。 每个项目的成本与项目的[！UICONTROL预算成本]相同，因为它显示在[！UICONTROL业务案例摘要]中。 </p> <p>有关[！UICONTROL Business Case]中项目财务字段的更多信息，请参阅<a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">为项目创建业务案例</a>一文中的“了解业务案例中的财务字段”一节。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL风险] </td> 
   <td> <p>项目组合中所有项目的所有[！UICONTROL潜在风险成本]的总和。 每个项目的[！UICONTROL潜在风险成本]都列在[！UICONTROL Portfolio Optimizer]的[！UICONTROL风险]列中。 </p> <p>有关计算项目风险的详细信息，请参阅文章<a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">计算潜在风险成本</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL优点]</td> 
   <td> <p>项目组合中所有项目的所有[！UICONTROL计划收益]值的总和。 每个项目的计划权益值都列在[！UICONTROL Portfolio Optimizer]的[！UICONTROL Benefit]列中。 </p> <p>有关项目的[！UICONTROL计划收益]的详细信息，请参阅文章<a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">项目计划收益概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL净值风险]指示器</td> 
   <td> <p>测量由[！UICONTROL潜在风险]值，同时考虑项目组合中所有项目提供的[！UICONTROL净值]。 为了在产品组合内实现最高效率，您需要看到[！UICONTROL风险]指示器低而[！UICONTROL净值]指示器高。 </p> <p>有关计算[！UICONTROL净值的风险的更多信息，请参阅文章<a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">计算投资组合中净值的风险</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自定义[!UICONTROL Portfolio优化器]

您只能使用设置更改列表中的信息，自定义[!UICONTROL Portfolio优化器]的项目列表区域。

以下图标和选项可用于[!UICONTROL Portfolio Optimizer]：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Portfolio Optimizer中的图标</strong></td> 
   <td><strong>名称</strong></td> 
   <td><strong>功能</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[！UICONTROL设置项目优先级]</td> 
   <td><p>当您要根据项目顺序的优先级保存项目顺序时，使用此图标。</p>
   <p>您必须对列表中的所有项目具有管理权限，才能使用<b>设置项目优先级</b></p>。
    </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[！UICONTROL优化项目组合]</td> 
   <td>使用此图标可根据项目的以下财务值优化项目组合：
    <ul>
     <li>[！UICONTROL成本]</li>
     <li>[！UICONTROL对齐方式]</li>
     <li>[！UICONTROL值]</li>
     <li>[！UICONTROL收益风险]</li>
     <li>[！UICONTROL ROI]</li>
    </ul><p>有关优化项目组合的详细信息，请参阅文章<a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">在[！UICONTROL Portfolio Optimizer中优化项目]</a>。</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>[！UICONTROL撤消]/[！UICONTROL重做]图标</td> 
   <td>使用这些图标可在保存之前取消或重做您对[！UICONTROL Portfolio Optimizer]所做的更改。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[！UICONTROL Show]/[！UICONTROL Hide]未勾选的项目</td> 
   <td>使用这些图标可显示或隐藏项目组合中您未勾选的项目。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[！UICONTROL Export] </td> 
   <td> <p>使用此图标可导出[！UICONTROL Portfolio Optimizer]的[！UICONTROL项目优先级]区域中的数据。 可将其导出为以下格式：</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[！UICONTROL选项卡]已分隔</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[！UICONTROL首选项]</td> 
   <td> <p>使用此图标可修改[！UICONTROL Portfolio Optimizer]的列中显示的项目字段，或根据其状态修改您在[！UICONTROL Optimizer]中显示的项目。 </p> <p>提示：  
     <ul> 
      <li> <p>并非所有[!DNL Workfront]标准字段都可在列中添加。 </p> </li> 
     </ul> 
     <ul> 
      <li> <p>您只能在项目组合中的任何项目中添加具有零以外的值的自定义字段。</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
