---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 为其他人标记更新
description: 在Adobe Workfront对象上提供更新注释时，项目中的所有用户都可以看到提交的信息。 但是，有时候，不在项目中的用户将受益于查看此信息。 您可以在更新中标记这些用户，以便与他们共享，而不是将这些用户包含在项目中。 已标记的用户会收到事件通知。
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 3a2745437e00ac968f2a4590be2637dbc01594ad
workflow-type: tm+mt
source-wordcount: '1626'
ht-degree: 0%

---

# 为其他人标记更新

<!--take "Beta" references out when we remove the beta and change "current" to "legacy" after October 26-->

<!--take new commenting and legacy commenting out when we remove the legacy commenting and the new one is the only experience-->

<span class="preview">此页面上高亮显示的信息是指尚未普遍可用的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。 </span>\
<span class="preview">有关快速版本的信息，请参阅 [为您的组织启用或禁用快速发布](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>

<span class="preview">有关当前发行计划的信息，请参阅 [2023年第四季度发行版概述](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span>

>[!IMPORTANT]
>
>我们当前正在重新设计Adobe Workfront中的评论体验。
>根据您从哪些环境和哪些对象中访问评论体验，您可能会在更新部分中看到不同的功能。
>
>有关新的评论体验及其可用性的更多信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>新的评论体验仅适用于“更新”部分，不适用于以下区域：
>
> * 主页
> * 列表中的摘要面板
> * 时间表中的“摘要”面板


<!--old note before August 17: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the commenting Beta experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).

-->

在更新对象时，如果想要吸引用户注意在其他情况下他们可能不会关注的对象，则可以标记用户。
您可以在更新中标记这些用户以与他们共享，而不是通过将其分配给对象或使其订阅来将这些用户包含在对象中。 已标记的用户将收到有关您输入的更新的通知。

>[!NOTE]
>
>用户必须在个人资料中启用个人通知，才能接收电子邮件通知。 有关更多信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>

有关向Workfront对象添加更新的信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>当问题转化为项目或任务时，更新将会复制到新项目或任务中，但标记的用户不会。 若要继续对话，必须再次标记参与者。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>针对问题和文档的请求或更高请求；针对所有其他对象的查看或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>问题和文档的请求者或更高；所有其他对象的查看者或更高</p> 
   <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>查看对对象的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 为其他人标记更新

根据您选择的体验和对象，为更新中的其他人添加标签会有所不同。

### 在当前更新部分中标记其他人的更新

<!--change "current" to "legacy" at the October 26, 2023 release-->

您可以在当前的更新部分中手动标记用户。

1. 开始更新工作项，如中所述 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 在 **通知** 字段中，开始键入要包含的用户或团队的名称，然后在名称出现在下拉列表中时单击该名称。

   或

   在中键入@符号 **开始新的更新** 区域，开始键入要包括在更新中的用户或团队的名称，然后在该名称出现在下拉列表中时单击该名称。

   >[!TIP]
   >
   >当存在名称相似或相同的用户时，要识别正确的用户，请注意头像、用户的主要角色或其电子邮件地址。
   >
   >用户必须与至少一个工作角色关联，才能在更新中标记这些用户时查看这些角色。
   >
   >您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅 [授予用户访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. （可选）要将更新设为私有，请启用 **我的公司私有** 在更新框的右下角。 这将使更新仅对您公司中的用户可见。 此 **我的公司私有** 仅当在Workfront配置文件中指定了公司时，选项才可用。

   >[!NOTE]
   >
   >公司外部的已标记用户仍可能会收到应用程序内通知或电子邮件，即使他们不会在“更新”选项卡上看到私人评论。 如果不想与外部用户共享信息，我们建议不要在更新时标记这些用户。

1. （可选）要添加多个用户和团队，请重复步骤2。

   >[!NOTE]
   >
   >在“通知”字段中列出的所有用户和团队成员都会收到更新的应用程序内通知，并且可能会收到一封电子邮件，具体取决于其电子邮件通知设置的配置。 在评论或回复中标记自己的用户会收到该评论或回复的通知，并可以在会话剩余时间的通知字段中看到他们的姓名，但除非他们再次标记自己，否则不会收到其他通知。 有关更多信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 和 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 单击 **更新**.\
   更新中包含的用户会被自动授予对象的“查看”权限，并且可以查看和响应对对象所做的更新。

   您可以在更新线程的顶部查看每个回复中标记了哪些人。 这些用户以及订阅了对象的任何用户将在对对象进行更新或回复时收到通知。

   ![](assets/tagging-transparency-350x192.png)

   有关更新工作项时可用的附加功能的信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

### 为其他人标记新评论体验中的更新

您可以通过以下方式为新评论体验中的更新标记其他人：

* **自动**：当用户启动跟帖、添加评论或添加回复时，会自动为其添加标记，并添加到评论框的标记人员或团队区域。 <!--remove the tip below when the new commenting stream is the only stream and the legacy commenting is removed-->

  >[!TIP]
  >
  >当线程在旧版评论体验中启动时，不会自动标记线程参与者。

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

   ![](assets/tag-others-unified-commenting.png)

1. （可选）要将更新设为私有，请启用 **我的公司私有** 在更新框的右下角。 这将使更新仅对您公司中的用户可见。 此 **我的公司私有** 仅当在Workfront配置文件中指定了公司时，选项才可用。

   >[!NOTE]
   >
   >* 仅当用户与公司关联时，才会显示此选项。
   >* 公司外部的已标记用户仍可能会收到应用程序内通知或电子邮件，即使他们不会在“更新”选项卡上看到私人评论。 如果不想与外部用户共享信息，我们建议不要在更新时标记这些用户。

1. （可选）要添加多个用户和团队，请重复步骤2。 <!--insure this stays accurate-->

   >[!NOTE]
   >
   >“标记人员或团队”字段中列出的所有用户和团队成员都会收到更新的应用程序内通知，并且可能会收到电子邮件，具体取决于其电子邮件通知设置的配置。 在评论或回复中标记自己的用户会收到该评论或回复的通知，并且可以在中看到其名称作为会话剩余时间的成员列出，但除非他们再次标记自己，否则不会收到其他通知。 有关更多信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 和 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 单击 **提交**.\
   更新中包含的用户会被自动授予对象的“查看”权限，并且可以查看和响应对对象所做的更新。

   <span class="preview">标记实体的名称显示在它们的头像旁边，最多两个实体。 如果标记了两个以上的实体，则除了显示标记了多少个其他实体外，还会显示第一个实体的名称。</span>

   ![](assets/members-icons-expanded-unshimmed.png)

   有关更新工作项时可用的附加功能的信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. （可选）单击 **更多** 菜单 ![](assets/more-menu.png) <span class="preview">在注释的右上角</span>，然后单击 **编辑**. 删除所有已标记的用户，然后单击 **提交**. 只有在输入评论后15分钟内才能对其进行编辑。 您只能编辑添加的注释。

   >[!TIP]
   >
   >使用旧版评论体验添加评论和回复时，未特别标记的评论所有者无法由使用新评论体验的用户手动删除。



