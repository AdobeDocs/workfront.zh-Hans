---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 回复更新
description: 当有人添加或回复工作对象上的更新时，他们的回复会出现在对象更新部分的通信线程中。 您可以向更新添加回复，或者如果您对对象具有“查看”权限，则可以向更新添加“赞”回复。
author: Nolan and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: 4c17466705873b06e7ea7bb08bb78a7e68078f8b
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# 回复更新

<!-- Audited: April 2024-->

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

当有人回复工作对象的注释或系统更新时，他们的回复会出现在通信线程中，该线程位于对象的“更新”部分的“注释”和“全部”选项卡中。

>[!IMPORTANT]
>
>无法在“System Activity（系统活动）”选项卡中回复系统更新。 在2024年4月11日之前的旧版评论体验中，对系统更新的任何回复均显示为只读。

本文介绍了如何回复Workfront中大多数对象的注释。 有关各种对象的“更新”部分之间的差异，请参阅[更新部分概述](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)。

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
   <td> <p>查看或编辑更新所在对象的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>查看对对象的访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关详细信息，请参阅Workfront文档的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 在Workfront中回复更新或回复

您可以回复可查看的对象线程中的注释，也可以以Workfront或组管理员身份登录并代表其他用户回复注释。 有关详细信息，请参阅[以其他用户身份登录](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)。

### 回复评论

对于Workfront中的大多数对象，在对象的“更新”部分中回复注释的方式都类似。

1. 转到要向其添加回复的对象。
1. 单击&#x200B;**更新**，然后单击对象的&#x200B;**注释**&#x200B;选项卡并查找要回复的注释或回复

   或

   单击“**全部**”选项卡，然后单击“**在评论中回复**”以在“评论”选项卡中打开评论并回复。 您不能在“全部”选项卡中回复。

1. （可选）若要在回复中包含来自上次更新的文本，请单击要回复的评论右上角的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**引用回复**。 上次更新的文本会显示在输入区域中，以垂直灰色线标记。
1. 单击&#x200B;**回复**。

   ![](assets/reply-to-update-empty-box.png)

   您可以在&#x200B;**添加回复……**&#x200B;框的底部看到积极参与对话的用户，然后您可以添加更多内容，或删除不再相关的内容。 这些用户以及订阅了对象的任何用户将在对对象进行更新或回复时收到通知。 您还可以标记更多用户以将其包含在回复中。  若要标记更多用户，请参阅[标记其他用户的更新](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)。

   >[!TIP]
   >
   >   若要向现有回复添加其他回复，您可以开始在&#x200B;**添加回复……**&#x200B;框中键入，或单击原始评论上的&#x200B;**回复**。 您的回复将添加到线程的末尾。

1. 开始键入回复，并使用富文本工具栏中的任何其他选项。 有关使用富文本或其他更新功能的信息，请参阅[更新工作](../updating-work-items-and-viewing-updates/update-work.md)。

1. 单击&#x200B;**提交**&#x200B;以保存回复。

1. （可选）单击要回复的评论右上角的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)以了解更多用于管理回复的选项。 有关详细信息，请参阅[更新工作](../updating-work-items-and-viewing-updates/update-work.md)。

<!--
### Reply to an update or reply in the legacy Updates section

1. Go to the object to which you want to add a reply.
1. On the **Updates** tab for the object, find the update or reply to which you want to reply.

1. (Optional) To view an image in the existing update do one of the following:

   * Click the **Preview** icon ![](assets/previewimageicon-31x31.png) on the image thumbnail to open the full-size image in a new browser tab.
   * Click the **Download** icon ![](assets/downloadimageicon.png) on the image thumbnail to download the image.

1. Click **Reply** on the update, then type a reply in the box that appears.

   You can see the users who are actively engaged in the conversation or tagged in each reply at the top of that update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object. You can also tag more users to include them in your reply.  To tag more users, see [Tag others on updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)
   
1. (Optional) To include text from a previous update in your reply, click the **More** menu next to the update or reply you want to quote, then click **Quote Reply**. Text from the previous update appears in the input area, marked with a vertical gray line.
1. (Optional) Use formatting, emojis, include links, or images as explained in the section "Use Rich Text in a Workfront update" in the article [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Click **Reply** to save the reply.

-->

## 回复电子邮件通知的更新

根据电子邮件通知的配置方式，当对您有权访问的特定对象进行更新时，您可能会收到电子邮件通知。

您可以通过以下方式回复电子邮件通知的更新：

* 回复您收到的电子邮件。 您的回复电子邮件将添加为Workfront对原始评论的回复。
* 使用电子邮件中的“评论”按钮可导航回Workfront并回复更新区域的更新。

以下是在任务的更新选项卡上更新后触发的电子邮件通知示例：

![email.png](assets/email-350x202.png)

有关信息，请参阅[回复电子邮件通知](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md)。






