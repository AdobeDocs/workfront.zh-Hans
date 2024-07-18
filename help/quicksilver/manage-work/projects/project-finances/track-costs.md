---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: 跟踪成本
description: 您可以在Adobe Workfront中跟踪项目、任务和问题的成本。
author: Lisa
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: d431ae178a157522e2b5d8d963da7b0623510d28
workflow-type: tm+mt
source-wordcount: '2480'
ht-degree: 0%

---

# 跟踪成本

<!-- Audited: 02/2024 -->

您可以在Adobe Workfront中跟踪项目、任务和问题的成本。

## Workfront如何计算成本

要跟踪成本，您必须将用户和职位角色与小时成本费率关联。

每小时成本率是与工作角色或用户关联的每个工作单位的成本额。 将费率乘以工作花费小时数会产生项目、任务或问题的成本。

存在以下情况：

* 如果任务的成本类型为“用户小时”，则用户小时费率会计算任务和项目成本。

  有关将用户与成本费率关联的信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

* 如果任务的成本类型为“每小时职责”，则工作职责小时费率会计算任务和项目成本。

  有关将工作角色与成本费率关联的信息，请参阅[创建和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

* Workfront只计算问题的实际成本，而问题没有成本类型。 有关详细信息，请参阅本文中的[Workfront如何跟踪问题的成本](#how-workfront-tracks-costs-for-issues)部分。

>[!TIP]
>
>您无法覆盖项目的成本费率。 一旦您建立了用户或工作角色的每小时成本费率，该费率将计算系统中的所有成本。

## Workfront成本绩效指数

Workfront会计算项目的许多成本绩效指数，以便可以跟踪项目以获得成本效益。\
有关计算成本 — 性能指标的详细信息，请参阅：

* [计算成本绩效指数(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [计算成本计划绩效指数(CSI)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [计算计划绩效指数(SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Workfront如何跟踪任务和项目的成本

任务和项目的成本类型计算方式不同。

### Workfront如何跟踪成本 {#how-workfront-tracks-costs}

在Workfront中，您可以跟踪任务和项目的多种类型成本。 总成本按以下公式计算：

`Costs = Labor Costs + Expense Costs`

* **劳力成本**&#x200B;与任务和项目的小时数以及与任务关联的资源的每小时成本费率相关联。 通常，Workfront会计算以下人工成本：

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>计划劳力成本</td> 
     <td> <p>它们使用以下公式计算：</p><code>Planned Labor Costs = Planned Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>预算劳力成本</td> 
     <td> <p>它们使用以下公式计算：</p><code>Budgeted Labor Costs = Budgeted Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>实际劳力成本</td> 
     <td> <p>它们使用以下公式计算：</p><code>Actual Labor Costs = Actual Hours * Cost per Hour rate</code> </td> 
    </tr> 
   </tbody> 
  </table>

  有关详细信息，请参阅本文中的[Workfront如何计算计划成本、预算成本和实际成本](#how-workfront-calculates-planned-budgeted-and-actual-costs)部分。

* **费用成本**&#x200B;与项目和任务上的费用相关联。\
  在创建项目时，您可以为整个项目设置计划费用。 此外，您可以将费用与新任务或现有任务关联。 有关信息，请参阅[管理项目费用](../../../manage-work/projects/project-finances/manage-project-expenses.md)。

* **固定成本**&#x200B;定义为项目的固定成本金额。 这是项目计划成本的一部分，它表示完成项目所需的资金额。

  >[!TIP]
  >
  >将模板附加到项目时，模板的固定成本将添加到项目的固定成本。 有关信息，请参阅[将模板附加到项目的概述](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md)。

### Workfront如何计算计划成本、预算成本和实际成本 {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront计算项目中每个单独任务的计划成本和实际成本。 Workfront将这些计算用于单个任务，以计算项目的计划成本和实际成本。

#### 规划成本 {#planned-cost}

项目的计划成本是与项目上的计划工作（计划小时数）关联的成本。

项目的计划成本按以下公式计算：

`Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project`

例如，任务的费用选项卡上有以下费用：100美元的营销费用和50美元的管理费用。 在“财务”标签中，选择“用户小时成本”类型。 用户被分配给任务，用户的小时费率为$15。 用户在该任务中被分派工作5小时。 在项目的“费用”选项卡中，您有一个称为“咨询”的费用的$100计划成本。 您还有项目的$200固定成本。

项目的计划成本计算如下：

`$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525`

公式中的小时费率会考虑该费率的任何日期有效更改。

#### 预算成本 {#budgeted-cost}

项目的预算成本是与项目的预算工作（预算小时数）关联的成本。

如果满足以下两个条件，则项目的预算成本与项目的计划成本相同：

* 项目上任务的计划小时数与预算小时数（在资源规划者中）匹配。
* 任务的计费类型为“每小时角色”。

如果满足以下条件，则使用下面的公式计算项目的预算成本：

* 项目上任务的计划小时数与预算小时数（在资源规划者中）不匹配。
* 任务的计费类型为“每小时角色”。

当满足上述条件时，Workfront使用以下公式计算项目的预算成本：

`Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project`

#### 实际成本 {#actual-cost}

项目的实际成本是与项目实际工时（记录的小时数）关联的成本。

实际成本使用以下公式计算：

`Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project`

例如，任务的费用选项卡上有以下费用：实际成本为$110的营销费用以及实际成本为$40的管理费用。 选择“每小时角色”成本类型，然后将“顾问”工作角色分配给任务。 顾问工作角色的费率为$15/小时，并且顾问工作角色的任务记录了6个小时。 有一个与项目关联的咨询费用（在“费用”选项卡中），其实际成本为$100，且用户配置文件中的每小时成本率为$20的用户在项目上记录了10小时。 您还有项目的$200固定成本。

项目的实际成本计算如下：

`$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740`

公式中的小时费率会考虑该费率的任何日期有效更改。

>[!NOTE]
>
>项目的实际费用成本计算如下：
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>在实际成本计算中不会复制这些成本。 例如，如果固定成本是项目实际费用成本的一部分，它不会单独添加到实际成本。

>[!NOTE]
>
>在记录项目时间时，在计算项目的实际人工成本时存在以下方案：
>
>* 默认情况下，Workfront使用用户的每小时成本费率来计算实际劳力成本。
>* 如果记录时间的用户未与任何成本相关联，则Workfront使用用户的主要角色的每小时成本费率。
>* 如果您的Workfront管理员在“设置”的“时间表和小时首选项”区域中启用了&#x200B;**手动将工作角色分配给小时条目**&#x200B;设置，并且项目的用户登录时间选择了其他要与此时间关联的角色，则项目的实际成本将根据在记录小时数时指定的角色进行计算。 有关为特定工作角色启用日志记录时间的信息，请参阅文章[配置时间表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

### Workfront如何计算任务的成本类型 {#how-workfront-calculates-cost-types-for-tasks}

任务的计划和实际成本及其人工成本由每个任务的成本类型确定。

您可以为项目中的各个任务配置成本类型。 每种成本类型都会影响计划成本和实际成本值。

有关如何修改任务的成本类型的信息，请参阅[更新任务成本类型](../../../manage-work/tasks/task-information/update-task-cost-type.md)。

下表介绍了Workfront中可用的任务成本类型：

<table style="table-layout:auto">
 <col> 
 <col> 
<tbody> 
  <tr> 
   <td> <p><strong>任务成本类型</strong> </p> </td> 
   <td> <p><strong>描述</strong> </p> </td> 
  </tr>
  <tr> 
   <td> <p>用户每小时</p> </td> 
   <td> <p>这是创建任务时的默认成本类型。</p> <p><strong>计划成本</strong>按以下公式计算： </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>其中计划劳力成本的计算方式：<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>注意： <p>考虑使用用户小时成本类型和计算计划成本的以下影响：</p> 
     <ul> 
      <li>如果将多个资源分配给任务，Workfront会根据分配给每个资源的任务的百分比来调整计划成本的计算。</li>
      <li>对于日期有效成本率，计划人工成本是任务中涵盖的每个时间期的计划成本的总和。</li>
      <li>根据您是从任务本身还是从“利用率”报表查看计划成本，计划成本字段的值可能会有所不同。<br><strong>从任务本身查看计划成本时：</strong>“计划成本”字段会考虑在工作角色级别设置的“成本/小时”字段（如果未在用户级别设置成本/小时）。<br><strong>从项目的利用率报告中查看计划成本时：</strong>计划成本字段未考虑在工作角色级别设置的成本/小时字段。 相反，如果您希望“利用率”报表考虑在“工作职责”层设置的“成本/小时”字段，则必须将任务的“成本类型”设置为“每小时职责”。 </li> 
     </ul> </p> <p><strong>实际成本</strong>按以下公式计算： </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>其中实际劳力成本的计算方法为：</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>例如，用户档案中的每小时成本费率为$20。 当他们为一项任务记录5个小时时，该任务的实际人工成本为$100。 如果用户没有与其关联的每小时成本费率，则实际成本会根据其主要工作角色的每小时成本费率计算。 如果他们没有工作角色，或者未定义其工作角色的每小时成本费率，则任务的实际成本为零。 </p> <p>注：实际成本是根据记录时间的用户的每小时成本费率计算的，而不考虑分配给任务的用户。 此外，公式中的开单小时费率会考虑该费率的任何日期有效更改。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>角色每小时</p> </td>
   <td> <p><strong>计划成本</strong>按以下公式计算： </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>其中任务计划劳力成本的计算方式：</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>注：如果将多个资源分配给任务，则Workfront会根据分配给每个资源的任务百分比来调整计划小时数的计算。 此外，公式中的小时费率会考虑该费率的任何日期有效更改。</p> <p><strong>实际成本</strong>按以下公式计算： </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>其中任务实际人工成本的计算方法为：</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>例如，将任务分配给工作角色或具有工作角色的用户，其每小时成本费率为$20。 当用户为任务记录5小时时，该任务的实际人工成本为$100。 如果分配给任务的用户在任务中没有与其关联的工作角色，则实际成本将根据其主要工作角色的每小时成本费率进行计算。 如果他们没有工作角色，或者未定义其工作角色的每小时成本费率，则任务的实际成本为零。 </p> <p>注：角色小时任务的实际小时数是根据与任务关联的用户的工作角色计算的，而不是根据与记录时间的用户关联的角色计算的。 此外，公式中的开单小时费率会考虑该费率的任何日期有效更改。</p> <p>如果您的Workfront管理员在“设置”的“时间表和小时首选项”区域中启用了<strong>手动将工作角色分配给小时条目</strong>设置，并且任务的用户登录时间选择了其他要与此时间关联的角色，则“角色每小时”任务的实际成本会根据记录小时数时指定的角色进行计算。 有关为特定工作角色启用日志记录时间的信息，请参阅文章<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">配置时间表和小时首选项</a>。</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定每小时</p> </td> 
   <td> <p><strong>计划成本</strong>按以下公式计算：</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>其中任务人工成本的计算方法为：</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>实际成本</strong>按以下公式计算： </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>其中，实际任务人工成本的计算方法为：</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>此成本类型不考虑个人用户或工作角色。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>无成本</p> </td> 
   <td> <p>此成本类型不会影响成本。 如果父任务具有此成本类型，则具有另一成本类型的子任务会根据其各自的成本类型进行计算，父任务的成本也会相应地受到影响。 </p> <p>当对财务数据没有访问权限的用户或对模板没有财务权限的用户从该模板创建项目时，这是项目上任务的默认成本类型。</p> <p>有关访问财务数据的信息，请参阅文章<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予对财务数据的访问权限</a>。</p> <p>有关对象的财务权限的信息，请参阅文章<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">共享对象的财务权限</a>。</p> <p>有关从模板创建项目的信息，请参阅文章<a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">使用模板创建项目</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront如何跟踪问题的成本 {#how-workfront-tracks-costs-for-issues}

问题不存在并且不会影响项目的以下成本类型：

* 规划成本
* 预算成本

但是，问题可能具有&#x200B;**实际成本**，这也会影响项目的实际成本。

下表说明如何根据问题的分配类型计算问题的实际成本：

<table style="table-layout:auto"> 
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td> <p>用户分配</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>实际成本</strong>按以下公式计算：</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>此处会考虑记录时间的用户的每小时成本率，而不管该问题是谁分配的。 </p> <p>如果记录时间的用户在其用户档案中没有每小时成本费率，则其主要工作角色的每小时成本费率会计算问题的实际成本。</p> <p>如果记录时间的用户在其配置文件中没有角色或没有与其关联的费率，则使用问题中主要受分配人的主要工作角色的每小时成本费率计算实际小时数。 如果该职责未定义费率，则问题的实际成本为零。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>角色分配</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>实际成本</strong>按以下公式计算：</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>此处考虑记录问题时间的用户的每小时成本率，而不管该问题被分配了什么角色。 </p> <p>如果记录时间的用户没有与其关联的每小时成本费率，则其主要角色的每小时成本费率会计算问题的实际成本。</p><p>如果记录时间的用户在配置文件中没有角色或没有与其关联的费率，则问题的实际成本为零。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>无分配</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>实际成本</strong>按以下公式计算：</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>如果记录时间的用户没有与其配置文件关联的每小时成本费率，则其主要工作角色的每小时成本费率将计算问题的实际成本。 </p> <p>如果记录时间的用户没有与其配置文件关联的工作角色，或其主要工作角色未定义每小时成本费率，则问题的实际成本为零。 </p> </td> 
  </tr> 
 </tbody> 
</table>
