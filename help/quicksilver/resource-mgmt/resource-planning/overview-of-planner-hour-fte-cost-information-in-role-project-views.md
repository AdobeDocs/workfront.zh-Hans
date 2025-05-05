---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: 资源计划员的项目和角色视图中的小时数、FTE和成本信息概览
description: 资源规划者的“项目”和“角色”视图中的小时数、FTE和成本信息概览
author: Lisa
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: c9e77e11fafbf224639289977783e95ccb45a9e2
workflow-type: tm+mt
source-wordcount: '3086'
ht-degree: 0%

---

# 资源规划者的“项目”和“角色”视图中的小时数、FTE和成本信息概览

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

为资源在项目中必须完成的工作编制预算，是资源规划者的主要功能。 您可以查看资源的可用时间，并将其时间分配给分配给分配它们的项目。

有关资源规划者中预算资源的信息，请参阅[使用项目和角色视图的资源规划者中的预算资源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

本文介绍了在资源规划者中开始预算资源之前需要了解的一些关键概念。

## 预算资源概述

使用资源规划程序对资源进行预算时，请考虑以下事项：

* 您可以通过指定资源可用于完成项目工作的小时数、FTE或成本金额来预算资源的分配。 在预算资源的时间或成本时，资源的可用小时数、FTE或成本将按预算金额减少。 因此，要为其编制预算的项目之后的项目的可用小时数、FTE或成本额会减少这些项目中的这些用户和职责。

  >[!IMPORTANT]
  >
  >您可以按15年的周期预算您的资源。 如果您为工期超过15年的项目预算资源，预算信息可能不准确。

* 您可以在资源规划者中显示的任何时间范围内为资源预算小时数、FTE或成本，这与项目的时间表无关。 例如，如果您想指出您的资源在项目时间线中可能不可用（这些资源与计划小时数关联），但在其他时间可能可用，则可以通过为计划小时数为零的时间范围编列预算来实现此目的，前提是这些资源在计划小时数变为可用时可用。 在执行此操作后，您可以手动更改项目的时间表以符合您的资源可用性。

  >[!NOTE]
  >
  >我们建议您首先为工作角色或用户手动预算小时数、FTE或成本。 只有在您确定计划小时数、FTE或成本金额应始终与预算小时数、FTE或成本相匹配时，您才可以使用自动选项为项目和资源预算时间。\
  >有关在资源规划者中使用自动预算选项的信息，请参阅[使用Adobe Workfront资源规划者查看资源可用性和分配](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md)一文中的“自动预算项目和角色”一节。

* 预算FTE或成本与预算小时数相同，其中Adobe Workfront使用FTE和成本值而不是预算资源的小时数。

  有关了解如何在资源规划程序中计算成本的更多信息，请参阅[在资源规划程序中计算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)。

* 在资源规划程序中为资源分配预算可通过以下方式完成：

   * 手动

     或

   * 通过使用&#x200B;**按项目查看**&#x200B;和&#x200B;**按角色查看**&#x200B;视图中的项目和角色选项，自动进行查看。

  有关详细信息，请参阅使用项目和角色视图的资源规划者中的[预算资源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)。

* 当用户更改工作角色，删除、停用或从资源池中删除时，为角色预算的小时数不会更改，并且会重新分配给角色中的其余用户。 如果没有用户再与工作角色关联，则角色的预算小时数将变为零。

有关项目和角色选项的更多信息，请参阅本文中的[了解资源规划者](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner)中的小时数、FTE和成本值部分。

## 了解资源规划者中的小时数、FTE和成本值 {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

在资源预算以及更新资源规划程序中的预算小时数信息之前，您必须熟悉以下概念

* **计划小时数、FTE或成本**：需要按任务和问题上的定义完成的工作。
* **可用小时数、FTE或成本**：根据与用户关联的时间表，用户或工作角色可用的工作时间。

此信息显示在每个资源（用户或角色）和每个项目的资源规划者中。

有关项目的项目和角色视图中所显示内容的信息，请参阅文章[资源规划者导航概述](../../resource-mgmt/resource-planning/resource-planner-navigation.md)。

有关了解如何在资源规划程序中计算成本的信息，请参阅文章[在资源规划程序中计算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)。

>[!NOTE]
>
>按成本编制预算与按小时或约当全职人数编制预算相同，但您必须了解Workfront如何计算资源规划者的成本。
>
>有关如何在资源规划者中计算成本的信息，请参阅文章[在资源规划者中计算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)。

下表显示了应用项目或角色视图时资源规划程序中显示的分配和可用性信息。 您可以按小时数、FTE或成本查看此信息：

* [AVL （可用）列](#the-avl-available-column)
* [计划（计划）列](#the-pln-planned-column)
* [预算列](#the-bdg-budgeted-column)
* [变量（变量）列](#the-var-variance-column)
* [NET列](#the-net-column)

### AVL （可用）列 {#the-avl-available-column}

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
   <td> <p>在所选时间范围内，项目中的所有用户根据其计划可工作的总小时、FTE或成本。 </p> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>在所选时间范围内，与此角色关联的所有用户根据其计划以及他们在该特定角色中的<strong>FTE可用性百分比</strong>而可工作的总小时数、FTE或成本。 </p> <p>请考虑以下事项： </p> 
    <ul> 
     <li>如果没有用户与工作角色关联，则工作角色的可用小时数值为零。 </li> 
     <li>如果用户与主要工作角色关联，但该角色的FTE可用性<strong>百分比</strong>为0%，则工作角色可用小时值为零。</li> 
     <li>如果用户与其他角色相关联，并且角色的FTE可用性的<strong>百分比</strong>为0%，则其他角色不会列在资源规划者中，并且用户仅显示在其主要角色下。</li> 
    </ul> <p>有关工作角色的FTE可用性<strong>百分比</strong>的详细信息，请参阅文章<a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户配置文件</a>。</p> <p>有关如何在“资源规划者”中计算工作角色可用性的更多信息，请参阅<a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">计算资源规划者中用户和角色的小时和FTE的概述</a>中的“计算资源规划者中工作角色的可用小时和FTE”一节。</p> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> <p>在所选时间范围内，用户根据其计划可工作的小时数、FTE或成本。 此数字减去与以下项关联的小时数：</p> 
    <ul> 
     <li>计划例外</li> 
     <li>用户的空闲时间</li> 
     <li>为其他项目预算的小时数。 </li> 
    </ul> <p>用户的可用小时数、FTE或成本会根据以下内容进行更改： </p> 
    <ul> 
     <li>如何根据系统级别的资源管理首选项计算其计划和FTE。<br><p>有关计算用户和工作角色可用性的详细信息，请参阅文章<a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">计算资源规划者</a>中用户和角色的小时和FTE的概述。</p>
     有关在Workfront中配置资源管理首选项的详细信息，请参阅<a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置资源管理首选项</a></li> 
    </ul> 
    <ul> 
     <li><strong>项目计划优先级</strong>（如果用户已编列工作预算）。<br>有关项目计划优先级如何影响用户可用小时数的详细信息，请参阅<a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">资源规划者导航概述</a>。 </li> 
    </ul> <p>如果计划停用用户，则停用日期后天内的可用小时数、FTE或成本为零。 <br>有关停用用户的详细信息，请参阅文章<a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新激活用户</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>



### PLN （计划）列 {#the-pln-planned-column}

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
   <td> <p>项目下列出的所有工作角色或用户（包括在<strong>无角色</strong>或<strong>无用户</strong>分区中）在所选时间范围内计划小时数、FTE或成本的总数，显示在项目的“项目详细信息”选项卡中。 </p> <p><b>注释</b>

手动调整每日用户分配可能会更改资源规划者中的每周、每月或每季度计划小时数值。 您可以使用工作负载均衡器手动调整任务和问题的每日用户分配。 有关详细信息，请参阅<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作负载均衡器</a>中管理用户分配。</p> </td>
</tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>在所选时间范围内分配给角色的所有任务的已计划小时数总计。 </p> <p><strong>无角色</strong>部分将显示与任务关联的计划小时数，这些任务或者未分配、已分配给团队（其小时数列在<strong>无用户</strong>部分中），或者已分配给未与工作角色关联的用户。 </p> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> <p>在所选时间范围内分配给特定角色中用户的所有任务的已计划小时数。 </p> <p><strong>无用户</strong>部分将显示与未分配或分配给团队的任务关联的计划小时数。 </p> </td> 
  </tr> 
 </tbody> 
</table>

查看计划小时数时，请考虑以下事项：

* 尽管在“项目”和“角色”视图的资源规划者中看不到有关任务分配的信息，但已计划小时数金额来自项目中任务的已计划小时数。
* 对于分配给任务的每个资源，计划小时数平均分配给任务持续时间内的每一天。 任务持续时间基于任务计划开始日期和完成日期，包括该时间段内的每个日历日。\
  在向用户或项目分配计划小时数时，Workfront会考虑用户或项目的计划。 在这种情况下，计划小时数平均分配到任务持续时间内的每一天，不包括周末、休息日和计划例外。\
  例如，如果按周显示资源规划者，并且您的任务在项目上跨越多周，则每周的计划小时数取决于该周内的多少天是任务持续时间的一部分。 在按月或季度显示资源规划者时以及任务跨越多个月或季度时，其工作方式类似。\
  周末日、计划例外和休息日将从此分配中排除。
* 计算每个资源的计划小时数时，包括以下任务类别：

   * 分配给资源池、职位角色或项目团队中的用户的任务\
     如果将任务分配给团队，则其分配将显示在&#x200B;**无角色**&#x200B;和&#x200B;**无用户**&#x200B;分区下。 您可以看到与团队关联的计划小时数，但无法预算小时数，因为没有任何角色或用户与任务关联。

   * 未分配任务

* 资源规划者中的计划小时数不包括与以下项关联的计划小时数：

   * 父任务
   * 分配给无资源池用户的任务
   * 问题，当&#x200B;**包括来自问题的小时数**&#x200B;设置禁用时。

* 如果任务持续时间为零，则计划小时数不会显示在资源规划者中。
* 未显示与已停用用户关联的计划小时数。

### BDG（预算）列 {#the-bdg-budgeted-column}

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
   <td> <p>一个手动条目，用于估计在选定的时间范围内为项目预算多少小时、FTE或成本。 </p> <p>在“项目”视图中，您为项目预算的小时数将分配给项目下列出的工作角色。 每个角色的已计划小时数决定了如何将预算小时数分配给角色。 预算小时数将分配给具有较高计划小时数的角色。 </p> <p>在“角色”视图中，您为项目预算的小时数未分配给项目中的角色或用户。 </p> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>一个手动条目，用于估计在选定的时间范围内为角色预算多少小时。 </p> <p>如果没有用户与工作角色关联，则无法估计工作角色的预算小时数。 </p> <p>在“角色”视图中，您为角色配置的小时数将分配给角色下列出的项目。 每个项目的计划小时数金额确定如何将预算小时数分配给项目。 预算小时数已分配给具有较高计划小时数值的项目。</p> <p>在项目视图中，您为角色预算的小时数未分配给项目或与角色关联的用户。 </p> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> <p>一个手动条目，用于估计在选定的时间范围内为用户预算多少小时。 </p> <p> <p><b>注释</b>   您可以为未分配给任务，但与项目中的资源池关联的用户估计预算小时数，因为这些用户也会出现在资源规划者中。 但是，如果它们未分配给任务，则其计划小时数应为零。 </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

使用预算小时数时，请考虑以下事项：

* 只有在您具有对资源管理和财务数据的编辑访问权限以及项目的管理财务权限时，才能预算资源。

  有关预算资源所需的访问权限的信息，请参阅文章[在Adobe Workfront中预算资源所需的访问权限](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)。

* 默认情况下，对于所有资源和所有项目，资源规划者中的预算小时数为零。
* 您可以手动估算用户和角色的预算小时数，也可以使用项目或工作角色&#x200B;**更多**&#x200B;菜单中的链接之一来根据计划小时数更新它们。\
  有关项目和角色选项的更多信息，请参阅本文中资源规划者[&#128279;](#Budget)的项目和角色视图中的小时概述、FTE和成本信息。

* 您可以为预算小时、FTE或成本的最小时间段是一周。 您不能为一天预算小时数、FTE或成本。
* 预算小时数平均分配给分配给分配给任务的每个资源的任务持续时间内的每一天。 任务持续时间基于任务计划开始日期和完成日期，包括该时间段内的每个日历日。

  在向用户或项目分配预算小时数时，Workfront会考虑用户或项目的计划。 在这种情况下，预算小时数平均分配到任务持续时间内的每一天，周末除外，但包括休假和计划例外。

  例如，如果按周显示资源规划者，并且您的任务跨越多周，则每周的预算小时数取决于该周内的天数是任务持续时间的一部分。 周末会从此分发中排除。 在按月或季度显示资源规划者时以及任务跨越多个月或季度时，其工作方式类似。

* 您可以通过选择预算小时数作为新报告的报告对象来报告预算小时数。

  有关可以在Workfront中报告哪些对象的信息，请参阅[了解Adobe Workfront中的对象](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)一文中的“报告对象”部分。

  有关生成预算小时数报表的信息，请参阅文章[报告：预算小时数](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md)。

* 之前为以后被停用用户预算的小时数不显示。

  请注意，项目的预算劳力成本仍然包括资源规划者中已停用的用户的预算小时数。

  例如：如果将某个角色分配给两个用户，并且添加了预算小时数（每个用户20小时，合计40小时），然后手动为该角色设置总计，则停用资源规划者中的其中一个用户会导致在计算中不再考虑其小时数（将总计减少到20小时）。 但是，项目预算正确地保留了角色手动设置的总数，因此停用的用户的小时数仍包含在计算中（仍为40小时）。

### VAR（差异）列 {#the-var-variance-column}

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
   <td> <p>小时数、FTE或成本差异显示您是否具有足够的预算小时数来完成项目的所有计划小时数。 </p> <p>使用以下公式计算项目小时、FTE或成本差异：</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>小时数、FTE或成本差异显示您是否具有足够的预算小时数、FTE或成本可供角色完成分配到的计划小时数。 </p> <p>角色小时数、FTE或成本差异使用以下公式计算：</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> <p>小时数、FTE或成本差异显示您是否有足够的预算小时数供用户完成分配给他们的计划小时数。 </p> <p>使用以下公式计算用户小时数、FTE或成本差异：</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>当小时、FTE或成本差异以红色显示时，您估计的预算小时数少于需要完成的实际工作的计划小时数。 在这种情况下，预算小时数可能不足以完成工作。

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
     <p>项目“净小时数”、“约当全职人数”或“成本”可能显示以下任一项： </p> 
     <ul> 
      <li> <p>项目的可用时间或成本与预算时间或成本之间的差额：</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>启用NET计算设置中的使用计划(PLN)值时，项目可用时间或成本与计划时间或成本之间的差异： </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>提示</b></p>        
  <p>仅当自定义显示选定项目部分中的视图时，才应用此选项。</p>
  <p>有关详细信息，请参阅<a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >使用Adobe Workfront资源规划者审查资源可用性和分配</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> 
    <div> 
     <p>“净小时数”、“FTE”或“成本”角色可以显示以下任一项： </p> 
     <ul> 
      <li> <p>角色的可用时间或成本与预算时间或成本之间的差额：</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>在NET计算设置中启用使用计划(PLN)值时，角色的可用时间或成本与计划时间或成本之间的差值：</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>提示</b> <span>

仅当您自定义显示选定项部分中的视图时，才应用此选项。</span> </p> <p><span>有关详细信息，请参阅</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">使用Adobe Workfront资源规划者审查资源可用性和分配</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>用户</td> 
   <td> 
    <div> 
     <p>用户“净小时数”、“约当全职人数”或“成本”可能显示以下任一项： </p> 
     <ul> 
      <li> <p>可用时间或成本与用户的预算时间或成本之间的差额：</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>启用NET计算设置中的使用计划(PLN)值时，可用时间或成本与用户的计划时间或成本之间的差值：</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>提示</b> <span>

仅当您自定义显示选定项部分中的视图时，才应用此选项。</span> </p> <p><span>有关详细信息，请参阅</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">使用Adobe Workfront资源规划者审查资源可用性和分配</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>当“净小时数”、“约当全职人数”或“成本”显示为红色时，没有足够的“可用时间”或“预算”覆盖与工作相关的预算或计划时间或成本。 在这种情况下，资源会过度分配。

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
