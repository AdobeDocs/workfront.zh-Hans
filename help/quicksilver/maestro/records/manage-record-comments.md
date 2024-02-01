---
title: 管理记录注释
description: 通过在记录的右侧面板中添加注释或回复，您可以对AdobeMaestro记录进行协作。 您还可以在此区域查看对记录所做的其他更改以及系统记录的更改。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '1155'
ht-degree: 0%

---


# 管理记录注释

{{maestro-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Maestro records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

通过在记录的右侧面板中添加评论或回复，可以对AdobeMaestro记录进行协作。 您还可以在此区域查看对记录所做的其他更改以及系统记录的更改。

记录的右侧面板显示以下部分：

* **评论**：显示用户添加到记录的评论和回复。
* **历史记录**：显示用户对记录字段进行的系统记录更改。 有关更多信息，请参阅 [“历史记录”部分概述](/help/quicksilver/maestro/records/history-section-overview.md).

>[!TIP]
>
>右侧面板显示操作记录和分类记录。


## 有关对记录进行注释的注意事项

* 您可以在Maestro中记录的Comments部分向操作记录和分类添加注释和回复。

* 添加到链接记录的评论不会显示在您链接到的记录中。 例如，如果您对链接到Campaign记录的Maestro Product记录添加注释，则该注释仅显示在Maestro的Product记录中，而不会显示在您从中链接的Campaign记录中。

* 您可以向由于Maestro记录与来自其他应用程序的对象之间的连接而创建的Maestro记录添加注释。

  例如，在将Workfront项目与Maestro记录连接后，您可以对Project Maestro记录进行评论。 有关更多信息，请参阅 [连接记录](/help/quicksilver/maestro/records/connect-records.md).

* 添加到其他应用程序中链接对象的注释不会显示在Maestro中，而添加到Maestro中链接对象的注释不会显示在其他应用程序中。

  例如，添加到Workfront中的项目的注释不会显示在链接到Maestro中的营销活动的同一项目中，并且添加到Maestro记录中的项目注释不会显示在Workfront中。

* 您可以标记用户以引起他们对更新的注意。 标记的用户不会收到应用程序内通知或有关您更新的电子邮件。 <!--this might change??-->

* 您可以向记录添加更新，并复查Maestro以下区域的更改历史记录：

   * 从记录或分类的“详细信息”页面。

  <!--* From the table view.-->

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵公司必须注册AdobeMaestro封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront计划</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Maestro中没有访问级别控制。 </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>查看工作区或更高权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

### 管理对记录的评论

{{step1-to-maestro}}

默认情况下，将打开上次访问的工作区。
1. 从中选择表格视图 **视图** 下拉菜单。
1. 单击表视图中记录的名称。

   记录的 **详细信息** 页面将打开。 默认情况下，“注释”区域会在右侧面板中打开。

1. （视情况而定）如果默认情况下未打开右侧面板，请单击 **显示评论** ![](assets/show-comments-icon.png) 图标，以打开“注释”部分。

1. 开始在 **新建评论** 盒子。

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >在完成键入并提交评论之前导航离开“评论”部分，即使用户注销并重新登录，该评论仍会在页面中保持草稿模式。 添加到注释的任何图像也会保存在草稿中。 草稿会保存7天，之后将丢弃它们并且无法恢复。 草稿注释仅对输入它们的用户可见。

1. （可选）要撤消或重做更改，请使用以下快捷键：
   * CTRL + Z(Mac为⌘ + z)可撤消更改
   * 按CTRL + Y(对于Mac，按⌘ + y)可重做更改
1. （可选）添加 **@** 后跟用于在更新中标记某人的用户的名称。
1. （可选）使用富文本工具栏中的选项设置文本格式，在更新中添加表情符号、链接或图像，以增强内容。 有关更多信息，请参阅文章中的“在Workfront更新中使用富文本”部分 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >如果另一用户向您正在更新的同一项目提交评论，则会显示一条带“新”指示器的红线，通知您较新的评论。
   >
   >指示符仅在提交项目的评论之后显示，而不会在评论仍在撰写时显示。
   >
   >![](assets/new-line-indicator-comments.png)

1. 单击 **提交** 将更新添加到记录。
1. （可选）要编辑评论，请单击 **更多** 菜单 ![](assets/more-menu.png) 单击注释右上角的 **编辑**.

   >[!IMPORTANT]
   >
   >您只能在提交评论后15分钟内对其进行编辑。

1. 编辑评论中的信息，添加或删除图像或删除任何已标记用户。 “已编辑”指示符将添加到评论的左侧。

   >[!TIP]
   >
   >当前年份的注释不会在日期戳中显示年份。 将鼠标悬停在时间戳上会显示完整日期，包括年份。

1. （可选且有条件）要搜索现有注释，请在 **评论** 区域。

   ![](assets/search-box-for-comments-area.png)

1. （可选）单击 **回复** 或开始在 **添加回复……** 区域，回复现有评论，然后执行上述步骤4-8。 <!--(**************accurate??***********)-->

1. （视情况而定，可选）如果其他用户添加了在添加注释时显示在“注释”部分的可见区域之外的注释，请单击 **视图** 内部 **新评论横幅** 在屏幕底部显示这些注释。

   ![](assets/new-comments-banner-on-record.png)

   屏幕底部会显示其他注释。

1. （可选）单击 **点赞** 图标表示喜欢更新或确认您已阅读该更新。 图标会随喜欢的数量而更新。
1. （视情况而定，可选）如果在注释中包含其他人员，请单击更新中包含的用户的头像，以显示与注释共享的用户列表。
1. （可选）单击 **更多** 图标 ![](assets/more-menu.png) 单击注释右上角的以下选项之一，从注释中复制信息：

   * **复制链接**：这会将指向评论的链接复制到剪贴板。
   * **复制正文文本**：这会将注释的文本复制到剪贴板。
   * **引用回复**：这会将您的评论内容复制到新回复中。 复制的回复中不包含图像。

   有关更多信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. （可选）单击 **更多** 图标 ![](assets/more-menu.png) 单击注释右上角的 **删除** 以删除注释。
1. （可选）单击 **隐藏评论** 图标 ![](assets/hide-comments-icon.png) 以关闭右侧面板。

## “历史记录”部分概述

您可以在操作记录或分类右侧面板的“历史记录”部分中查看对记录所做的更改。

有关更多信息，请参阅 [“历史记录”部分概述](/help/quicksilver/maestro/records/history-section-overview.md).

