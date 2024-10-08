---
title: 管理记录注释
description: 通过在记录的右侧面板中添加评论或回复，您可以对Adobe Workfront Planning记录进行协作。 您还可以在此区域查看对记录所做的其他更改以及系统记录的更改。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: 73f339b54985b725f265d582992a43b9f80dbd7c
workflow-type: tm+mt
source-wordcount: '980'
ht-degree: 0%

---

# 管理记录注释

{{planning-important-intro}}

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

通过在记录的右侧面板中添加评论或回复，您可以对Adobe Workfront Planning记录进行协作。 您还可以在此区域查看对记录所做的其他更改以及系统记录的更改。

记录的右侧面板显示以下部分：

* **个评论**：显示评论和用户添加到记录的回复。
* **历史记录**：显示用户对记录字段进行的系统记录更改。 有关详细信息，请参阅[历史记录部分概述](/help/quicksilver/planning/records/history-section-overview.md)。

## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

您必须具备以下条件才能访问Workfront Planning：

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 产品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront规划<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
<p>以下任意Workfront计划：</p> 
<ul><li>选择</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning不适用于旧版Workfront计划</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront规划计划*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入AdobeUnified Experience，才能访问Workfront Planning的所有功能。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 投稿人、浅色或标准</p>
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>查看工作区或更高权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>布局模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 有关对记录进行注释的注意事项

* 您可以在Workfront Planning的“注释”部分中为记录添加注释和回复。

* 添加到链接记录的评论不会显示在您链接到的记录中。 例如，如果您对链接到Campaign记录的Workfront Planning产品记录添加注释，则该注释仅在Workfront Planning的产品记录中显示，而不会在您链接的Campaign记录中显示。

* 您可以将注释添加到由于某个记录与来自另一个应用程序的对象之间的连接而创建的Workfront Planning记录中。

  例如，在将Workfront项目与Workfront Planning记录连接后，您可以对Workfront Planning项目记录进行评论。 有关详细信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

* 添加到其他应用程序中链接对象的注释不会显示在Workfront Planning中，而添加到Workfront Planning中链接对象的注释不会显示在其他应用程序中。

  例如，添加到Workfront中的项目的注释不会显示在链接到Workfront Planning中的营销活动的同一项目中，并且添加到Workfront Planning项目记录的注释不会显示在Workfront中。

* 您可以标记用户以引起他们对更新的注意。 标记的用户不会收到应用程序内通知或有关您更新的电子邮件。<!--this might change??-->

* 您可以标记用户以引起他们对更新的注意。 标记的用户将收到有关您更新的应用程序内通知或电子邮件通知。

  >[!NOTE]
  >
  >   只有已登记使用Unified ExperienceAdobe的客户的用户才会同时收到应用程序内通知和电子邮件通知。 要确定您的公司是否正在使用AdobeUnified Experience，请参阅[AdobeWorkfront的Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

* 您可以向记录添加更新，并复查Workfront Planning以下区域的更改历史记录：

   * 从记录详细信息页面。
   * 从视图中，在记录详细信息框中。

### 管理对记录的评论

{{step1-to-planning}}

1. 单击工作区的卡片。

   工作区将打开，记录类型显示在信息卡上。

1. 单击记录类型卡片。
此时将打开记录类型页面，并显示该类型的所有记录。

1. 从&#x200B;**视图**&#x200B;下拉菜单中选择一个表视图。
1. 单击表视图中记录的名称。

   记录的&#x200B;**详细信息**&#x200B;页面打开。 默认情况下，“注释”区域会在右侧面板中打开。

1. （视情况而定）如果默认情况下未打开右侧面板，请单击右上角的&#x200B;**显示评论** ![](assets/show-comments-icon.png)图标以打开“评论”部分。

1. 开始在&#x200B;**新建评论**&#x200B;框中输入评论。

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >在完成键入并提交评论之前导航离开“评论”部分，即使用户注销并重新登录，该评论仍会在页面中保持草稿模式。 添加到注释的任何图像也会保存在草稿中。 草稿会保存7天，之后将丢弃它们并且无法恢复。 草稿注释仅对输入它们的用户可见。

1. （可选）要撤消或重做更改，请使用以下快捷键：
   * CTRL + Z(Mac为⌘ + z)可撤消更改
   * 按CTRL + Y(对于Mac，按⌘ + y)可重做更改
1. （可选且有条件）如果您的Workfront实例是AdobeUnified Experience的一部分，请添加&#x200B;**@**，后跟用户名，以在更新中标记某人。 有关详细信息，请参阅本文中关于评论记录](#considerations-about-commenting-on-a-record)的[注意事项部分。

1. （可选）使用富文本工具栏中的选项设置文本格式，在更新中添加表情符号、链接或图像，以增强内容。

1. 继续向记录中添加注释。

   有关更新对象(包括Workfront Planning记录)的详细信息，请参阅[更新工作](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

<!--
      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![](assets/new-line-indicator-comments.png)

1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.

   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  

1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
   
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.

1. (Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.     

   ![](assets/search-box-for-comments-area.png)
     
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ...** area, to reply to an existing comment, then follow steps 4-8 above. (**************accurate??***********)

1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.

    ![](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
  
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 

    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body text**: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). -->

1. （可选）单击评论右上角的&#x200B;**更多**&#x200B;图标![](assets/more-menu.png)，然后单击&#x200B;**删除**&#x200B;以删除评论。
1. （可选）单击&#x200B;**隐藏评论**&#x200B;图标![](assets/hide-comments-icon.png)以关闭右侧面板。

## “历史记录”部分概述

您可以在记录的右侧面板的“历史记录”部分中查看对记录所做的更改。

有关详细信息，请参阅[历史记录部分概述](/help/quicksilver/planning/records/history-section-overview.md)。
