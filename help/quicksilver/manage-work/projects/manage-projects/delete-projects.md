---
title: 删除项目
product-area: projects
navigation-topic: manage-projects
description: 如果不再需要项目及其数据，您可以删除该项目。
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# 删除项目

如果不再需要项目及其数据，您可以删除该项目。

作为删除项目的替代方法，我们建议编辑项目并将状态更改为“完成”或“无效”。 这会从用户的任务列表中删除与项目相关的所有当前任务，但会保存与项目关联的所有数据。

## 访问要求

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Delete</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Edit access to Projects, Tasks,&nbsp;Issues with ability to Delete projects, tasks, and issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目、任务、删除项目、任务和问题功能的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目、任务和项目问题的权限，并能够删除项目、任务和问题。 </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。
您可以删除项目列表中或项目级别的项目。

## 了解删除项目的流程

* [删除项目的限制](#limitations-for-deleting-projects)
* [删除项目的影响](#the-impact-of-deleting-projects)

### 删除项目的限制  {#limitations-for-deleting-projects}

* 已删除的项目将移至回收站30天，且只能由Workfront管理员恢复。

   有关恢复对象的更多信息，请参阅文章 [恢复已删除的项目](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* 如果项目有任务或记录的小时数有问题，Workfront或组管理员必须通过在Workfront实例中配置任务和问题首选项来允许删除这些任务，以便能够删除包含任务的项目。

   有关启用删除记录了小时的任务、问题或项目的更多信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### 删除项目的影响 {#the-impact-of-deleting-projects}

* 删除项目时，您会影响链接到该项目的其他对象。

   在删除项目时，也会删除附加到项目的以下对象：

   * 文档

      无法删除包含已签出的附加文档的项目。 有关签出文档的更多信息，请参阅 [签出文档](../../../documents/managing-documents/check-out-documents.md).

   * 任务
   * 子任务
   * 问题
   * 注释
   * 审批
   * 费用

* 根据Workfront管理员在Workfront实例的“工时单和小时”首选项中配置项目、任务或问题删除首选项的方式，在删除项目时，将按以下方式之一处理任务、问题或项目的记录时数：

   * 小时作为一般时间保留在时间表上。
   * 这些小时将被删除，并在项目恢复后恢复。

   有关为记录问题的小时配置删除首选项的详细信息，请参阅 [配置工时单和工时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* 如果您删除的项目已链接到Workfront方案计划员中的方案：

   * 该计划仍保留在计划中，但指向项目的链接被删除。
   * 如果您删除的项目链接到计划中唯一已发布的方案，则也会删除已发布计划的指示。
   * 如果恢复已删除的项目，则会恢复项目，但不会恢复其与方案的链接，并且“方案计划员”区域不再显示在“项目详细信息”中。

      方案规划器仅在新的Adobe Workfront体验中可用，并且需要额外的许可证。 有关Workfront方案规划器的信息，请参阅 [方案计划员概述](../../../scenario-planner/scenario-planner-overview.md).

      有关与方案规划器中的方案链接的项目的信息，请参阅 [通过在方案规划器中发布方案来更新或创建项目](../../../scenario-planner/publish-scenarios-update-projects.md).

* 如果项目也是Workfront目标中目标的活动：

   * 项目将从目标中删除。 项目指示的目标进度也会被删除。

   * 如果恢复已删除的项目，该项目也会作为目标的活动进行恢复。

      这需要额外的许可证。 有关Workfront目标的信息，请参阅 [Adobe Workfront目标概述](../../../workfront-goals/goal-management/wf-goals-overview.md).

      有关将项目与目标关联的信息，请参阅 [将项目添加到Adobe Workfront目标中的目标](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## 删除列表中的项目

您可以从项目列表中删除项目。

1. 转到项目列表或项目报告。
1. 选择要删除的项目，然后单击 **删除** 列表顶部。

1. 单击 **是，删除它** 以确认删除。

   项目会被删除并存储在回收站中30天。 此时，您的Workfront管理员可以从回收站中恢复。

## 在项目级别删除项目

1. 转到要删除的项目。
1. 单击 **更多** 图标 ![](assets/qs-more-menu.png).

1. 单击 **删除项目**.

1. 单击 **是，删除它**.

   项目会被删除并存储在回收站中30天。 此时，您的Workfront管理员可以从回收站中恢复。

## 恢复已删除的项目

系统或组管理员可以在项目被删除后的30天内恢复项目，如文章所述 [恢复已删除的项目](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
