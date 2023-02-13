---
product-area: projects
navigation-topic: update-work-in-a-project
title: 项目的更新条件
description: 项目的“条件”是一个标记，用于指示与该项目关联的工作是否顺利进行，或您是否遇到任何障碍。 这与项目的状态不同，状态指示您是否在积极处理该项目。
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 1%

---

# 项目的更新条件

项目的“条件”是一个标记，用于指示与该项目关联的工作是否顺利进行，或您是否遇到任何障碍。 这与项目的状态不同，状态指示您是否在积极处理该项目。

您可以自动或手动设置项目的条件。 要手动更改项目的条件，您必须是项目所有者或具有项目的“管理”权限。

Adobe Workfront管理员可以为您的环境创建自定义条件，如 [创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## 访问要求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the current licenses:
  <p>Standard</p>
   
   For legacy licenses:
   <ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>编辑对项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 自动设置条件

自动设置项目的条件取决于项目的条件类型。 条件类型必须设置为进度状态，Workfront才能自动设置项目的条件。

当在“设置”区域中设置项目首选项时，Workfront或组管理员会为系统中的新项目确定“条件类型”字段的默认值。 有关更多信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

在创建项目时，会自动将项目的条件设置为与当时项目的进度状态匹配。 项目的进度状态基于项目任务的进度。

有关项目条件以及如何根据进度状态计算这些条件的信息，请参阅 [项目进度状态概述](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## 手动更新项目的条件

如果将项目的“条件类型”设置为“手动”而不是“进度状态”，则可以手动更新项目的“条件”。

1. 转到要更新条件的项目。
1. 单击 **项目详细信息** 中。

   ![](assets/project-details-overview-edit-enabled-with-condition-shot-nwe-350x251.png)

1. 确保 **条件类型** 字段设置为 **手动**.

1. 在 **条件** 字段中，从以下选项中选择与您对与其关联的工作是否顺利进行或是否存在延迟的理解相匹配的选项：

   * **准时**
   * **处于风险中**
   * **存在问题**

   有关项目条件的更多信息，请参阅 [项目条件和条件类型概述](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >可以针对您的环境自定义条件，因此您可能会在您的环境中找到三个以上的“条件”选项。 “条件”的名称可能与上面所列的名称不同。 有关在Workfront中自定义条件的信息，请参阅 [创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. 单击 **保存**.Click **保存更改**.
