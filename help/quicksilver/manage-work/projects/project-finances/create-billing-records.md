---
navigation-topic: financials
title: 创建开票记录
description: 除了设置收入和跟踪费用外，您还可以在项目上创建需要记帐的信息的记帐记录。
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '1635'
ht-degree: 0%

---

# 创建开票记录

<!-- Audited: 6/2025 -->

除了设置收入和跟踪费用外，您还可以在项目上创建需要记帐的信息的记帐记录。

您不能为任务创建开票记录；您只能为项目创建开票记录。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p></td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>编辑对项目和财务数据的访问权限</td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>管理具有管理财务权限的项目权限</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 开票记录概述

开单记录作为项目的附件创建，包含项目的财务数据以及项目任务的财务信息。

在计划使用开票记录时，请考虑以下事项：

* 如果您要向外部供应商或合作伙伴开出与项目相关的金额，则可以创建开票记录。 除了向外部来源开单固定金额外，有时您还需要向外部承包商开单项目工作量（从记录的小时数），以及发生的费用或固定收入金额。 您可以将所有这些信息包含在同一个开票记录中。
* 帐单记录一旦设置为“已记帐”，就无法编辑。

  >[!IMPORTANT]
  >
  >当费率不同并且您想要锁定项目的收入和费用信息时，这一点很重要。 将其添加到记帐记录并标记为已记帐，可防止在系统中更新费率时更新该记录。

* 不能删除已标记为已记帐的记帐记录项目。

## 创建开票记录

{{step1-to-projects}}

1. 在&#x200B;**项目**&#x200B;页面上，选择一个项目。
1. 单击左侧面板中的&#x200B;**记帐记录**。
1. 单击&#x200B;**新建开票记录**。
1. 在显示的&#x200B;**新开票记录**&#x200B;框中，输入以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>（必需）输入开票记录的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">计费状态</td> 
      <td> <p>如果此记录尚未记帐，请选择<strong>未记帐</strong>。</p> <p>如果记帐记录已经记帐，请选择<strong>已记帐</strong>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计费日期</td> 
      <td>通过单击日历图标选择对此开票记录的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">订单号</td> 
      <td>输入与此开票记录关联的PO编号。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">发票 ID</td> 
      <td>输入与此开票记录关联的发票。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">附加金额</td> 
      <td>输入开票记录的固定金额。 这是您计划为此项目向外部客户、承包商或合作伙伴支付的金额。 此金额在记帐记录状态更改为已记帐后无法修改。</td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）在&#x200B;**自定义Forms**&#x200B;下，选择要添加到记录的记帐记录自定义表单。

   必须先创建开票记录自定义表单，然后才能在此处选择它。 列表中仅显示活动的自定义表单。 有关信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. 单击&#x200B;**保存。**&#x200B;已创建开票记录。

## 在开票记录中包含可开票小时数、支出和固定收入

### 在开票记录中包含可开票小时数 {#include-billable-hours-in-a-billing-record}

您可以在账单记录中包含已登录任务、问题或项目的小时数。

如果记录小时数的用户或其主要工作角色与记帐/小时率关联，则来自这些小时的收入将添加到记帐记录。

* [可向开票记录添加哪些小时](#what-hours-can-be-added-to-a-billing-record)
* [向开票记录添加小时数](#add-hours-to-a-billing-record)

#### 可以向开票记录添加的小时数 {#what-hours-can-be-added-to-a-billing-record}

当满足以下条件时，您可以向开票记录添加小时数：

* 已记录任务、问题或项目的小时数。
* 记录的小时数的“小时类型”被标记为收入。

  有关详细信息，请参阅文章[管理小时类型](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md)。

* 如果记录时间的用户具有与其或其主要工作角色关联的每小时记帐费率，则为问题或项目记录的所有小时都可以添加到记帐记录。
* 如果任务记录了小时数，则任务必须具有以下收入类型：

   * 收入类型不能设置为不可记帐。
   * 如果收入类型设置为每小时用户，则记录时间的用户必须在他们的用户档案中设置每小时记帐费率。
   * 如果收入类型设置为每小时角色，则记录时间的用户的主要角色必须具有每小时记帐费率。

     >[!NOTE]
     >
     >您可以在项目级别覆盖工作角色的计费率。\
     >有关详细信息，请参阅[有关覆盖工作角色记帐费率和计算项目收入的概述](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)一文中的“覆盖项目级别的工作角色记帐费率”一节。

* 如果在“项目设置”下选择了“批准此项目需要时间”选项，则项目所有者必须批准记录的小时数。\
  有关详细信息，请参阅[需要时间来批准项目](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md)。

#### 向开票记录添加小时数 {#add-hours-to-a-billing-record}

{{step1-to-projects}}

1. 在&#x200B;**项目**&#x200B;页面上，选择一个项目。
1. 单击左侧面板中的&#x200B;**记帐记录**。
1. 单击记帐记录&#x200B;**描述**&#x200B;以打开&#x200B;**记帐记录详细信息**&#x200B;选项卡。
1. 单击左侧面板中的&#x200B;**可记帐小时数**。
1. 如果开票记录中可能包含小时，请单击&#x200B;**添加小时**。 将打开&#x200B;**添加可记帐小时数**&#x200B;框。

   >[!NOTE]
   >
   >如果未记录小时数，或者记录的小时数不符合添加到开票记录所需的条件，则不会显示&#x200B;**添加小时数**&#x200B;按钮。 有关详细信息，请参阅本文中的以下部分：[可向帐单记录添加哪些小时数](#what-hours-can-be-added-to-a-billing-record)。

1. 选择要包括在开票记录中的小时条目，然后单击&#x200B;**添加小时数**。 小时实际成本作为&#x200B;**可记帐小时**&#x200B;金额添加到&#x200B;**记帐记录总计**。

1. （可选）单击&#x200B;**记帐记录详细信息**&#x200B;以查看记帐记录标题中的&#x200B;**可记帐小时数**&#x200B;和&#x200B;**记帐记录总数**&#x200B;金额以及记帐记录总数。

### 在开票记录中包含可开票费用 {#include-billable-expenses-in-a-billing-record}

如果要将可记帐费用添加到记帐记录，请确保将任务和项目上的费用标记为可记帐。 未标记为可记帐的费用不可添加到记帐记录中。 有关添加费用的详细信息，请参阅文章[管理项目费用](../../../manage-work/projects/project-finances/manage-project-expenses.md)。

要将可记帐费用添加到记帐记录，请执行以下操作：

{{step1-to-projects}}

1. 在&#x200B;**项目**&#x200B;页面上，选择一个项目。
1. 单击左侧面板中的&#x200B;**记帐记录**。
1. 单击记帐记录&#x200B;**描述**&#x200B;以打开&#x200B;**记帐记录详细信息**&#x200B;选项卡。
1. 单击左侧面板中的&#x200B;**可记帐费用**。
1. （视情况而定）如果您已将费用添加到任务或项目并将它们标记为可记帐，请单击&#x200B;**添加费用**。

   >[!NOTE]
   >
   >如果您有费用但未标记为可记帐，则不会显示&#x200B;**添加费用**&#x200B;按钮。 只有实际金额大于零的可记帐费用才有资格包含在记帐记录中。

1. 选择可添加到记帐记录的可记帐费用，然后单击&#x200B;**添加费用**。  费用的实际金额作为&#x200B;**可记帐费用**&#x200B;金额添加到&#x200B;**记帐记录总计**。

1. （可选）单击&#x200B;**记帐记录详细信息**&#x200B;以查看记帐记录标题中的&#x200B;**可记帐费用**&#x200B;和&#x200B;**记帐记录总计**&#x200B;金额以及记帐记录总计。

### 在开票记录中包含固定收入 {#include-fixed-revenues-in-a-billing-record}

如果您的任务有可用的固定收入，您可以将固定收入添加到记帐记录。 没有其他类型的任务或项目收入可供添加到开票记录中。 有关收入类型的详细信息，请参阅文章[记帐和收入概览](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)中的“记帐和收入概览”部分。

{{step1-to-projects}}

1. 在&#x200B;**项目**&#x200B;页面上，选择一个项目。
1. 单击左侧面板中的&#x200B;**记帐记录**。
1. 单击开票记录的&#x200B;**描述**&#x200B;以打开&#x200B;**开票记录详细信息**&#x200B;选项卡。
1. 选择&#x200B;**固定收入**&#x200B;选项卡。
1. 如果您已将固定收入添加到任务，请单击&#x200B;**添加固定收入**。

   >[!NOTE]
   >
   >如果任务上有收入额，但它们未标记为固定，将不显示&#x200B;**添加固定收入**&#x200B;按钮。

1. 选择要将其固定收入包含在开票记录中的任务，然后单击&#x200B;**添加任务**。  任务的&#x200B;**固定收入**&#x200B;金额作为&#x200B;**可记帐收入**&#x200B;金额添加到&#x200B;**记帐记录总计**。

1. （可选）单击&#x200B;**记帐记录详细信息**&#x200B;以查看&#x200B;**可记帐收入**&#x200B;和&#x200B;**记帐记录总计**&#x200B;金额以及记帐记录标题中的记帐记录总计。

## 编辑开票记录

在创建开票记录并向其中添加小时、费用和收入后，您可以在将其标记为已开票之前编辑现有记录上的某些信息。

1. 导航到开票记录。
1. 在左侧面板中选择&#x200B;**记帐记录详细信息**。
1. 编辑任何可用字段中的信息。

   或

   单击右上角的&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)，然后编辑任何可用字段中的信息。

   更新以下内容：

   * **描述**
   * **记帐日期**
   * **记帐状态**

     >[!TIP]
     >
     >如果您为“记帐状态”选择&#x200B;**已记帐**，则在保存更改后无法编辑记帐记录。

   * **发票ID**
   * **PO编号**
   * **附加金额**

   以下字段不可编辑：

   * **可记帐小时数：**&#x200B;记帐记录中包含的小时数实际收入的总和。 有关详细信息，请参阅本文中的以下部分：[在帐单记录中包含可记帐小时数](#include-billable-hours-in-a-billing-record)。

   * **可记帐费用**：记帐记录中包含的可记帐费用的实际金额总计。 有关详细信息，请参阅本文中的以下部分：[在记帐记录中包括可记帐费用](#include-billable-expenses-in-a-billing-record)。

   * **可记帐收入**：记帐记录中包含的任务的固定收入总计。 有关详细信息，请参阅本文中的以下部分：[在开票记录中包含固定收入](#include-fixed-revenues-in-a-billing-record)。

   * **记帐记录总计**：所有可记帐金额的总计。 计算公式如下：

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. 单击&#x200B;**保存更改**。
