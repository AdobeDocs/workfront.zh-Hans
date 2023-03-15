---
content-type: overview
navigation-topic: business-case-and-scorecards
title: 业务案例领域概述
description: 本文介绍了项目业务案例的相关领域。
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 2%

---

# 业务案例领域概述

本文介绍了项目业务案例的相关领域。

有关为项目创建业务案例的信息，请参阅 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

您的Adobe Workfront管理员或组管理员必须先启用“业务案例”中的所有部分，然后才能在项目中看到这些部分，“项目信息”部分除外。 默认情况下，项目信息部分处于启用状态。

有关启用“业务案例”区域的更多信息，请参阅  [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

以下是项目“业务案例”中的各个方面：

* 项目信息
* 目标
* 费用
* 资源预算
* 风险
* 记分卡
* 自定义表单
* 商业论证摘要

## 项目信息

的 **项目信息** “业务案例”区域不可由Workfront管理员配置。 所有项目在“业务案例”中都有一个“项目信息”区域。 

“业务案例”的“项目信息”部分包含项目实际开始之前的基本信息。

请考虑编辑以下字段：

* **描述**:为项目指定描述。
* **项目所有者**

   默认情况下，创建项目的用户也是项目所有者。 您可以编辑此字段并指示另一个活动用户为项目所有者。

* **项目赞助者**

   考虑添加项目所有者以外的其他人作为项目的赞助人。 保荐机构受理《业务案例》的批准。 

* **Portfolio**:为项目指定Portfolio。 您必须创建Portfolio并将其置于 **活动** 才能在此下拉菜单中进行选择。

   有关组合的更多信息，请参阅 [PortfolioAdobe Workfront概述](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

   有关创建Portfolio的更多信息，请参阅 [创建项目组合](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **计划福利**:估计在完成此项目时计划为贵组织提供的货币利益。 它可以是任意金额的货币，并且必须是正值。 例如10,000美元。
* **状态**:默认情况下，项目请求的状态设置为 **构思**.

   如果将“状态”(Status)更改为“构思”(Idea)或“计划”(Planning)以外的任何内容，则 **提交** 按钮会从“业务案例摘要”区域中消失，您无法再提交“业务案例”进行审批。 

* **固定开始日期**:指定项目开始的日期。
* **固定结束日期**:指定项目结束的日期。

   >[!NOTE]
   >
   >业务案例的固定起始日期和终止日期不会影响项目的计划起始日期和完成日期。 这些日期表示项目创建者请求的项目理想开发日期。 相反，项目的计划起始日期和计划完成日期会显示项目的计划时间表，时间表基于项目中的任务。

## 目标

目标可定义项目的目标。 此区域在“业务案例”中默认启用，但Workfront管理员可能选择不显示。 此字段会按优先顺序显示目标。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
您可以为组织创建未与项目的单个业务案例关联的战略目标。 您必须有权访问Adobe Workfront目标才能创建战略目标。 然后，您可以将它们与业务案例之外的项目连接起来。 有关使用Workfront目标创建目标的信息，请参阅 [Adobe Workfront目标概述](../../../workfront-goals/goal-management/wf-goals-overview.md).

对于要在Portfolio优化程序中获得分数的项目，定义目标是可选的。 此部分是“业务案例”中的唯一可选部分。 “业务案例”的所有其他部分必须先完成，然后项目才能在“Portfolio优化程序”中得分。 在创建目标时，您可以指示目标的优先级。

有关目标的更多信息，请参阅  [创建业务案例目标](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## 费用

开支指在项目期间可能发生的非人工成本。 此区域在“业务案例”中默认启用，但Workfront管理员可能选择不显示。 

您在“业务案例”中输入的任何费用也会在项目的“费用”标签中按“计划费用”输入。

费用会影响项目的以下字段：

* 预算成本
* 净值

有关预算成本和净值的详细信息，请参阅 [业务案例财务字段概述](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

有关费用的详细信息，请参阅  [管理项目费用](../../../manage-work/projects/project-finances/manage-project-expenses.md) .

您的Workfront管理员可以设置自定义费用类型。

有关创建自定义费用类型的详细信息，请参阅 [创建自定义费用类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md). 

## 资源预算

您可以在“业务”案例的“资源预算”区域中执行以下操作：

* 将资源池与项目关联。
* 在项目级别对资源进行预算。

项目上资源的预算小时数显示在“业务案例”的“资源预算”区域，从而生成项目的预算人工成本。 默认情况下，“业务案例”的此区域处于启用状态。

有关“业务案例”中项目预算资源的详细信息，请参阅 [业务案例中的预算资源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![](assets/business-case-sp-selected-with-choose-button-350x121.png)

查看业务案例的“资源预算”部分时，请考虑以下事项：

* 您可以在此处使用以下工具对资源信息进行预算：

   * 资源计划员

      有关信息，请参阅 [使用资源计划员在业务案例中预算资源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * 方案计划员(如果您的公司为Adobe方案计划员购买了附加许可证)

      有关更多信息，请参阅 [使用方案计划员在业务案例中预算资源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

      方案规划器仅在新的Adobe Workfront体验中可用，并且需要额外的许可证。 有关Workfront方案规划器的信息，请参阅 [方案计划员概述](../../../scenario-planner/scenario-planner-overview.md).

* 此处显示的信息也显示在系统层资源计划员或方案计划员中。 

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* 在对资源进行预算后，如果角色与“每小时成本”费率关联，则项目的“预算人工成本”将显示在“资源预算”区域中。 预算的人工成本以项目的币种显示。

   >[!IMPORTANT]
   预算的人工成本是与项目中的角色相关的成本，而不是与用户相关的成本。 用户的所有预算人工成本的总和可能等于或不等于与用户关联的职务职责的预算人工成本。 

   有关预算人工成本的详细信息，请参阅 [业务案例财务字段概述](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

   有关创建任务角色并将“每小时成本”费率与其关联的详细信息，请参阅 [创建和管理作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## 风险

风险是可能阻止项目按时或按预算完成的因素。 定义这些因素对于Portfolio经理或项目赞助商在项目批准上做出有根据的决定至关重要。 此区域在“业务案例”中默认启用，但Workfront管理员可能选择不显示。

您可以将潜在成本与您定义的风险关联，以防它们发生。 项目的风险成本会影响项目的净值。 

有关项目净值的详细信息，请参阅 [业务案例财务字段概述](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

有关创造风险的更多信息，请参阅  [在项目中创建和编辑风险](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

您的Workfront管理员可以设置自定义风险类型。

有关创建和编辑自定义风险类型的更多信息，请参阅 [编辑和创建风险类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## 记分卡

记分卡可测量项目的对齐情况。 此区域在“业务案例”中默认启用，但Workfront管理员可能选择不显示。

有关将记分卡应用到项目并生成对齐分数的更多信息，请参阅 [将记分卡应用于项目并生成对齐分数](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

要应用记分卡，您的Workfront管理员必须创建一个记分卡。 的 **记分卡** 除非创建记分卡，否则不会显示“业务案例”区域。

有关创建记分卡的更多信息，请参阅  [创建记分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## 自定义表单

在定义业务案例时，您可以将自定义Forms附加到项目。 在“业务案例”中，默认情况下未启用此区域。 Workfront管理员必须将其启用，才能在业务案例中显示。

有关启用“业务案例”区域的详细信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

要应用自定义表单，您的Workfront管理员必须首先创建自定义表单。

有关创建自定义表单的更多信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

您可以使用自定义表单来收集未显示在“业务案例”其他字段中的其他信息。

有关应用自定义表单的更多信息，请参阅 [将自定义表单附加到业务案例](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## 商业论证摘要

* [业务案例摘要概述](#overview-of-the-business-case-summary)
* [导出业务案例](#export-the-business-case)

### 业务案例摘要概述 {#overview-of-the-business-case-summary}

您可以在业务案例摘要面板的右上角的商业案例摘要面板中查看主要项目财务以及项目是否与记分卡保持一致。

您无法编辑“业务案例摘要”。 这只是项目状态的概览，因为它与财务字段和记分卡相关。 \
 

“业务案例摘要”中显示以下字段：

* 项目净值
* 项目预算成本
* 潜在风险成本
* 计划的福利
* 对齐分数

有关这些字段的更多信息，请参阅 [业务案例财务字段概述](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### 导出业务案例 {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

您可以将业务案例导出到PDF文件，以备您打印该文件或以更精简的格式将其附加到电子邮件。 

有关信息，请参阅 [导出项目的业务案例](../../../manage-work/projects/define-a-business-case/export-business-case.md).

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
--&gt;
