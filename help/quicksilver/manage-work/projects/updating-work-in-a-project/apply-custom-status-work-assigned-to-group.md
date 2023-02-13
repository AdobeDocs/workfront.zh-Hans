---
product-area: projects
navigation-topic: update-work-in-a-project
title: 应用状态以处理与群组关联的工作
description: 如果某个项目与某个组关联，则可以将系统级别状态以及与该组关联的自定义状态应用到该项目、任务或该项目上的问题。
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# 应用状态以处理与群组关联的工作

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

如果某个项目与某个组关联，则您可以将系统级别状态以及与该组关联的自定义状态应用到该项目，或者将该项目的任务和问题应用到该项目。 有关Adobe Workfront中的组状态的信息，请参阅 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

>[!TIP]
>
>您只能将项目与组关联。 问题和任务将从其所属的项目继承组。

## 访问要求

<!--drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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

## 更新项目组和状态

在更新项目的组时，可用于任务、问题状态或项目状态的选项会发生更改，以便与组匹配。

1. 转到项目或创建新项目，如 [创建项目](../../../manage-work/projects/create-projects/create-project.md).
1. 单击 **更多** 图标 ![](assets/more-icon.png)，然后单击 **编辑**.

1. 在 **编辑项目** 在 **概述** ，选择 **组** 下拉菜单。

1. 在 **状态** 下拉菜单中，选择自定义状态。

   >[!NOTE]
   >
   >如果您在 **组** 下拉菜单中的自定义状态 **状态** 菜单会自动更改以与新组关联。
   >
   >
   >![](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)   >

1. 选择项目的状态。 您创建并应用于该群组的自定义状态将显示在列表中。
