---
title: 在Adobe Workfront中替换基于Flash的工具
description: 在Adobe Workfront中替换基于Flash的工具
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '2705'
ht-degree: 1%

---

# 在Adobe Workfront中替换基于Flash的工具

我们已从Adobe Workfront Classic中删除了所有基于Flash的工具。

基于当前标准的替换工具现在在Workfront中提供。 这些更改与Adobe宣布的停止对Flash产品的支持保持一致。

## 重要日期

以下日期对于在Workfront中删除所有基于Flash的工具非常重要：

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **2020年11月19日**:所有基于Flash的工具都已从所有Workfront产品中删除。

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## 基于Flash的旧版工具

以下部分中列出的工具已从Workfront系统中删除，并替换为新的解决方案。

有关替换工具的信息，请参阅 [旧版基于Flash的工具及其替代方法](#legacy-flash-based-tools-and-their-replacements) 在本文中。

### 资源管理

* “人员”区域中的“旧版资源计划”选项卡以及选项卡中包含的所有工具，包括以下内容：

   * 资源预算管理器
   * 性能规划者
   * 资源评估
   * 资源网格\
      有关更多信息，请参阅 [Adobe Workfront资源规划](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

* 项目业务案例中的“旧资源估计”区域

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  is displayed in view-only mode
  </MadCap:conditionalText>
  -->

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  For more information, see
  <a href="../../../resource-mgmt/resource-mgmt-overview/migrate-resource-estimates-to-budgeting.md" class="MCXref xref">Migrate from Legacy Resource Estimates to Resource Budgeting </a>
  </MadCap:conditionalText>
  -->

   。

* 项目“人员配备”选项卡中的“资源网格”子选项卡
* 项目“人员配备”选项卡的“计划”子标签中的“使用新计划区域”选项，该选项将删除旧计划区域或团队生成器。 在这种情况下，计划时间轴现在默认显示。
* 用户配置文件下的“分配”选项卡

### 报告

已删除以下报表功能和报表：

* 删除了报表功能：

   * 用户报表中的“资源网格”选项
   * 项目或任务报表中的“旧版甘特图”选项\
      有关更多信息，请参阅 [在甘特图中查看信息](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* 删除的报表：

   * 旧版资源池报表
   * 资源估计报告

   >[!NOTE]
   >
   >通过报表或API访问的所有旧版字段（旧版资源池、旧版预算成本、旧版成本、旧版预算小时数、旧版预算人工成本等）都会显示在各种报表中，但不会填充新信息。

### 传统甘特图

* 项目和任务列表中的所有旧版甘特视图，以及报表和报表选项
* “Portfolio”和“程序”中的“旧甘特图”子选项卡
* 模板上的模板任务列表中的“旧甘特图”子选项卡、模板任务的“子任务”选项卡中的“旧甘特图”视图以及模板任务报表中的“旧甘特图”子选项卡

### 验证

对于大多数客户而言，旧版校样查看器已被替换为新的Web校样查看器和桌面校样查看器，并且已于2020年11月为所有客户删除了旧版校样查看器。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

有关更多信息，请参阅以下资源：

* [Web校样查看器中的审阅校样](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [在桌面校对查看器中查看校样](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-proof/wp-work-proofsfiles/review-proofs-lpv/lpv-removed-2018.md" class="MCXref xref">Legacy proofing viewer removed in 2018.3</a> </li>
  -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Additional features to be removed</h3>
<ul>
<li>The Legacy Portfolio Optimizer<br>For more information, see <a href="../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md" class="MCXref xref">Portfolio Optimizer overview</a>.<br></li>
<li>The Legacy financial fields in the Business Case of the project and the Portfolio Optimizer</li>
<li>The dialog boxes used when sharing reports, calendars, and documents no longer rely on Flash-based technology</li>
</ul>
</div>
-->

## 旧版基于Flash的工具及其替代方法 {#legacy-flash-based-tools-and-their-replacements}

除非另有指定，否则所有旧版特征都已被新特征替换，如下表所示。

>[!CAUTION]
>
>基于Flash的旧版工具已从所有环境中删除。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>旧版工具</strong> </p> </th> 
   <th> <p><strong>新工具</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>传统资源池</strong> </p> <p>旧版资源池是完成项目同时需要的作业角色的组或集合。 旧版资源池存在许多缺点：</p> 
    <ul> 
     <li> 您可以将一个用户与一个旧版资源池相关联，但该资源池仅用于报告目的。 由于旧版资源池使用抽象作业角色实体运行，因此没有考虑用户的计划例外和休息时间，从而导致有关资源可用性的数据不准确。 </li> 
    </ul> 
    <ul> 
     <li>您只能为每个项目指定一个旧版资源池，这会导致多个旧版资源池仅支持独立工作且从不共享资源的不同组的流。 在所有其他情况下，建议保留一个包含系统中所有资源的旧版资源池，这会导致大量项目和数据出现性能问题。</li> 
    </ul> </td> 
   <td> <p><strong>资源池</strong> </p> <p>新资源池是完成项目同时需要的用户集合。 Workfront还认识到，在某些情况下，专业用户需要将工作单独分配给他们。 因此，您现在可以对用户进行预算，而不是对作业角色进行预算。 </p> 资源池相对于旧版资源池的优势包括： 
    <ul>
     <li>由于资源池基于用户，因此在计算用户和角色可用性时已考虑其休息时间和计划例外。 这样可生成精确且最新的数据，从而能够做出正确的预算决策，并最大限度地减少项目运行中发生更改的可能性。</li>
     <li>由于现在对资源可用性和数据准确性有了更多的控制，因此Workfront允许您将多个资源池与一个项目相关联。 一个用户也可以属于多个资源池，以防他们同时具有多个可在多个项目中使用的技能。 </li>
    </ul><p>由于对数据的这种控制，不再需要有一个资源池来包含分配可用预算的所有资源。 事实上，我们不建议这样做。 相反，我们建议您将资源池多样化，并仅将相关资源池与项目关联。</p><p> 有关资源池的详细信息，请参阅 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 资源池概述 </a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>资源预算管理器</strong> </p> <p>您可以使用资源预算管理器指定多个资源池中作业角色资源的可用性。 但是，由于旧版资源池的缺点，很少使用此功能。 使用时，它会强制用户手动输入作业角色的可用性，以使预算更准确。 计划例外和用户休假时间未被考虑在内。</p> </td> 
   <td> <p>通过根据资源池中的用户自动计算可用性，不再需要资源预算管理器。 该工具已被淘汰，同时计算可用性的所有手动工作也被取消。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>资源评估</strong> </p> <p>每个旧资源池下的“资源估计”选项卡与资源预算管理器具有相同的用途，仅在一个旧资源池的上下文中可用。 此工具具有与资源预算管理器和旧版资源池相同的限制：不准确的数据和手动输入可用性。 </p> </td> 
   <td> <p>随着用户可用性的自动计算，资源估计已过时并已被删除。</p> <p>该工具在项目业务案例的“旧版资源池”和“旧版资源估计”中被删除。 <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>性能规划者</strong> </p> <p>能力规划器是Workfront的一个工具，用于根据资源的可用性对资源进行预算编制并对旧资源库中的项目进行优先级排序。 鉴于资源估计和为能力规划员提供信息的资源预算管理员的数据不完整，必须根据用户的可用性对项目优先顺序进行重复检查。</p> <p>使用单个包含系统中所有作业角色的旧版资源池是最常见的情况，这会导致能力规划器尝试加载大量项目时出现性能问题。</p> </td> 
   <td> <p><strong>资源计划员的项目视图</strong> </p> <p>在“资源计划器”的“基于项目”视图中，您可以对资源进行预算，并按与在“旧能力计划器”中执行预算类似的方式对项目进行优先级排序。 与旧版工具不同，现在支持更多数据，通过考虑用户的休假时间和计划例外，可用信息将更加精确。</p> <p>可用、已计划和已编入预算的信息一目了然，以便资源经理可以同时查看是否有足够的人员来完成工作以及项目计划是否超出初始预算估计。</p> <p> 有关在资源计划器中使用项目视图的信息，请参阅 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">资源计划员概述</a></p> <p><strong>方案计划员</strong> </p> <p>对于长期能力规划、假设情景建模和优先级排序，我们还引入了Workfront情景规划器。 </p> <p>方案规划器仅在新的Adobe Workfront体验中可用，并且需要额外的许可证。 有关Workfront方案规划器的信息，请参阅 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">方案计划员概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>旧版资源估计（业务案例）</strong> </p> <p>您可以使用“业务案例”的“旧资源估计”区域，在项目计划和资源请求中预算一定数量的人工小时数和成本。 此视图未提供对资源可用性的任何可见性，这会导致大致的资源请求，并增加了被拒绝项目工作的机会。</p> </td> 
   <td> <p><strong>资源预算编制（业务案例）</strong> </p> <p>“业务案例”下的“资源预算”部分将“资源计划员”功能引入业务案例，从而提供用户和角色可用性的可见性，以及在用户层进行预算的能力。 </p> <p> 有关“业务案例”的“资源预算”区域的信息，请参阅 <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">业务案例领域概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>资源估计报表</strong> </p> <p>在使用旧版资源管理工具时，您可以从业务案例报告预算小时数和计划小时数。 这样，您就可以生成矩阵报表，其中显示特定时间范围内每个职务角色的预算工作和计划工作总数。 此报表不可编辑，您无法根据报表结果对资源预算进行任何更改。 </p> </td> 
   <td> <p><strong>利用率报表</strong> </p> <p>“内置利用率”报表并排显示“计划”、“预算”和“实际工时”、“成本”和“收入”。 </p> <p>有关使用“利用率”报表的信息，请参阅 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">查看资源利用信息 </a>. </p> 
    <div> 
     <p><strong>可报告预算小时数</strong> </p> 
     <p>为预算小时数创建报表，以在报表表单中复查资源计划员中预算的小时数。 </p> 
     <p>有关预算小时数的信息，请参阅 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Adobe Workfront术语表</a>.</p> 
     <p>有关创建报表的信息，请参阅 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报表</a>.</p> 
    </div> <p><strong>资源计划员的角色视图</strong> </p> <p>现在，在新的本机视图（即资源计划员的基于角色的视图）中，可以使用“旧版资源管理”工具中“业务”案例的预算小时数和计划小时数。 此视图提供了“可用”、“计划”和“预算小时数”信息概览，并允许您在同一位置控制和更改预算。 这可确保在高级职位角色规划期间做出更好的决策。 </p> <p> 有关资源计划员的“职责视图”中预算资源的信息，请参阅 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">使用项目和角色视图对资源进行预算 </a> 部分 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">资源计划员概述</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>资源网格</strong> </p> <p>在项目进入完成阶段时，资源网格可让您查看特定用户的分配情况。 </p> <p>例如，您可以轻松地查看项目团队中的某人何时提前完成了工作，何时有人落后，以及他们在特定时间段内是否被过度分配或分配不足。 </p> <p>遗憾的是，您未能在同一视图中对信息采取行动。 要纠正过度分配问题，您必须转到项目并手动调整其中的信息，而不能查看您的操作结果。</p> </td> 
   <td> <p>资源网格已被两个新工具替换。 根据您在资源规划的哪个阶段找到自己，您可以使用以下工具：</p> 
    <ul> 
     <li> <p><strong>对于分析阶段：</strong> </p> 
      <ul> 
       <li> <p><strong>工作负载平衡器</strong>:使用工作负载平衡器在更精细的粒度级别查看用户的工作负载。 使用工作负载平衡器时，可以查看哪些用户在其工作负载中具有可用性，以便按时完成任务。 这包括它们的休息时间和计划例外详细信息。 </p> <p>有关工作负载平衡器的信息，请参阅 <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">工作负载平衡器概述</a>.</p> </li> 
       <li> <p><strong>资源计划员的用户视图</strong><strong>:</strong> 在尝试更高层次地了解用户分配到哪些项目时，请使用资源计划员的“用户视图”。 这样，您就可以了解用户正在处理的内容，以及他们在特定时间范围内的过度分配和分配不足。 “资源计划器”还提供整体用户总体分配的可视化，以及“实际记录的小时数”的可见性，这有助于分析完成工作的进度。 </p> <p>有关在资源计划器中使用用户视图的信息，请参阅 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">使用“用户视图”可查看可用、计划和实际小时数或FTE </a> 部分 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">资源计划员概述</a></p> </li> 
      </ul> </li> 
     <li><strong>对于战术阶段：</strong> 
      <ul> 
       <li><strong>工作负载平衡器</strong> 您可以使用负载平衡器执行以下操作： 
        <ul>
         <li>将工作分配给用户。</li>
         <li>管理用户对工作项的分配。 </li>
         <li>与可能看不到“人员”区域的其他用户共享工作负载平衡器。 使用“可共享”链接功能共享指向工作负载平衡器的链接，并将其嵌入到自定义功能板中。 任何有权查看用户的用户在您共享这些功能板时都可以查看这些功能板。</li>
        </ul><p>工作负载平衡器在“人员”区域中可用。 </p><p>有关工作负载平衡器的信息，请参阅 <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">工作负载平衡器概述</a>.</p></li> 
      </ul> <!--
       <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <li><strong>The Resource Scheduling Areas</strong><strong>:</strong> When assigning your resources to the actual work that must be completed, use the Resource Scheduling areas in the People or Team areas, or at the project level. These areas allow you to visualize and manage the users' workload by day and rectify any problems from one view using the following actions: 
         <ul>
          <li> manual dragging and dropping of tasks to the correct assignee </li>
          <li> automatic assigning of tasks </li>
          <li> bulk swapping assignments </li>
          <li><p>adjusting Planned Hours according to the true availability of users. </p></li>
         </ul><p>These actions provide even more control over managing workload. </p><p> For information about managing user assignments and allocations in the Resource Scheduling areas, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p><p>With this new functionality, the Resource Grid is replaced by the User View of the Resource Planner and the Resource Scheduling areas in the following areas of the application: </p>
         <ul>
          <li>People - the Resource Grid is eliminated along with the Legacy Resource Planning tab.</li>
          <li>Project - the Scheduling area under the Staffing tab of the project is available to Work and Plan license users. They do not have to have Manage access to the project to view this area. </li>
          <li>Reporting - the ability to view User reports in the Resource Grid view is removed. Instead, there is an option to share a URL for the User View of the Resource Planner and embed it in custom dashboards, providing visibility into user utilization to virtually anyone in the system. Any users with access to View users are able to view these dashboards when you share them. </li>
          <li>User - the Allocation tab is eliminated as the same information can be accessed in the User View of the Resource Planner.</li>
         </ul></li> 
       </ul>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>旧甘特图、任务列表</strong> </p> <p> 任务列表上的“旧版甘特图”使用户能够直观地查看项目的时间轴并执行假设方案规划，而无需提交对数据库的更改。 旧版甘特图是基于Flash技术的，存在安全风险。 </p> </td> 
   <td> <p><strong>甘特图、</strong> <strong>任务列表</strong></p> <p> 基于HTML的新甘特图与旧版甘特图的用途相同。 用户可以通过从任务列表工具栏中更改为“手动保存”选项，在不将更改提交到数据库的情况下，可以显示项目的时间轴并执行假设方案规划。 </p> <p>使用自动保存选项时，新的甘特图是交互式的，当您希望在发生更改时自动保存更改时，可以使用该选项。 </p> <p>新的任务列表甘特图是基于最新技术构建的，并且可靠。 此新的甘特图直接位于任务列表上，在处理任务列表时，无需切换选项卡或更改视图即可轻松访问该甘特图。 </p> <p>尽管新甘特图提供的功能与上一图相同，但与旧版甘特图相比，其功能存在一些差异。 </p> <p> 模板上的模板任务列表中的“旧甘特图”子选项卡、模板任务的“子任务”选项卡中的“旧甘特图”视图，以及模板任务报表中的“旧甘特图”子选项卡也已替换为基于HTML的甘特图。 </p> <p>如果您使用旧甘特图主要用于简单视图和快速编辑，而不使用实际图表，则新的时间轴规划选项允许您对关键规划字段进行快速更改。 您可以从任务列表工具栏中选择时间轴计划，而不是自动保存。</p> <p>有关使用时间轴计划选项保存任务列表的详细信息，请参阅文章中的“选择时间轴计划选项时手动保存任务列表中的更改”部分 <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">在列表中编辑任务</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>项目列表的旧甘特图</strong> </p> <p>通过项目列表上的“旧版甘特图”，用户能够在一个视图中查看项目及其任务。 在不离开项目列表上下文的情况下，用户可以查看有关项目中任务的详细信息以及项目之间的依赖关系。 项目列表上的“旧甘特图”是基于Flash技术的，存在安全隐患。 </p> </td> 
   <td> <p><strong>甘特图、项目列表</strong> </p> <p>基于HTML的甘特图与旧版甘特图的用途相同。 用户可以在一个视图中查看项目及其任务，以便直观地识别项目和任务之间的依赖关系。 项目列表甘特图直接位于项目列表中。 新的甘特图具有现代化的界面，并基于最新技术构建。</p> <p>有关项目列表甘特图的信息，请参阅 <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">在甘特图中查看信息 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>报表、日历和文档的共享对话框</strong> </p> <p>在共享报表、日历和文档时，使用的对话框基于Flash技术。</p> </td> 
   <td> <p>在Workfront中共享报表、日历和文档的体验未发生更改。 但是，体验不再依赖于Flash。</p> <p>有关共享这些项目的更多信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">对象共享权限概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>旧版校对查看器</strong> </p> <p>旧版校对查看器是基于Web的校对查看器，它为静态、视频和交互式校样提供了校对功能。</p> </td> 
   <td> <p><strong>Web校对查看器和桌面校对查看器</strong> </p> <p>Web校对查看器提供了用于静态校样和视频校样的校样功能。</p> <p>桌面校对查看器除了提供对静态校样和视频校样的完全支持之外，还提供了用于交互式校样的校样功能。</p> <p>任何主要提供商都不再支持SWF文件格式，并且已用HTML5横幅替换，用于校样。 </p> <p>有关可用校对查看器之间差异的更多详细信息，请参阅 <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Web校对查看器与桌面校对查看器概述之间的差异</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
