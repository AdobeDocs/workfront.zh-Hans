---
product-area: projects
navigation-topic: manage-tasks
title: 删除任务
description: 您可以删除可能重复或创建有误的任务。
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: 7c373707f6e5ec1431e38cc0e103e25cd8cf2309
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# 删除任务

您可以删除可能重复或创建有误的任务。

对于具有历史信息（更新、计划更改、状态或其他字段）的任务，我们建议您关闭它们或将其标记为废弃，而不是删除它们。 这有助于您保留项目的历史信息。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对具有删除访问权限的任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关访问任务的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">授予任务访问权限</a>. 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>为项目分配权限并有权添加任务或更高版本</p> <p>创建任务时，您会自动收到该任务的“管理”权限</p> <p> 有关任务权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">共享任务 </a>. </p> <p>有关请求其他权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 了解删除任务的过程

* [删除任务的限制](#limitations-for-deleting-tasks)
* [删除任务的影响](#the-impact-of-deleting-tasks)

### 删除任务的限制  {#limitations-for-deleting-tasks}

* 当项目的状态为“完成”时，只有当Workfront管理员或组管理员在“项目首选项”区域中允许时，您才能删除任务。 有关设置项目首选项的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 如果任务记录了小时数，Workfront或组管理员必须通过在Workfront实例中配置任务和问题首选项来允许删除这些任务。 当您尝试删除具有已记录小时数的任务的项目时，这也适用。

  <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

  有关启用删除记录了小时数的任务的更多信息，请参阅中的“删除”部分。 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### 删除任务的影响 {#the-impact-of-deleting-tasks}

删除任务时，会影响链接到该任务的其他对象。

删除任务时，也会删除以下附加到任务的对象：

* 文档

  您无法删除具有已签出文档的任务。 有关检出文档的详细信息，请参阅 [签出文档](../../../documents/managing-documents/check-out-documents.md).

* 问题
* 子任务
* 注释
* 审批

根据Workfront管理员在Workfront实例的时间表和小时首选项中配置项目、任务或问题删除首选项的方式，在删除任务时，将以下列方式之一处理为任务记录的小时：

* 移到项目，如果稍后恢复任务，则不会恢复该任务。
* 被删除，如果稍后恢复任务，则将在任务上恢复。

  当您尝试删除具有已记录小时数的任务的项目时，这也适用。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

  有关为登录问题的小时数配置删除首选项的更多信息，请参阅 [配置时间表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* 任务上的费用将移至项目。

* 分配给任务或任务批准的用户仍保留在项目团队中。

  有关项目团队的详细信息，请参阅 [项目团队概述](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## 删除任务

* [同时删除项目中的多个任务](#delete-multiple-tasks-in-a-project-simultaneously)
* [删除单个任务](#delete-a-single-task)

### 同时删除项目中的多个任务  {#delete-multiple-tasks-in-a-project-simultaneously}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) Adobe Workfront的右上角。

1. 单击 **项目**.
1. 单击包含要删除的任务的项目名称。
1. 单击 **任务** （在左侧面板中）。
1. 执行下列操作之一：

   1. （视情况而定）当 **自动保存** 切换已启用：

      1. 选择要删除的任务，然后单击 **更多**
      1. 单击 **删除**，则 **是，删除它** 以确认删除。

         已删除任务。

   1. （视情况而定）单击 **计划模式** 图标并选择 **手动保存** 如果您要撤消对任务列表所做的更改。

      ![选择手动保存](assets/manual-save-option.png)

      执行以下操作：

      1. 选择要删除的任务。
      1. 单击 **删除**.
      1. （可选）单击 **撤消** 以撤消您的更改，而不删除任务。
      1. 单击 **重做** 如果您要保留更改并删除任务。
      1. 单击 **保存** 删除任务。

         只有在保存更改后，才会删除任务。

### 删除单个任务 {#delete-a-single-task}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) Adobe Workfront的右上角。

1. 单击 **项目**.
1. 单击包含要删除的任务的项目名称。
1. 单击 **任务** 在左侧面板中。
1. 单击要删除的任务的名称。
1. 单击 **更多** 图标 ![](assets/qs-more-menu.png)在右上角。

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. 单击 **删除任务**.
1. 如果允许删除，请单击 **是，删除它**.

   您的Workfront管理员或组管理员可能不允许删除记录了小时数的任务。

   有关删除任务所需的访问权限的更多信息，请参阅部分 [删除任务的限制](#limitations-for-deleting-tasks) 本文章中。

## 恢复已删除的任务

Workfront或组管理员可以在任务删除后30天内恢复任务，如中所述 [恢复已删除的项目](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
