---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: 管理项目团队
description: 项目团队由与项目关联的用户组成。 项目团队的成员显示在项目的“人员”部分或可用于创建项目的模板的“人员”部分中。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 3b5452c51c19edfafc9244c2cfd58d7174732375
workflow-type: tm+mt
source-wordcount: '1418'
ht-degree: 1%

---

# 管理项目团队

<!--take preview and production references out at production - August 7-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>

-->

项目团队由与项目关联的用户组成。 有关详细信息，请参阅[项目团队概述](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md)。

项目团队的成员将显示在项目的“人员”部分中。

从模板创建项目后，显示在项目模板的人员部分中的用户将成为项目团队。

以下用户将自动添加到项目和模板的项目团队中：

* 所有者
* 发起人
* 分配给任务的用户
* 分配给问题的用户（仅适用于项目）

项目团队中的用户会收到有关项目的通知。 有关详细信息，请参阅[事件通知类型](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)。

您可以通过添加和移除项目或模板团队中的用户（仅适用于项目），或者向他们发送更新来管理这些用户。

## 访问要求

+++ 展开以查看访问要求。 

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
   <td> <p>标准 </p>
    <p>规划 </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别</td> 
   <td> <p>编辑对项目和模板的访问权限</p> <p>查看或更高的用户访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或模板的或更高权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old access: 

You must have the following access to perform the steps in this article:

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
   <td> <p>Plan </p> </td> 
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

*To find out what plan, license type, or access you have, contact your Workfront administrator.-->

## 将用户添加到项目团队

将用户添加到项目团队时，他们将获得项目以及项目的任务、问题和文档的“查看”权限。 有关详细信息，请参阅文章[项目团队概述](../../../manage-work/projects/planning-a-project/project-team-overview.md)。

>[!TIP]
>
>项目团队中的用户不会自动添加到项目的资源管理工具中。

您可以通过以下方式将用户添加到项目团队：

* [自动将用户添加到项目团队](#automatically-add-users-to-a-project-team)
* [手动将用户添加到项目团队](#manually-add-users-to-a-project-team)

### 自动将用户添加到项目团队 {#automatically-add-users-to-a-project-team}

在项目上履行以下角色的用户会自动添加到项目团队中，并在创建项目时显示在“人员”部分中：

* 项目的创建者
* 项目所有者
* 项目发起人

当用户被分配到以下项目时，他们也会被自动添加到项目团队中：

* 任务
* 问题

### 手动将用户添加到项目团队 {#manually-add-users-to-a-project-team}

如果项目上不履行任何角色的用户希望在项目生命周期中收到有关某些更新或更改的通知，您可以手动将其添加到项目团队。

有关可以为项目团队中的用户启用哪些通知的更多信息，请参阅[事件通知类型](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)。

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

## 管理项目中的人员

1. 转到要管理项目团队的项目。

   >[!TIP]
   >
   >您必须将用户分配给项目的任务、问题或作为利益相关者，才能使其显示在人员部分中。

1. 单击左侧面板中的&#x200B;**人员**。

1. 单击&#x200B;**添加用户**。

   此时会显示&#x200B;**将用户添加到项目团队**&#x200B;框。

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. 在&#x200B;**添加用户**&#x200B;框中，开始键入要添加到项目团队中的活动Workfront用户的名称，然后当该名称出现在列表中时单击该名称。

   重复此步骤以将多个用户添加到项目团队。 用户必须属于与项目关联的组。

   >[!TIP]
   >
   >* 无法通过添加团队、组、公司或工作角色来添加用户。
   >* 添加用户时，请注意头像、用户的主要角色及其电子邮件地址，以区分具有相同名称的用户。 用户必须与至少一个工作角色关联，才能在添加时查看工作角色。
   >
   >  您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅[授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

1. 单击&#x200B;**添加**。

   用户将获得项目的“查看”权限，并作为项目团队的一部分接收有关项目的通知。

1. （可选）如果希望用户在其工作角色添加到任务、问题或项目审批时收到通知，请在用户的&#x200B;**工作角色**&#x200B;列中单击，然后选择与审批关联的工作角色。

   用户将收到与分配给所选工作角色的审批相关的通知。

   有关详细信息，请参阅[项目团队概述](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md)一文中的“基于角色的审批”一节。

1. 在列表中选择一个或多个用户，然后单击&#x200B;**删除**&#x200B;图标![删除图标](assets/remove-icon.png)以从团队中删除这些用户。

1. 单击&#x200B;**是，删除选定的用户**&#x200B;以确认并删除这些用户。

   用户将从未完成的工作项中删除和取消分配。

   有关详细信息，请参阅本文中有关从项目团队中删除用户的[注意事项](#considerations-for-removing-users-from-a-project-team)部分。
1. （可选）若要将此项目的更新发送给用户，请单击“全部更新”**&#x200B;**&#x200B;将更新发送给团队中的每个人

   或

   在列表中选择一个或多个用户，然后单击&#x200B;**将更新发送给用户**。

   <!--update screen shot when they fix the bug - the text above the box needs to match the OLD box, below-->

   ![将更新发送到项目上的用户框](assets/send-update-to-user-on-project-box-2025.png)

   <!--Old UI for projects but the text above the comment box is right and matches the functionality):
   ![OLD Send update to user on a project](assets/send-update-to-user-on-project-box.png)-->

   将打开&#x200B;**将更新发送给用户**&#x200B;框。

1. 执行下列操作之一：

   * 为所选用户添加更新。
   * 单击锁图标可将更新设为公司内用户私有。
   * 标记其他用户以接收相同的更新。
   * 单击&#x200B;**发送**。

   更新已添加到项目的&#x200B;**更新**&#x200B;部分，并且所有选定用户都显示为已标记用户。

   如果用户启用了电子邮件通知，他们可能会收到电子邮件通知，并且会收到有关新更新的应用程序内通知。

1. （可选）单击&#x200B;**导出**&#x200B;图标![导出图标](assets/export-icon.png)以将用户列表导出到文件

   或

   选择用户，然后单击&#x200B;**导出**&#x200B;图标以仅导出特定用户。

## 管理模板上的人员

1. 转到要为其管理项目团队的模板。

   >[!TIP]
   >
   >您必须将用户分配给任务或作为模板上的利益相关者，才能使其显示在“人员”部分中。

1. 单击左侧面板中的&#x200B;**人员**。

1. 在列表中选择一个或多个用户，然后单击&#x200B;**删除**&#x200B;图标以将其从团队中删除。

1. 单击&#x200B;**是，删除选定的用户**&#x200B;以确认并删除这些用户。

   将从模板任务中删除和取消分配用户。

   有关详细信息，请参阅本文中有关从项目团队中删除用户的[注意事项](#considerations-for-removing-users-from-a-project-team)部分。

1. （可选）若要向用户发送更新，请单击&#x200B;**全部更新**&#x200B;以将更新发送给列表中的所有用户

   或

   在列表中选择一个或多个用户，然后单击&#x200B;**将更新发送给用户**。

   <!--update screen shot for unshim production, notice the text above the box - it needs to say "Post an update to each person's profile"-->

   ![发送更新到模板](assets/send-update-to-user-on-template-box.png)上的用户框

   将打开&#x200B;**将更新发送给用户**&#x200B;框。

1. 执行以下操作：

   * 为所选用户添加更新。
   * 单击&#x200B;**标记人员**&#x200B;以标记接收相同更新的其他用户。
   * 选择&#x200B;**我的公司专用**&#x200B;选项，将更新设为公司用户专用。
   * 单击&#x200B;**发送**。

     >[!TIP]
     >
     >仅当Workfront配置文件与某个公司关联时，**私有到我的公司**&#x200B;设置才可用。

   该更新已添加到每个已标记用户配置文件的&#x200B;**更新**&#x200B;部分。

   如果用户启用了电子邮件通知，他们可能会收到电子邮件通知，并且会收到有关新更新的应用程序内通知。

1. 单击&#x200B;**导出**&#x200B;图标![导出图标](assets/export-icon.png)以将用户列表导出到文件

   或

   选择用户，然后单击&#x200B;**导出**&#x200B;图标以仅导出特定用户。

## 从项目团队中删除用户的注意事项

从用户在项目中的角色中删除用户时，这些用户仍然是项目团队的一部分。

您必须将其从项目团队和项目的“人员”部分中移除，这样他们才能停止接收发送给项目团队的通知。

如果从项目团队中删除用户，并且该用户被分配给项目中的任务或问题，则未完成的任务和问题中将取消分配该用户。 在这种情况下，任务和问题返回到工作负载均衡器中的未分配工作区域。

分配了已完成任务和问题的用户仍然分配了任务和问题，即使您从项目团队中删除了这些用户也是如此。

从项目或模板的“人员”部分删除以下用户时，会从他们在项目中的角色中将其删除：

* 分配给未完成任务的用户
* 分配给未完成问题的用户

从项目或模板的“人员”部分删除以下用户时，不会从他们在项目中的角色中将其删除：

* 所有者
* 发起人

有关从项目团队中删除用户的详细信息，请参阅[从项目中删除用户](../../../manage-work/projects/manage-projects/remove-users-from-projects.md)。

