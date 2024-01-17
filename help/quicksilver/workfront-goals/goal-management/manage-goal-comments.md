---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目标中管理目标注释
description: 您可以向可在Adobe Workfront目标中查看的所有目标添加注释。
author: Alina
feature: Workfront Goals
exl-id: 6cf2d2d2-5ba5-40f2-a803-01359c338541
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 0%

---

# 在Adobe Workfront目标中管理目标注释

<!--Audited: 01/2024-->

<!--consider retiring this article when goals and all objects are in parity and we remove the legacy commenting from the system. From then on, there is just ONE way to comment and that will be documented in the Update Work article-->

<!--take "legacy" and "new commenting" references out when we remove the legacy - April 2024???-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](../../product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>-->

<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

您可以向可在Adobe Workfront目标中查看的所有目标添加注释。

## 访问要求

您必须具有以下权限才能执行本文中所述的操作：

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront计划</td>
 <td>
 <p>任何</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront许可证*</td>
 <td>
 <p>新许可证：参与者或更高版本</p>
 或
 <p>当前许可证：请求或更高版本</p> </td>
 </tr>
 <tr>
 <td role="rowheader">产品*</td>
 <td>
 <p> 新产品要求：如果您拥有Select或Prime Adobe Workfront计划，则还必须购买额外的Adobe Workfront Goals许可证。 Workfront目标包含在Ultimate Workfront计划中。</p>
 或
 <p>当前产品要求：您必须为Adobe Workfront目标购买附加许可证，才能访问本文中所述的功能。 </p> <p>有关信息，请参阅 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront Goals的要求</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">访问级别配置</td>
 <td> <p>查看或更高的目标访问权限</p> <p><b>注释</b><p>如果您没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关更多信息，请参阅 <span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">授予对Adobe Workfront目标的访问权限</a></span></td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">对象权限</td>
 <td>
  <div>
  <p>查看目标的或更高权限</p>
  <p>默认情况下，用户无权访问目标 </p>
 <p>有关共享目标的信息，请参阅 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目标中共享目标</a>. </p>
  </div> </td>
 </tr>
</tbody>
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关更多信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 先决条件

在开始之前，您必须具备以下条件：

* 在主菜单中包含目标区域的布局模板。

## 管理目标注释

您可以在目标页面的“更新”部分中向目标添加评论。

您可以回复或喜欢您或其他人在此区域添加的评论。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 位于右上角，或 **主菜单** 图标 ![](assets/lines-main-menu.png) （如果可用），然后单击 **目标**.
这将打开目标列表。
1. 找到要添加注释的目标，然后单击其名称以打开目标页面。
1. 单击  **更新** 在左侧面板中。
1. （可选）要查找现有注释，请开始键入关键字 <!--or a user's name--> 在 **Search** 框（位于右上角） **评论** 选项卡。

   ![](assets/search-field-in-updates-tab-goals.png)

   关键字 <!--or user--> 所搜索的注释会突出显示，并且包含该注释的注释将显示在“更新”部分的顶部。

   <!--change the NOTE below when functionality changes-->

   >[!NOTE]
   >
   >   必须搜索注释或回复中包含的单词。 您无法搜索已标记的用户或团队。


   有关更多信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)

1. 单击 **x** 图标，以清除搜索结果并返回至开始状态。
1. 单击 **评论** 选项卡。
1. 开始在 **新建评论** 盒子。

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >在完成键入和提交评论之前导航离开更新部分，即使注销并重新登录后，页面上评论仍会以草稿模式保留。 添加到注释的任何图像也会保存在草稿中。 草稿会保存7天，之后将丢弃它们并且无法恢复。 草稿注释仅对输入它们的用户可见。

1. （可选）要撤消或重做更改，请使用以下快捷键：
   * CTRL + Z(Mac为⌘ + z)可撤消更改
   * 按CTRL + Y(对于Mac，按⌘ + y)可重做更改
1. （可选）要向更新、超链接或图像添加富文本格式，请使用富文本工具栏上的任意选项或其旁边的图标。 有关更多信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. （可选）在 **标记人员或团队** 区域，开始键入要包含在此注释中的用户或团队的名称或电子邮件，然后当其显示在列表中时将其选定。
1. 选择 **我的公司私有** 切换以使评论仅对您公司中的人员可见。

   >[!TIP]
   >
   >您必须在配置文件中指定公司，才能在更新区域提供此选项。

1. 单击 **提交**.

   >[!TIP]
   >
   >如果另一用户向您正在更新的同一项目提交评论，则会显示一条带“New”指示器的红线以通知您较新的评论，并且屏幕底部会显示一个蓝色通知，指示新评论的数量。
   >
   >指示符仅在提交项目的评论之后显示，而不在评论仍在撰写时显示。
   >![](assets/real-time-new-red-indicator-unified-commenting.png)

1. （可选）要编辑评论，请单击 **更多** 菜单 ![](assets/more-icon.png) 点按赞”图标右侧，然后单击 **编辑**.
1. 编辑评论中的信息，添加或删除图像，或删除任何已标记用户。
您可以在提交评论后15分钟内对其进行编辑。 “已编辑”指标将添加到更新评论时显示的日期戳的左侧。

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   > * 仅当提交原始更新时，才会生成电子邮件通知用户您的更新。 编辑更新后不会生成电子邮件。
   >
   > * 日期戳是原始注释的日期，而不是最新更新的日期。

1. （可选）单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击以下任意选项以将信息从评论复制到剪贴板或新回复中：

   * **复制链接** 复制更新的链接，而不复制回复。
   * **复制正文文本** 以复制更新的文本。
   * **引用回复** 打开新注释框，其中新回复中引用了原始注释，并标记为块引用。

     有关更多信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. （可选）单击 **更多** 菜单 ![](assets/more-icon.png) 单击注释右侧，然后单击 **删除** 以删除您添加的评论。 有关更多信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. （可选）单击 **回复** 要回复现有评论，请按照上述步骤5至9操作。 有关回复更新的详细信息，请参阅 [回复更新](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md). <!--insure this stays accurate-->
1. （视情况而定，可选）如果其他用户添加了显示在“更新”部分的可见区域之外的注释，请单击 **视图** 蓝色内部 **新评论横幅** 在屏幕底部显示这些注释。

   ![](assets/blue-new-comments-banner-with-view-button.png)

   屏幕底部会显示其他注释。
1. （可选）单击 **点赞** 图标![](assets/like-icon.png) 喜欢其他人添加的评论。 图标会随喜欢的数量而更新。

1. （可选）单击 **系统活动** 选项卡以查看系统记录的更新。 更新目标后，Workfront会生成有关该更新的注释，并将其显示在System Activity选项卡中。 在将结果、活动或项目添加到目标或进行更新时，Workfront还会记录系统更新。 <!--ensure the casing on the tab has not changed-->

