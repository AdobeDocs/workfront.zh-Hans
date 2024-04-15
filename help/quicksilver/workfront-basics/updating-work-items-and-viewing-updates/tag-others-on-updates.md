---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 为其他人标记更新
description: 在Adobe Workfront对象上提供更新注释时，项目中的所有用户都可以看到提交的信息。 但是，有时候，不在项目中的用户将受益于查看此信息。 您可以在更新中标记这些用户，以便与他们共享，而不是将这些用户包含在项目中。 已标记的用户会收到事件通知。
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 4c17466705873b06e7ea7bb08bb78a7e68078f8b
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 0%

---

# 为其他人标记更新

<!--Audited: April, 2024-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span> 
-->

在更新对象时，如果想要吸引用户注意在其他情况下他们可能不会关注的对象，则可以标记用户。

您可以在更新中标记这些用户以与他们共享，而不是通过将其分配给对象或使其订阅来将这些用户包含在对象中。 标记的用户将收到有关您输入的更新的Workfront通知。 根据他们的通知设置，他们还会收到有关您输入的更新的电子邮件。

## 关于在更新中标记用户的注意事项

* 在更新中标记的用户必须在他们的配置文件中启用个人通知，以便他们接收电子邮件通知。 有关更多信息，请参阅 [修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  有关向Workfront对象添加更新的信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* 当问题转化为项目或任务时，更新将会复制到新项目或任务中，但标记的用户不会。 若要继续对话，必须再次标记参与者。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>新文档：问题和文档的参与者或更高版本；所有其他对象的轻量级或更高版本</p>
   <p>当前：对问题和文档的请求或更高版本；对所有其他对象的审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>查看您要在其中发布回复的对象或对其拥有更高的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>查看您想发布回复的对象或对其拥有更高权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关更多信息，请参阅 [Workfront文档的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 为其他人标记更新

您可以通过以下方式为其他人标记更新：

* **自动**：当用户启动跟帖、添加评论或添加回复时，会自动为其添加标记，并添加到评论框的标记人员或团队区域。

  >[!TIP]
  >
  >   在开发周期中添加评论时，无法自动标记用户。  有关信息，请参阅 [管理开发周期注释](/help/quicksilver/agile/use-scrum-in-an-agile-team/iterations/manage-iteration-updates.md). \
  >添加来自其他应用程序的评论时，无法自动标记用户。


* **手动**：手动将用户添加到评论框的“标记人员”区域时。

您还可以在编辑或回复评论时删除被错误地标记的用户。

1. 开始更新工作项，如中所述 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 作为注释所有者，您会被自动标记并添加到注释框的“标记人员或团队”区域。

   >[!TIP]
   >
   >评论所有者无法在评论框的“标记人员”或“团队”区域中看到自己的名称。

1. 在 **标记人员或团队** 字段中，开始键入要包含的用户或团队的名称，然后在名称出现在下拉列表中时单击该名称。

   或

   在中键入@符号 **编写评论** 区域，开始键入要包括在更新中的用户或团队的名称，然后在该名称出现在下拉列表中时单击该名称。

   >[!TIP]
   > 
   >当存在名称相似或相同的用户时，要识别正确的用户，请注意头像、用户的主要角色或其电子邮件地址。
   > 
   >用户必须与至少一个工作角色关联，才能在更新中标记这些用户时查看这些角色。
   > 
   >您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅 [授予用户访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![标记用户](assets/tag-others-unified-commenting-with-all-tab.png)

1. （可选）要将更新设为私有，请启用 **我的公司私有** 在更新框的右下角。 这将使更新仅对您公司中的用户可见。 此 **我的公司私有** 仅当在Workfront配置文件中指定了公司时，选项才可用。

   >[!NOTE]
   >
   >* 仅当用户与公司关联时，才会显示此选项。
   >* 公司外部的已标记用户仍可能会收到应用程序内通知或电子邮件，即使他们不会在“更新”选项卡上看到私人评论。 如果不想与外部用户共享信息，我们建议不要在更新时标记这些用户。

1. （可选）要添加多个用户和团队，请重复步骤2。 <!--insure this stays accurate-->

   >[!NOTE]
   >
   >“标记人员或团队”字段中列出的所有用户和团队成员都会收到更新的应用程序内通知，并且可能会收到电子邮件，具体取决于其电子邮件通知设置的配置。 在评论或回复中标记自己的用户会收到该评论或回复的通知，并且可以在中看到其名称作为会话剩余时间的成员列出，但除非他们再次标记自己，否则不会收到其他通知。 有关更多信息，请参阅 [修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 和 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 单击 **提交**.\
   更新中包含的用户会被自动授予对象的“查看”权限，并且可以查看和响应对对象所做的更新。

   标记实体的名称显示在它们的头像旁边，最多两个实体。 如果标记了两个以上的实体，则除了显示标记了多少个其他实体外，还会显示第一个实体的名称。

   ![](assets/members-icons-expanded-unshimmed.png)

   当在注释文本中被标记时，您的名称将在这些注释中突出显示。

   有关更新工作项时可用的附加功能的信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. （可选）单击 **更多** 菜单 ![](assets/more-menu.png) 单击注释右上角的 **编辑**. 删除所有已标记的用户，然后单击 **提交**.

   >[!IMPORTANT]
   >
   >只有在输入评论后15分钟内才能对其进行编辑。 您只能编辑添加的注释。


<!--
   >[!TIP]
   >
   >When using the legacy commenting experience to add comments and replies, comment owners that were not specifically tagged cannot be manually removed by people who use the new commenting experience.
-->

<!--
### Tag others on updates in the legacy Updates section

You can manually tag users in the legacy Updates section. 

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Notify** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list.

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. 
   >
   >Users must be associated with at least one job role to view it as you tag them in an update. 
   >
   >You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company. The **Private to my company** option is available only when a Company is specified in your Workfront profile. 

   >[!NOTE]
   >
   >Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them.  

1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the Notify field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in the Notify field for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Update**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply at the top of the update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.

   ![](assets/tagging-transparency-350x192.png)
-->

有关更新工作项时可用的附加功能的信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).



