---
title: 配置组的项目首选项
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: 如果您是组管理员并且Adobe Workfront管理员为系统中的所有组解锁了项目首选项，则可以为组配置该首选项，以影响您的组创建的所有后续项目。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '2658'
ht-degree: 2%

---

# 配置组的项目首选项

如果您是组管理员并且Adobe Workfront管理员为系统中的所有组解锁了项目首选项，则可以为组配置该首选项，以影响您的组创建的所有后续项目。

如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员也是如此（适用于任何组）。

>[!NOTE]
>
>* 通常，已解锁的首选项会无限期地保持解锁状态。 如果Workfront管理员将其重新锁定，则系统设置将再次生效，并且组管理员所做的首选项设置将丢失。
>* 为与项目关联的组设置的首选项优先于为创建项目的用户的主组设置的首选项。
>* 某些组级首选项会影响您为组创建的项目模板。 有关更多信息，请参阅部分 [从组区域查看、处理和创建组模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) 在文章中 [创建和修改组的项目模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Workfront管理员在系统级别解锁首选项后，您可以对其进行配置，然后将其锁定，以确保您的组及其子组中的每个人都使用相同的配置。 此功能与Workfront管理员为系统中的每个人配置和锁定首选项的功能相同。 有关更多信息，请参阅 [锁定或解锁子组的项目、任务或问题偏好设置](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

此外，还可为任务和问题偏好设置以及时间表和小时偏好设置进行组级别配置。 有关信息，请参阅 [配置组的任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) 和 [配置组的工时表与小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

有关Workfront管理员如何解锁项目首选项的信息，请参阅 [锁定或解锁系统中所有组的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系Workfront管理员。

## 为组配置已解锁的项目首选项

>[!TIP]
>
>如果您是Workfront管理员，则可以绕过步骤1-4，方法是转到设置>项目偏好设置>项目，然后在页面顶部的框中搜索组的名称。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **组** ![](assets/groups-icon.png).

1. 单击要配置其项目首选项的组的名称。
1. 在左侧面板中，单击 **项目首选项**.
1. 在显示的页面上，继续下面列出的四个部分之一，以配置项目状态、时间线、业务案例和生存时间首选项。

   >[!TIP]
   >
   >如果将鼠标悬停在某个首选项上，并且会显示工具提示来告诉您该首选项已被锁定，则可以请求Workfront管理员为组织中的所有组解锁该首选项。

* [项目状态](#project-status)
* [时间线](#timelines)
* [商业案例](#business-cases)
* [结束后期限](#life-after-death)

### 项目状态 {#project-status}

为与该组关联的新创建项目配置以下任一首选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>允许用户在不使用模板的情况下创建项目</td>
<td><p>此首选项允许用户在从以下区域创建项目时创建项目，而不使用模板：</p>
<ul>
<li><p>在项目列表中使用新建项目选项</p></li>

<li><p>从问题页面将问题转化为项目</p></li>
</ul>

<p>默认情况下，此首选项在系统级别启用。</p>
<p><b>注释</b></p>
<p>当用户属于具有不同首选项的多个组时，如果用户至少有一个组启用了此首选项，则允许用户创建没有模板的项目。</p>
</td></tr>
  <tr> 
   <td role="rowheader">将新项目的状态设置为</td> 
   <td> <p>确定新项目的状态。</p> <p><b>注意</b>   
     <ul> 
      <li>如果您或其他Workfront管理员隐藏此处选择的状态，则默认状态将更改为状态列表中的第一个状态。</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">对于组项目首选项，您只能选择锁定状态或所需状态作为默认状态。</li> 
      <li> <p>如果将锁定的系统或组状态设置为默认状态，稍后有人将其解锁，则系统会尝试将其替换为相同状态类型的锁定状态。</p> <p>如果找不到，则会查找所需的状态：</p> 
       <ul> 
        <li>如果具有相当于已解锁默认状态的必需状态，则该必需状态将成为默认状态，即使已解锁也是如此。</li> 
        <li>如果任何所需状态都不等同于已解锁的默认状态，则状态列表中的第一个所需状态将成为默认状态。</li> 
       </ul> <p>有关所需状态的信息，请参阅文章 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">访问系统项目状态的列表</a>， <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">访问系统任务状态的列表</a>、和 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">访问系统问题状态的列表</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">计算完成百分比，依据为</td> 
   <td> <p>项目或父任务的完成百分比基于任务的总体进度。 此信息可根据项目上任务的持续时间或计划小时数计算。</p> <p>如果选择“持续时间”，项目中每个任务的持续时间将决定项目的整体完成百分比，而每个子任务的持续时间将决定其父任务的整体完成百分比。</p> <p>如果选择持续时间，请确保在时间线部分指定每工作日典型小时数和每周典型工作日。 在根据持续时间计算任务的完成百分比时，Workfront将使用此信息。 </p> <p>如果选择计划小时数，请确保每个项目的所有任务都定义了计划小时数金额，并且该金额不为零。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">自动根据进度状态设置项目的条件</td> 
   <td> <p>此首选项允许用户手动设置项目的条件（已设定目标、有风险、存在问题），或让Workfront根据项目在时间线上的进度自动设置条件（进度状态）。 有关项目条件的更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">项目完成情况和完成情况类型概览</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>自动创建基准</p> </td> 
   <td> <p>当项目状态更改为当前时，此首选项会自动创建任务和项目详细信息的基线（快照）。 有关创建基线的信息，请参见 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">创建项目基线</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>绩效指数方法 </p> </td> 
   <td> <p>项目的绩效指数方法(PIM)控制Workfront用于计算实现值指标的方法，例如成本绩效指数(CPI)和完工估算(EAC)。 有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">计算成本绩效指数(CPI)</a>和 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">计算完工估算(EAC)</a></p> 
    <ul> 
     <li><strong>基于小时</strong>：Workfront使用计划小时数计算性能量度，如EAC和CPI。 当基于小时数计算PIM时，EAC显示为小时数。 确保您具有除零以外的计划小时数的值。</li> 
     <li> <p><strong>基于成本</strong>：Workfront使用计划劳力成本计算绩效指标，如EAC和CPI。 确保您的工作角色或用户与每小时成本费率相关联。 当基于成本计算PIM时，EAC显示为货币值。</p> <p>项目经理可以使用项目详细信息中的财务区域，在项目级别修改此设置。有关详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">管理项目财务方面的信息</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>完工估算 </p> </td> 
   <td> <p>确定Workfront用于计算代表项目预计总成本的完工估算(EAC)的数据。</p> 
    <ul> 
     <li><strong>在项目级别计算</strong>：父任务和项目的EAC通过在EAC公式中输入实际小时数或实际人工成本来确定。 此计算包括直接添加到父级任务或项目的实际小时数或成本和费用。</li> 
     <li> <p><strong>从任务/子任务汇总</strong>：父任务和项目的EAC通过汇总每个子任务的EAC来确定。 此计算不包括直接添加到父任务或项目的实际小时数或实际成本和费用。</p> <p>项目经理可以使用项目详细信息中的财务区域，在项目级别修改此设置。有关详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">管理项目财务方面的信息</a>.</p> </li> 
    </ul> <p>有关EAC如何计算的更多信息，请参见 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">计算完工估算(EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 时间线 {#timelines}

为与该组关联的新创建项目配置以下任一首选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">时间表开始日期</td> 
   <td> <p>确定从创建新项目开始日期还是从创建项目完成日期开始计划新项目。</p> 
    <ul> 
     <li><strong>开始日期</strong>：新任务默认为尽快任务限制，并提示项目经理提供项目的计划开始日期。</li> 
     <li><strong>完成日期</strong>：新任务默认为“尽可能晚的任务限制”，并提示项目经理提供项目的计划完成日期。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">用户空闲时间</td> 
   <td> <p>确定任务的主要被分配人的休假是否调整了项目上该任务的计划日期。</p> 
    <ul> 
     <li> <p><strong>考虑任务持续时间中的用户空闲时间</strong>：如果为任务的主要被分配者安排的任何休息时间出现在任务持续时间中，则会调整任务的计划日期。 这是默认设置。 </p> <p>例如，如果一项带有尽可能早限制的任务的计划于6月1日开始并在6月3日完成，而主要被分配人将6月2日标记为休假，则该任务的计划日期将调整为6月1日至6月4日。</p> <p><b>重要</b>：选择此设置时，任务的持续时间不会更改。 根据任务限制，只有计划的日期会更改。</p> </li> 
     <li><strong>忽略任务持续时间中的用户空闲时间</strong>：项目上每个任务的计划日期仍保持原计划，即使任务的主要被分配人在任务持续时间里有空闲时间。</li> 
    </ul> <p>为此设置选择选项时，请考虑以下事项：</p> 
    <ul> 
     <li>在更改此设置时，只有更改后创建的项目和模板才会继承更新的设置。 </li> 
     <li> <p>任务的任务限制值确定要调整的计划任务日期： </p> 
      <ul> 
       <li>计划开始日期</li> 
       <li>计划完成日期</li> 
       <li>两个日期</li> 
       <li>两者都不是。 </li> 
      </ul> <p>例如，如果任务的限制为固定日期，则当主要被分配者具有空闲时间时，日期不会调整，即使选择了考虑任务持续时间中的用户空闲时间选项也是如此。 有关任务限制的信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">任务限制概述</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>将自动重新计算项目时间线</strong> </p> </td> 
   <td> <p>确定重新计算项目时间线的时间。 有关重新计算项目时间线的信息，请参阅 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新计算项目时间表</a>.</p> <p>默认启用以下选项。 您可以选择以下一个或多个设置：</p> 
    <ul> 
     <li> <p><strong>每晚</strong>：选择此项以每晚重新计算项目时间线。 您对项目所做的任何可能影响时间线的更改不会立即可见。 仅当同时满足以下两个条件时​ ​，Workfront​才在夜间重新计算项目的时间表：</p> <p> 
       <ul> 
        <li>状态为“当前”</li> 
        <li>在过去3个月中进行了更新</li> 
       </ul> </p> </li> 
     <li> <p><strong>当项目范围更改时</strong>：选择此项可在项目范围发生更改时立即重新计算项目时间线。 有关构成项目范围更改的内容的信息，请参见 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新计算项目时间表</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>当多个用户被分派到一个任务时，使用</strong> </p> </td> 
   <td> <p>如果项目未分配计划，或分配给其任务的用户未分配计划，则Workfront使用系统默认计划计算任务的时间线。</p> <p>如果将多个用户分配给一个项目中的同一任务，并且分配给该任务的用户也分配了计划，则Workfront将使用以下计划：</p> 
    <ul> 
     <li><strong>主要分配</strong>：Workfront使用任务中主要分配的时间表计算时间线。</li> 
     <li><strong>项目</strong>：Workfront使用项目的计划计算每项任务的时间表。</li> 
    </ul> <p>有关时间表的详细信息，请参见 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">创建计划</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>时间线计算 </p> </td> 
   <td> 
    <ul> 
     <li><strong>通常每工作日的小时数</strong>：为将处理项目的用户设置典型工作日的小时数。 默认值为8小时。</li> 
    </ul> 
    <ul> 
     <li><strong>通常每周的工作日数</strong>：为将处理项目的用户设置标准工作周。 默认值为5天。</li> 
    </ul> <p>这2个选项会将天转换为小时，或将周转换为天。</p> <p>例如，如果您有一个具有8个计划小时数的任务并且持续时间是根据计划小时数计算的，则Workfront会将这些小时数转换为天数，以便将持续时间显示为天。</p> <p>Workfront会从“每周典型工作日”字段计算系统的相当于全职(FTE)值。 这是Workfront在计算用户分配时使用的内容。</p> <p>当您计划项目时间线、资源预算或针对项目记录时间时，可以使用这些值。 </p> <p>在系统中为用户建立时间表时，不使用这些时间表，如中所述 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">配置时间表和小时首选项</a>.</p> <p><b>注意</b>：Workfront管理员无法解锁时间线计算首选项。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>自定义季度</strong> </p> </td> 
   <td> <p>为将处理项目的用户配置自定义年度季度。 自定义季度通常是不匹配日历年内传统季度划分的季度。 您可以添加多个自定义季度。 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">为项目启用自定义季度</a>.</p> <p><b>注意</b>：Workfront管理员无法解锁自定义季度首选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 业务案例 {#business-cases}

您可以为与组关联的新创建项目创建业务案例，以提交项目请求。 您可以定义首选项以确定哪些区域在 **商业论证** 表单。 我们建议您启用这些选项，以便其他工具(如Portfolio优化器)正确更新。 有关每个字段显示的内容的更多信息，请参阅 [定义业务案例：文章索引](../../../manage-work/projects/define-a-business-case/define-business-case.md).

在Workfront管理员启用业务案例的部分后，项目所有者可以在项目级别创建业务案例。 有关创建业务案例的信息，请参阅 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### 结束后期限  {#life-after-death}

为与该组关联的新创建项目配置以下任一首选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>将项目标记为完成之后，人员还可以</strong> </p> </td> 
   <td> <p>确定组织（或组，如果您正在为组配置项目首选项）的规则，这些规则涉及在项目状态标记为“完成”后是否可以删除任务或问题。</p> 
    <ul> 
     <li><strong>删除任务</strong>：允许用户在项目被标记为完成之后从项目中删除任务。<br></li> 
     <li><strong>删除问题</strong>：允许用户在项目被标记为完成之后从项目中删除问题。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>将项目标记为“完成”、“停止”或“未决批准”后，人员还可以</strong> </p> </td> 
   <td> <p>确定组织（或组，如果您正在为组配置项目首选项）的规则，这些规则涉及在标记项目状态后项目中任务、问题、文档和其他对象发生的情况 <strong>完成</strong>， <strong>废弃</strong>，或是 <strong>未决批准</strong>.</p> 
    <ul> 
     <li><strong>添加和编辑任务</strong> 允许用户执行以下操作： 
      <ul> 
       <li>在项目被标记为“完成”、“停止”或“未决批准”之后编辑项目中的任务。 这包括添加小时数和更改任务的费用条目。</li> 
       <li>将任务添加到项目。</li> 
      </ul></li> 
     <li><strong>添加和编辑问题</strong>：允许用户执行以下操作： 
      <ul> 
       <li>在项目被标记为“完成”、“停止”或“未决批准”后，编辑项目中的问题。</li> 
       <li>在项目被标记为完成或废弃后将问题添加到项目。 （您无法将问题添加到未决批准的项目。）</li> 
      </ul></li> 
     <li> <p><strong>将文档添加到项目及其任务和问题</strong>：允许用户在项目被标记为完成或终止后将文档添加到项目（或将文档添加到项目中的任务和问题）。</p> <p>此选项不适用于未决批准的项目。</p> </li> 
     <li> <p><strong>附加模板</strong>：允许用户在项目被标记为完成或停止后将模板附加到项目。</p> <p>此选项不适用于未决批准的项目。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
