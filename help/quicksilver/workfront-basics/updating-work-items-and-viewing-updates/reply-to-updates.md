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
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '1099'
ht-degree: 0%

---

# 回复更新

{{highlighted-preview}}

<!--remove legacy and new experience references when we remove the legacy updates in the UI - Jan 2024???-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 

-->

>[!IMPORTANT]
>
>我们当前正在重新设计Adobe Workfront中的评论体验。
>
>根据您访问评论体验的对象，您可能会看到更新部分的以下功能：
>* 新体验
>* 旧版体验
>* 新体验和旧体验
>
>有关新的评论体验及其可用性的更多信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>新评论体验仅适用于Workfront对象的“更新”部分，当您从以下区域访问对象时，该体验不可用：
>
> * 主页
> * 列表中的摘要面板
> * 时间表中的“摘要”面板
> * 工作负载均衡器中的“摘要”面板
>
><span class="preview">新的评论体验在“摘要”面板的列表、时间表以及预览环境的工作负载均衡器中可用。</span> <!--and in the Production environment for customers who have opted for the fast release process. For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).-->

当有人回复工作对象的评论或系统更新时，他们的回复会出现在对象更新部分的通信线程中。

>[!IMPORTANT]
>
>无法在新评论体验中回复系统更新。 有关更多信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--adjust the sentence before the second IMPORTANT and remove this important note when we remove legacy from the system-->

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>问题和文档的请求者或更高；所有其他对象的查看者或更高</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>查看对对象的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在Workfront中回复更新或回复

您可以回复可查看的对象线程中的注释，也可以以Workfront或组管理员身份登录并代表其他用户回复注释。 有关更多信息，请参阅 [以其他用户身份登录](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

回复注释或回复会因您选择的体验和对象而异。

### 使用新评论体验时回复评论

有关新的注释体验中可用的功能以及哪些对象的信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. 转到要向其添加回复的对象。
1. 单击 **更新**，然后单击 **评论** 选项卡，并查找要回复的注释或回复

   或

   <span class="preview">单击 **全部** 选项卡，然后单击 **在评论中回复** 在“注释”选项卡中打开注释并回复注释。 您不能在“全部”选项卡中回复。</span>

1. （可选）要在回复中包含来自先前更新的文本，请单击 **更多** 菜单，然后单击 **引用回复**. 上次更新的文本会显示在输入区域中，以垂直灰色线标记。
1. 单击 **回复**.

   ![](assets/reply-to-update-empty-box.png)

   您可以在页面底部看到积极参与对话的用户 **添加回复……** 框后，您可以添加更多内容，或删除不再相关的内容。 这些用户以及订阅了对象的任何用户将在对对象进行更新或回复时收到通知。 您还可以标记更多用户以将其包含在回复中。  要标记更多用户，请参阅 [为其他人标记更新](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   >[!TIP]
   >
   >   要向现有回复添加其他回复，您可以开始键入 **添加回复……** 框，或单击 **回复** 在原始注释上。 您的回复将添加到线程的末尾。

1. 开始键入回复，并使用富文本工具栏中的任何其他选项。 有关使用富文本或其他更新功能的信息，请参阅 [更新工作](../updating-work-items-and-viewing-updates/update-work.md).

1. 单击 **提交** 以保存回复。

1. （可选）单击 **更多** 菜单 ![](assets/more-menu.png) 在要回复的评论的右上角，查看更多用于管理回复的选项。 有关更多信息，请参阅 [更新工作](../updating-work-items-and-viewing-updates/update-work.md).

### 在旧版更新部分中回复更新或回复

1. 转到要向其添加回复的对象。
1. 在 **更新** 选项卡中，查找要回复的更新或回复。

1. （可选）要在现有更新中查看图像，请执行下列操作之一：

   * 单击 **预览** 图标 ![](assets/previewimageicon-31x31.png) 在图像缩略图上，在新的浏览器选项卡中打开全尺寸图像。
   * 单击 **下载** 图标 ![](assets/downloadimageicon.png) 在图像缩略图上下载图像。

1. 单击 **回复** 在更新时，在显示的框中键入回复。

   您可以在该更新线程的顶部看到积极参与对话或被标记在每次回复中的用户。 这些用户以及订阅了对象的任何用户将在对对象进行更新或回复时收到通知。 您还可以标记更多用户以将其包含在回复中。  要标记更多用户，请参阅 [为其他人标记更新](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)

1. （可选）要在回复中包含来自先前更新的文本，请单击 **更多** 菜单，然后单击要报价的更新或回复 **引用回复**. 上次更新的文本会显示在输入区域中，以垂直灰色线标记。
1. （可选）使用格式、表情符号、包含链接或图像，如文章中“在Workfront更新中使用富文本”一节中所述 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 单击 **回复** 以保存回复。

## 回复电子邮件通知的更新

根据电子邮件通知的配置方式，当对您有权访问的特定对象进行更新时，您可能会收到电子邮件通知。

您可以通过以下方式回复电子邮件通知的更新：

* 回复您收到的电子邮件。 您的回复电子邮件将添加为Workfront对原始评论的回复。
* 使用电子邮件中的“评论”按钮可导航回Workfront并回复更新区域的更新。

以下是在任务的更新选项卡上更新后触发的电子邮件通知示例：

![email.png](assets/email-350x202.png)

有关信息，请参阅 [回复电子邮件通知](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md).






