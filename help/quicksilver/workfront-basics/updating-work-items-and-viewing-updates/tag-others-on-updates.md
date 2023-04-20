---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新时标记其他人
description: 在Adobe Workfront对象上提供更新注释时，该项目的所有用户都可以查看已提交的信息。 但是，有时不在项目中的用户可能会从查看此信息中受益。 您可以在更新时标记这些用户，以便与他们共享，而不是将这些用户包含在项目中。 标记用户将收到事件通知。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 607e0523cf97fdf26b650dc441e52b4ae4528af4
workflow-type: tm+mt
source-wordcount: '1456'
ht-degree: 0%

---

# 更新时标记其他人

<!--take "Beta" references out when we remove the beta-->


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.-->

>[!NOTE]
>
>我们当前正在重新设计在Adobe Workfront中的注释体验。
>有关新更新体验的更多信息，请参阅 [新的注释体验](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).
>
>您可以访问以下对象的新设计：
> * 在启用注释测试版时出现问题。
   >
   >     此功能仅适用于问题的“更新”部分，不适用于以下区域：
   >
   >     * 主页
   >     * 列表中的“摘要”面板
   >     * 工时单中的“摘要”面板
>
> * 目标

   >
   >   新的评论体验是目标的默认体验。 您必须拥有其他许可证才能访问Workfront Goals。 有关更多信息，请参阅 [使用Workfront目标的要求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   >
   >    有关对目标进行评论的信息，请参阅 [在Adobe Workfront目标中管理目标注释](../../workfront-goals/goal-management/manage-goal-comments.md).



如果您希望引起用户对某个对象的注意，否则用户可能不会关注该对象，则可以在对该对象进行更新时标记用户。
您可以在更新时标记这些用户，以便与他们共享对象，而不是通过将这些用户分配给对象或让他们订阅对象来将其包含在对象中。 标记用户将收到有关您输入的更新的通知。

>[!NOTE]
>
>必须启用事件通知，用户才能收到电子邮件通知。 管理员可以为整个系统或顶级组启用通知。 用户还可以在自己的用户配置文件中启用或禁用单个事件通知。 有关更多信息，请参阅以下内容：
>
>* [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
>* [查看和配置群组的事件通知](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)
>* [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>


有关向Workfront对象添加更新的信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>将问题转换为项目或任务后，更新将复制到新项目或任务，但标记的用户不会。 要继续对话，必须再次标记参与者。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>（二）对问题和文件提出要求或更高要求；对所有其他对象进行审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>请求人或更高人员提出问题和文件；所有其他对象的审阅者或更高级别</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>查看对对象的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 更新时标记其他人

根据您选择的体验和对象，在更新中标记其他对象时会有所不同。

### 在当前更新部分中为其他用户标记更新

1. 开始更新工作项，如 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 在 **通知** 字段中，开始键入要包含的用户或团队的名称，然后在下拉列表中显示该名称时单击该名称。

   或

   在 **开始新更新** 区域，开始键入要包含在更新中的用户或团队的名称，然后在下拉列表中显示该名称时单击。

   >[!TIP]
   >
   >要在用户名称相似或相同时识别正确的用户，请注意头像、用户的主要角色或其电子邮件地址。 用户必须至少与一个作业角色关联，才能在您在更新中标记他们时查看该角色。

   ![](assets/tag-users-in-update.png)

1. （可选）要将更新设为私有，请启用 **对我的公司私有** 中。 这样，更新仅对公司中的用户可见。 的 **对我的公司私有** 选项仅在您的Workfront配置文件中指定了公司时可用。

   >[!NOTE]
   >
   >公司外的标记用户仍可能收到应用程序内通知或电子邮件，即使他们在“更新”选项卡中看不到私人评论。 如果您不想与外部用户共享信息，我们建议不要在更新时为其添加标签。

1. （可选）要添加多个用户和团队，请重复步骤2。

   >[!NOTE]
   >
   >“通知”字段中列出的所有用户和团队成员都将收到有关更新的应用程序内通知，并且可能会收到电子邮件，具体取决于其电子邮件通知设置的配置。 在评论或回复中标记自己的用户会收到该评论或回复的通知，并且在线程的其余时间内，可以在“通知”字段中看到其名称，但除非他们再次标记自己，否则他们不会收到其他通知。 有关更多信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 和 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 单击 **更新**.\
   更新中包含的用户会自动被授予对象的“查看”权限，并且可以查看和响应对对象所做的更新。

   您可以在更新线程顶部的每个回复中查看已标记的对象。 当对对象进行更新或回复时，这些用户以及订阅该对象的任何用户都会收到通知。

   ![](assets/tagging-transparency-350x192.png)

   有关更新工作项时可用的其他功能的信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

### 在评论测试版体验的更新中标记其他人

您可以在评论测试版体验的更新中为其他用户添加标记。 您还可以删除在编辑评论时被错误标记的用户。

1. 开始更新工作项，如 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 在 **标记人员或团队** 字段中，开始键入要包含的用户或团队的名称，然后在下拉列表中显示该名称时单击该名称。

   或

   在 **编写评论** 区域，开始键入要包含在更新中的用户或团队的名称，然后在下拉列表中显示该名称时单击。

   >[!TIP]
   >
   >要在用户名称相似或相同时识别正确的用户，请注意头像、用户的主要角色或其电子邮件地址。 用户必须至少与一个作业角色关联，才能在您在更新中标记他们时查看该角色。

   ![](assets/tag-others-unified-commenting.png)

1. （可选）要将更新设为私有，请启用 **对我的公司私有** 中。 这样，更新仅对公司中的用户可见。 的 **对我的公司私有** 选项仅在您的Workfront配置文件中指定了公司时可用。

   >[!NOTE]
   >
   >* 仅当用户与公司关联时，才会显示此选项。
   >* 公司外的标记用户仍可能收到应用程序内通知或电子邮件，即使他们在“更新”选项卡中看不到私人评论。 如果您不想与外部用户共享信息，我们建议不要在更新时为其添加标签。


1. （可选）要添加多个用户和团队，请重复步骤2。 <!--insure this stays accurate-->

   >[!NOTE]
   >
   >“标记人员或团队”字段中列出的所有用户和团队成员都将收到更新的应用程序内通知，并可能会收到电子邮件，具体取决于其电子邮件通知设置的配置。 在评论或回复中标记自己的用户会收到该评论或回复的通知，并且在线程的剩余时间中，他们的名称将列为线程的成员，但是，除非他们再次标记自己，否则他们不会收到其他通知。 有关更多信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 和 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 单击 **提交**.\
   更新中包含的用户会自动被授予对象的“查看”权限，并且可以查看和响应对对象所做的更新。

   您可以在成员区域的更新文本下查看每个回复中标记的对象。 当对对象进行更新或回复时，这些用户以及订阅该对象的任何用户都会收到通知。
1. （可选）单击 **成员** 更新中包含，以显示您输入的更新与之共享的实体列表。

   ![](assets/members-icons-expanded-unshimmed.png)

   有关更新工作项时可用的其他功能的信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. （可选）单击 **更多** 菜单 ![](assets/more-menu.png) 在“称赞”图标的右侧，单击 **编辑**. 删除任何已标记的用户，然后单击 **提交**. 您只能在输入评论后的15分钟内编辑该评论。 您只能编辑您添加的注释。