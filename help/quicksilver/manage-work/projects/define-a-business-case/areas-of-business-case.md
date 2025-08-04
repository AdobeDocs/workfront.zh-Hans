---
content-type: overview
navigation-topic: business-case-and-scorecards
title: 业务案例的领域概述
description: 本文介绍了项目的业务案例的方面。
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: 14b6b9c4a184131cfdc33b6156c578218ed9119a
workflow-type: tm+mt
source-wordcount: '1553'
ht-degree: 1%

---

# 业务案例领域概述

<!-- Audited: 4/2025 -->

本文介绍了项目的业务案例的方面。

有关为项目创建业务案例的信息，请参阅[为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

您的Adobe Workfront管理员或组管理员必须启用业务案例中的所有部分，然后才能在项目中显示它们，但项目信息部分除外。 默认情况下，项目信息部分处于启用状态。

有关启用业务案例区域的更多信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)一文中的业务案例部分。

以下是项目的业务案例中的部分：

* 项目信息
* 目标
* 费用
* 资源预算
* 风险
* 记分卡
* 自定义表单
* 商业论证摘要

## 项目信息

业务案例的项目信息部分包括项目实际开始之前的项目的基本信息。

所有项目在Business Case中都有一个带有预设字段的项目信息区域，这意味着Workfront管理员无法配置哪些字段出现在此区域中。

请考虑编辑以下字段：

* **描述**：为您的项目添加描述。

* **项目所有者**：默认情况下，创建项目的用户也是项目所有者。 编辑此字段以选择另一个活动用户作为项目所有者。

* **项目发起人**：选择将作为项目发起人的活动用户。 发起人获得业务案例的批准。

* **Portfolio**：为项目选择一个Portfolio。 您必须先创建Portfolio并将其置于活动状态，之后才能在此下拉菜单中选择它。

  有关项目组合的详细信息，请参阅Adobe Workfront中的[Portfolio概述](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md)。

  有关创建项目组合的详细信息，请参阅[创建项目组合](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)。

* **计划收益**：估算完成此项目后贵组织计划的货币收益。 它可以为任意数量的货币，并且必须是正值（例如$10,000）。

* **状态**：默认情况下，项目请求的状态设置为“想法”。 如果将“状态”更改为“想法”或“计划”以外的任何状态，则“提交”按钮将从“业务案例汇总”区域消失，并且您无法再提交业务案例以供审批。

* **固定开始日期**：指定您希望项目开始的日期。

* **固定结束日期**：指定您希望项目结束的日期。

  >[!NOTE]
  >
  >业务案例的固定开始和结束日期不会影响项目的计划开始和完成日期。 这些日期表示项目创建者请求的理想项目开发日期。 相反，项目的计划开始日期和计划完成日期显示项目的计划时间线，该时间线基于项目的任务。

## 目标

目标定义了项目的目标。 默认情况下，此区域在业务案例中处于启用状态，但Workfront管理员可能选择不显示该区域。 此字段按优先级显示目标。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
>
>您可以为组织创建未与项目的单个业务案例关联的战略目标。 您必须有权访问Adobe Workfront目标才能创建战略目标。 然后，您可以将他们与其业务案例之外的项目联系起来。 有关使用Workfront目标创建目标的信息，请参阅[Adobe Workfront目标概述](../../../workfront-goals/goal-management/wf-goals-overview.md)。

对于要在Portfolio优化器中接收分数的项目，可自行选择定义目标。 本节是业务案例中唯一的可选部分。 必须先完成业务案例的所有其他部分，然后才能在Portfolio Optimizer中为项目评分。 您可以在创建目标时指定目标的优先级。

有关详细信息，请参阅[创建业务案例目标](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md)。

## 费用

费用代表在项目期限内可能产生的非人工成本。 默认情况下，此区域在业务案例中处于启用状态，但Workfront管理员可以选择不显示该区域。

您在业务案例中输入的任何费用也作为计划费用在项目的“费用”选项卡上输入。

费用会影响项目中的以下字段：

* 预算成本
* 净值

Workfront管理员可以设置自定义费用类型。

有关预算成本和净值的详细信息，请参阅[业务案例财务字段概览](../../../manage-work/projects/define-a-business-case/business-case-finances.md)。

有关费用的详细信息，请参阅[管理项目费用](../../../manage-work/projects/project-finances/manage-project-expenses.md)。

有关创建自定义费用类型的详细信息，请参阅[创建自定义费用类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md)。

## 资源预算

您可以在Business case的“资源预算”区域中执行以下操作：

* 将资源池与项目关联。
* 在项目级别预算您的资源。

项目资源的预算小时数显示在业务案例的资源预算区域，并生成项目的预算劳力成本。 此区域默认处于启用状态。

有关业务案例中项目预算资源的详细信息，请参阅业务案例中的[预算资源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

<!--![Business case resource budgeting](assets/business-case-sp-selected-with-choose-button-350x121.png)-->

查看业务案例的资源预算编制部分时，请考虑以下事项：

* 您可以使用以下工具在此预算资源信息：

   * 资源规划者

     有关信息，请参阅使用资源规划程序[的业务案例中的](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md)预算资源。

   * 场景规划器

     有关详细信息，请参阅使用场景规划器[的业务案例中的](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md)预算资源。

     Scenario Planner仅在新的Adobe Workfront Experience中可用，并且需要额外的许可证。 有关Workfront Scenario Planner的信息，请参阅[Scenario Planner概述](../../../scenario-planner/scenario-planner-overview.md)。

* 此处显示的信息也会显示在系统层的资源规划者或方案规划者中。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* 在预算您的资源后，如果角色与每小时成本费率关联，则项目的预算劳力成本显示在资源预算区域。 预算劳力成本以项目的货币显示。

  >[!IMPORTANT]
  >
  >预算劳力成本是与项目中的角色关联的成本，而不是与用户关联的成本。 用户的所有预算劳力成本的总和可能等于或不等于与用户关联的工作角色的预算劳力成本。

  有关预算劳力成本的更多信息，请参阅[业务案例财务字段概览](../../../manage-work/projects/define-a-business-case/business-case-finances.md)。

  有关创建工作角色以及将每小时成本费率与其关联的详细信息，请参阅[创建和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

## 风险

风险是可能会阻止项目按时或按预算完成的因素。 定义这些因素对于Portfolio经理或项目发起人做出有关项目批准的教育性决定非常重要。 默认情况下，此区域在业务案例中处于启用状态，但Workfront管理员可以选择不显示该区域。

您可以将潜在成本与正在定义的风险关联，以防发生风险。 风险成本影响项目的净值。

您的Workfront管理员可以设置自定义风险类型。

有关项目净值的详细信息，请参阅[业务案例财务字段概览](../../../manage-work/projects/define-a-business-case/business-case-finances.md)。

有关创建风险的更多信息，请参阅[创建和编辑项目中的风险](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)。

有关创建和编辑自定义风险类型的详细信息，请参阅[编辑和创建风险类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md)。

## 记分卡

记分卡用于测量项目的对齐方式。 默认情况下，此区域在业务案例中处于启用状态，但Workfront管理员可以选择不显示该区域。

要应用记分卡，您的Workfront管理员必须首先创建记分卡。 除非创建记分卡，否则将不会显示业务案例的记分卡区域。

有关将记分卡应用于项目并生成一致性分数的详细信息，请参阅[将记分卡应用于项目并生成一致性分数](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)。

有关创建记分卡的更多信息，请参阅[创建记分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)。

## 自定义表单

您可以在定义业务案例时将自定义Forms附加到项目。 此区域在业务案例中默认未启用，Workfront管理员必须启用它才能在业务案例中显示它。

要应用自定义表单，您的Workfront管理员必须首先创建一个。

您可以使用自定义表单收集未在业务案例的其他字段中显示的附加信息。

有关启用业务案例区域的详细信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

有关创建自定义表单的详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

有关应用自定义表单的详细信息，请参阅[将自定义表单附加到业务案例](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md)。

## 商业论证摘要

* [业务案例摘要概述](#overview-of-the-business-case-summary)
* [导出业务案例](#export-the-business-case)

### 业务案例摘要概览 {#overview-of-the-business-case-summary}

您可以在位于业务案例右上角的业务案例摘要面板中查看主项目财务摘要以及项目是否与记分卡对齐。

业务案例摘要只是项目状态的快速视图，因为它与财务字段和记分卡相关，并且无法编辑。

业务案例汇总中将显示以下字段：

* 项目净值
* 项目预算成本
* 潜在风险成本
* 计划的收益
* 一致性分数

有关这些字段的更多信息，请参阅[业务案例财务字段概述](../../../manage-work/projects/define-a-business-case/business-case-finances.md)。

### 导出业务案例 {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

如果您需要打印商业案例文件，可以将其导出到PDF文件，或以更精简的格式将其附加到电子邮件中。

有关信息，请参阅[导出项目的业务案例](../../../manage-work/projects/define-a-business-case/export-business-case.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To export a Business Case:</p>
<ol>
<li value="1">Go to the <strong>Business Case</strong> area of a project. </li>
<li value="2"> <p>In the<strong>Business Case Summary</strong> area, click <strong>Export</strong>.<br>A PDF file is downloaded to your computer. The file contains all areas of the Business Case in an easy to read format.</p> <p> <img src="assets/bc-summary-exported-350x160.png" alt="BC_Summary_exported.png" style="width: 350;height: 160;"> </p> </li>
<li value="3">(Optional) You can attach the PDF file to an email, or print it.&nbsp;</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>You can export the Business Case to a PDF file, in case you need to print it or attach it to an email in a more condensed format.&nbsp; The file contains all areas of the Business Case in an easy to read format.</p>
<p>For information about how to export the Business Case, see <a href="../../../manage-work/projects/define-a-business-case/export-business-case.md" class="MCXref xref">Export the Business Case of a project </a></p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and will replace the info above, when the standalone arrticle is live >> Becky!)</p>
-->
</div>

