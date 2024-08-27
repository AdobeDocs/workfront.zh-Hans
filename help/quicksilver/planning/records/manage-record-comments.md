---
title: 管理记录注释
description: 通过在记录的右侧面板中添加评论或回复，您可以对Adobe Workfront Planning记录进行协作。 您还可以在此区域查看对记录所做的其他更改以及系统记录的更改。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '1269'
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
<p>有关每个Workfront计划中包含的内容的更多信息，请参阅<a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront定价和打包</a>。 </p> 
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

<!--OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>
-->

## 有关对记录进行注释的注意事项

* 您可以在Workfront Planning的“注释”部分中为记录添加注释和回复。

* 添加到链接记录的评论不会显示在您链接到的记录中。 例如，如果您对链接到Campaign记录的Workfront Planning产品记录添加注释，则该注释仅在Workfront Planning的产品记录中显示，而不会在您链接的Campaign记录中显示。

* 您可以将注释添加到由于某个记录与来自另一个应用程序的对象之间的连接而创建的Workfront Planning记录中。

  例如，在将Workfront项目与Workfront Planning记录连接后，您可以对Workfront Planning项目记录进行评论。 有关详细信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

* 添加到其他应用程序中链接对象的注释不会显示在Workfront Planning中，而添加到Workfront Planning中链接对象的注释不会显示在其他应用程序中。

  例如，添加到Workfront中的项目的注释不会显示在链接到Workfront Planning中的营销活动的同一项目中，并且添加到Workfront Planning项目记录的注释不会显示在Workfront中。

* 您可以标记用户以引起他们对更新的注意。 标记的用户不会收到应用程序内通知或有关您更新的电子邮件。<!--this might change??-->

<!--replace the bullet above with this: * You can tag users to bring their attention to an update. Tagged users receive an in-app notification or an email notification about your update. 
   The following scenario exists:   

   * Adobe Unified Experience users receive both an in-app notification and an email notification. 
   * Users who are not in the Adobe Unified Experience receive only an email notification. 

      For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md)
   
      To determine whether your company is using the Adobe Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
      -->

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
1. （可选）添加&#x200B;**@**，后跟用户名称，以在更新中标记某人。

   <!--Adobe Unified Experience users can receive an in-app and an email notification when they are tagged. All other users receive an email when they are tagged. For more information, see the section [Considerations about commenting on a record](#considerations-about-commenting-on-a-record) in this article. -->

1. （可选）使用富文本工具栏中的选项设置文本格式，在更新中添加表情符号、链接或图像，以增强内容。 有关详细信息，请参阅文章[更新工作](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)中的“在Workfront更新中使用富文本”部分。

   >[!TIP]
   >
   >如果另一用户向您正在更新的同一项目提交评论，则会显示一条带“新”指示器的红线，通知您较新的评论。
   >
   >指示符仅在提交项目的评论之后显示，而不会在评论仍在撰写时显示。
   >
   >![](assets/new-line-indicator-comments.png)

1. 单击&#x200B;**提交**&#x200B;将更新添加到记录。
1. （可选）要编辑评论，请单击评论右上角的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**编辑**。

   >[!IMPORTANT]
   >
   >您只能在提交评论后15分钟内对其进行编辑。

1. 编辑评论中的信息，添加或删除图像或删除任何已标记用户。 “已编辑”指示符将添加到评论的左侧。

   >[!TIP]
   >
   >当前年份的注释不会在日期戳中显示年份。 将鼠标悬停在时间戳上会显示完整日期，包括年份。

1. （可选且有条件）要搜索现有评论，请在&#x200B;**评论**&#x200B;区域右上角的搜索框中开始键入关键字。

   ![](assets/search-box-for-comments-area.png)

1. （可选）单击&#x200B;**回复**&#x200B;或开始在&#x200B;**添加回复……**&#x200B;区域键入评论以回复现有评论，然后执行上面的步骤4-8。<!--(**************accurate??***********)-->

1. （视情况而定，可选）如果您在添加评论时，其他用户在“评论”部分的可见区域之外添加了显示的评论，请单击屏幕底部的&#x200B;**新评论横幅**&#x200B;中的&#x200B;**查看**&#x200B;以显示这些评论。

   ![](assets/new-comments-banner-on-record.png)

   屏幕底部会显示其他注释。

1. （可选）单击&#x200B;**类似**&#x200B;图标以喜欢更新或确认您已阅读该更新。 图标会随喜欢的数量而更新。
1. （视情况而定，可选）如果在注释中包含其他人员，请单击更新中包含的用户的头像，以显示与注释共享的用户列表。
1. （可选）单击评论右上角的&#x200B;**更多**&#x200B;图标![](assets/more-menu.png)，然后单击以下选项之一，以从评论中复制信息：

   * **复制链接**：这会将指向评论的链接复制到剪贴板。
   * **复制正文文本**：这会将评论的文本复制到剪贴板。
   * **引用回复**：这会将您的评论内容复制到新回复中。 复制的回复中不包含图像。

   有关详细信息，请参阅[更新工作](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。
1. （可选）单击评论右上角的&#x200B;**更多**&#x200B;图标![](assets/more-menu.png)，然后单击&#x200B;**删除**&#x200B;以删除评论。
1. （可选）单击&#x200B;**隐藏评论**&#x200B;图标![](assets/hide-comments-icon.png)以关闭右侧面板。

## “历史记录”部分概述

您可以在记录的右侧面板的“历史记录”部分中查看对记录所做的更改。

有关详细信息，请参阅[历史记录部分概述](/help/quicksilver/planning/records/history-section-overview.md)。
