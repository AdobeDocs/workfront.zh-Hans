---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 配置系统范围的项目首选项
description: 作为 [!DNL Adobe Workfront] 管理员，您可以为在整个系统中创建的所有项目配置默认首选项。 这些首选项影响项目、任务和问题行为。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '2522'
ht-degree: 0%

---

# 配置系统范围的项目首选项

作为 [!DNL Adobe Workfront] 管理员，您可以为在整个系统中创建的所有项目配置默认首选项。 这些首选项影响项目、任务和问题行为。

>[!NOTE]
>
>默认情况下，这些首选项会被锁定，除非您为系统中的所有组解锁它们，否则组管理员无法在组级别修改它们。 有关更多信息，请参阅 [锁定或解锁系统中所有组的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[！UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是 [!DNL Workfront] 管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置整个组织的项目首选项

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **[!UICONTROL 项目首选项]** > **[!UICONTROL 项目]**.

1. 在出现的页面上，继续下面列出的四个部分之一以配置首选项 [!UICONTROL 项目状态]， [!UICONTROL 时间线]， [!UICONTROL 商业案例]、和 [!UICONTROL 死后期限].
1. 如果您希望整个组织中的所有组都使用相同的项目首选项，请确保锁定每个首选项 ![](assets/lock-toggle-button.png) （这是默认设置）。

   >[!IMPORTANT]
   >
   >锁定项目首选项后，对该首选项所做的任何更改都将由系统中的所有组继承。 务必与组织中的用户和组进行通信，以确保以配置项目首选项的方式考虑所有需求。

   有关解锁首选项以便所有组可以自行配置和管理该首选项的信息，请参阅 [锁定或解锁系统中所有组的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. 单击&#x200B;**[!UICONTROL 保存]**。

* [[!UICONTROL 项目状态]](#project-status)
* [[!UICONTROL 时间线]](#timelines)
* [[!UICONTROL 商业案例]](#business-cases)
* [[!UICONTROL 死后期限]](#life-after-death)

### 项目状态 {#project-status}

在整个系统中为新创建的项目配置以下任一首选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL允许用户在不使用模板的情况下创建项目]</td> 
   <td>  <p>此首选项允许用户在从以下区域创建项目时创建项目，而不使用模板： </p>
      <ul>
        <li>
        <p>在项目列表中使用[！UICONTROL新建项目]选项</p>
        </li>
          <li>
          <p>从问题页面将问题转化为项目</p>
          </li>
         </ul>
        <p>默认情况下，此首选项处于启用状态。 </p> 
        <p><b>注释</b></p>
        <p> 组管理员可以更改组的此首选项。 当用户属于具有不同首选项的多个组时，如果用户的主组启用了此首选项，则允许用户创建没有模板的项目。</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[！UICONTROL将新项目的状态设置为]</td> 
   <td> <p>确定新项目的状态。</p>  <p><b>注意</b>  
     <ul> 
      <li>如果您或另一个 [!DNL Workfront] 管理员将隐藏此处选择的状态，默认状态将更改为状态列表中的第一个状态。</li> 
     </ul> 
     <ul> 
      <li> <p>如果将锁定的系统或组状态设置为默认状态，稍后有人将其解锁，则系统会尝试将其替换为相同状态类型的锁定状态。</p> <p>如果找不到，则会查找所需的状态：</p> 
       <ul> 
        <li>如果具有相当于已解锁默认状态的必需状态，则该必需状态将成为默认状态，即使已解锁也是如此。</li> 
        <li>如果任何所需状态都不等同于已解锁的默认状态，则状态列表中的第一个所需状态将成为默认状态。</li> 
       </ul> <p>有关所需状态的信息，请参阅文章 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">访问系统项目状态的列表</a>， <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">访问系统任务状态的列表</a>、和 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">访问系统问题状态的列表</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL根据计算完成百分比]</td> 
   <td> <p>项目或父任务的完成百分比基于任务的总体进度。 此信息可根据项目上任务的持续时间或计划小时数计算。</p> <p>如果选择[！UICONTROL持续时间]，项目中每个任务的持续时间将决定项目的整体完成百分比，每个子任务的持续时间将决定其父任务的整体完成百分比。</p> <p>如果选择[！UICONTROL Duration]，请确保在[！UICONTROL时间线]部分中指定[！UICONTROL每工作日典型小时数]和[！UICONTROL每周典型工作日数]。 [!DNL Workfront] 在基于持续时间计算任务的完成百分比时，将使用此信息。 </p> <p>如果您选择[！UICONTROL计划小时数]，请确保每个项目上的所有任务都定义了[！UICONTROL计划小时数]的数量，并且该数量不为零。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL根据进度状态自动设置项目条件]</td> 
   <td> <p>此首选项允许用户手动设置项目的[！UICONTROL Condition] ([！UICONTROL On Target]、[！UICONTROL At Risk]、[！UICONTROL In Trouble])或具有 [!DNL Workfront] 根据项目在时间线上的进度自动设置[！UICONTROL条件]（进度状态）。 有关项目条件的更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">项目完成情况和完成情况类型概览</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL自动创建基线]</p> </td> 
   <td> <p>当项目状态更改为[！UICONTROL当前]时，此首选项会自动创建任务和项目详细信息的基线（快照）。 有关创建基线的信息，请参见 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">创建项目基线</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL绩效指数方法] </p> </td> 
   <td> <p>项目的绩效指数方法(PIM)控制此方法 [!DNL Workfront] 使用计算实现值指标，如[！UICONTROL成本绩效指数] (CPI)和[！UICONTROL完工估算] (EAC)。 有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">计算[！UICONTROL成本绩效指数] (CPI)</a> 和 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[！UICONTROL计算完工估算] (EAC)</a></p> 
    <ul> 
     <li><strong>[！UICONTROL Hour-based]</strong>： [!DNL Workfront] 使用[！UICONTROL计划小时数]计算性能量度，如EAC和CPI。 当基于小时数计算PIM时，EAC显示为小时数。 确保您有[！UICONTROL计划小时数]的值，而不是零。</li> 
     <li> <p><strong>[！UICONTROL Cost-based]</strong>： [!DNL Workfront] 使用[！UICONTROL计划劳力成本]计算EAC和CPI等绩效指标。 确保您的工作角色或用户与每小时成本费率相关联。 当基于成本计算PIM时，EAC显示为货币值。</p> <p>项目经理可以使用[！UICONTROL项目详细信息]中的[！UICONTROL财务]区域在项目级别修改此设置。 有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">管理项目[！UICONTROL财务]区域中的信息</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL完工估算]</p> </td> 
   <td> <p>确定哪些数据 [!DNL Workfront] 使用计算[！UICONTROL完工估算] (EAC)，它表示项目的预计总成本。</p> 
    <ul> 
     <li><strong>[！UICONTROL在项目级别计算]</strong>：父任务和项目的EAC通过在EAC公式中输入[！UICONTROL实际小时数]或[！UICONTROL实际劳力成本]来确定。 此计算包括直接添加到父级任务或项目的[！UICONTROL实际小时数]或[！UICONTROL成本和费用]。</li> 
     <li> <p><strong>[！UICONTROL从任务/子任务汇总]</strong>：父任务和项目的EAC通过汇总每个子任务的EAC来确定。 此计算不包括直接添加到父级任务或项目的[！UICONTROL实际小时数]或[！UICONTROL实际成本和费用]。</p> <p>项目经理可以使用[！UICONTROL项目详细信息]中的[！UICONTROL财务]区域在项目级别修改此设置。有关详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">管理项目[！UICONTROL财务]区域中的信息</a>.</p> </li> 
    </ul> <p>有关EAC如何计算的更多信息，请参见 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">计算[！UICONTROL完工估算] (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 时间线 {#timelines}

在整个系统中为新创建的项目配置以下任一首选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL计划来源]</td> 
   <td> <p>确定从创建新项目开始日期还是从创建项目完成日期开始计划新项目。</p> 
    <ul> 
     <li><strong>[！UICONTROL开始日期]</strong>：新任务默认为[！UICONTROL Task Constraint Leascast]，并且会提示项目经理提供项目的[！UICONTROL计划开始日期]。</li> 
     <li><strong>[！UICONTROL完成日期]</strong>：新任务默认为[！UICONTROL Task Constraint Latest Category]，并且系统会提示项目经理提供项目的[！UICONTROL规划完成日期]。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL用户空闲时间]</td> 
   <td> <p>确定任务的主要被分配人的休假是否调整了项目上该任务的计划日期。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL考虑任务持续时间中的用户空闲时间]</strong>：如果为任务的主要被分配者安排的任何休息时间出现在任务持续时间中，则会调整任务的计划日期。 这是默认设置。 </p> <p>例如，如果一项约束为[！UICONTROL的任务计划于6月1日开始并在6月3日完成，而主要被分配人将6月2日标记为休假，则该任务的计划日期将调整为6月1日至6月4日。</p> <p><b>重要</b>：选择此设置时，任务的持续时间不会更改。 根据任务限制，只有计划的日期会更改。</p> </li> 
     <li><strong>[！UICONTROL忽略任务持续时间中的用户空闲时间]</strong>：项目上每个任务的计划日期仍保持原计划，即使任务的主要被分配人在任务持续时间里有空闲时间。</li> 
    </ul> <p>为此设置选择选项时，请考虑以下事项：</p> 
    <ul> 
     <li>在更改此设置时，只有更改后创建的项目和模板才会继承更新的设置。 </li> 
     <li> <p>任务的任务限制值确定要调整的计划任务日期： </p> 
      <ul> 
       <li>计划开始日期</li> 
       <li>计划完成日期</li> 
       <li>两个日期</li> 
       <li>两者都不是。 </li> 
      </ul> <p>例如，如果任务的限制为[！UICONTROL固定日期]，则当主要被分配者具有空闲时间时，日期不会调整，即使选择了选项[！UICONTROL考虑用户在任务持续时间内的空闲时间]也是如此。 有关任务限制的信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">任务限制概述</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL项目时间表将自动重新计算]</p> </td> 
   <td> <p>确定重新计算项目时间线的时间。 有关重新计算项目时间线的信息，请参阅 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新计算项目时间表</a>.</p> <p>默认启用以下选项。 您可以选择以下一个或多个设置：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL，每晚]</strong>：选择此项以每晚重新计算项目时间线。 您对项目所做的任何可能影响时间线的更改不会立即可见。 [!DNL Workfront​​​] 仅当满足以下两个条件时，才在夜间重新计算项目的时间表：</p> <p> 
       <ul> 
        <li>状态为[！UICONTROL Current]</li> 
        <li>在过去3个月中进行了更新</li> 
        <li>具有下列更新类型之一：</li>
        <ul>
        <li>更改时自动更新</li>
        <li>仅在更改时更新</li>
        <li>仅自动更新</li> 
      </ul>       
    <b>提示</b>
    <p>更新类型为仅手动的项目不受此设置的影响。</p>
    <li> <p><strong>当项目范围更改时</strong>：选择此项可在项目范围发生更改时立即重新计算项目时间线。 有关构成项目范围更改的内容的信息，请参见 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新计算项目时间表</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL当多个用户被分配到任务时，使用]的计划</p> </td> 
   <td> <p>如果项目未分配计划，或分配给其任务的用户未分配计划， [!DNL Workfront] 使用系统默认计划计算任务的时间线。</p> <p>如果将多个用户分配给一个项目中的同一任务，并且分配给该任务的用户也分配了计划，则[！UICONTROL Workfront]将使用以下计划：</p> 
    <ul> 
     <li><strong>[！UICONTROL主要分配]</strong>： [!DNL Workfront] 使用任务上主要分配的时间表来计算时间表。</li> 
     <li><strong>[！UICONTROL项目]</strong>： [!DNL Workfront] 使用项目的计划来计算每项任务的时间表。</li> 
    </ul> <p>有关时间表的详细信息，请参见 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">创建计划</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[！UICONTROL时间表计算] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL通常每工作日小时数]</strong>：为将处理项目的用户设置典型工作日的小时数。 默认值为8小时。</li> 
    </ul> 
    <ul> 
     <li><strong>[！UICONTROL每周典型工作日]</strong>：为将处理项目的用户设置标准工作周。 默认值为5天。</li> 
    </ul> <p>这2个选项会将天转换为小时，或将周转换为天。</p> <p>例如，如果您有一个具有8个计划小时数的任务，并且持续时间基于计划小时数计算， [!DNL Workfront] 将那些小时转换为天，以便将持续时间显示为天。</p> <p>从典型的[！UICONTROL每周工作日]字段中， [!DNL Workfront] 计算系统的相当于全职(FTE)值。 这是什么 [!DNL Workfront] 在计算用户分配时使用。</p> <p>当您计划项目时间线、资源预算或针对项目记录时间时，可以使用这些值。 </p> <p>在系统中为用户建立时间表时，不使用这些时间表，如中所述 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[！UICONTROL配置]时间表和小时首选项</a>.</p> <p><b>注意</b>： [!DNL Workfront] 管理员无法解锁[！UICONTROL时间线计算]首选项。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[！UICONTROL自定义季度]</p> </td> 
   <td> <p>为将处理项目的用户配置自定义年度季度。 自定义季度通常是不匹配日历年内传统季度划分的季度。 您可以添加多个自定义季度。 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">为项目启用自定义季度</a>.</p>  <p><b>注意</b>： [!DNL Workfront] 管理员无法解锁[！UICONTROL自定义季度]首选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 商业案例] {#business-cases}

您可以为整个系统内新创建的项目创建业务案例，以提交项目请求。 您可以定义首选项以确定哪些区域在 **[!UICONTROL 商业论证]** 表单。 我们建议您启用这些选项，以便其他工具(例如 [!UICONTROL Portfolio优化器]，请正确更新。 有关每个字段显示的内容的更多信息，请参阅 [定义业务案例：文章索引](../../../manage-work/projects/define-a-business-case/define-business-case.md).

在 [!DNL Workfront] 管理员启用 [!UICONTROL 商业论证]之后，项目所有者可以在项目级别创建业务案例。 有关创建业务案例的信息，请参阅 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL 死后期限] {#life-after-death}

在整个系统中为新创建的项目配置以下任一首选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL将项目标记为完成之后，人员还可以] </p> </td> 
   <td> <p>确定组织（或组，如果您正在为组配置项目偏好设置）的有关在项目状态标记为[！UICONTROL完成]后是否可以删除任务或问题的规则。</p> 
    <ul> 
     <li><strong>[！UICONTROL删除任务]</strong>：允许用户在项目被标记为[！UICONTROL完成]后从项目中删除任务。<br></li> 
     <li><strong>[！UICONTROL删除问题]</strong>：允许用户在项目被标记为[！UICONTROL完成]后从项目中删除问题。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL将项目标记为“完成”、“废弃”或“未决批准”后，人员还可以]</p> </td> 
   <td> <p>确定组织（或组，如果您正在为组配置项目首选项）的规则，这些规则涉及在标记项目状态后项目中任务、问题、文档和其他对象发生的情况 <strong>[！UICONTROL完成]</strong>， <strong>[！UICONTROL终止]</strong>，或是 <strong>[！UICONTROL未决批准]</strong>.</p> 
    <ul> 
     <li><strong>[！UICONTROL添加和编辑任务]</strong> 允许用户执行以下操作：
      <ul>
       <li>在项目被标记为[！UICONTROL完成]、[！UICONTROL停止]或为[！UICONTROL未决批准]之后编辑项目中的任务。 这包括添加小时数和更改任务的费用条目。</li>
       <li>将任务添加到项目。</li>
      </ul></li> 
     <li><strong>[！UICONTROL添加和编辑问题]</strong>：允许用户执行以下操作：
      <ul>
       <li>将项目标记为[！UICONTROL完成]、[！UICONTROL停止]或[！UICONTROL未决批准后，编辑项目中的问题。</li>
       <li>将问题添加到标记为[！UICONTROL完成]或[！UICONTROL停止]的项目。 （您无法向处于[！UICONTROL未决批准]状态的项目添加问题。）</li>
      </ul></li> 
     <li> <p><strong>[！UICONTROL将文档添加到项目及其任务和问题]</strong>：允许用户在将该项目标记为[！UICONTROL完成]或[！UICONTROL停止]后，将文档添加到项目（或将文档添加到项目中的任务和问题）。</p> <p>此选项不适用于未决批准的项目。</p> </li> 
     <li> <p><strong>[！UICONTROL附加模板]</strong>：允许用户在项目被标记为[！UICONTROL完成]或[！UICONTROL停止]后将模板附加到项目。</p> <p>此选项不适用于未决批准的项目。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
