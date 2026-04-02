---
content-type: overview
product-area: projects
navigation-topic: financials
title: 开单和收入概览
description: 作为项目经理，您可以使用记帐费率来获取项目收入。
author: Lisa
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '4542'
ht-degree: 0%

---

# 开单和收入概览

<!-- Audited: 1/2024 -->

{{highlighted-preview}}

作为项目经理，您可以使用记帐费率来获取项目收入。

本文介绍了项目收入的跟踪。 收入的计算方式在利用率报表中有所不同。 有关利用率报告中的收入计算的信息，请参阅[查看资源利用率信息](../../../resource-mgmt/resource-utilization/view-utilization-information.md)。

## 记帐费率概述

处理记帐费率时，请考虑以下事项：

* 您需要具有财务数据（特别是记帐费率）编辑访问权限的计划或标准许可证以管理记帐费率。
有关授予对财务数据的访问权限的详细信息，请参阅[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

* 记帐费率是与工作角色或用户关联的每个工作单位的收入额。

  将费率乘以工作花费小时数可为您的项目产生收入。

* 建立记帐费率后，您可以通过创建记帐记录来跟踪收入，以记录已记帐和未记帐的内容。

  >[!TIP]
  >
  >将开票记录标记为已开票时，无法对其进行编辑。 当费率不同并且您想要锁定项目的收入和费用信息时，这一点很重要。 将其添加到记帐记录并标记为已记帐，可防止在系统中更新费率时更新该记录。

  有关创建开票记录的更多信息，请参阅文章[创建开票记录](../../../manage-work/projects/project-finances/create-billing-records.md)。

* 您可以为用户、工作角色创建记帐费率，也可以为项目或任务创建一次性记帐费率。

>[!IMPORTANT]
>
>计算收入的费率属于记录时间的用户，或属于其工作角色。

### 费率卡记帐费率

{{ultimate-package}}

当您有权编辑费率卡时，您可以根据地点和组或代理等属性定义每个角色具有多个记帐费率的费率卡。 属性最多可配置五个级别。

必须将费率卡附加到项目才能应用其费率。 当费率卡上锁定时，无法在项目级别覆盖该费率。

费率卡费率是层次结构的一部分，用于根据任务收入类型确定费率。

有关创建费率卡的详细信息，请参阅[管理费率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)。

有关费率层次结构的详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。

![采样率卡](assets/sample-rate-card-march2026.png)

### 用户记帐费率 {#user-billing-rates}

作为用户管理员，在创建用户时，您可以通过指定每小时计费字段的值以及费率的日期，将它们与日期有效的记帐费率相关联。

有关创建用户的详细信息，请参阅文章[添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

![编辑用户成本和记帐费率](assets/edit-user-cost-billing-rate-1.png)

### 工作角色记帐费率 {#job-role-billing-rates}

作为Adobe Workfront管理员，在创建工作职责时，您可以通过指定费率值和日期，将工作职责与日期有效的开单费率相关联。

您可以使用Workfront系统的基础货币或其他货币来定义工作角色记帐费率的值。 您还必须在系统汇率中定义其他货币。

有关创建工作角色的更多信息，请参阅文章[创建和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

![编辑工作角色成本和记帐费率](assets/edit-job-role-multiple-billing-rates-new.png)

### 项目或任务的固定记帐费率 {#fixed-billing-rates-for-projects-or-tasks}

除了用户和工作角色小时费率之外，您还可以使用以下固定记帐费率：

* 固定小时收入类型的固定金额
* 固定收入收入类型的固定金额

有关如何使用固定记帐费率计算收入的更多信息，请参阅[任务收入类型概览](#overview-of-task-revenue-types)。

<div class="preview">

### 覆盖记帐费率 — 工作流Ultimate包

>[!IMPORTANT]
>
>您可以覆盖与项目级别的工作角色或用户关联的计费率。 您无法覆盖固定费率。

在项目级别，您可以：

* 覆盖工作角色的记帐费率（应用了属性，如地点、组或代理）。
* 覆盖该项目上特定用户的记帐费率。

记帐费率覆盖不是通用的。 例如，您不会将“Designer”作为角色覆盖。 相反，您会在相关生效日期期间覆盖“Designer — 纽约 — 代理商X”。 改写遵循开单费率层次结构，因此系统始终按优先顺序应用它们。

</div>

### 覆盖记帐费率 — 所有其他包

>[!IMPORTANT]
>
>您可以覆盖与工作角色关联的记帐费率。 您无法覆盖用户记帐费率或固定费率。

您可以覆盖以下工作角色记帐费率：

* 特定公司

  有关创建特定于公司的工作角色记帐费率的详细信息，请参阅[创建和编辑公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

* 特定项目

  有关创建特定于项目的工作角色记帐费率的详细信息，请参阅文章[覆盖记帐费率和计算项目收入概述](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

## 跟踪收入金额

在根据任务的已计划小时数创建任务时，Workfront可以自动跟踪已计划收入。

当在任务、问题和项目上记录实际小时数时，它还可以自动跟踪实际收入。

下表显示与任务、问题和项目关联的收入类型。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">规划收入</td> 
   <td> <p>对于任务，这是与任务的计划小时数关联的收入。 所有任务的计划小时数累计到项目的计划小时数，有助于项目计划小时数的计算。 </p> <p>有关Workfront中计划小时数的详细信息，请参阅<a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">计划小时数概述</a>。 </p> <ul><li><p>Workfront使用此公式计算任务的计划收入：</p>
   <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code><p> <p><strong>注意</strong></br>公式中的计费小时费率会考虑该费率的任何日期生效更改。</p> </li><li><p>Workfront使用以下公式计算项目的计划收入：</p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) + Fixed Revenue</code></p>
   <p><b>注释</b>

<p>在项目详细信息区域和项目报表中显示的项目计划收入与利用率报表中显示的计划收入不同。 </p></li></ul> <p>项目详细信息区域中的计划收入反映与任务计划小时数以及项目的固定收入关联的任务收入。 利用率报表中的计划收入仅显示与项目任务分配的计划小时数关联的计划收入。 </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>如果项目有1个时数为10的任务，分配给顾问时费率为$20，并且项目有$100的固定收入，则利用率报表显示计划收入$200（与任务小时数关联的计划收入）。 项目详细信息部分显示$300（任务的计划收入和项目的固定收入）。 </p> 
     </div> </p> <p>任务计划收入使用分配给任务的用户或工作角色的计费小时费率计算。 任务的收入类型会影响用于计算计划收入的比率（用户或角色）。 有关更多信息，请参阅本文中的以下部分：</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">任务收入类型概述</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref">基于用户和角色分配的任务收入计算</a> </p> </li> 
    </ul> <p>有关利用率报告中计划收入计算的信息，请参阅<a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">查看资源利用率信息</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">实际收入*</td> 
   <td> <p>与任务、问题和项目的实际小时数关联的收入。 </p> <p>通常，Workfront会使用以下公式计算实际收入：</p> <p><code>Actual Revenue = Actual Hours * Billing rate</code> </p> <p><strong>注意</strong></br>公式中的计费小时费率会考虑该费率的任何日期生效更改。</p> <p>有关利用率报告中的实际收入计算的信息，请参阅<a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">查看资源利用率信息</a>。 </p> <p><b>提示</b>

您不能查看问题层的实际收入，但与问题中的实际小时数关联的收入将计入项目的实际收入。 </p> </td>
</tr> 
 </tbody> 
</table>

*对于实际小时数，用户的费率始终是指记录小时数的用户或其工作角色的费率。 有关Workfront何时使用用户费率和何时使用工作角色费率的信息，请参阅本文中的[收入计算](#revenue-calculations)部分。

例如，如果一项具有用户小时收入类型的任务计划需要2小时，而分配给它的用户的小时费率为$30/小时，则该任务的计划收入为$60。 当任务完成时，如果用户仅记录1.5小时作为完成任务所花费的实际时间，则实际收入金额为$45。 如果另一个未分配到任务的用户记录时间，则根据该用户的记帐费率计算实际收入。

您可以通过以下方式记录收入：

* 通过定义任务的收入类型，并将分配给工作项目的用户或角色与记帐费率相关联。 这将按工作项的计划小时数或实际小时数计算收入。 无论是否按小时费率收费，您都可以设置一个上限。\
  有关指定任务的收入类型的详细信息，请参阅文章[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

* 为任务或项目按统一固定收入费率计费。\
  如果您的任务具有固定收入，则固定收入金额将作为任务或项目的计划收入添加，任务的计划收入将作为固定收入添加到记帐记录。
* 通过为项目设置统一记帐固定收入费率，然后为项目中的任务设置小时费率。 Workfront将任务的小时费率添加到项目的统一费率。\
  例如，使用Workfront的机械师可以输入部件成本作为项目的固定收入，然后按小时对修理汽车所花费的时间计费。 然后，项目或任务的固定收入在完成时实现。

您还可以将任务标记为“不可记帐”，在这种情况下，没有与任务关联的计划或实际收入。

## 任务收入类型概览 {#overview-of-task-revenue-types}

默认情况下，所有新任务的收入类型均根据Workfront或组管理员指定的任务和问题首选项进行设置。

有关定义Workfront实例的任务和问题首选项的更多信息，请参阅文章[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

项目所有者可以修改任务的收入类型和项目的固定收入。

有关设置项目固定收入的详细信息，请参阅文章[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。
有关设置任务的收入类型的详细信息，请参阅文章[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

>[!NOTE]
>
><span class="preview">您必须具有工作流Ultimate程序包才能使用用户和角色每小时收入类型。</span>

您可以将以下收入类型应用于您的任务或项目：

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>收入类型</strong> </p> </th> 
   <th> <p><strong>描述</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>固定收入</p> </td> 
   <td> <p>此类型可用于项目和任务。 </p> <p>将模板附加到项目时，模板中的固定收入会添加到项目的固定收入。 有关信息，请参阅<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">将模板附加到项目的概述</a>。 </p> <p>对于任务，无论任务分配如何，始终使用任务上指定的固定金额计算任务收入。 </p> <p>子任务的固定收入将累计至父任务的收入，然后累计至项目的收入。 如果在父任务和/或项目上定义了固定金额，则该金额会添加到从任何子任务累计的计划收入中。</p> <p>任务的固定收入金额可以包含在项目的记帐记录中。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>用户每小时</p> </td> 
   <td> <p>此类型只能用于任务。 </p> <p>您为特定用户设置的记帐费率乘以该任务的计划小时数，即成为该任务的计划收入额。 您为特定用户设置的记帐费率乘以用户针对任务记录的小时数，即为任务的实际收入金额。 <br>例如，如果您创建用户，并为其每小时记帐字段设置$20，那么如果用户为时间表上的任务提交5小时，则该任务的实际记帐金额为$100。</p>
   <p>一个用户配置文件可以包含多个具有有效日期的记帐费率。 例如，第一个用户记帐费率$20于2023年4月30日结束，第二个用户记帐费率$25于2023年5月1日开始。 如果用户在4月28日提交2小时，在5月2日提交3小时用于任务，则任务的实际开单金额为$40 + $75 = $115。</p>
   <p><b>提示</b>

这是创建任务时的默认收入类型。</p> </td>
</tr> 
  <tr> 
   <td> <p>角色每小时</p> </td> 
   <td> <p>此类型只能用于任务。</p> <p>此类型类似于每小时用户数，但使用工作角色费率而不是用户费率。</p> <p><strong>注意</strong><br>工作角色也可以有多个具有有效日期的记帐费率。</p></td> 
  </tr> 
  <tr> 
   <td> <p><span class="preview">用户和角色按小时计</span></p> </td> 
   <td> <p><span class="preview">此类型只能用于任务。</span></p> <p><span class="preview">此类型会检查用户和角色信息，以确定适当的比率。</span></p></td> 
  </tr>
  <tr> 
   <td> <p>受限用户小时</p> </td> 
   <td> <p>此类型只能用于任务。</p> <p>任务按照用户小时计费，但它们具有您可以指定的上限金额。 <br>例如，如果用户的记帐费率是$25，但任务的上限金额是$20，并且用户记录了一个小时，则任务的实际收入是$20。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>受限角色小时</p> </td> 
   <td> <p>此类型只能用于任务。</p> <p>此类型类似于具有Cap的“每小时用户”，但使用工作角色费率而不是用户费率。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="preview">受限用户每小时和角色</span></p> </td> 
   <td> <p><span class="preview">此类型只能用于任务。</span></p> <p><span class="preview">任务按照用户和角色每小时计费，但它们具有您可以指定的上限金额。</span></p></td> 
  </tr>
  <tr> 
   <td> <p>用户小时加固定</p> </td> 
   <td> <p>此类型只能用于任务。 </p> <p>任务按用户小时计费，但具有您可以添加到用户费率的固定金额。 在任务上指定的固定金额可以包含在项目的记帐记录中。 固定数量不会乘以任务的小时数。 只有用户计费率有效。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>角色小时加固定</p> </td> 
   <td> <p>此类型只能用于任务。 </p> <p>任务按照角色每小时计费一次，但有一个附加的固定金额，您可以将其添加至角色费率。 在任务上指定的固定金额可以包含在项目的记帐记录中。 固定数量不会乘以任务的小时数。 只有工作角色记帐费率有效。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="preview">用户和角色按小时计加固定费用</span></p> </td> 
   <td> <p><span class="preview">此类型只能用于任务。</span></p> <p><span class="preview">任务按照用户和角色每小时计费，但具有额外的固定金额，您可以将其添加至费率。 在任务上指定的固定金额可以包含在项目的记帐记录中。 固定数量不会乘以任务的小时数。</span></p></td> 
  </tr>
  <tr> 
   <td> <p>固定每小时</p> </td> 
   <td> <p>此类型只能用于任务。</p> <p>您为任务设置的上限或固定金额乘以针对任务输入的小时数（无论用户或其职位角色如何）即是计费金额。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>不可计费</p> </td> 
   <td> <p>此类型只能用于任务。</p> <p>此收入类型对收入没有影响。 </p> <p>如果父对象具有此设置，则仍会正常应用具有计费类型的子任务。</p> <p>当对财务数据没有访问权限的用户或对模板没有财务权限的用户从该模板创建项目时，这是项目上任务的默认收入类型。</p> <p>有关访问财务数据的信息，请参阅文章<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予对财务数据的访问权限</a>。<br>有关对象的财务权限的信息，请参阅文章<a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">对象权限共享概述</a>。<br>有关从模板创建项目的信息，请参阅文章<a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">使用模板创建项目</a>。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 父任务的收入概览

如果将具有开单信息的独立任务更改为父任务，则新的父任务仍会保留以前应用的任何开单信息，以及以前应用的小时数。 来自记录到子任务小时数的任何计费信息将作为实际收入汇总到新的父任务中。

子任务的计划收入也会累计到父任务。

## 问题收入概述

问题没有计划或实际收入额，但它们可以具有实际成本。

如果您记录问题的小时数，并使用标记为“计为收入”的小时类型，则Workfront会根据登录该时间的用户的费率计算实际成本金额。 此数字将添加到项目的实际成本。 小时数也可以包含在开票记录中。

有关跟踪成本的更多信息，请参阅文章[跟踪成本](../../../manage-work/projects/project-finances/track-costs.md)。

有关小时类型的详细信息，请参阅文章[管理小时类型](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md)。

## 收入计算

* [基于用户和角色分配的任务的收入计算](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)
* [项目的收入计算](#revenue-calculations-for-projects)

### 基于用户和角色分配的任务的收入计算 {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

在计算任务的收入时，请考虑以下事项：

* 如果用户或工作角色显示费率$0.00，Workfront会将其读取为有效金额，然后将该金额乘以任务中的小时数来计算收入。 如果要不显示任务的收入，请确保用户或工作角色的记帐费率的字段为空。
* 应用工作角色记帐费率时，Workfront使用项目层的覆盖费率，而不是每次在项目上有覆盖费率时在系统层定义的该角色的记帐费率。
* 对于实际收入，如果用户或工作角色具有多个具有有效日期的记帐费率，则任务收入是用户已记录时间的每个时间期间的收入总和。 计划收入基于时间期的计划小时数。
* 如果任务中有多个被分配人，则以下列出的方案适用于每个被分配人。

系统使用层次结构来确定在基于任务分配的收入计算中使用的费率。

如果您的Workfront管理员在时间表和小时首选项区域中启用了&#x200B;**手动将工作角色分配给小时条目**&#x200B;设置，并且项目的用户日志记录时间选择了其他要与此时间关联的角色，则任务或项目的实际收入始终根据与小时条目关联的角色进行计算。 有关为特定工作角色启用日志记录时间的信息，请参阅文章[配置时间表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

<div class="preview">

对于“用户”和“角色每小时”收入类型，可以在项目层和分配层定义开单的工作角色。 如果在项目级别为特定用户定义了该角色，则该角色会在您应用该角色的日期有效期间自动传播到该用户的所有分配。 如果需要，您仍然可以在分配层改写此费率。 例如，用户的主要工作角色是Designer，但您将其在项目上的工作角色设置为八月份的高级Designer 。 在8月分配的所有任务都将自动使用高级Designer计费率。

但是，对于特定任务，您可以仅覆盖该分配的角色，以反映正在计费的工作。 这样，系统既支持项目范围的一致性，又支持任务级灵活性。 有关详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)和[创建高级分配](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md)。

</div>

根据收入类型和任务分配的性质计算任务收入时，存在以下方案：

* **任务的收入类型为“每小时用户”**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">记帐/小时费率</td> 
     <td>无分配</td> 
     <td>用户分配</td> 
     <td>工作角色分配</td> 
    </tr> 
    <tr> 
     <td role="rowheader">计划收入的每小时记帐费率</td> 
     <td>0.00美元</td> 
     <td> 如果用户档案中有记帐费率，则该费率用于计算计划收入。 否则，将使用其主要工作角色的系统记帐费率。 <br><p><b>注意</b>可以将用户分配到具有其中一个辅助工作角色的任务，但此处使用的是主要工作角色的速率。</p><p>如果在分配期间用户的角色发生了变化，则在重新计算项目财务时将应用正确的费率。</p></td> 
     <td>分配给任务的工作角色的系统记帐费率用于计算计划收入。 可以在项目级别覆盖记帐费率。</td> 
    </tr> 
    <tr> 
     <td role="rowheader">实际收入的每小时记帐费率</td> 
     <td>如果记录小时数的用户在其配置文件中具有记帐费率，则会使用该费率。
     <br>否则，将使用其主要工作角色的记帐费率。 如果没有与用户或其主要角色关联的记帐费率，则实际收入为$0.00。 <br><p><b>注释</b>

  计算时只考虑与记录时间的用户关联的费率，即使将另一个用户分配给任务也是如此。</p></td>

  <td>如果记录小时数的用户在其配置文件中具有记帐费率，则会使用该费率。 <br>否则，将使用其主要工作角色的记帐费率。 如果没有与用户或其主要角色关联的记帐费率，则实际收入为$0.00。 <br><p><b>注释</b>

  计算时只考虑与记录时间的用户关联的费率，即使将另一个用户分配给任务也是如此。</p></td>

  <td>如果记录小时数的用户在其配置文件中具有记帐费率，则会使用该费率。 否则，将使用其主要工作角色的记帐费率。<br><p><b>注释</b>

  如果用户日志记录时间没有关联的计费率，并且他们没有工作角色或其工作角色的计费率，则使用与任务关联的工作角色的费率。 如果此角色没有记帐费率，则收入为$0.00。</p></td>
  </tr> 
   </tbody> 
  </table>

* **任务的收入类型为“每小时角色”**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">记帐/小时费率</td> 
     <td>无分配</td> 
     <td>用户分配</td> 
     <td>工作角色分配</td> 
    </tr> 
    <tr> 
     <td role="rowheader">计划收入的每小时记帐费率</td> 
     <td>0.00美元</td> 
     <td><p>Workfront查看用户在任务中履行的工作角色以计算计划收入。 <br>如果用户未与任务上的任何角色关联，则收入为$0.00。</p> <p><strong>注意</strong><br>如果在分配期间更改了用户的角色，则重新计算项目财务时将应用正确的费率。</p> </td> 
     <td>分配给任务的工作角色的记帐费率用于计算计划收入。 可以在项目级别覆盖记帐费率。</td> 
    </tr> 
    <tr> 
     <td role="rowheader">实际收入的每小时记帐费率</td> 
     <td>Workfront使用记录时间的用户的主要工作角色的计费率。 <br>如果记录时间的用户没有与其关联的工作角色，或者如果主要工作角色没有记帐费率，则实际收入为$0.00。 </td> 
     <td> 如果将记录时间的用户分配给任务，则使用与任务中的用户相关联的工作角色的记帐费率来计算实际收入。 <br>否则，将使用其主要工作角色的记帐费率。 如果用户没有主要工作角色，或其主要工作角色没有记帐费率，则实际收入为$0.00。 </td> 
     <td>如果为该任务分配了记录时间的用户的某个工作角色，则使用该工作角色费率。 如果分配给任务的工作角色未与记录时间的用户关联，则使用用户主要角色的记帐费率计算实际收入。 如果用户没有工作角色，或者没有与其主要工作角色关联的费率，则使用分配给任务的工作角色的费率。 </td> 
    </tr> 
   </tbody> 
  </table>

<div class="preview">

* **任务的收入类型为每小时用户和角色**

| 记帐/小时费率 | 无分配 | 用户分配 | 工作角色分配 |
| --- | --- | --- | --- |
| 计划收入的每小时记帐费率 | 0.00美元 | 分配用户后，系统会按指定顺序查找费率，从保留的计费费率开始。 接下来是锁定费率卡费率、人工输入的分配费率、工作角色计费分配、项目层用户计费费率覆盖、工作角色计费项目、用户系统费率和用户的主要工作角色费率。 <p> 有关详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。 | 在分配工作角色时，系统首先查找保留的计费费率，然后查找分配上工作角色的锁定费率卡费率。 接下来，它会查找在分配中手动添加的工作角色费率。 如果未找到该费率，则会在项目级别查找工作角色费率，首先从费率卡中查找，然后从系统费率中查找。 <p> 有关详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。 |
| 实际收入的每小时记帐费率 | 计算时只考虑与记录时间的用户关联的费率，即使将另一个用户分配给任务也是如此。 <p> 系统按指定顺序查找费率，从保留的计费费率开始。 接下来是锁定费率卡费率、项目的记帐费率覆盖、记帐的工作角色、所有者用户配置文件上的系统级别费率，以及所有者主要工作角色的记帐费率。 <p> 有关详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。 | 分配用户后，系统会按指定顺序查找费率，从保留的计费费率开始。 接下来是锁定费率卡费率、人工输入的分配费率、工作角色计费分配、项目层用户计费费率覆盖、工作角色计费项目、用户系统费率和用户的主要工作角色费率。 <p> 有关详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。 | 在分配工作角色时，系统首先查找保留的计费费率，然后查找分配上工作角色的锁定费率卡费率。 接下来，它会查找在分配中手动添加的工作角色费率。 如果未找到该费率，则会在项目级别查找工作角色费率，首先从费率卡中查找，然后从系统费率中查找。 有关详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。 |

</div>

### 项目的收入计算

您可以跟踪项目的以下收入类型：

* 项目的计划收入按以下公式计算：

  `Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue`

  有关如何计算任务计划收入的信息，请参阅本文中[基于用户和角色分配的任务收入计算](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)部分。

* 项目的实际收入按以下公式计算：

  `Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)`

有关如何计算任务实际收入的信息，请参阅本文中[基于用户和角色分配的任务收入计算](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)部分。

对于与直接记录到项目或问题的小时数关联的实际收入，Workfront使用记录项目时间的用户的记帐费率。 如果用户没有与其配置文件关联的记帐费率，Workfront将使用其主要工作角色的记帐费率。 如果两个费率均为零，则与项目或问题记录的小时数关联的实际收入为零。
