---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: 管理项目团队
description: 项目团队由与项目关联的用户组成。 项目团队的成员显示在项目的“人员”部分或可用于创建项目的模板的“人员”部分中。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 00e693fc8b35a59f6ed212bc30da7f85cc78c845
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 2%

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

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p>
    <p>规划</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目和模板的访问权限</p> <p>查看或更高的用户访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或模板的或更高权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old access: 

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
   <td> <p>Standard </p>
    <p>Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects and Templates</p> <p>View or higher access to Users</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project or to a template</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## Add users to a Project Team

When you add users to the project team, they gain View permissions on the project and the tasks, issues, and documents of the project. For more information, see the article [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Users on the Project Team are not automatically added to the resource management tools for the project.

You can add users to the project team in the following ways:

* [Automatically add users to a Project Team](#automatically-add-users-to-a-project-team) 
* [Manually add users to a Project Team](#manually-add-users-to-a-project-team)

### Automatically add users to a Project Team {#automatically-add-users-to-a-project-team}

The users that fulfill the following roles on the project are automatically added to the project team and appear  in the People section when the project is created:

* The creator of the project
* The project owner
* The project sponsor

Users are also automatically added to the project team when they are assigned to the following:

* Tasks
* Issues

### Manually add users to a Project Team {#manually-add-users-to-a-project-team}

If users that don't fulfill any role on the project want to be notified about certain updates or changes during the life of the project, you can manually add them to the project team. 

 For more information about what notifications can be enabled for users on the project team, see [Event notification types](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md). 

 <!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 



## Manage people on a project

1. Go to the project you want to manage the project team for.

   >[!TIP]
   >
   >You must have users assigned to tasks, issues or as stakeholders on the project to have them display in the People section.

1. Click **People** in the left panel. 

1. Click **Add users**. 

   The **Add users to Project Team** box displays.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. In the **Add users** box, begin typing the name of an active Workfront user that you want to add to the project team, then click the name when it appears in the list.

   Repeat this step to add multiple users to the project team. The users must belong to the group associated with the project. 

   >[!TIP]
   >
   >* You cannot add users by adding their teams, groups, companies, or job roles.
   >* As you add the users, notice the avatar, the user's Primary Role, and their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them.
   >
   >  You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. Click **Add**.

   The users gain View permissions to the project and receive notifications about the project as part of the project team.

1. (Optional) If you want a user to receive a  notification when their job role is added to a task, issue, or project approval, click inside the **Job Role** column for the user, and select a job role that will be associated with the approval. 

   The users will receive notifications related to the approvals assigned to the selected job role. 

   For more information see the "Role-based approvals" section in the article [Project Team overview](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

1. Select one or several users in the list, then click the **Remove** icon ![Remove icon](assets/remove-icon.png) to remove them from the team. 
 
1. Click **Yes, Remove Selected Users** to confirm and remove the users.

   Users are removed and unassigned from incomplete work items.

   For more information, see the [Considerations for removing users from a project team](#considerations-for-removing-users-from-a-project-team) section in this article.
1. (Optional) To send an update for this project to users, click **Update All** to send the update to everyone on the team

   Or 

   Select one or multiple users in the list, then click **Send Update to User**.

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

