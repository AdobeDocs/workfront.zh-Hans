---
navigation-topic: financials
title: 创建帐单记录
description: 除了设置收入和跟踪费用之外，您还可以在项目上创建计费记录，以了解需要计费的信息。
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1934'
ht-degree: 1%

---

# 创建帐单记录

除了设置收入和跟踪费用之外，您还可以在项目上创建计费记录，以了解需要计费的信息。

您不能为任务创建计费记录。 您只能为项目创建计费记录。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目和财务数据的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限，并具有管理财务的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 账单记录概述

开单记录将作为项目的附件创建，并包含项目中的财务数据以及项目中任务的一些财务信息。

在计划使用计费记录时，请考虑以下事项：

* 如果要将与项目相关的金额开单给外部供应商或合作伙伴时，可以创建开单记录。 除了将固定金额开单给外部来源之外，有时您还需要将项目的工作量（从已记录的小时数）开单给外部承包商，以及已发生的费用或固定收入金额。 您可以将所有这些信息包含在同一账单记录中。
* 将帐单记录设置为“已计费”后，便无法编辑该记录。

   >[!IMPORTANT]
   >
   >当您的费率不同并且您希望锁定项目的收入和费用信息时，这一点很重要。 将其添加到账单记录并标记为已计费，会在费率在您的系统中更新时阻止更新该记录。

* 无法删除已标记为已开单的开单记录的项目。

## 创建账单记录

1. 导航到项目。
1. 单击 **帐单记录** 中。

   此部分可能位于 **显示更多**.

1. 使用 **帐单记录详细信息** 在左侧面板中选择，单击 **新帐单记录**.
1. 在 **新帐单记录** 框中，指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>这是必填字段. 为帐单记录指定描述，以反映此记录的用途或意图。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">记帐状态</td> 
      <td> <p>选择 <strong>未计费</strong>，则此记录尚未开单。</p> <p>选择 <strong>已计费</strong> 开单记录开单时。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">记帐日期</td> 
      <td>通过单击日历图标，选择此计费记录开单的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">订单号</td> 
      <td>如果存在与此开单记录关联的PO编号，请在此字段中指定此信息。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">发票 ID</td> 
      <td>如果有与此开单记录关联的发票，请在此字段中指定此信息。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">附加金额</td> 
      <td>输入开单记录的固定金额。 这是您打算为此项目向外部客户、承包商或合作伙伴开单的金额。 在帐单记录的状态更改为已开单后，无法修改此金额。</td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）在 **自定义Forms**，选择要添加到帐单记录的帐单记录自定义表单。

   您（或有权访问自定义表单的其他用户）必须先创建账单记录自定义表单，然后才能在此处选择该表单。 列表中仅显示活动的自定义表单。 有关创建自定义表单的信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   您可以重复此步骤，以添加您需要用于帐单记录的其他自定义表单。

1. 单击 **保存。**

   将创建帐单记录。 要在帐单记录中包含“可计费小时数”、“费用”和“固定收入”，请按照以下子部分中列出的步骤操作。

## 在计费记录中包括计费小时数、费用和固定收入

* [在计费记录中包括计费小时数](#include-billable-hours-in-a-billing-record)
* [在计费记录中包括计费费用](#include-billable-expenses-in-a-billing-record)
* [在账单记录中包含固定收入](#include-fixed-revenues-in-a-billing-record)

### 在计费记录中包括计费小时数 {#include-billable-hours-in-a-billing-record}

您可以将已登录任务、问题或项目的小时包含在帐单记录中。\
如果记录小时数或其主要职务角色的用户与每小时费率计费相关联，则这些小时的收入将添加到计费记录中。

* [可以将哪些小时添加到账单记录](#what-hours-can-be-added-to-a-billing-record)
* [将小时数添加到账单记录](#add-hours-to-a-billing-record)

#### 可以将哪些小时添加到账单记录 {#what-hours-can-be-added-to-a-billing-record}

在满足以下条件时，您可以向账单记录添加小时数：

* 任务、问题或项目已记录小时数。
* 记录小时的小时类型会标记为“计为收入”。

   有关小时类型的详细信息，请参阅文章 [管理小时类型](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* 如果记录时间的用户具有与他们或他们的主要作业角色相关联的每小时帐单费率，则针对问题或项目记录的所有小时都可以添加到帐单记录中。
* 如果任务记录了小时数，则任务必须具有以下收入类型：

   * “收入类型”不能设置为“不可计费”。
   * 如果“收入类型”设置为“用户每小时”，则记录该时间的用户在其配置文件中必须设置“每小时计费”费率。
   * 如果“收入类型”设置为“每小时”角色，则记录时间的用户的“主要角色”必须具有每小时开单费率。

      >[!NOTE]
      >
      >您可以在项目层改写职务角色的开单费率。\
      >有关改写职务职责开单费率的详细信息，请参阅文章中的“在项目层改写职务职责开单费率”一节 [改写职务职责开单费率和计算项目收入的概述](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* 如果 **需要时间批准此项目** 在“项目设置”下选中，则项目所有者必须批准记录的小时数。\
   有关要求在项目时间进行审批的详细信息，请参阅文章 [需要时间来批准项目](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### 将小时数添加到账单记录 {#add-hours-to-a-billing-record}

要向计费记录添加计费小时数，请执行以下操作：

1. 转到包含帐单记录的项目。
1. 单击 **帐单记录** 中。

   此部分可能位于 **显示更多**.

1. 单击 **描述** 开单记录的 **帐单记录详细信息** 选项卡。

1. 单击 **计费小时数** 中。
1. 如果账单记录中可能包含的小时数，请单击 **添加小时数**.\
   的 **添加计费小时数** 框中。

   >[!NOTE]
   >
   >如果没有记录小时数，或者记录的小时数不符合添加到账单记录所需的条件，则 **添加小时数** 按钮。 有关哪些小时可以记录到账单记录的更多信息，请参阅部分 [可以将哪些小时添加到账单记录](#what-hours-can-be-added-to-a-billing-record) 在本文中。

1. 选择要包含在帐单记录中的小时条目，然后单击 **添加小时数**.\
   小时的实际成本将作为 **计费小时数** 金额 **账单记录总计**.

1. （可选）单击 **帐单记录详细信息** 查看 **计费小时数** 和 **账单记录总计** 金额。 您还可以在开单记录标题中查看开单记录合计。

### 在计费记录中包括计费费用 {#include-billable-expenses-in-a-billing-record}

如果要将“可开单费用”添加到开单记录，请确保任务和项目的费用标记为“可开单”。 未标记为“可计费”的费用无法添加到帐单记录中。 有关添加费用的详细信息，请参阅文章 [管理项目费用](../../../manage-work/projects/project-finances/manage-project-expenses.md).

要将可计费费用添加到计费记录，请执行以下操作：

1. 转到包含帐单记录的项目。
1. 单击 **帐单记录** 中。

   您可能需要单击 **显示更多**，则 **帐单记录**.

1. 单击 **描述** 开单记录的 **帐单记录详细信息** 选项卡。

1. 单击 **可计费费用** 中。
1. （视情况而定）如果已在任务或项目中添加费用并将其标记为“可计费”，请单击 **添加费用**.

   >[!NOTE]
   >
   >如果您有费用，但未标记为“可计费”，则 **添加费用** 按钮。 只有实际金额大于零的可计费费用才有资格纳入开单记录。

1. 选择可添加到帐单记录的可计费费用，然后单击 **添加费用**.\
   费用的实际金额作为 **可计费费用** 金额 **账单记录总计**.

1. （可选）单击 **帐单记录详细信息** 查看 **可计费费用** 和 **账单记录总计** 金额。 您还可以在开单记录标题中查看开单记录合计。

### 在账单记录中包含固定收入 {#include-fixed-revenues-in-a-billing-record}

如果您的任务具有“固定收入”可用，则可以将“固定收入”添加到帐单记录中。 在开单记录中无法添加其他类型的任务或项目收入。 有关收入类型的更多信息，请参阅 [账单和收入概述](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) 部分 [账单和收入概述](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

要向计费记录添加固定收入，请执行以下操作：

1. 转到包含帐单记录的项目。
1. 单击 **帐单记录** 中。

   您可能需要单击 **显示更多**，则 **帐单记录**.

1. 单击 **描述** 开单记录的 **帐单记录详细信息** 选项卡。

1. 选择 **固定收入** 选项卡。
1. 如果您向任务中添加了固定收入，请单击 **添加固定收入**.

   >[!NOTE]
   >
   >如果任务的收入额未标记为“已修复”，则 **添加固定收入** 按钮。

1. 选择要在帐单记录中包含其固定收入的任务，然后单击 **添加任务**.\
   的 **固定收入** 任务量将作为 **计费收入** 金额 **账单记录总计**.

1. （可选）单击 **帐单记录详细信息** 查看 **计费收入** 和 **账单记录总计** 金额。 您还可以在开单记录标题中查看开单记录合计。

## 编辑账单记录

在创建账单记录并在账单记录中包括小时数、费用和收入后，您可以在将现有记录标记为已开单之前，编辑现有记录上的某些信息。

1. 转到帐单记录。
1. 使用 **帐单记录详细信息** 在左侧面板中选择，编辑任何可用字段中的信息

   或

   单击 **“编辑”图标** ![](assets/edit-icon.png) ，然后编辑任何可用字段中的信息。

   更新以下内容：

   * **描述**
   * **记帐状态**

      >[!TIP]
      >
      >如果您选择 **已计费** 对于“帐单状态”，在保存更改后，无法编辑帐单记录。

   * **记帐日期**
   * **订单号**
   * **发票 ID**
   * **附加金额**

   以下字段不可编辑：

   * **计费小时数：** 计费记录中包含的小时的实际收入总和。 有关在账单记录中包含小时数的更多信息，请参阅部分 [在计费记录中包括计费小时数](#include-billable-hours-in-a-billing-record) 在本文中。

   * **可计费费用**:计费记录中包含的计费费用的实际金额总数。 有关在账单记录中包含可计费费用的详细信息，请参阅 [在计费记录中包括计费费用](#include-billable-expenses-in-a-billing-record) 在本文中。

   * **计费收入**:计费记录中包含的任务的固定收入总数。 有关在账单记录中包含固定收入的更多信息，请参阅部分 [在账单记录中包含固定收入](#include-fixed-revenues-in-a-billing-record) 在本文中。

   * **账单记录总计**:所有可计费金额的合计。 这由以下公式计算：

      ```
      Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
      ```


1. 单击 **保存****更改**.
