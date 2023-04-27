---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: 跟踪成本
description: 您可以在Adobe Workfront中跟踪项目、任务和问题的成本。
author: Alina
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: d8c274d2153836647367c263cad8d786402cbe7f
workflow-type: tm+mt
source-wordcount: '2372'
ht-degree: 1%

---

# 跟踪成本

您可以在Adobe Workfront中跟踪项目、任务和问题的成本。

## Workfront如何计算成本

为了跟踪成本，您必须将用户和职务角色与每小时成本比率相关联。

每小时成本费率是与职务角色或用户关联的每个工作单位的成本金额。 将比率乘以工作所花费的小时数，可为您的项目、任务或问题生成成本。

存在以下情形：

* 如果任务的成本类型是“用户每小时”，则用户每小时费率会计算任务和项目成本。

   有关将用户与成本费率关联的信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 如果任务的成本类型是“职责：每小时”，则任务职责每小时费率将计算任务和项目成本。

   有关将任务职责与成本费率关联的信息，请参阅 [创建和管理作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront仅计算问题的实际成本，并且问题没有成本类型。 有关更多信息，请参阅 [Workfront如何跟踪问题成本](#how-workfront-tracks-costs-for-issues) 在本文中。

>[!TIP]
>
>您不能改写项目的成本费率。 在用户或任务职责上确定每小时成本费率后，该费率将计算系统中的所有成本。

## Workfront成本绩效指标

Workfront会为项目计算多个成本绩效指标，以便能够跟踪项目以提高成本效率。\
有关计算成本 — 性能指标的详细信息，请参阅：

* [计算成本绩效指数(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [计算成本计划绩效指数(CSI)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [计算计划性能索引(SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Workfront如何跟踪任务和项目成本

* [Workfront如何跟踪成本](#how-workfront-tracks-costs)
* [Workfront如何计算计划、预算和实际成本](#how-workfront-calculates-planned-budgeted-and-actual-costs)
* [Workfront如何计算任务的成本类型](#how-workfront-calculates-cost-types-for-tasks)

### Workfront如何跟踪成本  {#how-workfront-tracks-costs}

您可以在Workfront中跟踪任务和项目的几种成本类型。 整体成本按以下公式计算：

```
Costs = Labor Costs + Expense Costs
```

* **人工成本** 与任务和项目的小时数以及与任务关联的资源的每小时成本比率相关联。 通常，Workfront会计算以下人工成本：

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>计划人工成本</td> 
     <td> <p>使用以下公式计算这些值：</p><pre>计划人工成本=计划小时数x每小时成本费率</pre> </td> 
    </tr> 
    <tr> 
     <td>预算人工成本</td> 
     <td> <p>使用以下公式计算这些值：</p><pre>预算人工成本=预算小时数x每小时成本率</pre> </td> 
    </tr> 
    <tr> 
     <td>实际人工成本</td> 
     <td> <p>使用以下公式计算这些值：</p><pre>实际人工成本=实际工时数x每小时成本费率</pre> </td> 
    </tr> 
   </tbody> 
  </table>

   有关更多信息，请参阅 [Workfront如何计算计划、预算和实际成本](#how-workfront-calculates-planned-budgeted-and-actual-costs) 章节。

* **费用成本** 与项目和任务的费用相关联。\
   在创建项目时，您可以为整个项目设置计划费用。 此外，您还可以将费用与新任务或现有任务相关联。 有关信息，请参阅 [管理项目费用](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **固定成本** 定义为项目的固定成本金额。 这是项目计划成本的一部分，该成本表示完成项目所需的资金额。

   >[!TIP]
   >
   >将模板附加到项目时，模板的固定成本会添加到项目的固定成本中。 有关信息，请参阅 [将模板附加到项目的概述](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Workfront如何计算计划、预算和实际成本 {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront计算项目中每个任务的计划成本和实际成本。 Workfront将这些计算用于单个任务，以计算项目的计划成本和实际成本。

* [计划成本](#planned-cost)
* [预算成本](#budgeted-cost)
* [实际成本](#actual-cost)

#### 计划成本 {#planned-cost}

项目的计划成本是与项目的计划工作（计划时数）关联的成本。

项目的计划成本按以下公式计算：

```
Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project
```

例如，任务的“费用”标签中有以下费用：$100的营销费用和$50的管理费用。 在“财务”选项卡中，选择“用户每小时”成本类型。 为用户分配了任务，用户每小时的费率是$15。 分配用户在此任务上工作5小时。 在项目的“费用”标签中，您有一个名为“咨询”的费用的$100计划成本。 此外，您还有200美元的项目固定成本。

项目的计划成本计算如下：

```
$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525
```

#### 预算成本 {#budgeted-cost}

项目的预算成本是与项目的预算工作（预算小时数）相关的成本。

如果满足以下两个条件，则项目的预算成本与项目的计划成本相同：

* 项目上任务的计划小时数与预算小时数（在资源计划器中）匹配
* 任务“开单类型”为“角色每小时”。

如果满足以下条件，则使用下面的公式计算项目的预算成本：

* 项目任务的计划小时数与预算小时数（在资源计划器中）不匹配
* 任务的开单类型是“角色：每小时”。

满足上述条件后，Workfront将使用以下公式计算项目的预算成本：
<pre>预算项目成本=预算人工成本+预算费用所有任务的成本+预算费用项目成本</pre>

#### 实际成本 {#actual-cost}

项目的实际成本是与项目的实际工作（记录的小时数）相关的成本。

实际成本使用以下公式计算：

```
Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project
```

例如，任务的“费用”标签中有以下费用：a实际成本为$110的营销费用和实际成本为$40的管理费用。 您选择角色每小时成本类型，并为任务分配顾问职务角色。 顾问工作角色的费率为每小时15美元，并且顾问工作角色的任务已记录6小时。 与项目关联的咨询费用（在“费用”选项卡中）为100美元的实际成本，而用户在项目的用户配置文件日志中10小时的每小时成本费率为20美元。 此外，您还有200美元的项目固定成本。

项目的实际成本计算如下：

```
$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740
```

>[!NOTE]
>
>在项目上记录时间时，在计算项目的实际人工成本时，存在以下情况：
>
>* 默认情况下，Workfront使用用户的“每小时成本”比率来计算实际人工成本。
>* 如果用户记录时间与任何成本都无关联，则Workfront会使用用户主要角色的每小时成本费率。
>* 如果您的Workfront管理员启用了 **将作业角色手动分配给小时条目** 在“工时单和小时首选项”区域中进行设置，并且项目的用户日志记录时间会选择与此时间关联的其他角色，因此项目的实际成本会根据记录小时时指定的角色进行计算。 有关为特定作业角色启用日志记录时间的信息，请参阅文章 [配置工时单和工时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
>


### Workfront如何计算任务的成本类型 {#how-workfront-calculates-cost-types-for-tasks}

任务的计划成本和实际成本及其人工成本由每项任务的成本类型确定。

您可以为项目中的各个任务配置成本类型。 每个成本类型都会影响计划成本和实际成本值。

有关如何修改任务成本类型的信息，请参阅 [更新任务成本类型](../../../manage-work/tasks/task-information/update-task-cost-type.md).

下表介绍了Workfront中的可用任务成本类型：

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任务成本类型</strong> </p> </th> 
   <th> <p><strong>描述</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>用户小时</p> </td> 
   <td> <p>这是创建任务时的默认成本类型。</p> <p><strong>计划成本</strong> 使用以下公式计算： </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>计划人工成本的计算方式为：<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>注释:   <p>考虑使用用户每小时成本类型和计算计划成本的以下影响：</p> 
     <ul> 
      <li>如果您为任务分配了多个资源，则Workfront会根据分配给每个资源的任务的百分比来调整计划成本的计算。</li> 
      <li>“计划成本”字段的值可能会因您查看任务本身或“利用率”报表中的计划成本而异。<br><strong>从任务本身查看计划成本时：</strong> “计划成本”字段考虑在任务职责层设置的“成本/人力”字段（如果尚未在用户层设置“成本/人力”字段）。<br><strong>在从项目的“利用率”报表中查看计划成本时：</strong> “计划成本”字段不考虑在任务职责层设置的“成本/人力资源”字段。 相反，如果您希望利用率报表考虑在任务职责层设置的成本/人力资源字段，则必须将任务上的成本类型设置为“每小时”职责。 </li> 
     </ul> </p> <p><strong>实际成本</strong> 使用以下公式计算： </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>其中实际人工成本的计算方式为：</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>例如，用户的配置文件中的每小时成本费率为$20。 当他们记录某项任务的5小时时，该任务的实际人工成本为$100。 如果用户没有与其关联的每小时成本费率，则实际成本将根据其主要任务职责的每小时成本费率计算。 如果它们没有职务职责，或者未定义其职务职责的“每小时成本”费率，则任务的“实际成本”为零。 </p> <p>注意：实际成本是根据正在记录时间的用户的每小时成本费率计算的，而不管谁被分配给任务。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>角色小时</p> </td> 
   <td> <p><strong>计划成本</strong> 使用以下公式计算： </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>其中，任务计划人工成本的计算方式为：</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>注意：如果您为一个任务分配了多个资源，则Workfront会根据分配给每个资源的任务的百分比来调整“计划小时数”的计算。</p> <p><strong>实际成本</strong> 使用以下公式计算： </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>其中任务实际人工成本的计算方式为：</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>例如，任务被分配给职务角色或具有职务角色的用户，其每小时成本费率为$20。 当用户为某项任务记录5小时时，该任务的实际人工成本为$100。 如果分配给任务的用户在任务上没有与其关联的任务职责，则实际成本将根据其主要任务职责的每小时成本费率计算。 如果它们没有职务职责，或者未定义其职务职责的“每小时成本”费率，则任务的“实际成本”为零。 </p> <p>注释:   <p> 根据与任务关联的用户的作业角色计算角色的实际小时数任务，而不是根据与记录时间的用户关联的角色计算。</p> <p>如果您的Workfront管理员启用了 <strong>将作业角色手动分配给小时条目</strong> 在“时间表和小时首选项”区域中进行设置，并且任务的用户日志记录时间选择与此时间关联的其他角色，则根据记录小时时指定的角色计算角色每小时任务的实际成本。 有关为特定作业角色启用日志记录时间的信息，请参阅文章 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">配置工时单和工时首选项</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定小时</p> </td> 
   <td> <p><strong>计划成本</strong> 使用以下公式计算：</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>其中，任务人工成本的计算方式为：</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>实际成本</strong> 使用以下公式计算： </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>其中实际任务人工成本的计算方式为：</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>此成本类型不考虑个人用户或作业角色。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>无成本</p> </td> 
   <td> <p>此成本类型不影响成本。 如果父任务具有此成本类型，则具有其他成本类型的子任务将根据其各自的成本类型进行计算，并且父任务的成本会相应地受到影响。 </p> <p>当对模板没有财务数据访问权限的用户或对模板没有财务权限的用户从该模板创建项目时，这是项目任务的默认成本类型。</p> <p>有关访问金融数据的信息，请参阅文章 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予对财务数据的访问权限</a>.</p> <p>有关对象的财务权限信息，请参阅文章 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">共享对象的财务权限</a>.</p> <p>有关从模板创建项目的信息，请参阅文章 <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">使用模板创建项目</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because this was moved to its own how-to article linked above. Could be removed after some time.) </p>
<p>To configure the Cost Type of an individual task:</p>
<ol>
<li value="1">Go to the task where you want to configure the Cost Type. </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then expand the <strong>Finance</strong> area. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Double click <strong>Cost Type</strong> and select the cost type that you want to apply to the task. </p> </li>
<li value="4">Click <strong>Save.</strong></li>
</ol>
</div>
-->

## Workfront如何跟踪问题成本 {#how-workfront-tracks-costs-for-issues}

问题不存在，也不影响项目的以下类型成本：

* 计划成本
* 预算成本

但是，问题可以 **实际成本** 也会影响项目的实际成本。

下表说明了根据问题的分配类型，如何计算问题的实际成本：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th colspan="4">发放实际成本</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>用户分配</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>实际成本</strong> 使用以下公式计算：</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>此处会考虑记录时间的用户的每小时成本率，无论谁被分配给了该问题。 </p> <p>如果记录时间的用户的配置文件中没有每小时成本费率，则其主要任务角色的每小时成本费率将计算问题的实际成本。 如果正在记录时间的用户在其配置文件中没有角色或没有与其关联的费率，则实际小时数将使用主要工作负责人在问题上的主要任务职责的每小时成本费率来计算。 如果该角色未定义费率，则问题的实际成本为零。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>角色分配</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>实际成本</strong> 使用以下公式计算：</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>此处将考虑用户记录问题时间的每小时成本率，无论为问题分配了什么角色。 </p> <p>如果记录时间的用户没有与其关联的每小时成本费率，则其主要角色的每小时成本费率将计算问题的实际成本。<br>如果正在记录时间的用户在其配置文件中没有角色或没有与其关联的费率，则问题的实际成本为零。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>无分配</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>实际成本</strong> 使用以下公式计算：</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>如果记录时间的用户没有与其配置文件关联的每小时成本费率，则其主要任务角色的每小时成本费率将计算问题的实际成本。 </p> <p>如果正在记录时间的用户没有与其配置文件相关联的作业角色，或者其主要作业角色没有定义每小时成本费率，则问题的实际成本为零。 </p> </td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td colspan="4"> 
    <div> <MadCap:conditionalText data-mc-conditions="">
       If your Workfront administrator enabled the 
      <strong>Assign Job Roles to hour entries manually</strong> setting in the Timesheets &amp; Hours Preferences area, and the user logging time on the issue selects a different role to associate with this time, the Actual Cost of the issue calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article 
      <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>. 
     </MadCap:conditionalText> 
    </div> </td> 
  </tr> 
  -->
 </tbody> 
</table>
