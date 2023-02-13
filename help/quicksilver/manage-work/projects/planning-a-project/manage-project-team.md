---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: 管理项目团队
description: 项目团队由与项目关联的用户组成。 项目团队的成员将显示在项目的“人员”部分中。
author: Alina
feature: Work Management
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# 管理项目团队

项目团队由与项目关联的用户组成。 项目团队的成员将显示在项目的“人员”部分中。

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
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>编辑对项目的访问权限</p> <p>查看或更高权限用户</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目的或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 将用户添加到项目团队

将用户添加到项目团队后，他们将获得有关项目以及项目任务、问题和文档的“查看”权限。 有关更多信息，请参阅文章 [项目团队概述](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>项目团队中的用户不会自动添加到项目的资源管理工具中。

您可以通过以下方式将用户添加到项目团队：

* [自动将用户添加到项目团队](#automatically-add-users-to-a-project-team)
* [手动将用户添加到项目团队](#manually-add-users-to-a-project-team)

### 自动将用户添加到项目团队 {#automatically-add-users-to-a-project-team}

在项目中履行以下角色的用户会自动添加到项目团队中，并在创建项目时显示在“人员”部分：

* 项目的创建者
* 项目所有者
* 项目赞助人

在将用户分配到以下项目时，用户也会自动添加到项目团队中：

* 任务
* 问题

### 手动将用户添加到项目团队 {#manually-add-users-to-a-project-team}

如果对项目不履行任何角色的用户希望在项目生命周期内收到某些更新或更改的通知，则可以手动将它们添加到项目团队。

有关可以为项目团队的用户启用哪些通知的更多信息，请参阅 [事件通知在Adobe Workfront中可用](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. 转到要将用户添加到的项目。

1. 单击 **人员** 中。 您可能需要单击 **显示更多** 第一个。

1. 单击 **添加用户**.

   此时会显示将用户添加到项目团队对话框。

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. 在 **添加用户** 框中，开始键入要添加到项目团队的活动Workfront用户的名称，然后在下拉列表中显示该名称时单击该名称。

   重复此步骤，向项目团队添加多个用户。 用户必须属于与项目关联的组。

   >[!TIP]
   >
   >* 您无法通过添加用户的团队、组、公司或工作角色来添加用户。
   >* 在添加用户时，请注意头像、用户的主要角色及其电子邮件地址，以区分名称相同的用户。 用户必须至少与一个作业角色关联，才能在您添加时查看该角色。



1. 单击 **添加**.

   用户将获得项目的“查看”权限，并作为项目团队的一部分接收有关项目的通知。

## 从项目团队中删除用户

当您从用户在项目中的角色中删除用户时，这些用户仍将属于项目团队。

如果您从项目团队中删除了某个用户，并且该用户被分配到项目中的任务或问题，则该用户将从未完成的任务和问题中未分配。 在这种情况下，任务和问题将返回到负载平衡器中的“未分配的工作”区域。

分配给已完成任务和问题的用户即使在您将其从项目团队中删除后仍会继续分配。

有关从项目团队中删除用户的更多信息，请参阅 [从项目中删除用户](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
