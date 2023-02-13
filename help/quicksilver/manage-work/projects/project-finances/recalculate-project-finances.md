---
title: 重新计算项目财务
product-area: projects
navigation-topic: financials
description: 在项目中，当项目记录的小时数或用于计算成本和收入的比率发生更改时，会计算项目的财务。
author: Alina
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1590'
ht-degree: 0%

---

# 重新计算项目财务

在项目中，当项目记录的小时数或用于计算成本和收入的比率发生更改时，会计算项目的财务。

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

## 关于Adobe Workfront财务核算的思考

在Enhanced Analytics中，会通过以下方式计算财务：

* 您可以使用项目上的“重新计算财务”选项来人工重新计算项目的成本和收入。
* 此外，某些操作会触发自动重新计算。

当用户或角色的速率在项目生命周期中发生更改时，可能会发生以下情况：

* 进行更改后，更新后的费率将从记录小时数和计算财务信息时起使用。 更改比率不会影响更改前内容的计算方式。 对于记录的所有现有小时数，旧费率用于计算财务信息。
* 您可以使用“重新计算财务”选项，强制Adobe Workfront对迄今记录的所有小时使用新费率，以追溯方式计算。 这迫使Workfront根据新费率信息追溯重新计算以前输入的所有小时数、计划成本和收入。

>[!CAUTION]
>
>在手动重新计算给定项目的财务之前，您可能需要保留以前已计算的任何财务数据。 我们建议仅在您确定不更改现有信息时或仅在需要更改现有信息时才使用“重新计算财务”选项。

## 保留具有现有工时的任务的财务数据 {#preserve-financial-data-for-tasks-with-existing-hours}

在重新计算项目的财务数据时，Workfront会根据任何新的或更新的财务信息，追溯地重新计算所有以前记录的小时数、计划、实际成本以及计划和实际收入。

* [保留项目收入](#preserve-project-revenue)
* [保持项目成本](#preserve-project-cost)

### 保留项目收入  {#preserve-project-revenue}

在项目的生命周期内，收入率可能会发生变化。

有关帐单费率和收入的更多信息，请参阅文章 [账单和收入概述](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

收入率可能会在以下级别发生变化：

* 系统级别（用于作业角色）\
   有关在系统级别使用计费费率创建职务角色的详细信息，请参阅文章 [创建和管理作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* 用户级别\
   有关更改用户计费费率信息的更多信息，请参阅文章 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 公司级别（对于职务角色）\
   有关更多信息，请参阅 [在公司层改写职务职责开单费率](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* 项目级别（用于作业角色）\
   有关在项目级别改写职务角色费率的详细信息，请参阅文章 [改写职务职责开单费率和计算项目收入的概述](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

例如，用户在项目过程中的计费费率从每小时50美元更改为75美元，您希望所有现有数据仍按旧费率（50美元和小时）计算。 但是，在重新计算项目财务时，已具有现有财务数据的任务将更新收入，以反映新的计费费率（每小时75美元）。

* [通过创建开单记录来保留项目收入](#preserve-project-revenue-by-creating-a-billing-record)
* [使用多个开单费率覆盖来保留项目收入](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### 通过创建开单记录来保留项目收入 {#preserve-project-revenue-by-creating-a-billing-record}

当上述任何层的开单费率发生更改时，您可以通过避免使用人工重新计算财务选项或将记录在项目上并使用旧费率计算的时间锁定到状态为“已开单”的开单记录中，来保留已在项目上计算的现有收入。

当您不重新计算项目的财务或锁定记录到计费账单记录的小时数时，费率更改后记录的小时数将使用新费率计算，而费率更改前记录的小时数仍按旧费率计算。

有关创建账单记录的更多信息，请参阅文章 [创建帐单记录](../../../manage-work/projects/project-finances/create-billing-records.md).

#### 使用多个开单费率覆盖来保留项目收入 {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

当项目层职务角色的开单费率发生更改时，您可以使用多个开单费率覆盖来保留已在项目上计算的现有收入，这些费率覆盖在指定的时间范围内被锁定。

有关使用多个计费费率覆盖的详细信息，请参阅文章 [改写职务职责开单费率和计算项目收入的概述](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>这仅适用于在项目层更改的职务角色开单费率。

### 保持项目成本 {#preserve-project-cost}

成本率可在以下层次变化：

* 系统级别（用于作业角色）\
   有关在系统级别使用成本费率创建任务角色的详细信息，请参阅文章 [创建和管理作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* 用户级别\
   有关更改用户成本费率信息的详细信息，请参阅文章 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

当上述任何层的开单费率发生更改时，您可以通过将项目上记录的时间锁定到状态为“已开单”的开单记录中，并使用旧费率计算，来保留已在项目上计算的现有成本。 有关创建账单记录的更多信息，请参阅文章 [创建帐单记录](../../../manage-work/projects/project-finances/create-billing-records.md).

如果您不想创建开单记录（如一节中所述），也可以避免使用“人工重新计算财务”选项 [人工重新计算项目的财务](#manually-recalculate-finances-for-a-project) 在本文中。

当您不重新计算项目的财务或锁定记录到计费账单记录的小时数时，费率更改后记录的小时数将使用新费率计算，而费率更改前记录的小时数仍按旧费率计算。

## 人工重新计算项目的财务 {#manually-recalculate-finances-for-a-project}

如果费率在项目生命周期内发生更改，并且您希望成本和收入计算能够反映新费率，则必须人工重新计算项目的财务。

>[!NOTE]
>
>按照部分中的步骤，手动重新计算财务时，您可能会阻止更新收入值以反映新费率 [保留具有现有工时的任务的财务数据](#preserve-financial-data-for-tasks-with-existing-hours) 本文的。 在您人工重新计算项目财务时，系统始终会更新成本值以反映新费率。

您可以从项目页面或项目列表或报表重新计算Workfront中项目的财务。

您可以在批量编辑财务时重新计算这些财务。 有关信息，请参阅 [在“编辑项目”框中批量手动重新计算财务](#manually-recalculate-finances-in-bulk-in-the-edit-projects-box) 章节。

1. 转到要重新计算财务的项目，然后单击 **更多** 图标 ![](assets/qs-more-icon-on-an-object.png) 项目名称的权限

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   或

   转到项目列表或报表，选择一个或多个项目，然后单击 **更多** 图标 ![](assets/qs-more-icon-on-an-object.png) 列表顶部。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >根据项目的复杂性，我们建议在批量重新计算其财务时不要选择大量项目，以确保获得最佳性能。 某些可能导致项目过于复杂的因素可能是多个依赖关系或分配或大量自定义字段。

1. 单击 **重新计算财务**.

   项目的所有计划成本和收入都将重新计算，并包含任何新信息。

   您应会在浏览器顶部收到一条确认消息，确认项目的财务状况已成功重新计算。\
   现有成本值和一些尚未锁定的收入值更新以反映新费率。

## 在“编辑项目”框中批量手动重新计算财务 {#manually-recalculate-finances-in-bulk-in-the-edit-projects-box}

您可以通过批量编辑多个项目的财务信息来手动重新计算这些项目的财务信息。 这会导致项目收入重新计算追溯。

>[!IMPORTANT]
>
>按照部分中的步骤，手动重新计算财务时，您可能会阻止更新收入值以反映新费率 [保留具有现有工时的任务的财务数据](#preserve-financial-data-for-tasks-with-existing-hours) 本文的。 在您人工重新计算项目财务时，系统始终会更新成本值以反映新费率。

要人工重新计算多个项目的财务，请执行以下操作：

1. 转到项目列表。
1. 在列表中选择多个项目，然后单击 **编辑**.

   >[!TIP]
   >
   >根据项目的复杂性，我们建议在批量编辑项目时不要选择大量项目，以确保获得最佳性能。 某些可能导致项目过于复杂的因素可能是多个依赖关系或分配或大量自定义字段。

1. 单击 **设置**，然后选择 **重新计算成本和收入**.

1. 单击 **保存更改**.

## 触发自动重新计算财务的操作

以下操作会触发对Workfront项目的财务重新计算：

* 更改任务状态
* 将具有小时的任务移动到另一个项目
* 将项目状态从“完成”更改为“活动”状态

>[!NOTE]
>
>在更改项目状态时，只会重新计算计划值。

您还可以在 **更多** 菜单 ![](assets/qs-more-menu.png) 在项目级别，单击 **重新计算财务**.
