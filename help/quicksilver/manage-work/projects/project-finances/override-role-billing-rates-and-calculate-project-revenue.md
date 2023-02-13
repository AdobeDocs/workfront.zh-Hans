---
product-area: projects
navigation-topic: financials
title: 改写职务职责开单费率和计算项目收入的概述
description: 当您将项目的收入乘以项目花费的小时数时，您可以使用开单费率计算项目的收入。 有关帐单费率和收入的更多信息，请参阅账单和收入概述一文。
author: Alina
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '3644'
ht-degree: 0%

---

# 改写职务职责开单费率和计算项目收入的概述

当您将项目的收入乘以项目花费的小时数时，您可以使用开单费率计算项目的收入。 有关帐单费率和收入的更多信息，请参阅文章 [账单和收入概述](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because the only procedure here was moved to a different article.&nbsp;This stays as an overview)</p>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Any</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to Projects and Financial&nbsp;Data</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div>
-->

## 职务职责开单费率和职责每小时收入类型概览

作为Adobe Workfront管理员，您可以将帐单费率与用户和工作角色相关联。\
有关创建用户并将其与计费费率关联的详细信息，请参阅文章 [添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). 有关创建职务角色并将其与开单费率关联的详细信息，请参阅文章 [创建和管理作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

无法覆盖与用户关联的计费费率。

在公司或项目层，可以改写与职务角色关联的开单费率。

要根据职务角色的开单费率计算项目收入，请 **收入类型** 项目中的任务必须是以下任务之一：

* 角色小时
* 受限角色小时
* 每小时加固定角色

有关 **收入类型** 和账单费率，请参阅 [账单和收入概述](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 计算收入时开单费率覆盖的层次结构

职务角色可以通过以下方式为其关联计费费率：

* 作为Workfront管理员，您可以在创建作业角色时定义与作业角色关联的系统级别开单费率。\
   有关创建作业角色的更多信息，请参阅 [创建和管理作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* 作为Workfront管理员，您可以在创建公司时为同一职务角色定义公司级开单费率。\
   当Workfront计算与此公司关联的项目的收入时，在将角色分配给任务时，将使用公司开单费率，而不是此职务角色的系统级开单费率。\
   在公司级别更改的职务角色费率将影响与该公司关联的所有项目。

   >[!NOTE]
   >
   >如果您需要更新公司开单费率，则项目费率不会自动更新。 您必须先将公司从项目中删除，更新公司费率，然后将公司重新连接到项目，新公司费率才能对项目生效。 有关将公司附加到项目的说明，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

   有关创建特定于公司的职务角色开单费率的详细信息，请参阅 [创建和编辑公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* 作为Workfront管理员，您可以在编辑项目时启用一个选项，以在用户手动重新计算项目财务时，将对公司级开单费率所做的更改应用到项目。\
   有关更多信息，请参阅 [使用公司层开单费率改写项目层开单费率](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

* 作为项目经理，您可以在项目层为同一职务角色定义开单费率。\
   项目中更改的职务角色费率只会影响该项目。

   有关覆盖项目角色费率的信息，请参阅 [在项目层改写职务职责开单费率](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>如果职务职责与系统层、公司层和项目层的开单费率关联，则Workfront在使用职务职责费率时，使用项目层职务职责的开单费率计算任务的收入。 所有任务的收入累计到项目的收入。

## 在项目层改写职务职责开单费率

作为项目经理，您可以指定特定项目中某个职务角色的开单费率。 此项目层开单费率将覆盖此职务角色系统层的开单费率。 Workfront使用职务角色的项目层开单费率来计算收入，而不是使用系统层开单费率。

有关如何在项目层改写职务职责开单费率的信息，请参阅 [在项目层改写职务职责开单费率](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

有关用于计算项目收入的职务职责的详细信息，请参阅 [账单和收入概述](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>对于实际收入，对添加到标记为已开单的开单记录的小时适用的开单费率，不应受开单记录开单后发生的开单费率改写的影响。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and linked above to the stand-alone article for overriding billing rates on projects.)</p>
<p>You can override the billing rate of a job role on a project in the following ways:</p>
<ul>
<li>One time, by selecting a new rate for the job role.<br>The new rate is used for the entire duration of the project, to calculate revenue. </li>
</ul>
<ul>
<li>Several times, by selecting several new rates for specific date ranges. <br>A different rate can be used during each specified date range.</li>
</ul>
<p>To override a billing rate for a project:</p>
<ol>
<li value="1">Go to the project you want to override billing rates for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Billing Rates</strong> in the left panel. You might have to first click <strong>Show More</strong>. </p> </li>
<li value="3"> <p>Click <strong>Add Billing Rate</strong> > <strong>New Billing Rate</strong>.</p> <p>The New Billing Rate box opens</p> <p> <img src="assets/override-billing-rate-on-project-nwe-350x310.png" style="width: 350;height: 310;"> </p> <p> <br>The <strong>Default Billing Rate</strong> field displays the system-level rate for this job role.</p> </li>
<li value="4">In the <strong>Job Role</strong> field, select the job role you want to change the billing rate for.<br></li>
<li value="5">In the <strong>Billing Rates 1</strong> field, enter the one time billing rate override, then click <strong>Save</strong> to override the billing rate one time, <br>Or Click <strong>Add Rate</strong> to add more billing rate overrides.</li>
<li value="6">(Conditional) If you are adding more than one billing rate override, specify the following information:<br>- <strong>Billing Rates 1</strong>: the value of the Billing Rate from the beginning of the project to the first date of the first override. This is typically the same amount as the <strong>Default Rate</strong>.<br>- <strong>Start Date</strong>: this is the date when the Default Rate ends.<br>- <strong>End Date</strong>: the date when the new billing rate override ends. <br>Workfront applies the override job role rate to the hours that occur during the time frames specified when calculating revenue on the project.<br>There should be no gaps between the time frames of two override rates. The <strong>Start Date</strong> of an override rate should be the day immediately following the <strong>End Date</strong> of the previous override date.<br><note type="note">
You cannot specify a
<strong>Start Date</strong> for the first override rate, nor an
<strong>End Date</strong> for the last override rate. We recommend that you use the Default Rate for the first override rate.
<br>Workfront assumes that the first override rate is applied for all hours with a date older than the
<strong>End Date</strong> of the first override, and that the last override rate is applied for all hours with a date newer than the
<strong>Start Date</strong> of the last override.
<br>If an hour is logged before the Planned Start Date of the project the very first billing rate is used.
<br>If an hour is logged after the Planned Completion Date of the project the very last billing rate is used.
</note><br></li>
<li value="7">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## 项目的“计费费率”部分概述

在为与项目关联的职务角色指定改写开单费率后，您可以在 **计费费率** 选项卡。

请注意 **计费费率**:

* [作业角色分组](#job-role-grouping)
* [项目开单费率值](#project-billing-rate-value)
* [默认开单费率值](#default-billing-rate-value)
* [公司账单费率值](#company-billing-rate-value)
* [多个计费费率值和时间范围](#multiple-billing-rate-values-and-timeframes)

### 作业角色分组 {#job-role-grouping}

计费费率在 **计费费率** 区域。

### 项目开单费率值 {#project-billing-rate-value}

在对应于职务职责的分组行中，注意该职务职责在项目层的开单费率 **项目开单费率** 列。 如果职务职责具有多个改写率，则对应于当前日期的改写率将显示在 **项目开单费率** 列。

### 默认开单费率值 {#default-billing-rate-value}

在职务职责的分组行中，注意该职务职责在系统层的开单费率 **默认开单费率** 列。

>[!NOTE]
>
>如果职务职责的项目开单费率为 **默认开单费率** 不会应用于计算项目的收入。 仅 **项目开单费率** 用于计算收入。

### 公司账单费率值 {#company-billing-rate-value}

在职务职责的分组行中，注意该职务职责在公司层的开单费率 **公司账单费率** 列。 这意味着有一个公司与此项目关联，并且此职务角色对该公司的计费费率不同。 即使与项目费率相同，也会显示公司的开单费率。

>[!NOTE]
>
>如果职务职责的项目开单费率为 **公司账单费率** 不会用于计算项目的收入。 仅 **项目开单费率** 用于计算收入。

### 多个计费费率值和时间范围 {#multiple-billing-rate-values-and-timeframes}

如果您对特定职务职责具有多个改写开单费率，则这些费率将列在该职务职责的分组下。 使用内联编辑，您可以更改覆盖率和 **开始** **日期** 和 **结束日期** 覆盖计费费率的值。

>[!NOTE]
>
>您无法指定 **开始日期** ，并且您无法指定 **结束日期** 的值。 Workfront假定当日期早于 **结束日期** ，并且对于日期早于 **开始日期** 最后一次覆盖。\
>如果在项目的计划开始日期之前记录了一个小时，则使用第一个开单费率。\
>如果在项目的计划完成日期后记录了一个小时，则使用最后一个开单费率。

## 计算计划收入

* [根据一次性开单费率改写计算计划收入](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [根据多个开单费率改写计算计划收入](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [在任务持续时间内计划小时数的分配](#distribution-of-planned-hours-across-the-duration-of-a-task)

### 根据一次性开单费率改写计算计划收入 {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

在根据一次性开单费率改写计算计划收入时，请考虑以下事项：

* 当 **收入类型** 任务是 **每小时角色**,Workfront将任务的计划小时数乘以与任务关联的任务职责的开单费率，以计算任务的计划收入。

* 当任务角色的开单费率在项目层被改写时，Workfront会使用项目中的改写费率来计算计划收入。
* 当任务具有多个分配时，计划收入的计算方式是将每个分配的任务职责的开单费率与其各自的计划小时分配相乘。

>[!NOTE]
>
>对于多个分配，每个分配的计划小时数与任务的计划小时数不同。

有关用于计算计划收入的职务职责的详细信息，请参阅文章中的“了解基于用户和职责分配的任务的收入计算”一节 [账单和收入概述](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### 根据多个开单费率改写计算计划收入 {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

在根据多个开单费率改写计算计划收入时，请考虑以下事项：

* 当 **收入类型** 任务是 **每小时角色**,Workfront将任务的计划小时数乘以与任务关联的任务职责的开单费率，以计算任务的计划收入。

   有关用于计算计划收入的职务职责的详细信息，请参阅文章中的“了解基于用户和职责分配的任务的收入计算”一节 [账单和收入概述](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* 在多次开单费率改写的情况下，计划小时数乘以计划小时数的费率在任务期间发生更改。 默认情况下，Workfront会在任务的持续时间内平均分配计划小时数，为任务的每一天分配相等的小时数。 计算时 **计划收入** 对于任务，Workfront将计划小时数乘以当天的开单费率。 如果计费费率为多个，则该费率可能会每天不同。

   例如，您的任务具有“每小时”角色 **收入类型**. 任务的持续时间为5天，“计划小时数”值为40小时。 每天的计划时数为8小时。 为任务分配“项目经理”职务职责，并改写此职务职责在任务最后3天的开单费率，因此您将具有前两天的费率1开单费率，以及此职务职责剩余3天的费率2开单费率。

   计算 **计划收入** 其中：

   ```
   Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
   ```

有关在Workfront中查找每日计划小时数金额的更多信息，请参阅部分 [在任务持续时间内计划小时数的分配](#distribution-of-planned-hours-across-the-duration-of-a-task) 在本文中。

>[!NOTE]
>
>如果任务上有多个受分配人，则计划小时数会先分配给每个受分配人，然后分配给任务期间的每一天。 在这种情况下，计划收入将考虑每个受分配人的每日小时数以及每个任务职责的开单费率，在多个开单费率的情况下，这些开单费率在任务期间可能会发生变化。

### 在任务持续时间内计划小时数的分配 {#distribution-of-planned-hours-across-the-duration-of-a-task}

了解任务持续时间内计划时间的分配时，请考虑以下事项：

* 默认情况下，Workfront会在任务的持续时间内平均分配计划小时数，并根据项目计划的可用性为任务的每一天分配等数的计划小时数。

   有关了解任务持续时间内计划小时数分配的详细信息，请参阅文章中的“了解任务持续时间内计划小时数的分配”部分 [计划时数概述](../../../manage-work/tasks/task-information/planned-hours.md).

   >[!NOTE]
   >
   >“每日计划小时数”是任务持续时间内每天计划小时数的分配。 如果任务具有一个分配，则此数字表示每个分配每天的计划小时数。 如果任务具有多个分配，则每日计划小时数分配与任务的每日计划小时数不同。 对于具有多个分配的任务，Workfront中没有每个分配的每日计划时数的可视表示形式。
   >
   >
   >“每日计划小时数”乘以分配给该日任务的任务职责的开单费率，以计算该任务的“每日计划收入”。 以此方式计算的所有每日计划收入的总和等于该任务的计划收入。

## 计算实际收入

* [根据一次性开单费率改写计算实际收入](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [根据多个开单费率覆盖计算实际收入](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### 根据一次性开单费率改写计算实际收入 {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

在根据一次性开单费率改写计算实际收入时，请考虑以下事项：

* 当 **收入类型** 任务是 **每小时角色**, Workfront **实际小时数** 任务的开单费率，与任务关联以计算的任务职责 **实际收入** 任务。 实际小时数是直接记录到任务的小时数。

   有关用于计算哪个作业角色的详细信息 **实际收入**，请参阅文章中的“了解基于用户和角色分配的任务的收入计算”部分 [账单和收入概述](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* 如果任务角色的开单费率已在项目层改写，则Workfront会使用项目中的改写费率来计算实际收入。 当您改写项目上职务角色的开单费率时， **实际收入** 使用新的调整率自动重新计算项目的数量。

   有关覆盖项目角色费率的信息，请参阅 [在项目层改写职务职责开单费率](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>如果要在超过按原始费率计费的原始开单费率之前保留已登录项目的小时数，则必须将它们包含在 **账单记录**，并且您必须将 **账单记录** as **已计费**. 否则， **实际收入** 重新计算项目财务时，将使用新费率重新计算项目开单费率之前记录的小时数。\
>有关在账单记录中包含小时数并将其标记为 **已计费**，请参阅文章 [创建帐单记录](../../../manage-work/projects/project-finances/create-billing-records.md).

### 根据多个开单费率覆盖计算实际收入 {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

在计算基于多个开单费率覆盖的实际收入时，请考虑以下事项：

* 当 **收入类型** 任务是 **每小时角色**, Workfront **实际小时数** 任务的开单费率分配给任务以计算 **实际收入** 任务。 实际小时数是直接记录到任务的小时数。

* 如果计费费率覆盖多次， **实际小时数** 乘以计算 **实际收入** 可能会在任务持续期间发生更改。 Workfront使用其时间范围与 **登录日期** 为要计算的任务记录的小时数 **实际收入。**

   例如，某项任务具有 **收入类型** of **每小时角色** 和被分配给项目经理的作业角色。 在6月19日到6月25日之间的日期，使用费率1覆盖此职务角色的开单费率。 从6月26日开始，使用费用2覆盖计费费率。 6月20日为2小时，6月28日为3小时。

   Workfront计算 **实际收入** 使用以下公式执行此任务：

   ```
   Actual Revenue = 2 * Rate 1 + 3 * Rate 2
   ```

   有关用于计算哪个作业角色的详细信息 **实际收入**，请参阅文章中的“了解基于用户和角色分配的任务的收入计算”部分 [账单和收入概述](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 时区在基于多个计费费率计算收入时的影响

如果用户与Workfront中的其他实体之间存在时区差异，则用户每天可以看到与其他用户不同的计划小时数。 以下方案可能会将用户的每日计划时数信息与其他用户看到的信息产生偏差：

* 两个用户的计算机可能会设置为两个不同的时区
* Workfront中的两个用户配置文件可能会设置为两个不同的时区
* 与用户配置文件关联的时区可能与Workfront中的系统时区不同
* 与用户配置文件关联的时区可能与项目计划的时区不同。

在这些情况下，对于不共享相同时区设置的两个用户，每日计划时数可能会有所不同。 在项目上使用多个开单费率改写时，他们还会看到不同的计划收入编号。

* [计算不同时区中用户的计划收入](#calculate-planned-revenue-for-users-in-different-time-zones)
* [计算不同时区中用户的实际收入](#calculate-actual-revenue-for-users-in-different-time-zones)

### 计算不同时区中用户的计划收入 {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>如果不同时区的用户处理同一项目，我们建议您不要在一周内更改项目的开单费率改写。 这样做可能会由于用户计划中的时区与Workfront系统时区之间的时区之间的小时差，为您的项目显示错误的计划收入金额。 大多数计划允许将周末从“计划小时数”计算中排除。 如果在职务职责的开单费率改写中发生更改，则在周末期间发生更改比在一周中间发生更改时（与任务持续时间的中间时间一致）更好。

在为不同时区的用户计算计划收入时，请考虑以下事项：

* 对于具有 **收入类型** of **每小时角色** 并被分配给作业角色， **计划收入** 是乘以 **计划小时数** 任务的开单费率。

* 的 **计划小时数** 均布于 **持续时间** 任务。

* 的 **持续时间** 是 **计划开始** **日期** 和 **计划完成日期** 任务。 因为&#x200B;**计划开始日期** 和 **计划完成日期** 根据查看任务的用户所在时区的不同，其中的任务可能会有所不同，对于两个不同时区的两个用户，每天计划时数的值可能会有所不同。

* 如果任务职责的开单费率未更改，或者只有一个开单费率改写，则每日计划小时数金额不会更改项目的计划收入。 在这种情况下，即使来自两个不同时区的两个用户每天看到不同的计划小时数，项目的整体计划收入在两个用户之间也是相同的。

   但是，如果计费费率覆盖多次，则 **计划收入** 对于处于两个不同时区的两个用户而言，项目可能看起来有所不同，因为它依赖于每天计划小时数（对于两个用户而言，这可能不同）和计费率覆盖（当每个用户在各自时区中查看任务时，该时间可能不同）。

* 准确 **计划收入** amount是与Workfront实例的时区相同的用户看到的时区。 您的Workfront管理员在“系统客户信息”区域中定义Workfront时区。\
   有关为系统定义时区的详细信息，请参阅文章 [配置系统的基本信息](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### 计算不同时区中用户的实际收入 {#calculate-actual-revenue-for-users-in-different-time-zones}

在为不同时区的用户计算实际收入时，请考虑以下事项：

* 当 **收入类型** 任务是 **每小时角色**, Workfront **实际小时数** 任务的开单费率分配给任务以计算 **实际收入**. 实际小时数是直接记录到任务的小时数。

* 如果多次开单费率改写，Workfront会使用其时间范围与 **登录日期** 为要计算的任务记录的小时数 **实际收入**.

* 因为 **登录日期** 的日期范围上没有时间戳， **实际收入** 计算不受与用户关联的时区影响。

有关用于计算哪个作业角色的详细信息 **实际收入**，请参阅文章中的“了解基于用户和角色分配的任务的收入计算”部分 [账单和收入概述](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 重新计算项目财务

在项目记录的小时内发生更改时，会对项目计算财务。

如果在项目生命周期中费率发生更改，您可以使用项目上的“重新计算财务”选项人工重新计算项目的成本和收入。 此外，某些操作会触发自动重新计算。

有关重新计算项目财务的详细信息，请参阅文章 [重新计算项目财务](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## 使用API添加新的计费费率

要使用API为作业角色添加新计费率，请执行 *setRatesForRole* 操作 **比率** 对象使用 *PUT方法*.
上的操作和日期字段 **比率** 对象在API 8.0版中可用。如果您已经为项目上的职务角色定义了多个计费费率，并且希望为项目添加新的计费费率，并且该费率具有新的日期范围，则必须同时包含现有费率和要在同一API调用中添加的费率。 这类似于在对象上更新集合的方式。

以下API调用示例 **accableedID** 是 **项目ID** 的项目中添加了 **角色ID** 是 **作业角色ID** 您要为其添加新计费费率。<pre>{</pre><pre>&quot;accableedID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;accaptibeObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df000014148cda5136d4b79d09&quot;, </pre><pre>&quot;rates&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null，&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>有关使用Workfront API的更多信息，请参阅文章 [API基础知识](https://experience.workfront.com/s/article/API-Basics-638808549).
