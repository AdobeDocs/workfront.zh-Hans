---
content-type: overview
product-area: projects
navigation-topic: financials
title: 账单和收入概述
description: 作为项目经理，您可以使用计费率来获取项目的收入。
author: Alina
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
source-git-commit: 518a552845598a30fd547d432aa9d22dfef6ec8e
workflow-type: tm+mt
source-wordcount: '3313'
ht-degree: 0%

---

# 账单和收入概述

作为项目经理，您可以使用计费率来获取项目的收入。

本文介绍了如何跟踪项目的收入。 收入在利用率报表中的计算方式不同。 有关利用率报表中收入计算的信息，请参阅 [查看资源利用信息](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

## 计费费率概述

使用计费费率时，请考虑以下事项：

* 您需要具有“编辑”金融数据访问权限的计划许可证才能管理计费费率。\
   有关授予对金融数据的访问权限的更多信息，请参阅 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* 开单费率是与职务角色或用户关联的每个工作单位的收入额。

   将比率乘以工作所花费的小时数，可为您的项目产生收入。

* 在建立开单费率后，您可以通过创建开单记录来跟踪收入，以记录已开单和未开单的内容。

   >[!TIP]
   >
   >当您将账单记录标记为已计费时，将无法对其进行编辑。 当您的费率不同并且您希望锁定项目的收入和费用信息时，这一点很重要。 将其添加到账单记录并标记为已计费，会在费率在您的系统中更新时阻止更新该记录。

   有关创建账单记录的更多信息，请参阅文章 [创建帐单记录](../../../manage-work/projects/project-finances/create-billing-records.md).

* 您可以为用户、职务角色创建开单费率，也可以为项目或任务创建一次性开单费率。

>[!IMPORTANT]
>
>计算收入的费率属于记录时间的用户或其职务角色。

* [用户计费费率](#user-billing-rates)
* [职务职责开单费率](#job-role-billing-rates)
* [项目或任务的固定开单费率](#fixed-billing-rates-for-projects-or-tasks)
* [覆盖开单费率](#override-billing-rates)

### 用户计费费率 {#user-billing-rates}

作为用户管理员，在创建用户时，可以通过在用户配置文件中为“每小时计费”字段指定值，将用户与计费费率关联。\
有关创建用户的更多信息，请参阅文章 [添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)

![](assets/qs-user-edit-ui-with-rp-and-billing-per-hour-field-1-350x152.png)

### 职务职责开单费率 {#job-role-billing-rates}

作为Adobe Workfront管理员，在创建职务角色时，您可以通过为“帐单/小时”字段指定值，将其与帐单费率关联。

您可以使用Workfront系统的基本货币或使用其他自定义货币定义职务角色开单费率的值。

有关创建职务角色和覆盖其货币的更多信息，请参阅文章 [创建和管理作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

![](assets/billing-rate-for-role-1-350x294.png)

### 项目或任务的固定开单费率 {#fixed-billing-rates-for-projects-or-tasks}

除了用户和职务角色每小时费率外，您还可以使用以下固定开单费率：

* 固定小时收入类型的固定金额
* 固定收入类型的固定金额

有关如何使用固定开单费率计算收入的详细信息，请参阅 [任务收入类型概述](#overview-of-task-revenue-types).

### 覆盖开单费率 {#override-billing-rates}

>[!IMPORTANT]
>
>您可以改写与职务职责关联的开单费率。 您不能改写用户开单费率或固定费率。

您可以改写以下职务职责开单费率：

* 特定公司

   有关创建特定于公司的职务角色开单费率的详细信息，请参阅 [创建和编辑公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* 特定项目

   有关创建特定于项目的职务角色开单费率的详细信息，请参阅文章 [改写职务职责开单费率和计算项目收入的概述](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## 跟踪收入金额

当根据任务的计划时间创建任务时，Workfront可以自动跟踪计划收入。

当在任务、问题和项目上记录实际小时数时，它还可以自动跟踪实际收入。

下表显示了与任务、问题和项目关联的收入类型。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">计划收入</td> 
   <td> <p>对于任务，这是与任务计划小时数相关联的收入。 从所有任务到项目的计划小时数累计到项目的计划小时数，以便对项目计划小时数的计算做出贡献。 </p> <p>有关Workfront中计划时数的更多信息，请参阅 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">计划时数概述</a>. </p> <p>Workfront使用以下公式计算任务和项目的计划收入：</p> <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code> </p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) +&nbsp;Fixed Revenue</code> </p> 
   <p><b>注释</b>

<p>在“项目详细信息”区域和项目报表中显示的项目计划收入与在“利用率”报表中显示的计划收入不同。 </p> <p>“项目详细信息”区域中的“计划收入”反映与任务“计划时数”关联的任务收入以及项目的固定收入。 “利用率报表”中的“计划收入”显示仅与项目任务分配中的计划小时数关联的计划收入。 </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>如果项目有1个任务，10小时，该任务分配给顾问，每小时费率为$20，而项目有$100的固定收入，则“利用率”报表会显示“计划收入”为$200（与任务小时数关联的计划收入）。 “项目详细信息”部分显示$300（任务的计划收入和项目的固定收入）。 </p> 
     </div> </p> <p>任务计划收入使用分配给任务的用户或职务角色的开单小时费率来计算。 任务的收入类型会影响用于计算计划收入的费率（用户或角色）。 有关更多信息，请参阅本文的以下部分：</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">任务收入类型概述</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref">基于用户和角色分配的任务的收入计算</a> </p> </li> 
    </ul> <p>有关“利用率”报表中“计划收入”计算的信息，请参阅 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">查看资源利用信息 </a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">实际收入*</td> 
   <td> <p>与任务、问题和项目的实际工时数相关联。 </p> <p>通常，Workfront会使用以下公式计算实际收入：</p> <p><code>Planned Revenue = Planned Hours * Billing rate</code> </p> <p>有关利用率报表中实际收入计算的信息，请参阅 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">查看资源利用信息 </a>. </p> <p><b>笔尖</b>

您无法在问题层查看实际收入，但与问题上的实际小时数关联的收入会影响项目的实际收入。 </p> </td>
</tr> 
 </tbody> 
</table>

*对于“实际工时”，用户费率始终指记录工时或其工作角色费率的用户。 有关Workfront何时使用用户费率以及何时使用其工作角色费率的信息，请参阅 [收入计算](#revenue-calculations) 章节。

<!--Note from the table for Planned Revenue line: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    -->

例如，如果具有用户每小时收入类型的任务计划花费2小时，而分配给该任务的用户每小时费率为$30，则该任务的计划收入为$60。 任务完成后，如果用户仅将1.5小时记录为完成任务的实际花费时间，则实际收入金额为$45。 如果未分配到该任务的另一个用户记录了该时间，则实际收入将根据该用户的开单费率计算。

您可以通过以下方式记录收入：

* 通过定义任务的收入类型，并将分配给工作项的用户或角色与开单费率关联。 它将按工作项上的计划小时数或实际小时数计算收入。 您可以将上限设置为每小时费率的最高收费额，也可以不设置。\
   有关指定任务的“收入类型”的详细信息，请参阅文章 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

* 对任务或项目按固定收入费率开单。\
   如果您有具有固定收入的任务，则固定收入金额将作为任务或项目的计划收入添加，并且任务的计划收入将作为固定收入添加到开单记录中。
* 为项目设置固定开单固定收入费率，然后为项目中的任务设置每小时费率。 Workfront将任务的每小时费率添加为项目的固定费率。\
   例如，使用Workfront的机械工可以输入部件成本作为项目的固定收入，然后为修车所花费的时间按小时开单。 固定项目或任务的收入随后在完成时实现。

您还可以将任务标记为“不可计费”，在这种情况下，没有与它们关联的计划收入或实际收入。

## 任务收入类型概述 {#overview-of-task-revenue-types}

默认情况下，所有新任务的收入类型都根据Workfront或组管理员指定的任务和问题首选项来设置。\
有关为Workfront实例定义任务和问题首选项的更多信息，请参阅文章 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

项目责任人可以修改项目的“收入类型”任务和“固定收入”。\
有关指定项目固定收入的详细信息，请参阅文章 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).\
有关指定任务的“收入类型”的详细信息，请参阅文章 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

您可以将以下收入类型应用于任务或项目：

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
   <td> <p>此类型可用于项目和任务。 </p> <p>将模板附加到项目时，模板的固定收入会添加到项目的固定收入中。 有关信息，请参阅 <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">将模板附加到项目的概述</a>. </p> <p>对于任务，无论任务分配如何，任务的收入始终使用任务中指定的固定金额来计算。 </p> <p>“来自子项的固定收入”任务累计至父项任务的收入，然后累计至项目的收入。 如果在父任务和/或项目上定义了固定金额，则该金额会添加到从任何子任务累计的计划收入中。</p> <p>任务上的固定收入额可以包括在项目上的开单记录中。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>用户小时</p> </td> 
   <td> <p>此类型只能用于任务。 </p> <p>您为特定用户设置的开单费率乘以该任务的计划小时数，即成为该任务的计划收入金额。 您为特定用户设置的开单费率乘以用户针对任务记录的小时数，即为任务的实际收入额。 <br>例如，当您创建用户并为其“每小时计费”字段设置$20时，如果用户为时间表上的任务提交5小时，则任务的“实际开单”金额为$100。</p> <p><b>笔尖</b>

这是创建任务时的默认收入类型。</p> </td>
</tr> 
  <tr> 
   <td> <p>角色小时</p> </td> 
   <td> <p>此类型只能用于任务。</p> <p>此类型与“用户每小时”类似，但使用职务角色费率而不是用户费率。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>具有上限的用户每小时</p> </td> 
   <td> <p>此类型只能用于任务。</p> <p>任务按小时在用户每小时中计费，但您可以指定任务的最大上限额。 <br>例如，如果用户的计费费率为$25，但任务的上限金额为$20，而用户记录了一小时，则任务的实际收入为$20。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>每小时具有上限的角色</p> </td> 
   <td> <p>此类型只能用于任务。</p> <p>此类型与具有上限的用户每小时类似，但使用职务角色费率而不是用户费率。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>用户小时加固定</p> </td> 
   <td> <p>此类型只能用于任务。 </p> <p>任务按小时在用户每小时中计费，但具有可添加到用户费率的固定金额。 任务中指定的固定金额可以包含在项目的开单记录中。 固定金额不会乘以任务上的小时数。 只有用户计费费率才有。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>角色小时加固定</p> </td> 
   <td> <p>此类型只能用于任务。 </p> <p>任务每小时在角色中按小时计费，但具有附加的固定金额，您可以将其添加到角色费率中。 任务中指定的固定金额可以包含在项目的开单记录中。 固定金额不会乘以任务上的小时数。 只有作业角色开单费率才有。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定小时</p> </td> 
   <td> <p>此类型只能用于任务。</p> <p>您为任务设置的上限或固定金额乘以针对任务输入的小时数（无论用户或其职务角色如何）即为开单金额。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>不可记帐</p> </td> 
   <td> <p>此类型只能用于任务。</p> <p>此收入类型对收入没有影响。 </p> <p>如果父对象具有此设置，则具有帐单类型的子任务仍将正常应用。</p> <p>当对模板没有财务数据访问权限的用户或对模板没有财务权限的用户从该模板创建项目时，这是项目任务的默认收入类型。</p> <p>有关访问金融数据的信息，请参阅文章 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予对财务数据的访问权限</a>.<br>有关对象的财务权限信息，请参阅文章 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">对象共享权限概述</a>.<br>有关从模板创建项目的信息，请参阅文章 <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">使用模板创建项目</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## 父任务的收入概述

如果将单独任务更改为父任务，则新父任务仍保留以前应用于该任务的任何开单信息以及以前应用的小时数。 从记录到子任务的小时数开始的任何开单信息将作为实际收入汇总到新的父任务。

子任务的计划收入也会累计到父任务。

## 收入问题概述

问题没有计划收入额或实际收入额，但它们可能具有实际成本。

如果您为问题记录小时数，并且使用标记为“计为收入”的小时类型，则Workfront会根据正在登录该时间的用户的比率计算实际成本金额。 此数字将添加到项目的实际成本中。 小时也可以包含在账单记录中。

有关跟踪成本的更多信息，请参阅文章 [跟踪成本](../../../manage-work/projects/project-finances/track-costs.md).

有关小时类型的更多信息，请参阅文章 [管理小时类型](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## 收入计算

* [基于用户和角色分配的任务的收入计算](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)

### 基于用户和角色分配的任务的收入计算 {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

在计算任务的收入时，请考虑以下事项：

* 如果用户或职务角色显示的费率为$0.00,Workfront会将其读作有效金额，并将此金额乘以任务上的小时数，以计算收入。 如果要不显示任务的收入，请确保用户或职务角色的计费费率字段为空。
* 在应用职务角色开单费率时，Workfront会使用项目层的改写费率，而不是在项目上每次存在改写费率时在系统层定义的该职责的开单费率。
* 如果任务上有多个受分配人，则下面概述的方案适用于每个受分配人。

在基于任务分配的收入计算中使用费率的层次结构。

如果您的Workfront管理员启用了 **将作业角色手动分配给小时条目** 在“时间表和小时首选项”区域中进行设置，并且项目的用户日志记录时间选择与此时间关联的其他角色，则任务或项目的实际收入始终根据与小时条目关联的角色进行计算。 有关为特定作业角色启用日志记录时间的信息，请参阅文章 [工时单和工时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

根据“收入类型”和任务分配的性质计算任务收入时，存在以下方案：

* **任务的收入类型是“用户每小时”**

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">每小时计费率</td> 
     <td>无分配</td> 
     <td>用户分配</td> 
     <td>职务角色分配</td> 
    </tr> 
    <tr> 
     <td role="rowheader">计划收入的每小时开单费率</td> 
     <td>$0.00</td> 
     <td> 如果用户的配置文件中有一个计费费率，则该费率将用于计算计划收入。 否则，将使用其主要作业角色的系统计费率。 <br><p><b>注意</b>  可以将用户分配到具有其其中一个辅助作业角色的任务，但此处将改用主作业角色的比率。</p></td> 
     <td>分配给任务的任务职责的系统开单费率用于计算计划收入。 </td> 
    </tr> 
    <tr> 
     <td role="rowheader">实际收入的每小时开单费率</td> 
     <td>如果记录小时数的用户在其配置文件中具有计费费率，则会使用该费率。 <br>否则，将使用其主要作业角色的开单费率。 如果没有与用户或其主要角色关联的计费费率，则实际收入为$0.00。 <br><p><b>注释</b>

   计算时只考虑与用户记录时间相关的费率，即使将其他用户分配到该任务时也是如此。</p></td>
   <td>如果记录小时数的用户在其配置文件中具有计费费率，则会使用该费率。 <br>否则，将使用其主要作业角色的开单费率。 如果没有与用户或其主要角色关联的计费费率，则实际收入为$0.00。 <br><p><b>注释</b>

   计算时只考虑与用户记录时间相关的费率，即使将其他用户分配到该任务时也是如此。</p></td>
   <td>如果记录小时数的用户在其配置文件中具有计费费率，则会使用该费率。 否则，将使用其主要作业角色的开单费率。<br><p><b>注释</b>

   如果用户日志记录时间没有与其关联的开单费率，并且他们没有职务职责或其职务职责的开单费率，则使用与任务关联的职务职责中的费率。 如果此角色没有计费费率，则收入为$0.00</p></td>
   </tr> 
   </tbody> 
  </table>

* **任务的收入类型是“职责：每小时”**

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">每小时计费率</td> 
     <td>无分配</td> 
     <td>用户分配</td> 
     <td>职务角色分配</td> 
    </tr> 
    <tr> 
     <td role="rowheader">计划收入的每小时开单费率</td> 
     <td>$0.00</td> 
     <td>Workfront查看用户在计算计划收入的任务上履行的职务角色。 <br>如果用户未与任何任务角色关联，则收入为$0.00。 </td> 
     <td>分配给任务的任务职责的开单费率用于计算计划收入。</td> 
    </tr> 
    <tr> 
     <td role="rowheader">实际收入的每小时开单费率</td> 
     <td>Workfront使用用户记录时间的主要作业角色的计费率。 <br>如果记录时间的用户没有与其关联的职务角色，或者如果主要职务角色没有开单费率，则实际收入为$0.00。 </td> 
     <td> 如果将记录时间的用户分配给任务，则任务上与用户关联的任务角色的开单费率将用于计算实际收入。 否则，将使用其主要作业角色的开单费率。 如果用户没有主要职务角色或其主要职务角色没有开单费率，则实际收入为$0.00。 </td> 
     <td>如果将记录时间的用户的某个作业角色分配给该任务，则使用该作业角色比率。 如果分配给任务的任务角色与记录时间的用户没有关联，则将使用用户主要角色的开单费率来计算实际收入。 如果用户没有作业角色或没有与其主要作业角色相关联的费率，则使用分配给该任务的作业角色的费率。 </td> 
    </tr> 
   </tbody> 
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Ideal table but does not come across Markdown</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td colspan="3">Revenue Type = User Hourly</td>
<td colspan="4">Revenue Type = Role Hourly</td>
</tr>
<tr>
<td> <p> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Planned Revenue</strong> </p> </td>
<td> <p>$0.00</p> </td>
<td> <p> If a user has a billing rate in their profile, then that rate is used to calculate Planned Revenue. Otherwise, the system billing rate of their primary job role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> </td>
<td> <p> The system billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> </td>
<td> <p>$0.00</p> </td>
<td> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Revenue. <br>If the user is not associated with any role on the task, the Revenue is $0.00. </p> </td>
<td> <p>The billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Actual Revenue</strong> </p> </td>
<td colspan="2"> <p>If the user logging the hours has a billing rate in their profile, that rate is used. <br>Otherwise, the billing rate of their primary job role is used. If there is no billing rate associated with the user or their primary role, the Actual Revenue is $0.00. <br><note type="note">
Only the rates associated with the user logging the time are taken into account for the calculation, even when another user is assigned to the task.
</note></p> </td>
<td> If the user logging the hours has a billing rate in their profile, that rate is used. Otherwise, the billing rate of their primary job role is used.<br><note type="note">
If the user logging time has no billing rate associated with them, and they do not have a job role or a billing rate for their job role, then the rate from the job role associated with the task is used. If there is no billing rate for this role, the revenue is $0.00
</note></td>
<td> <p>Workfront uses the billing rate of the primary job role of the user logging the time. <br>If the user logging the time has no job role associated with them, or if the primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p> If the user logging the time is assigned to the task, the billing rate of the job role associated with the user on the task is used to calculate the Actual Revenue. Otherwise, the billing rate of their primary job role is used. If the user has no primary job role or if their primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p>If one of the job roles of the user logging the time is assigned to the task, that job role rate is used. If the job role assigned to the task is not associated with the user logging the time, then the billing rate of the primary role of the user is used to calculate the Actual Revenue. If the user does not have a job role or there is no rate associated with their primary job role, then the rate of the job role assigned to the task is used. </p> </td>
</tr>
</tbody>
</table>
</div>
-->

### 项目的收入计算

您可以跟踪项目的以下收入类型：

* 项目的计划收入按以下公式计算：

   ```
   Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue
   ```

   有关如何计算“计划收入”任务的信息，请参阅 [基于用户和角色分配的任务的收入计算](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) 章节。

* 项目的实际收入按以下公式计算：

   ```
   Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)
   ```

有关如何计算“实际收入”任务的信息，请参阅 [基于用户和角色分配的任务的收入计算](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) 章节。

对于与直接记录到项目的小时数或相关问题相关的实际收入，Workfront会使用记录项目时间的用户的帐单费率。 如果用户没有与其配置文件关联的开单费率，则Workfront会使用其主要职务角色的开单费率。 如果两个费率均为零，则与项目登录小时数或问题相关的实际收入为零。
