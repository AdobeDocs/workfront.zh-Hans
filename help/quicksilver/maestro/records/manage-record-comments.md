---
title: 管理记录注释
description: 可通过在记录的“Adobe”区域添加更新并询问问题或回复，对Comments Maestro记录进行协作。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 3ffb6fdebb54682abc737e55186850458a133f7c
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 管理记录注释

您可以在AdobeMaestro记录的“备注”区域添加更新并询问问题或回复，从而对其进行协作。

## 有关对记录进行注释的注意事项

* 您可以在Maestro中记录的Comments部分向操作记录和分类添加注释和回复。

* 添加到链接记录的评论不会显示在您链接到的记录中。 例如，如果您对链接到Campaign记录的项目添加注释，则该注释仅在Maestro中的项目记录中显示，而不会在要链接的Campaign记录中显示。

* 添加到其他应用程序中链接对象的注释不会显示在Maestro中。
添加到Maestro中链接对象的注释不会显示在其他应用程序中。\
  例如，添加到Workfront中的项目的评论不会显示在链接到Maestro中的营销活动的相同项目中。

* 您可以标记用户以引起他们对更新的注意。 标记的用户不会收到应用程序内通知或有关您更新的电子邮件。 无法在Maestro评论中标记团队。

  >[!TIP]
  >
  >* 更新时不会自动标记评论所有者。
  >
  >* 当您回复更新时，无法从更新中删除已标记的用户。

* 您可以从Maestro的以下区域向记录添加更新：

   * 从“详细信息”页面。

  <!--* From the table view.-->

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe产品</p> </td>
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
   <td role="rowheader">访问级别</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">布局模板</td>
   <td> <p>系统管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/grant-access.md">授予对Adobe大师的访问权限</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permissions - replace the table with: **************CHECK ON THE VIEW PERMISSIONS TO THE WORKSPACE; RIGHT NOW, WE SAY THAT VIEW USERS CAN COMMENT BUT THE PAGE BLOWS OUT WHEN I TRY - ASKED PM TO CONFIRM*****************

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
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
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

### 管理对记录的评论

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](assets/dots-main-menu.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](assets/lines-main-menu.png) 图标，然后单击 **[!UICONTROL 大师]**.

   默认情况下，将打开上次访问的工作区。
1. 从中选择表格视图 **视图** 下拉菜单。
1. 单击表视图中记录的名称。

   记录的 **详细信息** 页面将打开。

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
   * **复制正文文本** t：这会将注释的文本复制到剪贴板。
   * **引用回复**：这会将您的评论内容复制到新回复中。 复制的回复中不包含图像。

   有关更多信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. （可选）单击 **更多** 图标 ![](assets/more-menu.png) 单击注释右上角的 **删除** 以删除注释。

