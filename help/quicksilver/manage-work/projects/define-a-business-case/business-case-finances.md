---
content-type: overview
navigation-topic: business-case-and-scorecards
title: 业务案例财务字段概述
description: “业务案例”子选项卡包含项目的财务字段。 为了使某些财务字段具有值，必须填写商业案例的相应区域。
author: Alina
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 2%

---

# 业务案例财务字段概述

“业务案例”子选项卡包含项目的财务字段。 为了使某些财务字段具有值，必须填写商业案例的相应区域。  

以下项目财务字段显示在“业务案例”中：

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
   <td> <p>根据项目的记分卡显示项目的对齐方式。 高百分比值表示项目与组织宗旨和目标完全一致。 <br>有关使用记分卡的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">创建记分卡</a>.</p> <p>此字段显示在“业务案例汇总”区域中。 </p> </td> 
  </tr> 
  <tr> 
   <td>预算成本</td> 
   <td> <p>项目启动时与项目关联的预计总成本。</p> <p>项目的预算成本按以下公式计算：<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront使用资源计划员中的预算小时数来计算预算人工成本。<br>有关计算预算成本的详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">计算预算成本</a>. </p> <p>此字段显示在“业务案例汇总”区域中。</p> </td> 
  </tr> 
  <tr> 
   <td>预算支出成本</td> 
   <td> <p>项目所有费用的预算成本。 </p> <p>这由以下公式计算：</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>有关计算费用的详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">管理项目费用 </a>.</p> <p>此字段显示在“费用”区域中。</p> </td> 
  </tr> 
  <tr> 
   <td>预算劳力成本</td> 
   <td> <p>与分配给完成项目工作的资源关联的成本。</p> <p>项目的预算人工成本按以下公式计算：<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code></p> <p>Workfront使用资源计划员中的预算小时数来计算预算人工成本。<br>有关计算预算人工成本的详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">了解项目的预算人工成本和预算工时</a>.</p> <p>此字段显示在“业务案例”的“资源预算”区域中。 </p> </td> 
  </tr> 
  <tr> 
   <td>费用计划成本</td> 
   <td> <p>这与预算费用成本相同。 </p> <p>注意：费用计划成本与项目的计划成本不同。 “费用计划成本”是按项目费用的计划金额计算的，而“计划成本”是按项目的计划小时数计算的。 </p> <p>此字段显示在“费用”区域中，用于每项费用。</p> </td> 
  </tr> 
  <tr> 
   <td>净值</td> 
   <td> <p>这是在计算项目收益并排除成本后项目的预计总价值。</p> <p>项目的净值按以下公式计算：<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>。 <br></p> <p>有关计算净值的详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">计算净值</a>.<br></p> <p>此字段显示在“业务案例汇总”区域中。</p> </td> 
  </tr> 
  <tr> 
   <td>计划收益</td> 
   <td>此项目完成时对贵组织的货币利益的手动估计。 它可以是任意金额的货币，并且它特定于您以及您管理的每个项目。 计划福利不能具有负值。 此字段显示在“业务案例汇总”区域，并可在“业务案例”的“项目信息”区域进行编辑。 </td> 
  </tr> 
  <tr> 
   <td>潜在风险成本</td> 
   <td> <p>这是项目所有风险的潜在成本。 </p> <p>使用以下公式计算此值：</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>有关项目风险的详细信息，请参阅 <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">在项目中创建和编辑风险</a>.</p> <p>此字段显示在“业务案例汇总”区域中。</p> </td> 
  </tr> 
  <tr> 
   <td>潜在风险</td> 
   <td> <p>在“业务案例摘要”中，这是所有风险（如果它们应发生）的成本金额，基于它们的概率。 例如，如果“风险”的潜在成本为$100，发生概率为10%，则“潜在风险”为$10。 “业务案例概要”中的潜在风险按以下公式计算：</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> 所有风险。 </p> </td> 
  </tr> 
  <tr> 
   <td>风险降低成本</td> 
   <td> <p>针对您估计的风险的缓解计划的成本可能会在项目中发生。<br>有关项目风险的详细信息，请参阅 <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">在项目中创建和编辑风险</a>.</p> <p>此字段显示在项目中指定的每个风险的“风险”区域中。</p> </td> 
  </tr> 
  <tr> 
   <td>一种风险的潜在成本</td> 
   <td> <p>当项目所界定的风险实际发生时（不论其可能性）的估计财务成本。 </p> <p>这是一个手动更新的字段，用于显示“业务案例”的“风险”区域中的每个风险。 </p> </td> 
  </tr> 
  <tr> 
   <td>风险总潜在成本</td> 
   <td> <p>这是项目实际发生时确定的所有风险的估计财务成本总额。 </p> <p>这由以下公式计算：</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>它在“业务案例”的“风险”区域的标题旁显示为货币编号。</p> </td> 
  </tr> 
 </tbody> 
</table>
