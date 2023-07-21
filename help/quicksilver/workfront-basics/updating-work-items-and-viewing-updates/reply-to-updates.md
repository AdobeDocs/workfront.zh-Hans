---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 回复更新
description: 当有人在工作对象上添加或回复更新时，他们的回复会出现在对象更新部分的通信线程中。 您可以向更新添加回复，如果您对对象具有“查看”访问权限，则您可以对其添加“赞”。
author: Lisa and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: 4a4efe7d8a354bc9ec22a607fe6e75040e7cca24
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 0%

---

# 回复更新

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers only in the Preview environment.</span>-->

>[!NOTE]
>
>我们目前正在重新设计Adobe Workfront中的评论体验。
>
>有关新评论体验的更多信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>您可以访问以下对象的新体验：
> * 问题、项目、任务和文档。
>
>     当您启用备注测试版体验时，该选项可用。
>
>     此功能仅适用于“更新”部分，不适用于以下区域：
>
>     * 主页
>     * 列表中的摘要面板
>     * 时间表中的“摘要”面板
>
> * 讨论区中的目标、信息卡
>
>   新的评论体验是目标和信息卡的唯一体验。 您必须拥有其他许可证才能访问Workfront目标。 有关更多信息，请参阅 [使用Workfront目标的要求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     在信息卡上启用“注释”和“系统活动”部分时，您可以在“信息卡”区域中添加和查看信息卡的更新。 有关更多信息，请参阅 [向展示板添加临时信息卡](../../agile/get-started-with-boards/add-card-to-board.md).


当有人回复工作对象的评论或系统更新时，他们的回复会出现在对象更新部分的通信线程中。

>[!IMPORTANT]
>
>无法回复新评论测试版体验中的系统更新。 有关更多信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>对于问题和文档，请求或更高版本；对于所有其他对象，审阅或更高版本</p> </td> 
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

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 回复更新或回复

您可以回复对象线程中可查看的注释，也可以以Workfront或组管理员身份登录并代表其他用户回复注释。 有关更多信息，请参阅 [以其他用户身份登录](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

回复评论或回复会因您选择的体验和对象而异。

### 在当前更新部分中回复更新或回复

1. 转到要向其添加回复的对象。
1. 在 **更新** 选项卡，查找要回复的更新或回复。

1. （可选）要在现有更新中查看图像，请执行下列操作之一：

   * 单击 **预览** 图标 ![](assets/previewimageicon-31x31.png) 在图像缩略图上，在新的浏览器选项卡中打开全尺寸图像。
   * 单击 **下载** 图标 ![](assets/downloadimageicon.png) 在图像缩略图上下载图像。

1. 单击 **回复** 在更新时，在显示的框中键入回复。

   您可以在该更新会话的顶部看到活跃参与对话或被标记在每次回复中的用户。 这些用户以及订阅了对象的任何用户将在对对象进行更新或回复时收到通知。 您还可以标记更多用户，以将其包含在回复中。  要标记更多用户，请参阅 [为其他人标记更新](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)

1. （可选）要在回复中包含来自上次更新的文本，请单击 **更多** 菜单，然后单击要报价的更新或回复 **引用回复**. 上次更新的文本显示在输入区域中，以垂直灰色线标记。
1. （可选）按照文章中“在Workfront更新中使用富文本”一节中所述，使用格式、表情符号、包含链接或图像 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 单击 **回复** 以保存回复。

### 使用评论Beta版体验时回复评论

有关哪些功能可用于新注释体验以及哪些对象的信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. 转到要向其添加回复的对象。
1. 单击 **更新**，然后单击 **评论** 按Tab键查找要回复的注释或回复。
1. （可选）要在回复中包含来自上次更新的文本，请单击 **更多** 菜单，然后单击要报价的更新或回复 **引用回复**. 上次更新的文本显示在输入区域中，以垂直灰色线标记。
1. 单击 **回复**.

   您可以在页面底部看到积极参与对话的用户 **新建评论** 框后，您可以添加更多内容，或删除不再相关的内容。 这些用户以及订阅了对象的任何用户将在对对象进行更新或回复时收到通知。 您还可以标记更多用户，以将其包含在回复中。  要标记更多用户，请参阅 [为其他人标记更新](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. 开始键入回复，并使用“富文本”工具栏中的任何其他选项。 有关使用富文本或其他更新功能的信息，请参阅 [更新工作](../updating-work-items-and-viewing-updates/update-work.md).

1. 单击 **提交** 以保存回复。

1. （可选）单击 **更多** 菜单 ![](assets/more-menu.png) 在更新旁边，了解更多用于管理回复的选项。 有关更多信息，请参阅 [更新工作](../updating-work-items-and-viewing-updates/update-work.md).


## 通过电子邮件通知回复更新

根据电子邮件通知的配置方式，当对您有权访问的特定对象进行更新时，您可能会收到电子邮件通知。

>[!NOTE]
>
>对于群集6上的环境，无法通过电子邮件回复更新。

以下是在任务的更新选项卡上进行更新后触发的电子邮件通知示例：

![email.png](assets/email-350x202.png)

通过电子邮件，您可以轻松地将回复直接添加到Workfront中对象的通信线程中。 您也可以在不登录Workfront的情况下，通过评论以下对象而生成的电子邮件添加回复：

* 项目
* 任务
* 问题
* 文档
* 模板和模板任务
* 项目组合
* 项目群
* 迭代
* 时间表

### 回复电子邮件通知的更新

当您收到电子邮件通知时，可以快速打开关联的Workfront对象，并直接向通信会话添加回复。

1. 单击 **注释** 在电子邮件通知上。

   此时，将在Workfront中打开对象的“详细信息”页面。

1. 转到要向其添加回复的更新。

   除了查看积极参与对话的用户外，您还可以在该更新会话的顶部查看每个回复中标记了谁。 这些用户以及订阅了对象的任何用户将在对象上进行更新或回复时收到通知。 要标记更多用户，请参阅 [为其他人标记更新](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. 单击 **回复，** 输入您的回复，然后单击 **回复**.

### 向Workfront外部的对象添加更新

当您收到Workfront电子邮件通知时，无需登录Workfront即可快速向通信线程添加更新。

要向Workfront电子邮件添加更新，请执行以下操作：

1. 在电子邮件应用程序中，打开要回复的Workfront电子邮件，然后打开回复电子邮件窗口。
1. 键入您的更新。\
   不允许使用附件，并且在“更新”选项卡中查看更新时，应用到电子邮件中更新的任何富文本格式都不会显示在更新中。
1. 单击 **发送**.

   您的更新将添加到对象的通信线程中。
