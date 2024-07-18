---
navigation-topic: financials
title: 创建开票记录
description: 除了设置收入和跟踪费用外，您还可以在项目上创建需要记帐的信息的记帐记录。
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1934'
ht-degree: 0%

---

# 创建开票记录

除了设置收入和跟踪费用外，您还可以在项目上创建需要记帐的信息的记帐记录。

无法创建任务的开票记录。 您只能为项目创建开票记录。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目和财务数据的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理具有管理财务权限的项目权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 开票记录概述

开单记录作为项目的附件创建，包含项目的财务数据以及项目中任务的一些财务信息。

在计划使用开票记录时，请考虑以下事项：

* 如果您要向外部供应商或合作伙伴开出与项目相关的金额，则可以创建开票记录。 除了向外部来源开单固定金额外，有时您还需要向外部承包商开单项目工作量（从记录的小时数），以及发生的费用或固定收入金额。 您可以将所有这些信息包含在同一个开票记录中。
* 开票记录一旦设置为“已开票”，就无法编辑。

  >[!IMPORTANT]
  >
  >当费率不同并且您想要锁定项目的收入和费用信息时，这一点很重要。 将其添加到记帐记录并标记为已记帐，可防止在系统中更新费率时更新该记录。

* 不能删除已标记为已记帐的记帐记录的项目。

## 创建开票记录

1. 导航到项目。
1. 单击左侧面板中的&#x200B;**记帐记录**。

   此分区可能位于&#x200B;**显示更多**&#x200B;下。

1. 在左侧面板中选择&#x200B;**记帐记录详细信息**，单击&#x200B;**新建记帐记录**。
1. 在显示的&#x200B;**新账单记录**&#x200B;框中，指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>这是必填字段。 指定开票记录的描述，以反映此记录的目的或意图。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">记帐状态</td> 
      <td> <p>如果此记录尚未记帐，请选择<strong>未记帐</strong>。</p> <p>在记帐记录时选择<strong>已记帐</strong>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计费日期</td> 
      <td>通过单击日历图标，选择对此开票记录记帐的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">订单号</td> 
      <td>如果存在与此开票记录关联的PO编号，请在此字段中指定此信息。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">发票 ID</td> 
      <td>如果存在与此开票记录关联的发票，请在此字段中指定此信息。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">附加金额</td> 
      <td>输入开票记录的固定金额。 这是您计划为此项目向外部客户、承包商或合作伙伴支付的金额。 当记帐记录的状态更改为“已记帐”后，无法修改此金额。</td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）在&#x200B;**自定义Forms**&#x200B;下，选择要添加到开票记录的开票记录自定义表单。

   您（或其他有权访问自定义表单的用户）必须先创建账单记录自定义表单，然后才能在此处选择。 列表中仅显示活动的自定义表单。 有关创建自定义表单的信息，请参阅[使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

   您可以重复此步骤以添加账单记录所需的其他自定义表单。

1. 单击&#x200B;**保存。**

   创建开票记录。 要在开票记录中包括可开票小时数、费用和固定收入，请按照以下子部分中列出的步骤操作。

## 在开票记录中包括可开票小时数、费用数和固定收入

* [在开票记录中包含可开票小时数](#include-billable-hours-in-a-billing-record)
* [在记帐记录中包含可记帐费用](#include-billable-expenses-in-a-billing-record)
* [在开票记录中包含固定收入](#include-fixed-revenues-in-a-billing-record)

### 在开票记录中包含可开票小时数 {#include-billable-hours-in-a-billing-record}

您可以在账单记录中包含已登录任务、问题或项目的小时数。\
如果记录小时数的用户或其主要工作角色与记帐/小时率关联，则来自这些小时的收入将添加到记帐记录。

* [可向开票记录添加哪些小时](#what-hours-can-be-added-to-a-billing-record)
* [将小时数添加到开票记录](#add-hours-to-a-billing-record)

#### 可以向开票记录添加的小时数 {#what-hours-can-be-added-to-a-billing-record}

当满足以下条件时，您可以向开票记录添加小时数：

* 任务、问题或项目记录了小时数。
* 记录的小时数的“小时类型”被标记为收入。

  有关小时类型的详细信息，请参阅文章[管理小时类型](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md)。

* 如果记录时间的用户具有与其或其主要工作角色关联的按小时计费率，则为问题或项目记录的所有小时数可以添加到计费记录。
* 如果任务记录了小时数，则任务必须具有以下收入类型：

   * 收入类型不能设置为不可记帐。
   * 如果收入类型设置为每小时用户，则记录时间的用户必须在他们的用户档案中设置每小时记帐费率。
   * 如果收入类型设置为每小时角色，则记录时间的用户的主要角色必须具有每小时计费率。

     >[!NOTE]
     >
     >您可以在项目级别覆盖工作角色的计费率。\
     >有关覆盖工作角色记帐费率的详细信息，请参阅[有关覆盖工作角色记帐费率和计算项目收入的概述](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)一文中的“在项目级别覆盖工作角色记帐费率”一节。

* 如果在“项目设置”下选中&#x200B;**此项目需要批准时间**，则项目所有者必须批准记录的小时数。\
  有关要求批准项目小时数的详细信息，请参阅文章[要求批准项目的时间](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md)。

#### 将小时数添加到开票记录 {#add-hours-to-a-billing-record}

要将可记帐小时数添加到记帐记录，请执行以下操作：

1. 转到包含开票记录的项目。
1. 单击左侧面板中的&#x200B;**记帐记录**。

   此分区可能位于&#x200B;**显示更多**&#x200B;下。

1. 单击开票记录的&#x200B;**描述**&#x200B;以打开&#x200B;**开票记录详细信息**&#x200B;选项卡。

1. 单击左侧面板中的&#x200B;**可记帐小时数**。
1. 如果开票记录中可能包含小时，请单击&#x200B;**添加小时**。\
   将打开&#x200B;**添加可记帐小时**&#x200B;框。

   >[!NOTE]
   >
   >如果未记录小时数，或者记录的小时数不符合添加到开票记录所需的条件，则不会显示&#x200B;**添加小时数**&#x200B;按钮。 有关哪些小时可以记录到开票记录的更多信息，请参阅本文中的[哪些小时可以添加到开票记录](#what-hours-can-be-added-to-a-billing-record)部分。

1. 选择要包括在开票记录中的小时条目，然后单击&#x200B;**添加小时数**。\
   小时实际成本作为&#x200B;**可记帐小时**&#x200B;金额添加到&#x200B;**记帐记录总计**。

1. （可选）单击&#x200B;**记帐记录详细信息**&#x200B;以查看&#x200B;**可记帐小时数**&#x200B;和&#x200B;**记帐记录总数**&#x200B;金额。 您还可以在开票记录的标题中查看开票记录总计。

### 在开票记录中包含可开票费用 {#include-billable-expenses-in-a-billing-record}

如果要将可记帐费用添加到记帐记录，请确保将任务和项目上的费用标记为可记帐。 未标记为可记帐的费用不可添加到记帐记录中。 有关添加费用的详细信息，请参阅文章[管理项目费用](../../../manage-work/projects/project-finances/manage-project-expenses.md)。

要将可记帐费用添加到记帐记录，请执行以下操作：

1. 转到包含开票记录的项目。
1. 单击左侧面板中的&#x200B;**记帐记录**。

   您可能需要单击&#x200B;**显示更多**，然后单击&#x200B;**记帐记录**。

1. 单击开票记录的&#x200B;**描述**&#x200B;以打开&#x200B;**开票记录详细信息**&#x200B;选项卡。

1. 单击左侧面板中的&#x200B;**可记帐费用**。
1. （视情况而定）如果您已将费用添加到任务或项目并将它们标记为可记帐，请单击&#x200B;**添加费用**。

   >[!NOTE]
   >
   >如果您有费用但未标记为可记帐，则不会显示&#x200B;**添加费用**&#x200B;按钮。 只有实际金额大于零的可记帐费用才有资格包含在记帐记录中。

1. 选择可添加到记帐记录的可记帐费用，然后单击&#x200B;**添加费用**。\
   费用的实际金额作为&#x200B;**可记帐费用**&#x200B;金额添加到&#x200B;**记帐记录总计**。

1. （可选）单击&#x200B;**记帐记录详细信息**&#x200B;以查看&#x200B;**可记帐费用**&#x200B;和&#x200B;**记帐记录总数**&#x200B;金额。 您还可以在开票记录的标题中查看开票记录总计。

### 在开票记录中包含固定收入 {#include-fixed-revenues-in-a-billing-record}

如果您的任务有可用的固定收入，您可以将固定收入添加到记帐记录。 没有其他类型的任务或项目收入可供添加到开票记录中。 有关收入类型的详细信息，请参阅[帐单和收入概览](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)中的[帐单和收入概览](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)部分。

要将固定收入添加到开票记录，请执行以下操作：

1. 转到包含开票记录的项目。
1. 单击左侧面板中的&#x200B;**记帐记录**。

   您可能需要单击&#x200B;**显示更多**，然后单击&#x200B;**记帐记录**。

1. 单击开票记录的&#x200B;**描述**&#x200B;以打开&#x200B;**开票记录详细信息**&#x200B;选项卡。

1. 选择&#x200B;**固定收入**&#x200B;选项卡。
1. 如果您已将固定收入添加到任务，请单击&#x200B;**添加固定收入**。

   >[!NOTE]
   >
   >如果您的任务上有收入额，但它们未标记为“固定”，则不会显示&#x200B;**添加固定收入**&#x200B;按钮。

1. 选择要将其固定收入包含在开票记录中的任务，然后单击&#x200B;**添加任务**。\
   任务的&#x200B;**固定收入**&#x200B;金额作为&#x200B;**可记帐收入**&#x200B;金额添加到&#x200B;**记帐记录总计**。

1. （可选）单击&#x200B;**记帐记录详细信息**&#x200B;以查看&#x200B;**可记帐收入**&#x200B;和&#x200B;**记帐记录总数**&#x200B;金额。 您还可以在开票记录的标题中查看开票记录总计。

## 编辑开票记录

创建开票记录并在开票记录中包含小时数、费用和收入后，您可以在将其标记为已开票之前编辑现有记录的一些信息。

1. 转到开票记录。
1. 在左侧面板中选择&#x200B;**账单记录详细信息**，编辑任何可用字段中的信息

   或

   单击右上角的&#x200B;**编辑图标** ![](assets/edit-icon.png)，然后编辑任何可用字段中的信息。

   更新以下内容：

   * **描述**
   * **记帐状态**

     >[!TIP]
     >
     >如果您选择&#x200B;**Billed**&#x200B;作为“记帐状态”，则在保存更改后，将无法编辑记帐记录。

   * **记帐日期**
   * **PO编号**
   * **发票ID**
   * **附加金额**

   以下字段不可编辑：

   * **可记帐小时数：**&#x200B;记帐记录中包含的小时数实际收入的总和。 有关在开票记录中包括小时数的详细信息，请参阅本文中的[在开票记录中包括可开票小时数](#include-billable-hours-in-a-billing-record)部分。

   * **可记帐费用**：记帐记录中包含的可记帐费用的实际金额总计。 有关将可记帐费用包含在记帐记录中的更多信息，请参阅本文中的[将可记帐费用包含在记帐记录中](#include-billable-expenses-in-a-billing-record)部分。

   * **可记帐收入**：记帐记录中包含的任务的固定收入总计。 有关在开票记录中包括固定收入的详细信息，请参阅本文中的[在开票记录中包括固定收入](#include-fixed-revenues-in-a-billing-record)部分。

   * **记帐记录总计**：所有可记帐金额的总计。 计算公式如下：

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. 单击&#x200B;**保存****更改**。
