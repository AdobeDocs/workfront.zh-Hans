---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 配置系统范围的项目首选项
description: 作为 [!DNL Adobe Workfront] 管理员，您可以为整个系统中创建的所有项目配置默认首选项。 这些首选项会影响项目、任务和问题行为。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '2475'
ht-degree: 1%

---

# 配置系统范围的项目首选项

作为 [!DNL Adobe Workfront] 管理员，您可以为整个系统中创建的所有项目配置默认首选项。 这些首选项会影响项目、任务和问题行为。

>[!NOTE]
>
>默认情况下，这些首选项会被锁定，组管理员无法在组级别修改它们，除非您为整个系统中的所有组解锁它们。 有关更多信息，请参阅 [锁定或解锁系统中所有组的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 为整个组织配置项目首选项

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **[!UICONTROL 项目首选项]** > **[!UICONTROL 项目]**.

1. 在显示的页面上，继续下面列出的4个部分之一，以配置 [!UICONTROL 项目状态], [!UICONTROL 时间轴], [!UICONTROL 商业案例]和 [!UICONTROL 死后生命].
1. 如果您希望组织内的所有组都使用相同的项目首选项，请确保锁定每个首选项 ![](assets/lock-toggle-button.png) （这是默认设置）。

   >[!IMPORTANT]
   >
   >锁定项目首选项后，系统中的所有组都会继承您对该首选项所做的任何更改。 务必要与整个组织中的用户和组进行通信，以确保在配置项目首选项时满足所有需求。

   有关解锁首选项以便所有组都可以自行配置和管理首选项的信息，请参阅 [锁定或解锁系统中所有组的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. 单击&#x200B;**[!UICONTROL 保存]**。

* [[!UICONTROL 项目状态]](#project-status)
* [[!UICONTROL 时间线]](#timelines)
* [[!UICONTROL 业务案例]](#business-cases)
* [[!UICONTROL 结束后期限]](#life-after-death)

### 项目状态 {#project-status}

在系统中为新创建的项目配置以下任何首选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL允许用户在不使用模板的情况下创建项目]</td> 
   <td>  <p>此首选项允许用户在从以下区域创建项目时不使用模板来创建项目： </p>
      <ul>
        <li>
        <p>在项目列表中使用[!UICONTROL新建项目]选项</p>
        </li>
          <li>
          <p>将问题从问题页面转换为项目</p>
          </li>
         </ul>
        <p>默认情况下，此首选项处于启用状态。 </p> 
        <p><b>注释</b></p>
        <p> 群组管理员可以更改群组的此首选项。 当用户属于具有不同首选项的多个组时，如果用户的主组启用了此首选项，则允许该用户创建不带模板的项目。</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL将新项目的状态设置为]</td> 
   <td> <p>确定新项目的状态。</p>  <p><b>注释</b>  
     <ul> 
      <li>如果您或其他 [!DNL Workfront] 管理员将隐藏此处选择的状态，默认状态将变为状态列表中的第一个状态。</li> 
     </ul> 
     <ul> 
      <li> <p>如果锁定的系统或组状态设置为默认状态，稍后有人将其解锁，则系统会尝试将其替换为相同状态类型的锁定状态。</p> <p>如果找不到，则会查找必需的状态：</p> 
       <ul> 
        <li>如果存在等同于已解锁默认状态的必需状态，则必需状态将变为默认状态，即使它已解锁也是如此。</li> 
        <li>如果所有必需状态均不等于已解锁的默认状态，则状态列表中的第一个必需状态将成为默认状态。</li> 
       </ul> <p>有关必需状态的信息，请参阅文章 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">访问系统项目状态列表</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">访问系统任务状态列表</a>和 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">访问系统问题状态列表</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL根据]计算完成百分比</td> 
   <td> <p>项目或父任务的完成百分比取决于任务的整体进度。 此信息可以根据项目任务的持续时间或计划小时数来计算。</p> <p>如果选择[!UICONTROL持续时间]，项目中每个任务的持续时间将确定项目的总体完成百分比，而每个子任务的持续时间将确定其父任务的整体完成百分比。</p> <p>如果选择[!UICONTROL Duration]，请确保在[!UICONTROL Timelines]部分中指定[!UICONTROL Typical hours per work day]和[!UICONTROL Typical work days per week]。 [!DNL Workfront] 根据持续时间计算任务完成百分比时，会使用此信息。 </p> <p>如果选择[!UICONTROL计划时间]，请确保每个项目上的所有任务都定义了[!UICONTROL计划时间]，并且该金额不为零。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL根据进度状态自动设置项目的条件]</td> 
   <td> <p>此首选项允许用户手动设置项目的[!UICONTROL条件]（在Target中为[!UICONTROL]、[!UICONTROL At Risk]、[!UICONTROL In Foure]），或者 [!DNL Workfront] 根据项目在时间轴上的进度自动设置[!UICONTROL条件]（进度状态）。 有关项目条件的详细信息，请参阅 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">项目条件和条件类型概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL自动创建基线]</p> </td> 
   <td> <p>当项目状态更改为[!UICONTROL Current]时，此首选项会自动创建任务和项目详细信息的基线（快照）。 有关创建基线的信息，请参阅 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">创建项目基线</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL性能索引方法] </p> </td> 
   <td> <p>项目的性能指数方法(PIM)控制该方法 [!DNL Workfront] 用于计算挣值量度，如[!UICONTROL成本绩效指数](CPI)和[!UICONTROL Estimate At Completion](EAC)。 有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">计算[!UICONTROL成本绩效指数](CPI)</a> 和 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL完成时计算估计](EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL基于小时]</strong>: [!DNL Workfront] 使用[!UICONTROL计划时数]来计算EAC和CPI等性能量度。 当PIM基于小时计算时，EAC将显示为小时数。 确保您的[!UICONTROL计划时数]值为零，而不是零。</li> 
     <li> <p><strong>[!UICONTROL基于成本]</strong>: [!DNL Workfront] 使用[!UICONTROL计划人工成本]来计算EAC和CPI等绩效指标。 确保您的工作角色或用户与每小时成本费率相关联。 当根据成本计算PIM时，EAC将显示为货币值。</p> <p>项目经理可以使用[!UICONTROL项目详细信息]中的[!UICONTROL Finance]区域在项目级别修改此设置。 有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">在项目[!UICONTROL Finance]区域中管理信息</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL完成时估计]</p> </td> 
   <td> <p>确定哪些数据 [!DNL Workfront] 用于计算[!UICONTROL完成时估计](EAC)，它表示项目的预计总成本。</p> 
    <ul> 
     <li><strong>[!UICONTROL在项目级别计算]</strong>：通过在EAC公式中输入[!UICONTROL实际工时]或[!UICONTROL实际人工成本]，可确定父任务和项目的EAC。 此计算包括直接添加到父任务或项目的[!UICONTROL实际小时数]或[!UICONTROL成本和费用]。</li> 
     <li> <p><strong>[!UICONTROL从任务/子任务汇总]</strong>:父任务和项目的EAC通过汇总每个子任务的EAC来确定。 此计算不包括直接添加到父任务或项目的[!UICONTROL实际小时数]或[!UICONTROL实际成本和费用]。</p> <p>项目经理可以使用[!UICONTROL项目详细信息]中的[!UICONTROL Finance]区域在项目级别修改此设置。有关详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">在项目[!UICONTROL Finance]区域中管理信息</a>.</p> </li> 
    </ul> <p>有关EAC如何计算的更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">在完成时计算[!UICONTROL估计](EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 时间线 {#timelines}

在系统中为新创建的项目配置以下任何首选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL计划自]</td> 
   <td> <p>确定新项目是从开始日期还是从创建时的完成日期开始计划。</p> 
    <ul> 
     <li><strong>[!UICONTROL开始日期]</strong>:新任务默认为[!UICONTROL As Op H A Pess Of Sh Pess] Task Constraint，并提示项目经理为项目提供[!UICONTROL Planed Start Date]。</li> 
     <li><strong>[!UICONTROL完成日期]</strong>:新任务默认为[!UICONTROL As Late Ap A Poss Task Constraint]（尽可能晚）任务约束，系统会提示项目经理为项目提供[!UICONTROL计划完成日期]。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL用户关闭时间]</td> 
   <td> <p>确定任务的主要任务负责人的休假时间是否调整项目上该任务的计划日期。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL考虑任务持续时间中的用户超时]</strong>:为任务的主要任务负责人计划的任何休息时间，如果该休息时间在任务的持续时间内发生，则会调整任务的计划日期。 这是默认设置。 </p> <p>例如，如果某项具有[!UICONTROL Ass Op Hop Sop Hop]约束的任务计划在6月1日开始，并在6月3日完成，并且主要受分配人将6月2日标记为“超时”，则任务的计划日期将调整为6月1日至6月4日。</p> <p><b>重要信息</b>:选择此设置后，任务的持续时间不会更改。 只有计划日期会更改，具体取决于任务约束。</p> </li> 
     <li><strong>[!UICONTROL忽略任务持续时间中的用户超时]</strong>:项目上每个任务的计划日期仍保持原计划状态，即使任务的主要受分配人在任务的持续时间内有超时。</li> 
    </ul> <p>选择此设置的选项时，请考虑以下事项：</p> 
    <ul> 
     <li>当您更改此设置时，只有在更改后创建的项目和模板才会继承更新的设置。 </li> 
     <li> <p>任务的“任务约束”值确定要调整的计划任务日期： </p> 
      <ul> 
       <li>计划开始日期</li> 
       <li>计划完成日期</li> 
       <li>两个日期</li> 
       <li>都没约会。 </li> 
      </ul> <p>例如，如果任务的约束为[!UICONTROL固定日期]，则当主要任务负责人有时间关闭时，即使选择了选项[!UICONTROL Conser fuxed time in task duration]，日期也不会调整。 有关任务约束的信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">任务约束概述</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL项目时间轴将自动重新计算]</p> </td> 
   <td> <p>确定项目的时间表何时重新计算。 有关重新计算项目时间轴的信息，请参阅 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新计算项目时间表</a>.</p> <p>默认启用以下选项。 您可以选择以下一个或多个设置：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Vey night]</strong>:选择此选项可每天晚上重新计算项目时间轴。 您对项目所做的任何可能影响时间轴的更改不会立即显示。 [!DNL Workfront​​​] 仅在满足以下两个条件的项目晚上重新计算时间表：</p> <p> 
       <ul> 
        <li>状态为[!UICONTROL Current]</li> 
        <li>过去3个月里有过更新</li> 
       </ul> </p> </li> 
     <li> <p><strong>当项目的范围发生更改时</strong>:选择此选项可在项目范围发生更改时立即重新计算项目时间轴。 有关构成项目范围更改的内容的信息，请参阅 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新计算项目时间表</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL当将多个用户分配到任务时，请使用的计划]</p> </td> 
   <td> <p>如果项目未分配计划，或者如果分配给其任务的用户没有分配计划， [!DNL Workfront] 使用系统默认计划来计算任务的时间轴。</p> <p>如果在项目中为同一任务分配了多个用户，并且分配给这些任务的用户也分配了一个计划，[!UICONTROL Workfront]将使用以下计划：</p> 
    <ul> 
     <li><strong>[!UICONTROL主要分配]</strong>: [!DNL Workfront] 使用任务上的主要分配计划来计算时间轴。</li> 
     <li><strong>[!UICONTROL项目]</strong>: [!DNL Workfront] 使用项目的计划来计算每个任务的时间轴。</li> 
    </ul> <p>有关计划的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">创建计划</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL时间轴计算] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL每个工作日的典型小时数]</strong>:为正在项目中工作的用户设置典型工作日的小时数。 默认为8小时。</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL每周典型工作日]</strong>:为将要处理项目的用户设置标准工作周。 默认值为5天。</li> 
    </ul> <p>这2个选项会将天转换为小时，或将周转换为天。</p> <p>例如，如果您的任务具有8个计划小时，并且持续时间是根据计划小时计算的， [!DNL Workfront] 将这些小时转换为天，以将持续时间显示为天。</p> <p>从典型[!UICONTROL每周工作日]字段中， [!DNL Workfront] 计算系统的全时等效值(FTE)值。 这就是 [!DNL Workfront] 在计算用户分配时使用。</p> <p>当您计划项目时间表、资源预算或记录项目的时间时，会使用这些值。 </p> <p>在为系统中的用户建立工时单时，不会使用这些工时单，如 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL配置]工时单和小时首选项</a>.</p> <p><b>注意</b>: [!DNL Workfront] 管理员无法解锁[!UICONTROL时间轴计算]首选项。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL自定义季度]</p> </td> 
   <td> <p>为将要处理项目的用户配置自定义每年季度。 自定义季度通常是与日历年中传统的季度划分不匹配的季度。 您可以添加多个自定义季度。 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">为项目启用自定义季度</a>.</p>  <p><b>注意</b>: [!DNL Workfront] 管理员无法解锁[!UICONTROL自定义季度]首选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 业务案例] {#business-cases}

您可以为整个系统中新创建的项目创建业务案例，以提交项目请求。 您可以定义首选项以确定哪些区域在 **[!UICONTROL 商业案例]** 表单。 我们建议您启用这些选项，以便其他工具(例如 [!UICONTROL Portfolio优化程序]，请正确更新。 有关每个字段显示内容的更多信息，请参阅 [定义业务案例](../../../manage-work/projects/define-a-business-case/define-business-case.md).

在 [!DNL Workfront] 管理员在 [!UICONTROL 商业案例]，项目所有者随后可以在项目级别创建业务案例。 有关创建业务案例的信息，请参阅 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL 结束后期限] {#life-after-death}

在系统中为新创建的项目配置以下任何首选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL将项目标记为完成后，仍然可以] </p> </td> 
   <td> <p>确定贵组织（或组，如果您正在为组配置项目首选项）的规则，以确定在项目状态标记为[!UICONTROL完成]后是否可以删除任务或问题。</p> 
    <ul> 
     <li><strong>[!UICONTROL删除任务]</strong>:允许用户在将项目标记为[!UICONTROL完成]后从项目中删除任务。<br></li> 
     <li><strong>[!UICONTROL删除问题]</strong>:允许用户在项目被标记为[!UICONTROL Complete]后从项目中删除问题。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL在项目被标记为“完成”、“已停用”或“待批准”后，仍然可以]</p> </td> 
   <td> <p>确定贵组织（或组，如果要为组配置项目首选项）的规则，以了解在标记项目状态后项目中的任务、问题、文档和其他对象会发生什么情况 <strong>[!UICONTROL Complete]</strong>, <strong>[!UICONTROL Dead]</strong>或 <strong>[!UICONTROL Pending Approval]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL添加和编辑任务]</strong> 允许用户：
      <ul>
       <li>在项目被标记为[!UICONTROL Complete]、[!UICONTROL Dead]或为[!UICONTROL Pending Approval]后，编辑项目中的任务。 这包括添加小时和更改任务中的费用条目。</li>
       <li>将任务添加到项目。</li>
      </ul></li> 
     <li><strong>[!UICONTROL添加和编辑问题]</strong>:允许用户：
      <ul>
       <li>在将项目标记为[!UICONTROL Complete]、[!UICONTROL Dead]或[!UICONTROL Pending Approval]后，编辑项目中的问题。</li>
       <li>在项目被标记为[!UICONTROL Complete]或[!UICONTROL Dead]后，向项目添加问题。 （您无法向[!UICONTROL待批准]的项目添加问题。）</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL向项目及其任务和问题中添加文档]</strong>:允许用户在项目被标记为[!UICONTROL Complete]或[!UICONTROL Dead]后，向项目添加文档（或向项目中的任务和问题添加文档）。</p> <p>此选项不适用于待批准的项目。</p> </li> 
     <li> <p><strong>[!UICONTROL附加模板]</strong>:允许用户在项目被标记为[!UICONTROL Complete]或[!UICONTROL Dead]后，将模板附加到项目。</p> <p>此选项不适用于待批准的项目。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
