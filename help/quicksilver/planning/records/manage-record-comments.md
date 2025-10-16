---
title: 管理记录注释
description: 通过在记录的右侧面板中添加评论或回复，您可以对Adobe Workfront Planning记录进行协作。 您还可以在此区域查看对记录所做的其他更改以及系统记录的更改。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '874'
ht-degree: 0%

---

# 管理记录注释

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

通过在记录的右侧面板中添加评论或回复，您可以对Adobe Workfront Planning记录进行协作。 您还可以在此区域查看对记录所做的其他更改以及系统记录的更改。

记录的右侧面板显示以下部分：

* **个评论**：显示评论和用户添加到记录的回复。
* **历史记录**：显示用户对记录字段进行的系统记录更改。 有关详细信息，请参阅[历史记录部分概述](/help/quicksilver/planning/records/history-section-overview.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>任何Workfront和任何Planning包</p> <p>任何工作流和任何计划包</p>
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>参与者或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>查看或更高权限的工作区和记录类型</p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p> </td> 
  </tr> 
  </tr> 
  <tr>
   <td role="rowheader"><p>版面模板</p></td>
   <td> 必须为具有轻度或参与者许可证的用户分配一个包括Planning的布局模板。
   <p>默认情况下，标准用户和系统管理员已启用Planning区域。</p></div></li></ul>
</td>
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++  

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Contributor or higher license</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>

</td>
  </tr>
</tbody> 
</table> -->



## 有关对记录进行注释的注意事项

* 您可以在Workfront Planning的“注释”部分中为记录添加注释和回复。

* 添加到链接记录的评论不会显示在您链接到的记录中。 例如，如果您对链接到Campaign记录的Workfront Planning产品记录添加注释，则该注释仅在Workfront Planning的产品记录中显示，而不会在您链接的Campaign记录中显示。

* 您可以将注释添加到由于某个记录与来自另一个应用程序的对象之间的连接而创建的Workfront Planning记录中。

  例如，在将Workfront项目与Workfront Planning记录连接后，您可以对Workfront Planning项目记录进行评论。 有关详细信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

* 添加到其他应用程序中链接对象的注释不会显示在Workfront Planning中，而添加到Workfront Planning中链接对象的注释不会显示在其他应用程序中。

  例如，添加到Workfront中的项目的注释不会显示在链接到Workfront Planning中的营销活动的同一项目中，并且添加到Workfront Planning项目记录的注释不会显示在Workfront中。

* 您可以标记用户或团队，以引起他们对更新的注意。 已单独标记的用户和已标记团队的用户都会收到有关您更新的应用程序内通知和电子邮件。

  >[!NOTE]
  >
  >   只有已登记使用Adobe Unified Experience的客户的用户才会同时收到应用程序内通知和电子邮件通知。 要确定您的公司是否正在使用Adobe Unified Experience，请参阅[适用于Workfront的Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

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

1. （视情况而定）如果默认情况下未打开右侧面板，请单击右上角的&#x200B;**显示评论** ![显示评论图标](assets/show-comments-icon.png)图标以打开“评论”部分。

1. 开始在&#x200B;**新建评论**&#x200B;框中输入评论。

   ![记录上的评论框为空](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >在完成键入并提交评论之前导航离开“评论”部分，即使用户注销并重新登录，该评论仍会在页面中保持草稿模式。<!--this is no longer possible for records: Any images that are added to the comment are also saved in the draft. Drafts are saved for 7 days after which they are discarded and cannot be recovered. Drafted comments are only visible to the user entering them.-->

1. （可选）要撤消或重做更改，请使用以下快捷键：
   * 按CTRL + Z(对于Mac，按⌘ + z)可撤消更改
   * 按CTRL + Y组合键(Mac为⌘+y)以重做更改
1. （可选且有条件）如果您的Workfront实例是Adobe Unified Experience的一部分，请添加&#x200B;**@**，后跟用户名或团队名称，以便在更新中标记它们。 有关详细信息，请参阅本文中关于评论记录[的](#considerations-about-commenting-on-a-record)注意事项部分。

1. （可选）使用富文本工具栏中的选项设置文本格式、添加表情符号或链接到更新，以增强内容。

   >[!TIP]
   >
   >无法将图像添加到录制注释。


1. 继续向记录中添加注释。

   有关更新对象(包括Workfront Planning记录)的详细信息，请参阅[更新工作](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

1. （可选）单击评论右上角的&#x200B;**更多**&#x200B;图标![更多菜单](assets/more-menu.png)，然后单击&#x200B;**删除**&#x200B;以删除评论。
1. （可选）单击&#x200B;**隐藏评论**&#x200B;图标![隐藏评论图标](assets/hide-comments-icon.png)以关闭右侧面板。

<!--
      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![New line indicator in comments](assets/new-line-indicator-comments.png)
1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.
   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  
1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.
1. (Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.     
   ![Search box for comments](assets/search-box-for-comments-area.png)
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ..** area, to reply to an existing comment, then follow steps 4-8 above. (**************accurate??***********)
1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.
   ![New comments banner on record](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![More menu](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 
    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body text**: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). -->

## “历史记录”部分概述

您可以在记录的右侧面板的“历史记录”部分中查看对记录所做的更改。

有关详细信息，请参阅[历史记录部分概述](/help/quicksilver/planning/records/history-section-overview.md)。
