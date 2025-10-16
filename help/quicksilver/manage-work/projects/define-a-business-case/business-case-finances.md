---
content-type: overview
navigation-topic: business-case-and-scorecards
title: 业务案例财务字段概述
description: “业务案例”子标签包括项目的财务字段。 为了使某些财务字段具有值，必须完成业务案例的相应区域。
author: Becky
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: fa0b4322b9f7c1d506cf194645c7ae50ad8c0f0b
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 2%

---

# 业务案例财务字段概述

“业务案例”子标签包括项目的财务字段。 为了使某些财务字段具有值，必须完成业务案例的相应区域。 

以下项目财务字段显示在业务案例中：

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="col">字段名称</th> 
   <th scope="col">描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>已对齐 </td> 
   <td> <p>根据记分卡显示项目的对齐方式。 较高的百分比值表示项目与组织的目的和目标很好地保持一致。 <br>有关使用记分卡的更多信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">创建记分卡</a>。</p> <p>此字段显示在“业务案例摘要”区域中。 </p> </td> 
  </tr> 
  <tr> 
   <td>预算成本</td> 
   <td> <p>项目启动时预计与项目关联的总成本。</p> <p>项目的预算成本按以下公式计算：<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront使用资源规划者中的预算小时数计算预算劳力成本。<br>有关计算预算成本的更多信息，请参阅<a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">计算预算成本</a>。 </p> <p>此字段显示在“业务案例摘要”区域中。</p> </td> 
  </tr> 
  <tr> 
   <td>预算支出成本</td> 
   <td> <p>项目所有支出的预算成本。 </p> <p>计算公式如下：</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>有关计算支出的详细信息，请参阅<a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">管理项目支出</a>。</p> <p>此字段显示在费用区域。</p> </td> 
  </tr> 
  <tr> 
   <td>预算劳动力成本</td> 
   <td> <p>与分配用于完成项目工作的资源关联的成本。</p> <p>项目的预算劳力成本按以下公式计算：<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><br></p> <p>Workfront使用资源规划者中的预算小时数计算预算劳力成本。<br>有关计算预算劳力成本的更多信息，请参阅<a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">了解项目的预算劳力成本和预算小时数</a>。</p> <p>此字段显示在业务案例的资源预算区域。 </p> </td> 
  </tr> 
  <tr> 
   <td>费用计划成本</td> 
   <td> <p>这与预算支出成本相同。 </p> <p>注：费用计划成本与项目的计划成本不同。 费用计划成本使用项目费用的计划金额计算，而计划成本使用项目上的计划小时数计算。 </p> <p>对于每个费用，此字段显示在费用区域中。</p> </td> 
  </tr> 
  <tr> 
   <td>净值</td> 
   <td> <p>这是计算项目的效益和扣除成本后的项目总预期价值。</p> <p>项目的“净值”按以下公式计算：<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>。 <br></p> <p>有关计算净值的详细信息，请参阅<a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">计算净值</a>。<br></p> <p>此字段显示在“业务案例摘要”区域中。</p> </td> 
  </tr> 
  <tr> 
   <td>规划收益</td> 
   <td>此项目完成时组织货币收益的手动估计。 它可以是任意数量的货币，并且特定于您以及您管理的每个项目。 计划福利不能具有负值。 此字段显示在业务案例摘要区域中，并且可在业务案例的项目信息区域中进行编辑。 </td> 
  </tr> 
  <tr> 
   <td>潜在风险成本</td> 
   <td> <p>这是项目所有风险的潜在成本。 </p> <p>可使用以下公式计算此值：</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>有关项目风险的更多信息，请参阅<a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">创建和编辑项目风险</a>。</p> <p>此字段显示在“业务案例摘要”区域中。</p> </td> 
  </tr> 
  <tr> 
   <td>潜在风险</td> 
   <td> <p>在“业务案例摘要”中，这是所有风险（如果发生）的成本金额，基于风险发生的概率。 例如，如果风险的潜在成本为$100，发生概率为10%，则潜在风险为$10。 业务案例摘要中的潜在风险按以下公式计算：</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> 冒着所有风险。 </p> </td> 
  </tr> 
  <tr> 
   <td>风险缓解成本</td> 
   <td> <p>针对您正在估计的风险而制定的缓解计划的成本可能会出现在项目中。<br>有关项目风险的更多信息，请参阅<a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">创建和编辑项目风险</a>。</p> <p>此字段显示在项目上指定的每个风险的“风险”区域中。</p> </td> 
  </tr> 
  <tr> 
   <td>一项风险的潜在成本</td> 
   <td> <p>当项目上定义的风险实际发生时的估计财务成本，无论其可能性如何。 </p> <p>这是一个手动更新的字段，显示在业务案例的风险区域的每个风险。 </p> </td> 
  </tr> 
  <tr> 
   <td>风险总潜在成本</td> 
   <td> <p>这是项目上定义的所有风险实际发生时的总估计财务成本。 </p> <p>计算公式如下：</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>它会在业务案例的风险区域标题旁边显示为一个货币编号。</p> </td> 
  </tr> 
 </tbody> 
</table>
