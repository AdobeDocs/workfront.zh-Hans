---
title: 为组配置项目首选项
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: 如果您是组管理员，并且Adobe Workfront管理员解锁系统中所有组的项目首选项，则可以将该首选项配置为组以影响组创建的所有后续项目。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: 11c4028038fe3d410ee0d4f238d2138435d9a3fa
workflow-type: tm+mt
source-wordcount: '2643'
ht-degree: 2%

---

# 为组配置项目首选项

如果您是组管理员，并且Adobe Workfront管理员解锁系统中所有组的项目首选项，则可以将该首选项配置为组以影响组创建的所有后续项目。

如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。

>[!NOTE]
>
>* 通常，已解锁的首选项会无限期地保持解锁状态。 如果Workfront管理员重新锁定它，则系统设置将再次生效，并且组管理员所做的首选项设置将丢失。
>* 与项目关联的组的首选项集优先于为创建项目的用户的“主页组”设置的首选项集。
>* 某些组级别首选项会影响您为组创建的项目模板。 有关更多信息，请参阅 [从“组”区域查看、处理和创建组的模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) 在文章中 [创建和修改组的项目模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* 在Workfront管理员解锁系统级别的首选项后，您可以对其进行配置，然后将其锁定，以确保组及其子组中的每个人都使用相同的配置。 这与Workfront管理员必须为系统中的每个人配置和锁定首选项的功能平行。 有关更多信息，请参阅 [锁定或解锁子组的项目、任务或问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


任务和问题首选项以及工时单和小时首选项也可以进行组级配置。 有关信息，请参阅 [为组配置任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) 和 [为组配置工时单和小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

有关Workfront管理员如何解锁项目首选项的信息，请参阅 [锁定或解锁系统中所有组的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 为组配置已解锁的项目首选项

>[!TIP]
>
>如果您是Workfront管理员，则可以绕过步骤1-4，方法是转到设置>项目首选项>项目，然后在页面顶部的框中搜索组名称。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组** ![](assets/groups-icon.png).

1. 单击要配置其项目首选项的组的名称。
1. 在左侧面板中，单击 **项目首选项**.
1. 在显示的页面上，继续下面列出的4个部分之一，以配置项目状态、时间轴、业务案例和死亡后生命的首选项。

   >[!TIP]
   >
   >如果将鼠标悬停在某个首选项上，则会显示一个工具提示来告知您该首选项已锁定，则可以请求Workfront管理员为组织中的所有组解锁该首选项。

* [项目状态](#project-status)
* [时间线](#timelines)
* [业务案例](#business-cases)
* [结束后期限](#life-after-death)

### 项目状态 {#project-status}

为与群组关联的新创建项目配置以下任何首选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>允许用户在不使用模板的情况下创建项目</td>
<td><p>此首选项允许用户在从以下区域创建项目时不使用模板来创建项目：</p>
<ul>
<li><p>在项目列表中使用“新建项目”选项</p></li>

<li><p>将问题从问题页面转换为项目</p></li>
</ul>

<p>默认情况下，系统级别会启用此首选项。</p>
<p><b>注释</b></p>
<p>当用户属于具有不同首选项的多个组时，如果用户的组中至少有一个组启用了此首选项，则允许该用户创建不带模板的项目。</p>
</td></tr>
  <tr> 
   <td role="rowheader">将新项目的状态设置为</td> 
   <td> <p>确定新项目的状态。</p> <p><b>注释</b>   
     <ul> 
      <li>如果您或其他Workfront管理员隐藏了此处选择的状态，则默认状态将变为状态列表中的第一个状态。</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">对于组项目首选项，您只能选择锁定状态或必需状态作为默认状态。</li> 
      <li> <p>如果锁定的系统或组状态设置为默认状态，稍后有人将其解锁，则系统会尝试将其替换为相同状态类型的锁定状态。</p> <p>如果找不到，则会查找必需的状态：</p> 
       <ul> 
        <li>如果存在等同于已解锁默认状态的必需状态，则必需状态将变为默认状态，即使它已解锁也是如此。</li> 
        <li>如果所有必需状态均不等于已解锁的默认状态，则状态列表中的第一个必需状态将成为默认状态。</li> 
       </ul> <p>有关必需状态的信息，请参阅文章 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">访问系统项目状态列表</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">访问系统任务状态列表</a>和 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">访问系统问题状态列表</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">根据</td> 
   <td> <p>项目或父任务的完成百分比取决于任务的整体进度。 此信息可以根据项目任务的持续时间或计划小时数来计算。</p> <p>如果选择“持续时间”，则项目中每项任务的“持续时间”将确定项目的总体完成百分比，而每个子任务的“持续时间”则确定其父任务的整体完成百分比。</p> <p>如果选择持续时间，请确保在时间轴部分中指定每个工作日的典型小时数和每周的典型工作日。 Workfront在根据持续时间计算任务完成百分比时会使用此信息。 </p> <p>如果选择“计划小时数”，请确保每个项目上的所有任务都定义了计划小时数，并且该金额不为零。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">自动根据进度状态设置项目的条件</td> 
   <td> <p>此首选项允许用户手动设置项目的条件（在Target中、在风险中、在故障中），或让Workfront根据项目在时间轴上的进度自动设置条件（进度状态）。 有关项目条件的详细信息，请参阅 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">项目条件和条件类型概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>自动创建基准</p> </td> 
   <td> <p>当项目状态变为“当前”时，此首选项会自动创建任务和项目详细信息的基线（快照）。 有关创建基线的信息，请参阅 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">创建项目基线</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>绩效指数方法 </p> </td> 
   <td> <p>项目的绩效指数方法(PIM)控制Workfront用于计算挣值量度(如成本绩效指数(CPI)和完成时估计(EAC))的方法。 有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">计算成本绩效指数(CPI)</a>和 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">完成时计算估计(EAC)</a></p> 
    <ul> 
     <li><strong>基于小时</strong>:Workfront使用“计划时数”来计算EAC和CPI等绩效指标。 当PIM基于小时计算时，EAC将显示为小时数。 确保您的“计划小时数”值不是零。</li> 
     <li> <p><strong>基于成本</strong>:Workfront使用计划人工成本来计算EAC和CPI等绩效指标。 确保您的工作角色或用户与每小时成本费率相关联。 当根据成本计算PIM时，EAC将显示为货币值。</p> <p>项目经理可以使用项目详细信息中的“财务”区域在项目级别修改此设置。有关详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">在项目财务区管理信息</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>完工估算 </p> </td> 
   <td> <p>确定Workfront用哪些数据来计算“完成时估计”(EAC)，该数据表示项目的预计总成本。</p> 
    <ul> 
     <li><strong>在项目级别计算</strong>：父任务和项目的EAC通过在EAC公式中输入“实际工时”或“实际人工成本”来确定。 此计算包括直接添加到父任务或项目的实际工时或成本和费用。</li> 
     <li> <p><strong>从任务/子任务汇总</strong>:父任务和项目的EAC通过汇总每个子任务的EAC来确定。 此计算不包括直接添加到父任务或项目的实际工时数或实际成本和费用。</p> <p>项目经理可以使用项目详细信息中的“财务”区域在项目级别修改此设置。有关详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">在项目财务区管理信息</a>.</p> </li> 
    </ul> <p>有关EAC如何计算的更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">完成时计算估计(EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 时间线 {#timelines}

为与群组关联的新创建项目配置以下任何首选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">时间表开始日期</td> 
   <td> <p>确定新项目是从开始日期还是从创建时的完成日期开始计划。</p> 
    <ul> 
     <li><strong>开始日期</strong>:新任务默认为“尽快”任务约束，并提示项目经理为项目提供计划起始日期。</li> 
     <li><strong>完成日期</strong>:新任务默认为“尽可能晚的任务约束”，系统会提示项目经理为项目提供计划完成日期。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">用户空闲时间</td> 
   <td> <p>确定任务的主要任务负责人的休假时间是否调整项目上该任务的计划日期。</p> 
    <ul> 
     <li> <p><strong>考虑任务持续时间中的用户休息时间</strong>:为任务的主要任务负责人计划的任何休息时间，如果该休息时间在任务的持续时间内发生，则会调整任务的计划日期。 这是默认设置。 </p> <p>例如，如果具有“尽快约束”的任务计划在6月1日开始，并在6月3日完成，而主要受分配人将6月2日标记为“超时”，则任务的计划日期将调整为6月1日至6月4日。</p> <p><b>重要信息</b>:选择此设置后，任务的持续时间不会更改。 只有计划日期会更改，具体取决于任务约束。</p> </li> 
     <li><strong>忽略任务持续时间中的用户超时</strong>:项目上每个任务的计划日期仍保持原计划状态，即使任务的主要受分配人在任务的持续时间内有超时。</li> 
    </ul> <p>选择此设置的选项时，请考虑以下事项：</p> 
    <ul> 
     <li>当您更改此设置时，只有在更改后创建的项目和模板才会继承更新的设置。 </li> 
     <li> <p>任务的“任务约束”值确定要调整的计划任务日期： </p> 
      <ul> 
       <li>计划开始日期</li> 
       <li>计划完成日期</li> 
       <li>两个日期</li> 
       <li>都没约会。 </li> 
      </ul> <p>例如，如果任务具有固定日期约束，则当主要任务负责人有时间关闭时，即使选择了“考虑任务持续时间中的用户时间”选项，日期也不会调整。 有关任务约束的信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">任务约束概述</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>将自动重新计算项目时间线</strong> </p> </td> 
   <td> <p>确定项目的时间表何时重新计算。 有关重新计算项目时间轴的信息，请参阅 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新计算项目时间表</a>.</p> <p>默认启用以下选项。 您可以选择以下一个或多个设置：</p> 
    <ul> 
     <li> <p><strong>每晚</strong>:选择此选项可每天晚上重新计算项目时间轴。 您对项目所做的任何可能影响时间轴的更改不会立即显示。 Workfront​只​​会在夜间重新计算满足以下两个条件的项目的时间表：</p> <p> 
       <ul> 
        <li>状态为“当前”</li> 
        <li>过去3个月里有过更新</li> 
       </ul> </p> </li> 
     <li> <p><strong>当项目的范围发生更改时</strong>:选择此选项可在项目范围发生更改时立即重新计算项目时间轴。 有关构成项目范围更改的内容的信息，请参阅 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新计算项目时间表</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>当多个用户被分配到任务时，请使用</strong> </p> </td> 
   <td> <p>如果项目没有分配计划，或者如果分配给其任务的用户没有分配计划，则Workfront会使用系统默认计划来计算任务的时间表。</p> <p>如果在项目中为同一任务分配了多个用户，并且分配给这些任务的用户也分配了计划，则Workfront会使用以下计划：</p> 
    <ul> 
     <li><strong>主要分配</strong>:Workfront使用任务上的主要分配计划来计算时间轴。</li> 
     <li><strong>项目</strong>:Workfront使用项目计划来计算每个任务的时间轴。</li> 
    </ul> <p>有关计划的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">创建计划</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>时间线计算 </p> </td> 
   <td> 
    <ul> 
     <li><strong>每个工作日的典型小时数</strong>:为正在项目中工作的用户设置典型工作日的小时数。 默认为8小时。</li> 
    </ul> 
    <ul> 
     <li><strong>每周的典型工作日</strong>:为将要处理项目的用户设置标准工作周。 默认值为5天。</li> 
    </ul> <p>这2个选项会将天转换为小时，或将周转换为天。</p> <p>例如，如果您的任务具有8个计划小时，并且持续时间是根据计划小时计算的，则Workfront会将这些小时转换为天，以便将持续时间显示为天。</p> <p>从每周典型工作天数字段中，Workfront计算系统的全职等效(FTE)值。 这是Workfront在计算用户分配时使用的方法。</p> <p>当您计划项目时间表、资源预算或记录项目的时间时，会使用这些值。 </p> <p>在为系统中的用户建立工时单时，不会使用这些工时单，如 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">配置工时单和工时首选项</a>.</p> <p><b>注意</b>:Workfront管理员无法解锁“时间轴计算”首选项。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>自定义季度</strong> </p> </td> 
   <td> <p>为将要处理项目的用户配置自定义每年季度。 自定义季度通常是与日历年中传统的季度划分不匹配的季度。 您可以添加多个自定义季度。 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">为项目启用自定义季度</a>.</p> <p><b>注意</b>:Workfront管理员无法解锁“自定义季度”首选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 业务案例 {#business-cases}

您可以为与组关联的新创建项目创建业务案例，以提交项目请求。 您可以定义首选项以确定哪些区域在 **商业案例** 表单。 我们建议您启用这些选项，以便其他工具(如Portfolio优化器)能够正确更新。 有关每个字段显示内容的更多信息，请参阅 [定义业务案例](../../../manage-work/projects/define-a-business-case/define-business-case.md).

在Workfront管理员启用“业务案例”部分后，项目所有者可以在项目级别创建“业务案例”。 有关创建业务案例的信息，请参阅 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### 结束后期限  {#life-after-death}

为与群组关联的新创建项目配置以下任何首选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>将项目标记为“完成”后，仍然可以</strong> </p> </td> 
   <td> <p>确定贵组织（或组，如果要为组配置项目首选项）的规则，以确定在项目状态标记为“完成”后是否可以删除任务或问题。</p> 
    <ul> 
     <li><strong>删除任务</strong>:允许用户在将项目标记为完成后从项目中删除任务。<br></li> 
     <li><strong>删除问题</strong>:允许用户在将项目标记为完成后从项目中删除问题。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>项目被标记为“完成”、“已停用”或“待批”后，仍然可以</strong> </p> </td> 
   <td> <p>确定贵组织（或组，如果要为组配置项目首选项）的规则，以了解在标记项目状态后项目中的任务、问题、文档和其他对象会发生什么情况 <strong>完成</strong>, <strong>死亡</strong>或 <strong>待批准</strong>.</p> 
    <ul> 
     <li><strong>添加和编辑任务</strong> 允许用户： 
      <ul> 
       <li>在项目被标记为“完成”、“无效”或“待批准”后，编辑项目中的任务。 这包括添加小时和更改任务中的费用条目。</li> 
       <li>将任务添加到项目。</li> 
      </ul></li> 
     <li><strong>添加和编辑问题</strong>:允许用户： 
      <ul> 
       <li>在项目被标记为“完成”、“无效”或“待批准”后，编辑项目中的问题。</li> 
       <li>在项目标记为“完成”或“已停止”后，向项目添加问题。 （您无法向处于“待批准”状态的项目添加问题。）</li> 
      </ul></li> 
     <li> <p><strong>向项目及其任务和问题中添加文档</strong>:允许用户在项目被标记为“完成”或“无效”后向项目添加文档（或向项目中的任务和问题添加文档）。</p> <p>此选项不适用于待批准的项目。</p> </li> 
     <li> <p><strong>附加模板</strong>:允许用户在项目被标记为完成或停用后将模板附加到项目。</p> <p>此选项不适用于待批准的项目。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
