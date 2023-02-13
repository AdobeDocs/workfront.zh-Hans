---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: 资源计划员的“项目”和“职责”视图中的工时、FTE和成本信息概览
description: 资源计划员的“项目”和“职责”视图中的工时、FTE和成本信息概览
author: Alina
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '2958'
ht-degree: 0%

---

# 资源计划员的“项目”和“职责”视图中的工时、FTE和成本信息概览

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

资源计划员的主要功能是将资源用于他们必须在项目中完成的工作。 您可以查看资源的可用时间，并将其时间分配到已分配资源的项目。

有关资源计划员中预算资源的信息，请参阅 [使用“项目”和“职责”视图在资源计划员中预算资源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

本文介绍了在开始在资源计划器中预算资源之前您需要了解的一些关键概念。

## 预算资源概述

使用资源计划器对资源进行预算时，请考虑以下事项：

* 您可以通过指定资源可用于完成项目工作的小时数、FTE或成本金额来对资源分配进行预算。 在预算资源的时间或成本时，资源的可用小时数、FTE或成本将按预算金额减少。 因此，在您为其预算的项目之后，这些用户和角色在这些项目上的可用小时数、FTE或成本金额会减少。

   >[!IMPORTANT]
   >
   >您可以将资源预算为15年。 如果您对持续时间超过15年的项目的资源进行预算，则预算信息可能不准确。

* 您可以为资源在资源计划器中显示的任意时间范围预算小时数、FTE或成本，而与项目的时间表无关。 例如，如果您想要指明资源可能在项目时间轴期间不可用（在该时间轴中，资源与计划时间关联），但可能在另一时间可用，则可以通过将资源预算到计划时间为零的时间范围（如果计划时间为零，则当资源可用时）来执行此操作。 在执行此操作后，您可以手动更改项目的时间轴以匹配资源可用性。

   >[!NOTE]
   >
   >我们建议您首先为工作角色或用户手动预算小时数、FTE或成本。 只有在您确定计划小时数、FTE或成本的金额应始终与预算小时数、FTE或成本相匹配时，才能使用自动选项对项目和资源的预算时间进行预算。\
   >有关在资源计划员中使用预算的自动选项的信息，请参阅文章中的“自动预算项目和职责”一节 [使用Adobe Workfront资源计划员复查资源可用性和分配](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* 预算FTE或成本与预算小时数相同，其中Adobe Workfront使用FTE和成本值，而不是您预算的资源的小时数。

   有关了解如何在资源计划器中计算成本的详细信息，请参阅 [在资源计划器中计算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* 在资源计划器中为您的资源分配预算的方法如下：

   * 手动

      或

   * 自动，通过在 **按项目查看** 和 **按角色查看** 视图。
   有关更多信息，请参阅 [使用“项目”和“职责”视图在资源计划员中预算资源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* 当用户更改作业角色、从资源池中删除、停用或删除时，为角色编入预算的小时数不会更改，并且这些小时数会重新分配给角色中的其余用户。 如果用户不再与职务角色关联，则该角色的预算工时将变为零。

有关项目和角色选项的更多信息，请参阅部分 [了解资源计划员中的“小时”、“FTE”和“成本”值](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) 在本文中。

## 了解资源计划员中的“小时”、“FTE”和“成本”值 {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

在对资源进行预算编制以及在资源计划器中更新预算小时数信息之前，您必须熟悉以下概念

* **计划小时数、FTE或成本**:需要根据任务和问题的定义完成的工作。
* **可用小时数、FTE或成本**:根据与用户关联的计划，用户或作业角色可以工作的时间。

此信息显示在资源计划器中，用于每个资源（用户或角色）和每个项目。

有关项目视图和项目角色视图中显示内容的信息，请参阅文章 [资源计划员导航概述](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

有关了解如何在资源计划器中计算成本的信息，请参阅文章 [在资源计划器中计算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>按成本编制预算与按小时或FTE编制预算相同，但您必须了解Workfront如何为资源计划员计算成本。
>
>有关如何在资源计划器中计算成本的信息，请参阅文章 [在资源计划器中计算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

下表显示了在应用“项目”或“职责”视图时在资源计划器中显示的分配和可用性信息。 您可以按小时、FTE或成本查看此信息：

* [AVL（可用）列](#the-avl-available-column)
* [“PLN（已计划）”列](#the-pln-planned-column)
* [BDG（预算）栏](#the-bdg-budgeted-column)
* [“变量（差异）”列](#the-var-variance-column)
* [NET列](#the-net-column)

### AVL（可用）列 {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>显示者</strong> </td> 
   <td><strong>描述</strong> </td> 
  </tr> 
  <tr> 
   <td>项目 </td> 
   <td> <p>在选定的时间范围内，项目中所有用户都可以根据其计划工作的小时数、FTE或成本总和。 </p> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>与此角色关联的所有用户都可以根据其计划和其工作时间来工作的小时、FTE或成本总数 <strong>FTE可用性百分比</strong> 对于该特定角色，对于选定的时间范围。 </p> <p>请考虑以下事项： </p> 
    <ul> 
     <li>如果没有用户与作业角色关联，则作业角色的“可用小时数”值为零。 </li> 
     <li>如果用户与主作业角色关联，但 <strong>FTE可用性百分比</strong> 对于角色为0%，作业角色“可用小时数”值为零。</li> 
     <li>如果用户与“其他角色”关联，则 <strong>FTE可用性百分比</strong> 对于角色为0%，“其他角色”未列在“资源计划器”中，并且用户仅显示在其“主要角色”下。</li> 
    </ul> <p>有关 <strong>FTE可用性百分比</strong> 有关职务角色，请参阅文章 <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户的配置文件</a>.</p> <p>有关如何在资源计划器中计算任务角色可用性的详细信息，请参阅文章中的“计算资源计划器中任务角色的可用小时数和FTE”一节 <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">资源计划员中用户和角色的小时数和FTE计算概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> <p>根据用户的计划，在选定的时间范围内，用户可以工作的小时数、FTE或成本。 此数字减去与以下项目关联的小时数：</p> 
    <ul> 
     <li>计划例外</li> 
     <li>用户的关闭时间</li> 
     <li>为其他项目编列的小时数。 </li> 
    </ul> <p>用户的可用小时数、FTE或成本会根据以下情况进行更改： </p> 
    <ul> 
     <li>如何根据系统级别的“资源管理首选项”来计算其计划和FTE。<br>有关计算用户和作业角色可用性的详细信息，请参阅文章 <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">资源计划员中用户和角色的小时数和FTE计算概述</a>.</li> 
    </ul> 
    <ul> 
     <li>the <strong>项目计划优先级</strong>，则为用户编入工作预算。<br>有关项目计划优先级如何影响用户可用小时数的详细信息，请参阅 <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">资源计划员导航概述 </a>. </li> 
    </ul> <p>如果用户已计划停用，则停用日期后天的可用小时数、FTE或成本为零。 <br>有关取消激活用户的更多信息，请参阅文章 <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新激活用户</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### “PLN（已计划）”列 {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>显示者</strong> </td> 
   <td><strong>描述</strong> </td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td> <p>项目下列出的所有工作角色或用户的计划小时数、FTE或成本总和，包括 <strong>无角色</strong> 或 <strong>无用户</strong> 部分，并显示在项目的“项目详细信息”选项卡中。 </p> <p><b>注释</b>

人工调整每日用户分配可以更改资源计划员中的每周、每月或每季计划小时值。 您可以使用工作负载平衡器手动调整任务和问题的每日用户分配。 有关更多信息，请参阅 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作负载平衡器中管理用户分配</a>.</p> </td>
</tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>在选定的时间范围内，分配给角色的所有任务中的计划小时数总和。 </p> <p>的 <strong>无角色</strong> 部分将显示与未分配、分配给团队(其小时在 <strong>无用户</strong> 部分)，或分配给未与作业角色关联的用户。 </p> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> <p>在选定的时间范围内，计划小时数来自分配给特定角色用户的所有任务。 </p> <p>的 <strong>无用户</strong> 部分将显示与未分配或分配给团队的任务关联的计划小时数。 </p> </td> 
  </tr> 
 </tbody> 
</table>

查看计划时间时，请考虑以下事项：

* 虽然在“项目”和“职责”视图的“资源计划员”中看不到有关任务分配的信息，但“计划小时数”的金额来自项目中任务的“计划小时数”。
* 计划小时数在任务持续时间内的每一天均分配给分配给它们的每个资源。 任务持续时间基于任务计划起始日期和完成日期，并包括该时间段内的每个日历日。\
   Workfront在向用户或项目分发计划时间时，会考虑用户或项目的计划。 在这种情况下，计划小时数在任务持续时间内平均分配给每天，但不包括周末、超时天数和计划例外。\
   例如，如果按周显示资源计划员，并且您有跨多个周的项目任务，则每周计划小时数取决于该周内有多少天是任务持续时间的一部分。 在按月或季度显示资源计划员以及任务跨越多个月或季度时，此功能的工作方式类似。\
   此分发中不包括周末日、计划例外和休息日。
* 在计算每个资源的计划时数时，包括以下各类任务：

   * 在项目的资源池、作业角色或团队中分配给用户的任务\
      如果任务被分配给团队，则其分配将显示在 **无角色** 和 **无用户** 中。 您可以看到与团队关联的计划小时数，但无法预算小时数，因为没有角色或用户与任务关联。

   * 未分配的任务

* 资源计划员中的计划小时数不包括与以下项目关联的计划小时数：

   * 父任务
   * 分配给没有资源池的用户的任务
   * 问题， **包含问题后的小时数** 设置处于禁用状态。

* 如果任务持续时间为零，则计划小时数不会显示在资源计划器中。
* 与已停用用户关联的计划小时数不显示。

### BDG（预算）栏 {#the-bdg-budgeted-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>显示者</strong> </td> 
   <td><strong>描述</strong> </td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td> <p>用于估算选定时间范围内项目预算的小时数、FTE或成本的人工输入。 </p> <p>在“项目”视图中，您为项目预算的小时数将分配给项目下列出的作业角色。 每个角色的计划小时数确定如何将预算小时数分配给角色。 预算小时数将分配给具有较高计划小时数值的角色。 </p> <p>在“角色”视图中，您为项目预算的小时数不会分配给角色或项目用户。 </p> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>用于估算选定时间范围内某个角色的预算小时数的人工录入。 </p> <p>如果没有用户与职务角色关联，则无法估计职务角色的预算小时数。 </p> <p>在“角色”视图中，您为角色预算的小时数将分配给角色下列出的项目。 每个项目的计划小时数确定如何将预算小时数分配给项目。 预算小时数将分配给计划小时数值较高的项目。</p> <p>在“项目”视图中，您为角色预算的小时数不会分配给项目或与角色关联的用户。 </p> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> <p>用于估算选定时间范围内用户预算小时数的人工录入。 </p> <p> <p><b>注意</b>   您可以估计未分配给任务，但与项目上的资源池关联的用户的预算小时数，因为这些用户也显示在资源计划器中。 但是，如果未将计划小时数分配给任务，则其计划小时数应为零。 </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

使用预算小时数时，请考虑以下事项：

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* 只有在具有对项目的“编辑”资源管理和财务数据的访问权限以及“管理财务”权限时，才能对资源进行预算。

   有关预算资源所需访问权限的信息，请参阅文章 [在Adobe Workfront获得预算资源所需的资源](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* 默认情况下，资源计划员中所有资源和所有项目的预算小时数为零。
* 您可以人工估算用户和角色的预算小时数，也可以使用项目或职务角色中的链接之一 **更多** 菜单，以根据计划小时数更新它们。\
   有关项目和角色选项的更多信息，请参阅部分 [资源计划员的“项目”和“职责”视图中的工时、FTE和成本信息概览](#Budget) 在本文中。

* 您可以预算小时数、FTE或成本的最小时间段为一周。 您不能预算一天的小时数、FTE或成本。
* 在任务持续期内，预算小时数平均分配给分配给它们的每个资源。 任务持续时间基于任务计划起始日期和完成日期，并包括该时间段内的每个日历日。\
   Workfront在向用户或项目分发预算小时数时，会考虑用户或项目的计划。 在这种情况下，预算小时数在任务持续时间（不包括周末）内平均分配给每天，但包括超时和计划例外。\
   例如，如果按周显示资源计划员，并且您的任务跨越多周，则每周预算小时数取决于该周内有多少天是任务持续时间的一部分。 此分发中不包括周末日。 在按月或季度显示资源计划员以及任务跨越多个月或季度时，此功能的工作方式类似。

* 通过选择“已编入预算的小时”作为新报表的报表对象，可以报告“已编入预算的小时数”。\
   有关可以在Workfront中报告哪些对象的信息，请参阅文章中的“报告对象”一节 [了解Adobe Workfront中的对象](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
   有关生成预算小时报表的信息，请参阅文章 [报表：预算小时数](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* 以前为后来被停用的用户编列的小时数不会显示。

### “变量（差异）”列 {#the-var-variance-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>显示者</strong> </td> 
   <td><strong>描述</strong> </td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td> <p>“小时”、“FTE”或“成本差异”显示您是否有足够的预算小时数来完成项目的所有计划小时数。 </p> <p>项目小时数、FTE或成本差异使用以下公式计算：</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>“小时”、“FTE”或“成本差异”显示您是否具有足够的预算小时数、FTE或成本，以便角色完成分配给它的计划小时数。 </p> <p>使用以下公式计算“角色小时数”、“FTE”或“成本差异”：</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> <p>“小时”、“FTE”或“成本差异”显示用户是否有足够的预算小时数来完成分配给他们的计划小时数。 </p> <p>使用以下公式计算“用户小时数”、“FTE”或“成本差异”：</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>当“小时”、“FTE”或“成本差异”以红色显示时，您预计的“预算小时数”少于需要完成的实际工作的“计划小时数”。 在这种情况下，预算小时数可能不足以完成工作。

### NET列  {#the-net-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>显示者</strong> </td> 
   <td><strong>描述</strong> </td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td> 
    <div> 
     <p>项目净工时数、FTE或成本可能显示以下任一值： </p> 
     <ul> 
      <li> <p>项目的可用时间或成本与预算时间或成本之间的差额：</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>启用NET计算设置中的“使用计划(PLN)”值时，项目的可用时间或成本与计划时间或成本之间的差值： </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>笔尖</b></p>        
  <p>仅当您在显示选定项目部分中自定义视图时，才应用此选项。</p>
  <p>有关更多信息，请参阅 <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >使用Adobe Workfront资源计划员复查资源可用性和分配</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> 
    <div> 
     <p>“净小时数”、“FTE”或“成本”角色可能显示以下任一内容： </p> 
     <ul> 
      <li> <p>职责的可用时间或成本与预算时间或成本之间的差额：</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>启用NET计算设置中的“使用计划(PLN)”值时，“可用时间”或“成本”与“计划时间”或“成本”之间的差值：</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>笔尖</b> <span>

仅当您在显示选定项目部分中自定义视图时，才应用此选项。</span> </p> <p><span>有关更多信息，请参阅</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">使用Adobe Workfront资源计划员复查资源可用性和分配</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>用户</td> 
   <td> 
    <div> 
     <p>用户净工时数、FTE或成本可能显示以下任一值： </p> 
     <ul> 
      <li> <p>用户的可用时间或成本与预算时间或成本之间的差额：</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>启用NET计算设置中的“使用计划(PLN)”值时，“可用时间”或“成本”与“计划时间”或“成本”之间的差值：</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>笔尖</b> <span>

仅当您在显示选定项目部分中自定义视图时，才应用此选项。</span> </p> <p><span>有关更多信息，请参阅</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">使用Adobe Workfront资源计划员复查资源可用性和分配</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**当NET小时数、FTE或成本以红色显示时，可用时间或预算不足，无法覆盖预算的时间或预算** 或与工作关联的计划时间或成本。 在这种情况下，资源会被过度分配。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the table below is ideal but it does not transfer to Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours, FTE, or Cost)</strong> </td>
<td><strong>Displayed by</strong> </td>
<td><strong>Description</strong> </td>
</tr>
<tr>
<td rowspan="3">AVL <br>(Available Hours, FTE, or Cost)</td>
<td>Project </td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users on the project are available to work according to their schedule, for the time frame selected. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users associated with this role are available to work according to their schedule and their <strong>Percentage of FTE Availability</strong> for that specific role, for the time frame selected. </p> <p>Consider the following: </p>
<ul>
<li>If no user is associated with a job role, then the value for the Available Hours for the job role is zero. </li>
<li>If a user is associated with a Primary Job Role, but the <strong>Percentage of FTE Availability</strong> for the role is 0%, the job role Available Hours value is zero.</li>
<li>If the user is associated with Other Roles and the <strong>Percentage of FTE Availability</strong> for the roles is 0%, the Other Roles are not listed in the Resource Planner and the user displays only under their Primary Role.</li>
</ul> <p>For more information about the <strong>Percentage of FTE Availability</strong> for a job role, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> <p>For more information about how the job role availability is calculated in the Resource Planner, see the section "Calculate the Available Hours and FTE for a job role in the Resource Planner" in the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>Hours, FTEs, or Cost that the user is available to work, according to their schedule, for the time frame selected. This number subtracts the hours associated with the following:</p>
<ul>
<li>schedule exceptions</li>
<li>time off of the user</li>
<li>hours budgeted for other projects. </li>
</ul> <p>The Available Hours, FTEs, or Cost for a user change according the following: </p>
<ul>
<li>how their schedule and FTE are calculated based on the Resource Management Preferences at the system level.<br>For more information about calculating user and job role availability, see the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</li>
</ul>
<ul>
<li>the <strong>Project Planning Priority</strong>, if the user is budgeted for work.<br>For more information about how Project Planning Priority affects the Available Hours of a user, see <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Resource Planner navigation overview </a>. </li>
</ul> <p>If the user is scheduled for deactivation, the Available Hours, FTEs, or Cost for the days after the deactivation date are zero. <br>For more information about deactivating users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </td>
</tr>
<tr>
<td rowspan="4">PLN <br>(Planned Hours, FTE, or Cost)</td>
<td>Project</td>
<td> <p>The total of the Planned Hours, FTEs, or Cost from all the job roles or users listed under the project, including in the <strong>No Role</strong> or <strong>No User</strong> sections, for the time frame selected, and as displayed in the Project Details tab of the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of the Planned Hours from all the tasks assigned to the role, during the time frame selected. </p> <p>The <strong>No Role</strong> section will show the Planned Hours associated with tasks that are either unassigned, assigned to teams (whose hours are listed in the <strong>No User</strong> section), or assigned to users who are not associated with a job role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Planned Hours from all the tasks assigned to the user in a specific role, during the time frame selected. </p> <p>The <strong>No User</strong> section will show the Planned Hours associated with tasks that are either unassigned or assigned to teams. </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<ul>
<li>Although you cannot see information about task allocations in the Resource Planner in the Project and Role views, the amount of Planned Hours comes from the Planned Hours on the tasks in the projects. </li>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks excluding weekends, time-off days, and schedule exceptions.<br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> The following categories of tasks are included in calculating the Planned Hours for each resource:
<ul>
<li> tasks assigned to users in Resource Pools, job roles, or teams on the project<br>If tasks are assigned to teams, their allocation will appear under <strong>No Role</strong> and <strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks. </li>
<li> unassigned tasks </li>
</ul></li>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>tasks assigned to users with no Resource Pools</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> </td>
</tr>
<tr>
<td rowspan="4"> BDG <br>(BudgetedHours, FTE, or Cost) </td>
<td>Project</td>
<td> <p>A manual entry to estimate how many hours, FTE, or Cost you budget for a project, for a selected time frame. </p> <p>In the Project view, the hours you budget for the project are distributed to the job roles listed under the project. The amount of Planned Hours for each role determines how the Budgeted Hours are distributed to the roles. The Budgeted Hours are distributed to the roles with higher Planned Hours values. </p> <p>In the Role view, the hours you budget for the project are not distributed to the roles or the users on the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>A manual entry to estimate how many hours you budget for a role, for a selected time frame. </p> <p>If no user is associated with the job role, you cannot estimate the Budgeted Hours for the job role. </p> <p>In the Role view, the hours you budget for the role are distributed to the projects listed under the role. The amount of Planned Hours for each project determines how the Budgeted Hours are distributed to the projects. The Budgeted Hours are distributed to the projects with higher Planned Hours values.</p> <p>In the Project view, the hours you budget for the role are not distributed to the projects or the users associated with the role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>A manual entry to estimate how many hours you budget for a user, for a selected time frame. </p> <p> <note type="note">  You can estimate the Budgeted Hours for users who are not assigned to tasks, but are associated with a Resource Pool on a project because these users also appear in the Resource Planner. Their Planned Hours should be zero, however, if they are not assigned to tasks.
</note> </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when working with Budgeted Hours:</p> <li>
<ul>
<li> <p>You can budget resources only when you have Edit access to Resource Management and Financial Data and Manage Finance permissions on the projects.</p> <p>For information about the access needed for budgeting resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this bullet: Duplicated below)</p>
</li>
</ul> </li>
<ul>
<li>By default, the Budgeted Hours in the Resource Planner are zero for all resources and for all the projects.</li>
<li>You can manually estimate the Budgeted Hours for users and roles, or you can use one of the links in the Project or Job Role <strong>More</strong> menus to update them according to the number of Planned Hours.<br>For more information about project and role options, see the section <a href="#Budget" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a> in this article.</li>
<li> The smallest period of time you can budget hours, FTE, or Cost for is a week. You cannot budget hours, FTE, or Cost for a day. </li>
<li> Budgeted Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time. <br>Workfront takes into account the schedule of the user or of the project when distributing Budgeted Hours to users or projects. In this case, Budgeted Hours are equally distributed to each day within the Duration of tasks excluding weekends, but including time-off and schedule exceptions. <br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks, the number of Budgeted Hours per week depends on how many days within that week are part of the task Duration. Weekend days are excluded from this distribution. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters. </li>
<li>You can report on Budgeted Hours, by selecting Budgeted Hour as your report object for a new report.<br>For information about what objects you can report on in Workfront, see the section "Report on objects" in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. <br>For information about building a Budgeted Hour report, see the article <a href="../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</li>
<li>Hours previously budgeted for users who were later deactivated do not display. <br></li>
</ul> </td>
</tr>
<tr>
<td rowspan="4">VAR <br>(Hour, FTE, or ,Cost Variance)</td>
<td>Project</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the project to accomplish all the Planned Hours for the project. </p> <p>The Project Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours, FTE, or Cost for the role to accomplish the Planned Hours assigned to it. </p> <p>The Role Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Hours, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the user to accomplish the Planned Hours assigned to them. </p> <p>The User Hours, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
When the Hours, FTE, or Cost Variance displays in red, you have estimated less Budgeted Hours than the Planned Hours of the actual work that needs to be completed. In this case, the Budgeted Hours might not be enough to complete the work.
</note> </td>
</tr>
<tr>
<td rowspan="4"> NET <br>(Net Hours, FTEs, or Cost) </td>
<td>Project</td>
<td>
<div>
<p>The project Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the project:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the project, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>Role</td>
<td>
<div>
<p>The role Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the role:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the role, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span class="preview"><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>User</td>
<td>
<div>
<p>The user Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the user:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the user, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
<span>When the NET Hours,&nbsp;FTE, or Cost display in red, there is not enough Available time or budget to cover either the Budgeted</span> or the Planned time or cost associated with the work. In this case, the resources are overallocated.
</note> </td>
</tr>
</tbody>
</table>
-->
