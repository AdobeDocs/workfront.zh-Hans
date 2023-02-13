---
product-area: projects;user-management
navigation-topic: manage-projects
title: 从项目中删除用户
description: 当用户不再参与完成项目工作时，您可以从项目中删除用户。
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: 301c86152340a184345bd39cec77fdcf28258196
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 从项目中删除用户

当用户不再参与完成项目工作时，您可以从项目中删除用户。 将用户从项目中删除会对任务和问题分配以及项目角色产生影响。 已删除用户，用户将停止接收专门面向项目团队的通知。 有关项目团队通知的更多信息，请参阅 [事件通知在Adobe Workfront中可用](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

与项目关联的用户会列在项目的“人员”区域中。 他们代表项目团队。 有关项目团队的更多信息，请参阅 [项目团队概述](../../../manage-work/projects/planning-a-project/project-team-overview.md).

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
   <td> <p>编辑对项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 删除用户对现有任务、问题和项目有何影响

从项目中删除用户时，分配给用户的任何任务或问题都可能会受到影响，具体取决于用户被删除后任务或问题是否已完成：

* **如果删除用户时未完成该项目：** 如果已经分配了作业角色，则会将项目重新分配给作业角色，或者将项目分配给用户在项目上履行的作业角色。 如果项目或用户未分配作业角色，则必须手动重新分配该项目。
* **如果在删除用户时项目已完成：** 已删除用户的名称将保留在项目上。
* **如果删除的用户也是项目的创建者：** 项目不会从 **我正在执行的项目** 列表。 对于所有其他用户，如果用户通过输入方式字段对该项目进行筛选，则会从列表中删除该项目。
* **如果用户是项目所有者或赞助商：** 用户仍担任项目的赞助商或所有者的角色。

## 从项目和项目团队中删除用户

您可以通过从项目团队中删除用户来从项目中删除这些用户。

当用户在项目中履行角色时，他们将成为项目团队的一部分。

当您从用户在项目中的角色中删除用户时，这些用户仍将属于项目团队。

有关用户在项目中的角色的信息，请参阅 [管理项目团队](../planning-a-project/manage-project-team.md).

要从项目团队中删除用户，请执行以下操作：

1. 转到要删除用户的项目。

1. 单击 **人员** 在左侧面板中，选择要删除的用户。 您可能需要单击 **显示更多**，则 **人员**.

1. 单击 **删除** 图标  ![删除项目](assets/remove-icon---x-in-circle.png) 列表顶部的。

1. 单击 **是，删除选定用户** 确认删除。

   这些用户将从项目团队和可能分配给他们的任何未完成任务或问题中删除。 他们不再接收面向项目团队的通知。
