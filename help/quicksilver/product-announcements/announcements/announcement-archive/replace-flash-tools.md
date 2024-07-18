---
title: Adobe Workfront中基于Flash的工具的替换
description: Adobe Workfront中基于Flash的工具的替换
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: c80d9b0b7eb2a638af9e0a11ca3038ed99ecf1ee
workflow-type: tm+mt
source-wordcount: '2701'
ht-degree: 0%

---

# Adobe Workfront中基于Flash的工具的替换

我们已从Adobe Workfront Classic中删除所有基于Flash的工具。

Workfront中现在提供了基于当前标准的替换工具。 这些更改与Adobe宣布的Flash产品支持终止一致。

## 重要日期

以下日期对于Workfront中所有基于Flash的工具的删除过程非常重要：

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **2020年11月19日**：已从所有Workfront产品中删除所有基于Flash的工具。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## 基于Flash的传统工具

以下部分列出的工具已从Workfront系统中删除并替换为新的解决方案。

有关替换工具的信息，请参阅本文中的[基于Flash的旧版工具及其替换工具](#legacy-flash-based-tools-and-their-replacements)。

### 资源管理

* “人员”区域中的“旧版资源计划”选项卡以及该选项卡中包含的所有工具，其中包括以下内容：

   * 资源预算管理器
   * 性能规划者
   * 资源评估
   * 资源网格\
     有关详细信息，请参阅[资源规划：文章索引](../../../resource-mgmt/resource-planning/resource-planning-overview.md)。

* 项目业务案例中的旧版资源评估区域

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

* 项目的“员工”选项卡中的“资源网格”子选项卡
* 在项目的“人员配备”标签的“计划”子标签中的“使用新计划区域”选项，该标签删除了原有计划区域或小组生成器。 在这种情况下，现在默认显示计划时间线。
* 用户配置文件下的分配选项卡

### 报告

已删除以下报告功能和报告：

* 已删除报表功能：

   * 用户报表中的“资源网格”选项
   * 项目或任务报告中的“传统甘特图”选项\
     有关详细信息，请参阅[在甘特图中查看信息](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)。

* 删除的报表：

   * “传统资源池”报告
   * “资源评估”报表

  >[!NOTE]
  >
  >通过报表或通过API访问的所有旧版字段（旧版资源池、旧版预算成本、旧版成本、旧版预算小时数、旧版预算劳力成本等）都会显示在各种报表中，但不会填充新信息。

### 传统甘特图

* 项目和任务列表以及报表和报告选项中的所有旧版甘特图
* Portfolio和程序中的“旧版甘特图”子选项卡
* 模板上的模板任务列表中的“旧甘特图”子选项卡，模板任务的“子任务”选项卡中的“旧甘特图”视图，以及“模板任务”报告中的“旧甘特图”视图

### 校对

旧版验证查看器已替换为适用于大多数客户的新Web验证查看器和桌面验证查看器，并且已于2020年11月为所有客户删除。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

有关更多信息，请参阅以下资源：

* [在Web验证查看器中查看验证](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [在桌面校对查看器中查看校对](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

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

## 基于Flash的旧版工具及其替代工具 {#legacy-flash-based-tools-and-their-replacements}

除非另有指定，否则所有旧版功能都已替换为新功能，如下表所示。

>[!CAUTION]
>
>已删除所有环境中基于Flash的旧工具。

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
   <td> <p><strong>旧版资源池</strong> </p> <p>传统资源池是完成项目时同时需要的职务角色的组或集合。 传统资源池存在许多缺点：</p> 
    <ul> 
     <li> 您可以将一个用户与一个旧版资源池关联，但该资源池仅用于报告目的。 由于传统资源池使用抽象工作角色实体运行，因此未考虑用户的计划例外和空闲时间，从而导致有关资源可用性的数据不准确。 </li> 
    </ul> 
    <ul> 
     <li>您只能为每个项目指定一个传统资源池，这将导致多个传统资源池仅支持独立工作的各个组的流，并且永远不会共享资源。 在所有其他情况下，建议保留一个包含系统中所有资源的传统资源池，这会导致大量项目和数据出现性能问题。</li> 
    </ul> </td> 
   <td> <p><strong>资源池</strong> </p> <p>新资源池是完成项目时同时需要的用户的集合。 Workfront还认识到，在某些情况下，专门用户需要单独为其分配工作。 因此，您现在可以预算用户而非工作角色。 </p> 与旧版资源池相比，资源池具有以下优势： 
    <ul>
     <li>由于资源池基于用户，因此计算用户和角色可用性时已考虑其休息时间和计划例外情况。 这样可以提供准确和最新的数据，从而做出正确的预算决定，并在项目实施期间最大限度地降低变更的可能性。</li>
     <li>由于现在可以更好地控制资源的可用性和数据的准确性，因此Workfront允许您将多个资源池与一个项目关联。 一个用户也可以属于多个资源池，前提是他们拥有多种技能，可以同时用于多个项目。 </li>
    </ul><p>由于对数据有这样的控制，不再需要有一个包含所有资源的资源池来分配可用预算。 事实上，我们不推荐这样做。 为此，我们建议多元化您的资源池并仅将相关资源池与项目相关联。</p><p> 有关资源池的详细信息，请参阅<a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">资源池概述</a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>资源预算管理器</strong> </p> <p>您可以使用资源预算管理器指定多个资源池中工作角色资源的可用性。 但是，由于旧版资源池的缺点，此功能很少使用。 在使用时，它会强制用户手动输入工作角色的可用性，以使预算更准确。 未考虑计划例外情况和用户的休息时间。</p> </td> 
   <td> <p>随着基于资源池中的用户的可用性自动计算，不再需要资源预算管理器。 该工具已经淘汰，同时取消了计算可用性的所有手动工作。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>资源估计</strong> </p> <p>每个传统资源池下的资源估计值选项卡与资源预算管理器具有相同的用途，但仅限于一个传统资源池的上下文。 此工具与资源预算管理器和旧版资源池具有相同的限制：数据不准确和手动输入可用性。 </p> </td> 
   <td> <p>随着用户可用性的自动计算，资源估计已过时并已删除。</p> <p>在项目的业务案例中，该工具在旧版资源池和旧版资源评估中消除。 <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>能力规划者</strong> </p> <p>Capacity Planner是一种Workfront工具，用于根据资源的可用性为传统资源池中的资源编制预算并安排项目的优先级。 鉴于来自资源估算和资源预算管理器（为能力规划者提供信息）的数据不完整，必须根据用户的可用性对项目优先顺序进行双重检查。</p> <p>最常见的情况是，使用包含系统中所有工作角色的单个传统资源池，这会导致能力规划者尝试加载大量项目时出现性能问题。</p> </td> 
   <td> <p><strong>资源规划者的项目视图</strong> </p> <p>在资源规划者的基于项目的视图中，您可以像在传统能力规划者中那样预算资源和优先处理项目。 与旧版工具不同，现在支持更多数据，因为考虑到用户的休息时间和计划例外情况，可用信息更加精确。</p> <p>可用信息、计划信息和预算信息一目了然，以便资源管理器能够查看是否有足够的人员来完成工作以及项目计划是否超出初始预算估计。</p> <p> 有关在资源规划者中使用项目视图的信息，请参阅<a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">资源规划者概述</a></p> <p><strong>方案规划者</strong> </p> <p>对于长期容量规划、假设情景建模和优先排序，我们还引入了Workfront场景规划器。 </p> <p>Scenario Planner仅在新的Adobe Workfront Experience中可用，并且需要额外的许可证。 有关Workfront Scenario Planner的信息，请参阅<a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Scenario Planner概述</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>旧版资源评估（商业案例）</strong> </p> <p>您可以使用业务案例的旧版资源估算区域来预算特定的人工小时数和成本，作为项目规划和资源请求的一部分。 此视图未提供资源可用性的任何可见性，从而导致资源请求的大致性以及被拒绝项目工作的可能性增加。</p> </td> 
   <td> <p><strong>资源预算（商业案例）</strong> </p> <p>Business Case下的Resource Budgeting部分将Resource Planner功能引入Business Case，从而提供用户和角色可用性可见性以及在用户级别进行预算的能力。 </p> <p> 有关业务案例的资源预算编制区域的信息，请参阅<a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">业务案例区域概览</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>资源评估报告</strong> </p> <p>使用资源管理的旧版工具时，您可以从业务案例中报告预算和计划小时数。 这允许您生成矩阵报告，其中显示特定时间范围内每个工作角色的预算和计划工作总量。 此报告不可编辑，您无法在报告发现的基础上对资源的预算进行任何更改。 </p> </td> 
   <td> <p><strong>利用率报告</strong> </p> <p>内置利用率报告并排显示计划小时数、预算小时数和实际小时数、成本和收入。 </p> <p>有关使用利用率报告的信息，请参阅<a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">查看资源利用率信息</a>。 </p> 
    <div> 
     <p><strong>可报告预算小时数</strong> </p> 
     <p>为预算小时数创建报告以审查报告表单中资源规划者中预算的小时数。 </p> 
     <p>有关预算小时数的信息，请参阅<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Adobe Workfront术语词汇表</a>。</p> 
     <p>有关创建报告的信息，请参阅<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报告</a>。</p> 
    </div> <p><strong>资源规划者的角色视图</strong> </p> <p>传统资源管理工具中业务案例的预算和计划小时数现在可在新的本机视图（资源规划者的基于角色的视图）中获取。 此视图提供可用小时数、计划小时数和预算小时数概览，并允许您在同一位置控制和更改预算。 这确保在高级职位角色规划期间做出更好的决策。 </p> <p> 有关在资源规划者的角色视图中预算资源的信息，请参阅<a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">资源规划者概述</a>中的<a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">使用项目和角色视图预算资源</a>部分</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>资源网格</strong> </p> <p>资源网格让您能够查看在项目走向完成时特定用户的分配情况。 </p> <p>例如，您可以轻松地查看您项目团队中的某人何时提前完成工作、何时落后，以及他们是否在特定时间范围内分配过多或不足。 </p> <p>很遗憾，您无法根据同一视图中的信息执行操作。 要纠正过度分配问题，您必须转到项目并手动调整那里的信息，而看不到操作的结果。</p> </td> 
   <td> <p>资源网格已由两种新工具取代。 您可以使用以下工具，具体取决于您所在的资源计划阶段：</p> 
    <ul> 
     <li> <p>分析阶段的<strong>：</strong> </p> 
      <ul> 
       <li> <p><strong>工作负载均衡器</strong>：使用工作负载均衡器在更精细的级别查看用户的工作负载。 使用工作负载均衡器时，可以查看哪些用户在其工作负载中具有可用性以按时完成任务。 这包括他们的休息时间和计划例外详细信息。 </p> <p>有关工作负载均衡器的信息，请参阅<a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">工作负载均衡器概述</a>。</p> </li> 
       <li> <p><strong>资源规划者的用户视图</strong><strong>：</strong>当试图从更高级别了解您的用户分配到哪些项目时，请使用资源规划者的用户视图。 这让您能够查看用户正在处理什么以及他们在特定时间范围内的过度分配和过度分配。 Resource Planner还提供了用户总体分配的可视化信息，以及记录的实际小时数的可视化信息，这有助于分析完成工作的进度。 </p> <p>有关在资源规划者中使用用户视图的信息，请参阅<a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">资源规划者概述</a>中的<a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">使用用户视图查看可用、计划和实际小时数或FTE </a>部分</p> </li> 
      </ul> </li> 
     <li>战术阶段<strong>：</strong> 
      <ul> 
       <li><strong>工作负载均衡器</strong>您可以使用工作负载均衡器执行以下操作： 
        <ul>
         <li>将工作分配给用户。</li>
         <li>管理用户对工作项的分配。 </li>
         <li>与可能没有人员区域可见性的其他用户共享工作负载均衡器。 使用可共享链接功能可共享指向工作负载均衡器的链接，并将其嵌入自定义功能板。 当您共享这些仪表板时，任何有权查看用户的用户都可以查看这些仪表板。</li>
        </ul><p>工作负载均衡器位于人员区域。 </p><p>有关工作负载均衡器的信息，请参阅<a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">工作负载均衡器概述</a>。</p></li> 
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
   <td> <p><strong>旧版甘特图，任务列表</strong> </p> <p> 任务列表上的旧版甘特图使用户能够直观地查看项目的时间表并执行假设情景计划，而无需将更改提交到数据库。 传统甘特图基于Flash技术，存在安全隐患。 </p> </td> 
   <td> <p><strong>甘特图，</strong> <strong>任务列表</strong></p> <p> 新的基于HTML的甘特图与旧版甘特图具有相同的用途。 用户可以通过更改任务列表工具栏中的“手动保存”选项来可视化项目的时间表并执行假设情景计划，而无需将更改提交到数据库。 </p> <p>使用自动保存选项时，新的甘特图是交互式的，当您想要在更改发生时自动保存时，可以使用该选项。 </p> <p>新的任务列表甘特图基于最新的技术构建并可靠。 此新甘特图直接位于任务列表中，在处理任务列表时可轻松访问，无需切换选项卡或更改视图。 </p> <p>尽管新的甘特图提供了与上一个图表相同的功能，但与旧版甘特图相比，在功能上存在一些差异。 </p> <p> 模板任务列表中的旧版甘特图子选项卡、模板任务子任务选项卡中的旧版甘特图以及模板任务报告中的旧版甘特图也已替换为基于HTML的甘特图。 </p> <p>如果您将旧版甘特图主要用于简单视图和快速编辑，而不使用实际图表，则新的“时间线计划”选项允许您对关键计划字段进行快速更改。 您可以从任务列表工具栏中选择“时间线计划”而不是“自动保存”。</p> <p>有关使用“时间线计划”选项保存任务列表的详细信息，请参阅<a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">编辑列表中的任务</a>一文中的“选择“时间线计划”选项时手动在任务列表中保存更改”部分。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目列表的<strong>旧版甘特图</strong> </p> <p>项目列表上的旧版甘特图使用户能够在一个视图中查看项目及其任务。 在不离开项目列表上下文的情况下，用户可查看有关项目中任务的详细信息以及项目之间的依赖关系。 项目清单上的旧版甘特图基于Flash技术，存在安全风险。 </p> </td> 
   <td> <p><strong>甘特图，项目列表</strong> </p> <p>基于HTML的甘特图与旧版甘特图的用途相同。 用户可以在一个视图中查看项目及其任务，以直观地识别项目之间以及任务之间的依赖关系。 项目列表甘特图直接位于项目列表中。 新的甘特图具有现代化的界面，并且基于最新的技术构建。</p> <p>有关项目列表甘特图的信息，请参阅<a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">在甘特图</a>中查看信息。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>共享报告、日历和文档的对话框</strong> </p> <p>共享报告、日历和文档时，使用的对话框基于Flash技术。</p> </td> 
   <td> <p>在Workfront中共享报告、日历和文档时的体验未发生更改。 但是，该体验不再依赖于Flash。</p> <p>有关共享这些项目的详细信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">对象权限共享概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>旧版验证查看器</strong> </p> <p>旧版验证查看器是基于Web的验证查看器，为静态、视频和交互式验证提供了验证功能。</p> </td> 
   <td> <p><strong>Web验证查看器和桌面验证查看器</strong> </p> <p>Web校对查看器提供静态校对和视频校对的校对功能。</p> <p>桌面校对查看器为交互式校对提供校对功能，此外还提供对静态校对和视频校对的完全支持。</p> <p>SWF文件格式不再受任何主要提供商的支持，并已由HTML5校对横幅取代。 </p> <p>有关可用校对查看器之间差异的更多详细信息，请参阅<a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Web校对查看器和桌面校对查看器之间的差异</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>
