---
title: 重新计算项目财务
product-area: projects
navigation-topic: financials
description: 当项目记录的小时数或用于计算成本和收入的费率发生更改时，在项目上计算财务。
author: Lisa
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: 69afad9af3f1e703487fdab092bc84457ee00922
workflow-type: tm+mt
source-wordcount: '1678'
ht-degree: 0%

---

# 重新计算项目财务

当项目记录的小时数或用于计算成本和收入的费率发生更改时，在项目上计算财务。

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

## 在Adobe Workfront中计算财务的注意事项

在Enhanced Analytics中，财务计算方式如下：

* 您可以使用项目中的“重新计算财务”选项，手动重新计算项目的成本和收入。
* 此外，某些操作会触发自动重新计算。

当用户或角色的速率在项目生命周期中发生更改时，可能会出现以下情况：

* 进行更改后，在记录小时数和计算财务信息时，将从那时起使用更新的费率。 更改速率不会影响进行更改之前计算事情的方式。 对于记录的所有现有小时数，使用旧比率计算财务信息。
* 通过使用“重新计算财务”选项，您可以强制Adobe Workfront以追溯方式使用迄今为止记录的所有小时的新费率。 这强制Workfront根据新的费率信息追溯重新计算所有以前输入的小时数、计划成本和收入。

报表类型项目（财务数据）在加载数据之前不会自动重新计算。 要更新此报表类型中的数据，您必须手动重新计算单个项目的财务。

>[!CAUTION]
>
>在手动重新计算给定项目的财务之前，您可能希望保留已按先前比率计算的任何财务数据。 我们建议仅在您确定不更改现有信息时或者仅在需要此类更改时才使用重新计算财务选项。
>
>请注意，运行项目（财务数据）报表会执行财务数据的重新计算，因此在运行报表之前，您应该考虑相同的因素。

## 保留具有现有小时数的任务的财务数据 {#preserve-financial-data-for-tasks-with-existing-hours}

在重新计算项目的财务数据时，Workfront会根据任何新的或更新后的财务信息，追溯重新计算所有以前记录的小时数、计划成本、实际成本以及计划和实际收入。

* [保留项目收入](#preserve-project-revenue)
* [保留项目成本](#preserve-project-cost)

### 保留项目收入  {#preserve-project-revenue}

在项目的存留期内，收入率可能会发生变化。

有关记帐费率和收入的更多信息，请参阅文章[记帐和收入概览](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)。

收入率可于以下层次变动：

* 系统级别（针对工作角色）\
  有关在系统级别使用记帐费率创建工作角色的更多信息，请参阅文章[创建和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

* 用户级别\
  有关更改用户记帐费率信息的详细信息，请参阅文章[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

* 公司级别（针对职位角色）\
  有关详细信息，请参阅[覆盖公司级别的工作角色记帐费率](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)。

* 项目级别（针对工作角色）\
  有关在项目级别覆盖工作角色费率的详细信息，请参阅文章[有关覆盖工作角色记帐费率和计算项目收入的概述](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

例如，用户的记帐费率在项目过程中从每小时50美元更改为75美元，您希望所有现有数据保持按旧费率（$50和小时）计算。 但是，在重新计算项目财务时，已有财务数据的任务将更新收入以反映新的计费率（每小时75美元）。

* [通过创建记帐记录保留项目收入](#preserve-project-revenue-by-creating-a-billing-record)
* [使用多个记帐费率覆盖保留项目收入](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### 通过创建开票记录保留项目收入 {#preserve-project-revenue-by-creating-a-billing-record}

当上述任何级别的记帐费率发生更改时，您可以通过避免使用手动重新计算财务选项，或者通过将项目上记录的时间锁定并使用旧费率计算的时间，来保留已在项目上计算的现有收入（状态为“已记帐”）。

如果您不重新计算项目财务或锁定已记帐记帐记录的小时数，则在费率更改之后记录的小时数将使用新费率计算，并且在成本费率更改之前记录的小时数仍按旧费率计算。

有关创建开票记录的更多信息，请参阅文章[创建开票记录](../../../manage-work/projects/project-finances/create-billing-records.md)。

#### 使用多个记帐费率覆盖保留项目收入 {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

当项目级别工作角色的记帐费率更改时，您可以使用在指定时间范围内锁定的多个记帐费率覆盖来保留已在项目上计算的现有收入。

有关使用多个记帐费率覆盖的更多信息，请参阅文章[有关覆盖工作角色记帐费率并计算项目收入的概述](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

>[!NOTE]
>
>这仅适用于在项目级别更改的工作角色记帐费率。

### 保留项目成本 {#preserve-project-cost}

成本率可在以下级别变动：

* 系统级别（针对工作角色）\
  有关在系统级别创建具有成本费率的工作角色的更多信息，请参阅文章[创建和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

* 用户级别\
  有关更改用户成本费率信息的详细信息，请参阅文章[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

当上述任何级别的记帐费率发生更改时，您可以通过锁定项目上记录的时间并使用旧费率计算来将项目上已计算的现有成本保留到状态为“已记帐”的记帐记录中。 有关创建开票记录的更多信息，请参阅文章[创建开票记录](../../../manage-work/projects/project-finances/create-billing-records.md)。

如果您不想创建记帐记录，也可以避免使用手动重新计算财务选项，如本文中的[手动重新计算项目财务](#manually-recalculate-finances-for-a-project)部分所述。

如果您不重新计算项目财务或锁定已记帐记帐记录的小时数，则在费率更改之后记录的小时数将使用新费率计算，并且在成本费率更改之前记录的小时数仍按旧费率计算。

## 手动重新计算项目财务 {#manually-recalculate-finances-for-a-project}

如果在项目生命周期中费率发生更改，并且希望成本和收入计算能够反映新的费率，则必须手动重新计算项目的财务状况。

>[!NOTE]
>
>在手动重新计算财务时，您可以按照[保留具有本文中现有小时数的任务的财务数据](#preserve-financial-data-for-tasks-with-existing-hours)一节中的步骤来阻止更新收入值以反映新费率。 在您手动重新计算项目财务时，始终会更新成本值以反映新费率。

您可以从项目页面、项目列表或报表重新计算Workfront中的项目财务。

您可以在批量编辑财务时重新计算它们。 有关信息，请参阅本文中的[手动批量重新计算财务](#manually-recalculate-finances-in-bulk)部分。

1. 转到要重新计算财务的项目，然后单击项目名称右侧的&#x200B;**更多**&#x200B;图标![](assets/qs-more-icon-on-an-object.png)。

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   或

   转到项目列表或报告并选择一个或多个项目，然后单击列表顶部的&#x200B;**更多**&#x200B;图标![](assets/qs-more-icon-on-an-object.png)。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >根据项目的复杂性，我们建议不要在批量重新计算其财务时选择大量项目以确保最佳性能。 某些因素可能会使项目过于复杂，例如多个依赖项或分配或者大量自定义字段。

1. 单击&#x200B;**重新计算财务**。

   使用任何新信息重新计算项目的所有计划成本和收入。

   您应该在浏览器顶部收到一条确认消息，确认项目的财务已成功重新计算。
现有成本值和某些未锁定的收入值将更新以反映新费率。

## 手动批量重新计算财务{#manually-recalculate-finances-in-bulk}

您可以通过批量编辑多个项目来手动重新计算其财务状况。 这会导致项目收入进行追溯性重新计算。

>[!IMPORTANT]
>
>在手动重新计算财务时，您可以按照[保留具有本文中现有小时数的任务的财务数据](#preserve-financial-data-for-tasks-with-existing-hours)一节中的步骤来阻止更新收入值以反映新费率。 在您手动重新计算项目财务时，成本值始终更新以反映新费率。

要手动重新计算多个项目的财务，请执行以下操作：

1. 转到项目列表。
1. 在列表中选择多个项目，然后单击列表顶部的&#x200B;**更多**&#x200B;图标![](assets/qs-more-icon-on-an-object.png)。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >根据项目的复杂性，我们建议不要在批量编辑项目时选择大量项目以确保最佳性能。 某些因素可能会使项目过于复杂，例如多个依赖项或分配或者大量自定义字段。

1. 单击&#x200B;**重新计算财务**。

   使用任何新信息重新计算选定项目的所有计划成本和收入。

   您应该在浏览器顶部收到一条确认消息，确认项目的财务已成功重新计算。

## 触发自动重新计算财务的操作

以下操作会触发Workfront中项目的财务重新计算：

* 更改任务状态
* 将具有小时数的任务移动到另一个项目
* 将项目状态从完成更改为活动状态

>[!NOTE]
>
>当您更改项目状态时，只会重新计算计划值。

您还可以在项目级别的&#x200B;**更多**&#x200B;菜单![](assets/qs-more-menu.png)下手动重新计算财务，方法是单击&#x200B;**重新计算财务**。
