---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目标中管理目标注释
description: 您可以向可在Adobe Workfront目标中查看的所有目标添加注释。
author: Alina
feature: Workfront Goals
exl-id: 6cf2d2d2-5ba5-40f2-a803-01359c338541
source-git-commit: 52e8ce6dd5146d72f698583b531b3db6bc5dbf25
workflow-type: tm+mt
source-wordcount: '1092'
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
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> 
   <p>对于新计划和许可证结构：
  <ul><li>最终计划 </li>
  或
  <li>适用于Prime或Select Adobe Workfront计划的Adobe Workfront目标的附加许可证。 </li></ul> </p>
<p>对于当前计划和许可证结构： 
<ul><li> Pro或更高版本 </li>
  <li>除了Adobe Workfront许可证之外，还提供了Workfront目标许可证。</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront许可证</td>
 <td>
 <p>任何</td>
 </tr>
 <tr>
 <td role="rowheader">产品*</td>
 <td>
 <p> 新产品要求：如果您拥有Select或Prime Adobe Workfront计划，则还必须购买额外的Adobe Workfront Goals许可证。 Workfront目标包含在Ultimate Workfront计划中。</p>
 或
 <p>当前产品要求：您必须为Adobe Workfront目标购买附加许可证，才能访问本文中所述的功能。 </p> <p>有关信息，请参阅<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目标的要求</a>。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">访问级别配置</td>
 <td> <p>查看或更高的目标访问权限</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">对象权限</td>
 <td>
  <div>
  <p>查看目标的或更高权限</p>
  <p>默认情况下，用户无权访问目标 </p>
 <p>有关共享目标的信息，请参阅<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目标中共享目标</a>。 </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>必须为包括Workfront管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的目标区域。 </p>  
</td>
  </tr>
</tbody>
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 先决条件

在开始之前，您必须具备以下条件：

* 在主菜单中包含目标区域的布局模板。

## 管理目标注释

您可以在目标页面的“更新”部分中向目标添加评论。

您可以回复或喜欢您或其他人在此区域添加的评论。

1. 单击右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)或左上角的&#x200B;**主菜单**&#x200B;图标![](assets/lines-main-menu.png)（如果可用），然后单击&#x200B;**目标**。
这将打开目标列表。
1. 找到要添加注释的目标，然后单击其名称以打开目标页面。
1. 单击左侧面板中的&#x200B;**更新**。
1. （可选）要查找现有评论，请在&#x200B;**评论**&#x200B;选项卡右上角的&#x200B;**搜索**&#x200B;框中开始键入关键字<!--or a user's name-->。

   ![](assets/search-field-in-updates-tab-goals.png)

   您搜索的关键字<!--or user-->已突出显示，包含该关键字的注释将显示在“更新”部分的顶部。

   <!--change the NOTE below when functionality changes-->

   >[!NOTE]
   >
   >必须搜索注释或回复中包含的单词。 您无法搜索已标记的用户或团队。

   有关详细信息，请参阅[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

1. 单击搜索字段中的&#x200B;**x**&#x200B;图标以清除搜索结果并返回完整更新。
1. 单击“更新”区域左上角的&#x200B;**注释**&#x200B;选项卡。
1. 开始在&#x200B;**新建评论**&#x200B;框中输入评论。

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >在完成键入和提交评论之前导航离开更新部分，即使注销并重新登录后，页面上评论仍会以草稿模式保留。 草稿会保存7天，之后将丢弃它们并且无法恢复。 草稿注释仅对输入它们的用户可见。

1. （可选）要撤消或重做更改，请使用以下快捷键：
   * CTRL + Z(Mac为⌘ + z)可撤消更改
   * 按CTRL + Y(对于Mac，按⌘ + y)可重做更改
1. （可选）要将富文本格式添加到更新、超链接或表情符号中，请使用富文本工具栏上的任意选项或其旁边的图标。 有关详细信息，请参阅[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。
1. （可选）在&#x200B;**为人员或团队添加标签**&#x200B;区域，开始键入要包含在此评论中的用户或团队的名称或电子邮件，然后当该评论显示在列表中时将其选定。
1. 选择&#x200B;**我的公司私有**&#x200B;切换开关以使评论仅对公司中的人员可见。

   >[!TIP]
   >
   >您必须在配置文件中指定公司，才能在更新区域提供此选项。

1. 单击&#x200B;**提交**。

   >[!TIP]
   >
   >如果另一用户向您正在更新的同一项目提交评论，则会显示一条带“New”指示器的红线以通知您较新的评论，并且屏幕底部会显示一个蓝色通知，指示新评论的数量。
   >
   >指示符仅在提交项目的评论之后显示，而不在评论仍在撰写时显示。
   >![](assets/real-time-new-red-indicator-unified-commenting-copy.png)

1. （可选）要编辑评论，请单击“赞”图标右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-icon.png)，然后单击&#x200B;**编辑**。
1. 编辑评论中的信息或移除任何已标记的用户。
您可以在提交评论后15分钟内对其进行编辑。 “已编辑”指标将添加到更新评论时显示的日期戳的左侧。

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   > * 仅当提交原始更新时，才会生成电子邮件通知用户您的更新。 编辑更新后不会生成电子邮件。
   >
   > * 日期戳是原始注释的日期，而不是最新更新的日期。

1. （可选）单击&#x200B;**更多**&#x200B;菜单![](assets/more-icon.png)，然后单击以下任一选项以将信息从评论复制到剪贴板或复制到新回复中：

   * **复制链接**&#x200B;以复制更新的链接，而不复制回复。
   * **复制正文文本**&#x200B;以复制更新的文本。
   * **引用回复**&#x200B;打开新评论框，其中原始评论被引用在新回复中并标记为块引用。

     有关详细信息，请参阅[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

1. （可选）单击评论右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-icon.png)，然后单击&#x200B;**删除**&#x200B;以删除您添加的评论。 有关详细信息，请参阅[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。
1. （可选）单击&#x200B;**回复**&#x200B;以回复现有评论，然后执行上述步骤5-9。 有关回复更新的详细信息，请参阅[回复更新](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md)。<!--insure this stays accurate-->
1. （有条件，可选）如果其他用户在“更新”部分的可见区域之外添加了注释，请单击屏幕底部的蓝色&#x200B;**新注释横幅**&#x200B;中的&#x200B;**查看**&#x200B;以显示这些注释。

   ![](assets/blue-new-comments-banner-with-view-button.png)

   屏幕底部会显示其他注释。
1. （可选）单击&#x200B;**类似**&#x200B;图标![](assets/like-icon.png)可喜欢其他人添加的评论。 图标会随喜欢的数量而更新。

1. （可选）单击&#x200B;**系统活动**&#x200B;选项卡以查看系统记录的更新。 更新目标后，Workfront会生成有关该更新的注释，并将其显示在System Activity选项卡中。 在将结果、活动或项目添加到目标或进行更新时，Workfront还会记录系统更新。<!--ensure the casing on the tab has not changed-->


