---
product-area: resource-management
navigation-topic: resource-utilization
title: 查看资源利用率信息
description: 您可以使用“利用率”报表查看资源的利用率。
author: Alina, Lisa
feature: Resource Management
exl-id: 785ee3e9-1b2d-4180-bc78-c41e71c5244d
source-git-commit: d2b62f2ec2f52c54129b342d68c336c782601242
workflow-type: tm+mt
source-wordcount: '7854'
ht-degree: 0%

---

# 查看资源利用率信息

{{highlighted-preview}}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is linked to the UI from the Utilization report. ALWAYS keep this information. DO NOT DELETE!!)</p>
-->

您可以使用“利用率”报表查看资源的利用率。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Vazgen's response about these hours ie below and he asked us to NOT document them:</p>
<p>It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours.</p>
<p>In some cases, like for Planned Hours, it takes them from Assignments</p>
<p>But Budgeted Hours come from projects.</p>
<p>And Actual Hours are their own object - Hour)</p>
</div>
-->

<!--
<p style="color: #dc143c;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This report displays information about the assignments on work items for projects in your environment, like Planned, Actual, and Budgeted Hours, FTE, or Cost.&nbsp;These are hours,&nbsp;FTE, or costs associated with the assignments and not with the tasks and issues themselves.(PRIVATE NOTE:&nbsp;Vazgen's response about these hours: It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours. In some cases, like for Planned Hours, it takes them from Assignments; But Budgeted Hours come from projects. And Actual Hours are their own object - Hour.)</p>
-->

## 访问要求

您必须具备以下条件才能访问利用率报告：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业或专业以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限访问以下内容：</p> 
    <ul> 
     <li> <p>资源管理 </p> </li> 
     <li> <p>项目</p> </li> 
     <li> <p>项目组合</p> </li> 
     <li> <p>项目群</p> </li> 
     <li> <p>财务数据（如果要按成本查看信息）</p> </li> 
    </ul> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看对项目、项目组合和项目的访问权限，以访问“资源”区域中的“利用率”部分</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>管理对项目的访问权限以访问项目的“利用率”部分</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have View access to the projects you want to view utilization information for as described in this section. If you are still unable to access this information, contact your Workfront administrator. (NOTE:&nbsp;replaced with above table)</p>
-->

以下各节介绍如何查看和使用利用率信息。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Prerequisites for accessing utilization information</h2>
<p>(NOTE: drafted, replaced with above table)</p>
<p>To access utilization information as described in this section, ensure that the following conditions are met:</p>
<ul>
<li>You have at least&nbsp;View access to the project, program, or portfolio for which you want to view the utilization information.</li>
<li>Your Workfront administrator must grant you at least View access to&nbsp;Financial&nbsp;Data in your Access Level to be able to view cost and revenue information in the Utilization report. The Workfront administrator must enable both View Role Billing & Cost Rates as well as View User Billing &&nbsp;Cost Rates when they grant you the View access to Financial Data. For information about granting access to&nbsp;Financial&nbsp;Data, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. </li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;drafted. No longer the case.) </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Reporting area. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Resourcing area. </p>
</li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is available by default in the Reporting area if the system administrator has not assigned a custom layout template to you. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is available by default in the Resourcing area if the system administrator has not assigned a custom layout template to you. </p>
</li>
</ul>
</div>
-->

## 利用率报表概览 {#overview-of-the-utilization-report}

通过使用利用率报表，您可以在单个报表中查看项目、项目群或项目组合的进度、成本或收入。 您还可以将收入与成本进行比较。

您可以在“资源分配”区域中查看“利用率”报告，以显示多个项目中的利用率，也可以在一个项目级别查看它，以显示与该项目关联的单个资源（工作角色和用户）的利用率。

有关访问和使用利用率报告的信息，请参见 [使用利用率报告跟踪进度、成本和收入](#track-progress-cost-and-revenue-with-the-utilization-report) 章节。

* [跟踪小时数（进度）](#track-hours-progress)
* [跟踪成本](#track-cost)
* [跟踪收入](#track-revenue)
* [将收入与计划成本和实际成本进行比较](#compare-revenue-against-planned-and-actual-costs)

### 跟踪小时数（进度） {#track-hours-progress}

您可以通过查看预算和计划小时数与实际小时数的比较来跟踪进度。

在跟踪项目、项目群或项目组合的进度时，任务和问题的进度都包含在利用率报告中。

在跟踪小时数时，“利用率”报表中提供了以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>查看小时数时的列标题</strong> </th> 
   <th><strong>功能</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>预算小时</strong> </td> 
   <td scope="col"> <p>包含的项目上的总预算小时数。 您可以查看所包含项目整个生命周期的总预算小时数，也可以仅查看指定日期范围内的总预算小时数（您可以指定单独的周或月）。 </p> <p>预算小时数由业务案例或资源规划者的新资源预算编制区域中的可用信息填充<em>.</em></p> <p>预算小时数显示在利用率报表的以下任意行中：</p> 
    <ul> 
     <li> 预算小时数在利用率报告中按工作角色和单个用户汇总如下：<br><strong>个人用户：</strong> 在利用率报告中汇总了每个用户的预算小时数。 这些预算小时数与用户在所包含项目上分配的任务和问题相关联。 （您可以展开相应工作角色的行，以查看具有该工作角色的用户列表。）<br><strong>工作角色：</strong> 预算小时数按工作角色汇总在利用率报告中。<br>预算小时数由于以下任意方案显示在特定工作角色中： 
     <li>工作角色被定义为分配给与预算小时数关联的任务或问题的用户的主要工作角色。 </li> 
       <li>在查看单个项目的利用率信息时，无论任务或问题中没有分配、分配给另一个用户而没有分配工作角色、分配给另一个用户具有不同的工作角色，还是分配了另一个团队，都会使用分配了小时数的用户的工作角色。</li> 
       <li>查看多个项目、项目群或项目组合的利用率信息时，仅当为项目中的任务或问题分配角色时，才使用分配了小时数的用户的工作角色。 </li> 
       <li>工作角色已分配给与预算小时数关联的任务或问题，分配给任务或问题的用户没有在系统中定义的工作角色。</li> 
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><strong>未分配小时</strong>：当预算小时数与任务或问题关联，并且没有分配给任务或问题的用户或角色时，预算小时数显示在未分配小时数部分的利用率报告中。<br>仅当项目上的小时数与此描述匹配时，以及在按项目查看利用率报告或从项目查看利用率报告时，才会显示此部分。 </p> <p>仅当项目上的小时数与此描述匹配时，以及在按项目查看利用率报告或从项目查看利用率报告时，才会显示此部分。 </p> </li> 
    </ul> <p>有关预算小时数的详细信息，请参阅 <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">了解项目的预算劳力成本和预算小时数</a> 文章。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>计划小时</strong> </td> 
   <td scope="col"> <!-- Yay, no errors, warnings, or alerts! -->

<p>
与每个任务和问题的工作分配相关联的已包含项目上的已计划小时数。 您可以查看所包含项目整个生命周期中项目上所有分配的总计划小时数，也可以仅查看指定日期范围内的总计划小时数（您可以指定单独的周或月）。 
</p>
<p>
<strong>笔尖 </strong>
</p>
<p>
持续时间为0的项目的计划小时数未考虑在内。 
</p>
<p>
利用率报表中的已计划小时数会考虑已计划小时数是否已跨任务或问题的持续时间重新分配。 
</p>
<p>
当使用工作负载均衡器修改了用户每日小时分配时，如果在利用率报告中选择的日期仅包含任务或问题持续时间的一部分，则利用率报告中的数据可能会受到影响。 
</p>
<p>
有关修改用户分配的信息，请参见 <a href="../workload-balancer/manage-user-allocations-workload-balancer.md">在工作负载均衡器中管理用户分配</a>.


</p>
<p>
计划小时数显示在利用率报表的以下任意行中：
</p>
<ul>

<li>在利用率报表中，按工作角色和单个用户汇总的已计划小时数如下所示： 
<ul>

<li><strong>个人用户</strong>：在利用率报告中为每个用户汇总计划小时数。 这些已计划小时数与已包含项目中分配给用户的任务和问题相关联。 （您可以展开相应工作角色的行，以查看具有该工作角色的用户列表。）

<li><strong>工作角色</strong>：在单个项目的利用率报告中，按工作角色汇总计划小时数。<br>由于以下任何情况，计划小时数显示在特定工作角色中：  
<ul>

<li>工作角色被定义为分配给与计划小时数关联的任务或问题的用户的主要工作角色。

<li>在查看单个项目的利用率信息时，与工作角色关联的小时数不会显示在以下方案中的工作角色：   
<ul>

<li>任务或问题上没有分配

<li>用户未分配工作角色

<li>用户被分配了不同的工作角色

<li>已将团队分配给任务或问题
</li>   
</ul>

<li>查看多个项目、项目群或项目组合的利用率信息时，仅当为项目中的任务或问题分配角色时，才使用分配了小时数的用户的工作角色。 查看多个项目的利用率报告时，工作角色小时数未单独显示。

<li>工作角色被分配给与计划小时数相关联的任务或问题，并且分配给任务或问题的用户没有在系统中定义的工作角色。
</li>  
</ul>

<li><strong>未分配小时</strong>：当计划小时数与任务或问题关联并且未向任务或问题分配用户或角色时，计划小时数显示在利用率报告的“未分配小时数”部分中。仅当项目上的小时数与此描述匹配以及查看单个项目的利用率报告时，才会显示此部分。 <br>有关计划小时数的详细信息，请参见 <a href="../../manage-work/tasks/task-information/planned-hours.md">计划小时数概述</a>.
</li> 
</ul>
</li> 
</ul> </td> 
  </tr> 
  <tr> 
   <td><strong>实际小时数</strong> </td> 
   <td> <p> 在任务、问题和 <span>在项目上和</span> 对于包含的项目。 您可以查看所包含项目在整个生命周期中的总实际小时数，也可以仅查看指定日期范围内的总实际小时数（您可以指定单独的周或月）。 </p> <p>警告：利用率报告包括记录到项目的小时数、子代任务、问题和至少具有一个分配的父代任务。 它不包括已记录到无分配的父任务的小时数。 我们建议您不要将父任务用作工作任务，而只将子任务分配给资源。 </p> <p>实际小时数显示在利用率报表的以下任意行中：</p> 
    <ul> 
     <li> 在项目的利用率报告中，按工作角色和单个用户汇总实际小时数，如下所示：<br><strong>个人用户：</strong> 实际小时数显示在利用率报表中记录小时数的用户的行中。 （您可以展开相应工作角色的行，以查看具有该工作角色且已记录小时数的用户列表。）<br><strong>工作角色：</strong> 用户记录的与这些角色关联的实际小时数汇总在相应工作角色行的利用率报告中。<br>实际小时数由于以下任意方案显示在特定工作角色中： 
      <ul> 
       <li>工作角色被定义为记录小时数的用户的主要工作角色。</li> 
       <li>任务或问题上没有分配</li> 
       <li>分配了另一个用户，但未分配工作角色</li> 
       <li>另一个用户被分配了不同的工作角色</li> 
       <li> <p>已分配团队。</p> </li> 
      </ul></li>  
     <p>如果记录小时数的用户没有与其配置文件关联的工作角色，则用于利用率报告的工作角色是分配给记录了小时数的任务或问题的工作角色，或与任务或问题的主要所有者关联的工作角色。 </p> 
     <li><strong>其他小时：</strong> 实际小时数显示在利用率报告的其他小时数部分中，即记录小时数的用户的行中。<br>当记录小时数的用户未在系统中定义工作角色时，小时数将显示在此部分中。<br>仅当项目中的小时数与此描述匹配时，才会显示此部分。 </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>预算差异（用于小时）</strong> </td> 
   <td> <p>总预算小时数减去所包含项目的总实际小时数。 您可以查看所包含项目整个生命周期的预算差异合计，也可以仅查看指定日期范围内的预算差异合计（您可以指定单个周或月）。 </p> <p>如果该值为正，则以绿色显示。 这表示总预算小时数大于实际小时数。</p> <p>如果该值为负，则以红色显示。 这表示总预算小时数小于实际小时数。</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>计划差异（用于小时）</strong> </td> 
   <td> <p>总计划小时数减去所包含项目的总实际小时数。 您可以查看所包含项目整个生命周期的计划差异合计，也可以仅查看指定日期范围内的计划差异合计（您可以指定单个周或月）。</p> <p>如果该值为正，则以绿色显示。 这表示总计划小时数大于实际小时数。</p> <p>如果该值为负，则以红色显示。 这表示总计划小时数小于实际小时数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 跟踪成本 {#track-cost}

您可以通过查看预算成本和计划成本与实际成本的比较来跟踪成本。

在跟踪项目、项目群或项目组合的成本时，“利用率”报告中的信息来自任务。 任务中的成本信息始终可在“利用率”报表中找到。 根据任务的成本类型计算任务成本。 有关任务的成本类型的信息，请参阅中的“修改单个任务的成本类型” [跟踪成本](../../manage-work/projects/project-finances/track-costs.md).

您可以通过以下方式在“利用率”报表中显示成本信息：

* 对于给定的周或月，或者对于整个项目、项目群或项目组合。
* 按角色或个人，用于项目。

利用率报表中使用的币种由项目上设置的币种确定。 有关如何调整项目货币的信息，请参阅 [更改项目货币](../../manage-work/projects/project-finances/change-project-currency.md).

在跟踪成本时，“利用率”报表中提供了以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>查看成本时的列标题</strong> </th> 
   <th> <p><strong>功能</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>预算成本</strong> </td> 
   <td scope="col"> <p>已包含项目的预算成本。 您可以查看所包含项目整个生命周期的总预算成本，也可以仅查看指定日期范围内的总预算成本（您可以指定单个周或月）。</p> <p>由于利用率报表中的预算成本侧重于按角色列出的成本，因此该计算与Workfront其他区域中的预算劳力成本相同。 有关如何计算预算劳力成本的信息，请参阅 <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">了解项目的预算劳力成本和预算小时数</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>计划成本</strong> </td> 
   <td scope="col"> <p>已包含项目的总计划成本。 您可以查看所包含项目整个生命周期的计划成本合计，也可以仅查看指定日期范围内的计划成本合计（您可以指定单个周或月）。</p> <p><span class="preview">请注意，对于周、月和季度视图，计划成本计算为在工作角色或用户的成本费率生效之时所选期间的平均值。</span></p><p>有关如何计算项目计划成本的信息，请参阅文章中的“Workfront如何计算计划成本、预算成本和实际成本”部分 <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>实际成本</strong> </td> 
   <td scope="col"> <p>包含的项目上的总实际成本。 您可以查看所包含项目整个生命周期的实际成本合计，也可以仅查看指定日期范围内的实际成本合计（您可以指定单个周或月）。</p> <p>有关如何计算项目实际成本的信息，请参阅本文中的“Workfront如何计算计划成本、预算成本和实际成本”部分 <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>预算差异（用于成本）</strong> </td> 
   <td scope="col"> <p>总预算成本减去所包含项目的总实际成本。 您可以查看所包含项目整个生命周期的预算差异合计，也可以仅查看指定日期范围内的预算差异合计（您可以指定单个周或月）。</p> <p>如果该值为正，则以绿色显示。 这表示总预算成本大于实际成本。</p> <p>如果该值为负，则以红色显示。 这表示总预算成本小于实际成本。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>计划差异（成本）</strong> </td> 
   <td> <p>总计划成本减去所包含项目的总实际成本。 您可以查看所包含项目整个生命周期的计划差异合计，也可以仅查看指定日期范围内的计划差异合计（您可以指定单个周或月）。 </p> <p>如果该值为正，则以绿色显示。 这表示总计划成本大于实际成本。</p> <p>如果该值为负，则以红色显示。 这表示总计划成本小于实际成本。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 跟踪收入 {#track-revenue}

您可以通过查看预算和计划收入与实际收入的比较来跟踪收入。

在跟踪项目、项目群或项目组合的收入时，“利用率”报表中仅包含来自任务的收入。

在跟踪收入时，“利用率”报表中提供了下表中的信息。

有关特定字段以及Workfront如何计算这些字段的信息，另请参阅以下文章：

* [跟踪成本](../../manage-work/projects/project-finances/track-costs.md)
* [开单和收入概览](../../manage-work/projects/project-finances/billing-and-revenue-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>查看收入时的列标题</strong> </th> 
   <th> <strong>功能</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>预算收入</strong> </td> 
   <td scope="col"> <p>总预算小时数乘以所包含项目中的角色记帐费率。 您可以查看所包含项目整个生命周期的总预算收入，也可以仅查看指定日期范围内的总预算收入（您可以指定单个周或月）。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>计划收入</strong> </td> 
   <td scope="col"> <p>利用率报表中的计划收入是与分配给项目任务的资源的计划小时数关联的收入。</p> <p>Workfront使用以下公式计算利用率报表的项目计划收入：</p> <p><code>Project Planned Revenue = SUM&nbsp;(All Tasks Planned Revenue)</code> </p> 
   <p><b>注释</b>
   <p>利用率报表中显示的项目计划收入与项目详细信息区域和项目报表中显示的计划收入不同。 </p> <p>项目详细信息区域中的计划收入反映任务收入以及项目的固定收入。 利用率报表中的计划收入仅显示与项目中的任务关联的计划收入。 </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p>如果项目有1个任务，时长为10小时，分配给顾问时长为$20小时费率，并且项目有$100的固定收入，则利用率报表显示计划收入$200（与任务小时数关联的计划收入）。 项目详细信息部分显示$300（任务的计划收入和项目的固定收入）。 </p> 
     </div> <p>有关利用率报告之外的任务和项目计划收入的详细信息，请参阅 <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">开单和收入概览</a>.</p> </p> <p>利用率报表计算和显示所包含项目的计划收入的方式考虑到了在任务上设置的收入类型。 </p> <p>根据项目中每个任务的收入类型，存在以下方案： </p> <p><strong>固定收入：</strong> 无论任务分配如何，始终使用在任务上指定的固定金额计算任务收入。</p> <p><b>重要</b>

与Workfront的其他区域不同，“利用率”报表通过将固定收入平均除以任务的计划小时数，来计算固定收入任务的计划收入。 </p> <p>例如，一项任务的收入为$200。 如果任务中有4个计划小时数，则每小时费用为$50。 该工作流在用户和角色级别上分发。 此分布对于利用率报表是唯一的。</p> <p><b>注释</b>

如果您有“固定收入”任务，并且该任务没有计划小时数，则收入不会显示在利用率报表中，因为没有办法将其分配给小时数。 如果您在任务中具有固定收入且没有分配的计划小时数，则收入显示为未分配收入。 </p> <p><strong>角色小时：</strong> 使用为特定角色设置的记帐费率乘以与该角色关联的已计划小时数来计算任务收入。 Workfront使用以下公式：</p> <p><code>角色小时计划收入= SUM（所有任务中角色的计划小时数） *角色开单费率</code></p><p><span class="preview"><b>注意：</b> 公式中的开单小时费率会考虑费率的任何日期有效更改。</span></p>   <p><strong>用户小时：</strong> 任务收入的计算方法是使用为特定用户设置的记帐费率，乘以该用户关联的已计划小时数。 Workfront使用以下公式：</p> <p><code>用户小时计划收入= SUM（所有任务中用户的计划小时数）*用户记帐费率</code> </p> <p><span class="preview"><b>注意：</b> 公式中的开单小时费率会考虑费率的任何日期有效更改。</span></p> <p><b>角色小时或用户小时加固定</b> </p> <p><b>重要</b>

与Workfront的其他区域不同，“利用率”报表通过将固定收入平均除以任务的计划小时数来计算计划收入。 </p> <p>存在以下情况： </p>
<ul>
<li> <p><strong>角色小时加固定：</strong> 任务收入的计算方法是使用为特定角色设置的记帐费率，乘以与该角色关联的已计划小时数。 此外，任务中指定的固定数量会添加到角色比率。 Workfront使用以下公式：</p> <p><code>角色小时加固定计划收入= [SUM（所有任务中角色的计划小时数）*角色记帐费率] + SUM（任务的上限或固定数量/任务的计划小时数）</code> </p> </li>
</ul>
<ul>
<li> <p><strong>用户小时加固定：</strong> 为特定用户设置的记帐费率，乘以该用户在该任务上计划的小时数。 此外，任务中指定的固定数量会添加到用户费率。 Workfront使用以下公式：</p> <p><code>用户小时加固定计划收入= [SUM（所有任务中用户的计划小时数）*用户记帐费率] + SUM（任务的上限或固定数量/任务的计划小时数）</code> </p> </li>
</ul> <p><b>受限角色或用户小时</b> </p> <p><b>重要</b>

与Workfront的其他区域不同，如果计划收入超过上限，则超过上限金额的金额被视为固定收入。 计划收入的计算方法是：将固定收入平均除以任务的计划小时数，然后加上上限金额和角色或用户小时收入。 <br></p> <p>存在以下情况： </p>
<ul>
<li> <p><strong>受限角色小时：</strong> 任务按照角色每小时计费，但它们具有您可以指定的上限金额。 Workfront使用以下公式：</p> <p><code>具有最高计划收入的角色小时= [SUM（所有任务和问题中角色的计划小时数）*角色记帐费率] +任务的上限数量+ SUM（超过任务上限数量/计划小时数的数量）</code> </p> </li>
</ul>
<ul>
<li> <p><strong>受限用户小时：</strong> 任务按用户小时计费，但它们具有您可以指定的上限金额。 Workfront使用以下公式： </p> <p><code>计划收入上限的用户小时= [SUM（所有任务中用户的计划小时数）*用户记帐费率] +任务的上限数量+ SUM（超过任务上限数量/计划小时数的数量）</code> </p> </li>
</ul> <p>有关计算计划收入时考虑哪个角色或用户的更多信息，请参阅 <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">开单和收入概览</a>.</p> </td>
</tr> 
  <tr> 
   <td><strong>实际收入</strong> </td> 
   <td> <p>实际收入是与任务的实际小时数关联的收入 <span>和项目</span>. 有关实际收入的更多信息，请参阅文章中的“跟踪收入金额”部分 <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">开单和收入概览</a>.</p>

<p>根据任务上设置的收入类型，“利用率”报表计算所包含项目实际收入的方式有所不同，如下所示：</p> <p><strong>固定收入：</strong> 无论任务分配如何，始终使用在任务上指定的固定金额计算任务收入。</p> <p><b>重要</b>

与Workfront的其他区域不同，“利用率”报表通过将固定收入平均除以任务记录的小时数来计算实际收入。 </p> <p> </p> <p>例如，一项任务的实际收入为$200。 如果任务中有4个实际小时，则每个小时将为$50。 该工作流在用户和角色级别上分发。 此分布对于利用率报表是唯一的。</p> <p><b>注释</b>

如果您有“固定收入”任务，并且该任务中没有实际小时数，则实际收入不会显示在利用率报表中，因为无法分配小时数。 </p> <p><strong>角色小时：</strong> 任务收入的计算方法是使用为特定职责设置的开单费率乘以实际小时数。</p> <p>Workfront使用以下公式：</p> <p><code>角色小时实际收入= SUM（所有任务中角色的实际小时数） *角色开单费率</code> </p> <p><span class="preview"><b>注意：</b> 公式中的开单小时费率会考虑费率的任何日期有效更改。</span></p> <p><strong>用户小时：</strong> 任务收入的计算方法是：使用为特定用户设置的记帐费率，乘以针对该用户的任务记录的小时数。 Workfront使用以下公式：</p> <p><code>用户小时实际收入= SUM（用户在所有任务中的实际小时数）*用户记帐费率</code></p> <p><span class="preview"><b>注意：</b> 公式中的开单小时费率会考虑费率的任何日期有效更改。</span></p> <p><b>角色或用户小时加固定</b> </p> <p><b>重要</b>

与Workfront的其他区域不同，“利用率”报表通过将固定收入平均除以任务记录的小时数来计算实际收入。 </p> <p>存在以下情况： </p>
<ul>
<li> <p><strong>角色小时加固定：</strong> 为特定角色设置的记帐费率，乘以该角色的用户针对任务记录的小时数。 此外，任务中指定的固定数量会添加到角色比率。 </p> <p>Workfront使用以下公式：</p> <p><code>角色小时加固定实际收入= [SUM（所有任务中角色的实际小时数）*角色记帐费率] + SUM（任务的上限或固定数量/任务的实际小时数）</code> </p> </li>
</ul>
<ul>
<li> <p><strong>用户小时加固定：</strong> 为特定用户设置的记帐费率，乘以该用户对该任务记录的小时数。 此外，任务中指定的固定数量会添加到用户费率。 </p> <p>Workfront使用以下公式：</p> <p><code>用户小时加固定实际收入= [SUM（所有任务中角色的实际小时数）*用户记帐费率] + SUM（任务的上限或固定数量/任务的用户小时数）</code> </p> </li>
</ul> <p><b>受限角色或用户小时</b> </p> <p><b>重要</b>

与Workfront的其他区域不同，如果计划收入超过上限，则超过上限金额的金额被视为固定收入。 计划收入的计算方法是：将固定收入平均除以任务的计划小时数，然后加上上限金额和角色或用户小时收入。 <br></p> <p>存在以下情况：</p>
<ul>
<li> <p><strong>受限角色小时：</strong> 任务按照角色每小时计费，但它们具有您可以指定的上限金额。 Workfront使用以下公式：</p> <p><code>具有最高实际收入的角色小时= [SUM（所有任务和问题中角色的实际小时数）*角色记帐费率] +任务的上限数量+ SUM（超过任务上限数量/实际小时数的数量）</code></p> </li>
</ul>
<ul>
<li> <p><strong>受限用户小时：</strong> 任务按用户小时计费，但它们具有您可以指定的上限金额。</p> <p> Workfront使用以下公式：</p> <p><code>实际收入上限的用户小时= [SUM（所有任务和问题中角色的实际小时数）*用户记帐费率] +任务的上限数量+ SUM（超过任务上限数量/实际小时数的数量）</code> </p> </li>
</ul>
<div>
<p><strong>项目收入</strong>：与项目记录的小时数关联的收入的计算考虑了记录时间的用户的主要工作角色的每小时计费数量。 我们不建议记录项目的时间。 </p>
<p><b>注释</b>

如果用户未与工作角色关联，或者如果主要角色的每小时记帐数为零，则Workfront使用用户的每小时记帐数金额计算实际收入。 如果用户档案中没有每小时计费金额，则实际收入为零。 </p>
</div> </td>
</tr> 
  <tr> 
   <td><strong>预算差异（收入）</strong> </td> 
   <td> <p>包含的项目中的总实际收入减去预算收入。<br>您可以查看所包含项目整个生命周期的预算差异合计，也可以仅查看指定日期范围内的预算差异合计（您可以指定单个周或月）。</p> <p>如果该值为正，则以绿色显示。 这表示总预算收入大于实际收入。</p> <p>如果该值为负，则以红色显示。 这表示总预算收入小于实际收入。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>计划差异（收入）</strong> </td> 
   <td> <p>总实际收入减去所包含项目的总计划收入。<br>您可以查看所包含项目整个生命周期的计划差异合计，也可以仅查看指定日期范围内的计划差异合计（您可以指定单个周或月）。 </p> <p>如果该值为正，则以绿色显示。 这表示总计划收入大于实际收入。</p> <p>如果该值为负，则以红色显示。 这表示总计划收入小于实际收入。</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--Note from the table about Actual revenue: 
     <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p>
    -->

<!--More notes from the table: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the note below is duplicated in this article: /Content/Manage work/Projects/Project Finances/billing-and-revenue-overview.html and in the glossary)</p>
   -->

### 将收入与计划成本和实际成本进行比较 {#compare-revenue-against-planned-and-actual-costs}

您可以查看计划或实际成本以及计划收入。 系统还会显示毛利(%)（毛利的计算方法为收入 — 成本/收入）。

在将收入与计划成本和实际成本进行比较时，“利用率”报表中提供了以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>查看收入与成本时的列标题（计划）</strong> </th> 
   <th> <strong>功能</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>计划成本</strong> </td> 
   <td scope="col"> 已包含项目的总计划成本。 您可以查看所包含项目整个生命周期的计划成本合计，也可以仅查看指定日期范围内的计划成本合计（您可以指定单个周或月）。 </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>计划收入</strong> </td> 
   <td scope="col"> <p>计划收入是指与任务的计划小时数关联的收入。 </p> <p>根据任务上设置的收入类型，“利用率”报表计算和显示所包含项目的计划收入的方式会有所不同，具体如下所述： <a href="#track-revenue" class="MCXref xref">跟踪收入</a> 章节。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>边距</strong> </td> 
   <td scope="col"> <p>利润百分比计算如下：</p> <p><code>Planned Revenue - Planned Cost / Planned Revenue * 100. </code></p> <p><b>注释</b>

如果计划收入等于0，则毛利显示为0。 </p> </td>
</tr> 
  <tr> 
   <td scope="col"> <p scope="col"><strong>查看收入与成本时的列标题（实际）</strong> </p>  </td> 
   <td scope="col"><p><strong>功能</strong></p></td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>实际成本</strong> </td> 
   <td scope="col"> <p>包含的项目上的总实际成本。 您可以查看所包含项目整个生命周期的实际成本合计，也可以仅查看指定日期范围内的实际成本合计（您可以指定单个周或月）。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>实际收入</strong> </td> 
   <td> <p>实际收入是与任务的实际小时数关联的收入。</p> <p>仅当任务标记为“完成”或“完成”（或与“完成”等同的状态）后，“实际收入”才会显示在“利用率”报表中。</p> <p>“利用率”报表计算所包含项目实际收入的方式因任务上设置的收入类型而异，具体如 <a href="#track-revenue" class="MCXref xref">跟踪收入</a> 章节。 </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>边距</strong> </td> 
   <td> <p>利润百分比计算如下：</p> <p>实际收入 — 实际成本/实际收入x 100。 </p> <p><b>注释</b>

如果实际收入等于0，则毛利显示为0。 </p> </td>
</tr> 
 </tbody> 
</table>

<!--Note from the table from above "Function" header in the middle of the table; right after the "Planned Revenue"/"Margin" definition: 
     <p scope="col" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This needs to be either split in two tables of formatted differently)</p>
    -->

## 使用利用率报告跟踪进度、成本和收入 {#track-progress-cost-and-revenue-with-the-utilization-report}

您可以跟踪项目、项目群或项目组合的进度或成本。

您可以显示在给定周或月的利用率报告上或项目整个生命周期中的信息。

要使用利用率报告跟踪一个或多个项目的进度或成本，请执行以下操作：

1. 根据您查看的是单个项目、多个项目、项目群还是项目组合的利用率信息，执行以下任一操作：

   * 要查看单个项目的利用率信息，请执行以下操作：

      1. 转到要查看其利用率信息的项目，然后单击 **显示更多>利用率**.
      1. 查看单个项目时，利用率信息会自动显示，并且不需要应用过滤器。\
         如果要过滤利用率报表，可以应用过滤器，然后单击 **运行**.\
         有关如何筛选“利用率”报表的信息，请参阅部分 [筛选器利用率信息](#filter-utilization-information) 本文章中。\
         显示单个用户和角色（用户在其关联的角色中分组）的使用情况信息。

   * 要查看多个项目的利用率信息，请执行以下操作：

      1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Workfront的右上角)，然后单击 **资源**，则 **利用率** （在左侧面板中）。
      1. 将过滤器应用于利用率报表，然后单击 **运行**.\
         在运行利用率报告之前，您必须在筛选器中指定一个或多个项目。 有关如何筛选“利用率”报表的信息，请参阅部分 [筛选器利用率信息](#filter-utilization-information) 本文章中。\
         显示单个角色和项目（角色在其关联项目中分组）的利用率信息。

   * 要查看方案的利用率信息，请执行以下操作：

      1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Workfront的右上角)，然后单击 **资源**，则 **利用率** ，然后单击 **显示**>**程序**.
      1. 将过滤器应用于利用率报表，然后单击 **运行**.\
         运行“Utilization”报告之前，必须在过滤器中指定一个或多个程序。 有关如何筛选“利用率”报表的信息，请参阅部分 [筛选器利用率信息](#filter-utilization-information) 本文章中。\
         显示单个项目和方案（项目在其关联的方案中进行分组）的利用率信息。

   * 要查看项目组合的利用率信息，请执行以下操作：

      1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Workfront的右上角)，然后单击 **资源**，则 **利用率** （在左侧面板中）并单击 **显示**>**Portfolio**.
      1. 将过滤器应用于利用率报表，然后单击 **运行**.\
         在运行利用率报告之前，您必须在过滤器中指定一个或多个项目组合。 有关如何筛选“利用率”报表的信息，请参阅部分 [筛选器利用率信息](#filter-utilization-information) 本文章中。\
         显示单个项目、项目群和项目组合的利用率信息（项目群归入其关联的项目群中，项目群归入其关联的项目群中）。

1. 在“Utilization”报告的右上角，单击 **视图** 下拉菜单，然后从以下菜单中选择：

   * **成本**
   * **小时**
   * **收入**
   * **收入和成本（计划）**
   * **收入vs成本（实际）**.

   您选择的选项决定了报告中可用的列和信息。 有关每列中可用信息的更多详细信息，请参阅步骤5中的表。\
   ![](assets/utilization-view-dropdown.png)

1. （可选）选择显示利用率信息的日期范围。 您可以在左侧显示给定周或月的信息 **总体** 列。 整个项目、项目群或项目组合的信息始终显示在 **总体** 列。\
   有关更多信息，请参阅部分 [调整显示信息的日期范围](#adjust-the-date-range-for-which-information-is-displayed) 本文章中。

1. （可选）单击任意列标题以按该列中的信息对利用率报告进行排序。 仅当您的报表中包含多个项目时，排序才有效。 例如，您可以在查看多个项目（或项目组合或项目群）时对报表结果进行排序。 当您一次只查看一个项目（或一个项目组合或一个项目群）时，无法对结果进行排序。
1. 使用部分中的信息 [利用率报表概览](#overview-of-the-utilization-report) 了解利用率报告中的每一列。

## 筛选器利用率信息 {#filter-utilization-information}

您可以筛选在项目的利用率报告中显示的内容。 您可以按任务、问题、角色和自定义数据筛选。 将过滤器应用于“利用率”报表时，“利用率”报表包含基于所选标准的信息。

您可以创建过滤器，也可以应用之前创建的过滤器。

* [创建或修改筛选器](#create-or-modify-a-filter)
* [应用已保存的过滤器](#apply-a-saved-filter)
* [复制筛选器](#duplicate-a-filter)
* [重命名筛选器](#rename-a-filter)
* [删除筛选器](#delete-a-filter)

### 创建或修改筛选器 {#create-or-modify-a-filter}

创建过滤器时，所有有权访问“利用率”报告的Workfront用户也都有权访问您创建的过滤器。 同样，在修改现有过滤器时，也会为有权访问利用率报告的所有用户修改该过滤器。

要创建或修改过滤器，请执行以下操作：

1. 要筛选单个项目的利用率信息，请转到要筛选其利用率信息的项目，然后单击 **显示更多>利用率** （在左侧面板中）。

   或

   要筛选多个项目、项目群或项目组合的利用率信息，请单击主菜单图标 ![](assets/main-menu-icon.png) 在Workfront的右上角， **资源**， **利用率** 在左侧面板中，然后 **显示**>**程序** 或 **Portfolio** 或&#x200B;**项目**.

1. 单击 **筛选条件** 图标以显示过滤器选项。

1. （视情况而定）要修改现有筛选器，请单击 **筛选条件** 下拉菜单，然后选择要修改的筛选器。
1. 指定以下信息以创建或修改筛选器：

   * **Portfolio：** 开始键入项目组合的名称，其中包含您要包含在“Utilization”报表中的信息，然后在下拉菜单中单击该名称。\
     重复此过程，在利用率报告中包含来自多个项目组合的信息。\
     要在筛选器中包含系统中的所有项目组合，请单击 **全部添加**. （仅当您的系统中拥有的项目组合少于10个时，此选项才可用。）

   * **程序：** 开始键入包含要包含在利用率报告中的信息的程序名称，然后在下拉菜单中单击该名称。\
     重复此过程，在利用率报告中包含多个任务的信息。\
     如果您已在筛选器中指定了任何项目组合，则您指定的项目组合必须来自已包含在筛选器中的项目组合。 如果不包含，则程序中的数据不会包含在利用率报表中。\
     要将系统中的所有程序都包含在过滤器中，请单击 **全部添加**. （仅当系统中程序少于20个时，此选项才可用。）

   * **项目：** 开始键入包含要包含在利用率报告中的信息的项目名称，然后在下拉菜单中单击该名称。\
     重复此过程以在“利用率”报告中包含来自多个项目的信息。\
     如果您已在筛选器中指定了任何项目组合或程序，则您指定的项目必须来自筛选器中已包含的某个项目组合或程序。 如果不包含，则项目中的数据不会包含在利用率报表中。\
     要在筛选器中包括系统中的所有项目，请单击 **全部添加**. （仅当系统中项目少于250个时，此选项才可用。）

   * **任务：** 开始键入任务名称，该任务包含要包含在利用率报告中的信息，然后在下拉菜单中单击该名称。\
     重复此过程，在利用率报告中包含多个任务的信息。\
     如果您已在筛选器中指定了任何项目组合、项目群或项目，则您指定的任务必须来自筛选器中已包含的某个项目组合、项目群或项目。 如果不包含，则任务中的数据不会包含在利用率报表中。

   * **问题：** 开始键入问题的名称，该名称包含您要包含在“Utilization”报告中的信息，然后在下拉菜单中单击该名称。\
     重复此过程以在利用率报告中包含多个问题的信息。\
     如果您已在筛选器中指定了任何项目组合、项目群或项目，则指定的问题必须来自筛选器中已包含的某个项目组合、项目群或项目。 如果不包含，则问题中的数据不会包含在利用率报表中。\
     问题的成本信息并不总是包含在利用率报表中。 有关问题的成本信息何时包含在利用率报表中的更多信息，请参阅部分 [使用利用率报告跟踪进度、成本和收入](#track-progress-cost-and-revenue-with-the-utilization-report) 本文章中。

   * **角色：** 开始键入要在“利用率报告”中显示的角色的名称，然后在下拉菜单中单击该名称。 重复此过程以包含其他角色。\
     利用率报告仅包含指定角色的信息。 例如，一个任务包含10个实际小时数。 其中6个小时来自设计师角色，4个小时来自开发人员角色。 如果您按设计者的角色筛选利用率报表，则来自开发人员角色的4小时将从报表中排除。

   * **添加筛选规则：** 单击 **添加筛选规则**，单击第一个字段，然后开始键入要过滤的字段名称。 如果该字段可用，则会填充可与其关联的每个对象。 单击字段名称以将其添加到过滤器。

     >[!IMPORTANT]
     >
     >您必须键入字段名称，而不是字段标签。 字段标签显示在附加到对象的自定义表单上。 有关自定义字段的标签和名称之间差异的信息，请参阅  [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

     有关您在列中看到的字段的更多信息，请参阅 [Adobe Workfront术语表](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).\
     选择过滤器的过滤器和条件修饰符。 有关可用的修饰符的描述，请参见 [过滤器和条件修饰符](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. 要创建新筛选器，请单击 **保存筛选器**.\
   或\
   要修改现有筛选器，请单击 **保存筛选器** 按钮，然后单击 **保存新筛选器**.\
   在 **筛选器名称** 字段中，指定过滤器的名称，然后单击 **保存**.\
   “利用率”区域使用您在过滤器中包含的信息进行过滤。

### 应用已保存的过滤器 {#apply-a-saved-filter}

1. 要在单个项目的利用率报告上应用过滤器，请转到要过滤的项目，然后单击 **显示更多>利用率** （在左侧面板中）。

   或

   要对多个项目、项目群或项目组合的利用率报告应用过滤器，请单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角， **资源**， **利用率** 在左侧面板中，然后 **显示**>**程序** 或&#x200B;**Portfolio** 或&#x200B;**项目**.

1. 单击 **保存的筛选条件**，然后从下拉菜单中选择要应用的过滤器。

### 复制筛选器 {#duplicate-a-filter}

1. 要在单个项目的利用率报告上复制过滤器，请转到要复制过滤器的项目，然后单击 **显示更多>利用率** （在左侧面板中）。

   或

   要复制多个项目、项目群或项目组合的使用情况报告上的过滤器，请单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Workfront的右上角)，然后单击 **资源**，则 **利用率** （在左侧面板中）。

1. 单击 **保存的筛选条件**，将鼠标悬停在下拉菜单中要复制的过滤器上，然后单击 **复制** 图标。

   ![](assets/utilization-filter-duplicate.png)\
   此时将显示“复制筛选器”对话框。

1. 在 **筛选器名称** 字段中，为新筛选器指定名称，然后单击 **保存**.

### 重命名筛选器 {#rename-a-filter}

在重命名过滤器时，所有有权访问“利用率”报告的Workfront用户都会看到您选择的新名称。

要重命名过滤器，请执行以下操作：

1. 要重命名单个项目利用率报告上的筛选器，请转到要为其重命名筛选器的项目，然后单击 **显示更多>利用率** （在左侧面板中）。

   或

   要重命名多个项目、项目群或项目组合的使用情况报告上的过滤器，请单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Workfront的右上角)，然后单击 **资源**，则 **利用率** （在左侧面板中）。

1. 单击 **保存的筛选条件**，将鼠标悬停在下拉菜单中要复制的过滤器上，然后单击 **重命名** 图标。\
   ![](assets/utilization-filter-rename.png)\
   将显示“重命名筛选器”对话框。

1. 在 **筛选器名称** 字段中，为新筛选器指定名称，然后单击 **保存**.

### 删除筛选器 {#delete-a-filter}

当您删除某个过滤器时，将会为所有有权访问利用率报告的Workfront用户删除该过滤器。

要删除过滤器，请执行以下操作：

1. 要删除单个项目利用率报告上的筛选器，请转到要删除该筛选器的项目，然后单击 **显示更多>利用率** （在左侧面板中）。

   或

   要删除多个项目、项目群或项目组合的使用情况报告上的过滤器，请单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Workfront的右上角)，然后单击 **资源**，则 **利用率** （在左侧面板中）。

1. 单击 **保存的筛选条件**，将鼠标悬停在下拉菜单中要复制的过滤器上，然后单击 **删除** 图标。

   ![](assets/utilization-filter-delete.png)

1. 单击 **删除** 系统提示是否要删除过滤器时。

## 调整显示信息的日期范围 {#adjust-the-date-range-for-which-information-is-displayed}

您可以调整显示利用率信息的日期范围。 您可以选择过去或未来的日期。 您所做的更改仅对您可见。

1. 要调整单个项目的利用率报表日期范围，请转到要调整日期范围的项目，然后单击 **显示更多>利用率** （在左侧面板中）。

   或

   要调整多个项目、项目群或项目组合的利用率报表的日期范围，请单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Workfront的右上角)，然后单击 **资源**，则 **利用率** （在左侧面板中）。

1. 单击旁边的 **导出** 按钮。

   默认情况下会选择当前周。

1. 从以下选项中选择：

   * **周：** 选择此选项可选择给定的周（从星期日到星期六）。
   * **月：** 选择此选项可选择给定的月份。

   您选择的日期范围将显示在利用率报表中，位于左侧 **总体** 列。\
   Workfront会记住您是要查看周视图还是月视图。 下次访问利用率报告时，将会根据您选择的选项显示本周或当月。

## 导出利用率信息

您可以从Workfront导出项目、项目群或项目组合的利用率信息。 信息只能以XLSX、TSV和PDF格式导出。

在Microsoft Excel中查看时，负数显示在括号中。

要导出利用率信息，请执行以下操作：

1. 要导出单个项目的利用率信息，请转到要导出利用率信息的项目，然后单击 **利用率** 选项卡(根据布局设置，这可能位于 **更多** 选项卡)。

   或

   要导出多个项目、项目群或项目组合的利用率信息，请单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Workfront的右上角)，然后单击 **资源**，则 **利用率** （在左侧面板中）。

1. 单击 **导出**，位于左侧的 **利用率** 选项卡。

1. 从以下选项中选择：

   * **PDF：** 以PDF格式导出报告。 如果您计划打印报表，则建议使用此格式。\
     选择 **信件 — 纵向**， **字母 — 横向**，或 **其他尺寸** (提供用于在Legal(8.5&quot; x 14&quot;)、Ledger(11&quot; x 17&quot;)和A4中导出的选项。\
     根据您使用的操作系统，您可以选择打开或保存文件。 使用关联的应用程序打开文件，或将其保存到硬盘驱动器。

   * **Excel：** 以XLSX格式导出报告。 如果您计划进一步分析Excel中的数据，建议使用此格式。\
     根据您使用的操作系统，您可以选择打开或保存文件。 使用关联的应用程序打开文件，或将其保存到硬盘驱动器。

   * **制表符分隔：** 以TSV格式导出报告。 如果您计划将数据导入第三方软件以供进一步分析，则建议使用此格式。\
     根据您使用的操作系统，您可以选择打开或保存文件。 使用关联的应用程序打开文件，或将其保存到硬盘驱动器。

1. 阅读本文中的信息 [导出数据](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) 以了解如何使用导出的文件。

## 在图表中查看利用率信息

您可以在图表视图中可视化利用率报告中的数据。

1. 要以图表格式查看单个项目的利用率报告，请转到要查看的项目，然后单击 **显示更多>利用率** （在左侧面板中）。

   或

   要以图表格式查看多个项目、项目群或项目组合的利用率报告，请单击 **报告** 在全局导航栏中，转到报表区域，然后单击 **利用率** 选项卡。

1. 在“Utilization”报告的右上角，单击 **图表** 图标。\
   ![](assets/utilization-chart.png)\
   利用率报告以图表视图显示。

1. （可选）通过从“ ”中选择相应的选项，将其配置为显示项目、项目群或Portfolio **显示** 下拉菜单。
1. （可选）将鼠标悬停在报表上的特定时间点上可查看该时间点的数据。

   ![](assets/utilization-chart-hover-350x176.png)

1. （可选）调整筛选器以确定图表中显示的信息。 有关调整筛选器的信息，请参阅部分 [筛选器利用率信息](#filter-utilization-information) 本文章中。
1. （可选）配置图表报表的时间范围，如部分所述 [调整显示信息的日期范围](#adjust-the-date-range-for-which-information-is-displayed) 本文章中。
