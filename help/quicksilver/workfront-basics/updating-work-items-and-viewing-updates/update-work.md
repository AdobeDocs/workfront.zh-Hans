---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新工作
description: 您可以对Adobe Workfront对象（项目、任务或问题）添加更新，以告知对象的进度。 为对象分配或订阅了该对象的用户可以查看您的更新。 您还可以标记用户以引起用户对更新的注意。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '1956'
ht-degree: 1%

---

# 更新工作

<!-- Drafted for commenting experience: 

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the way you update work when using the Updates section of an object. 
>You can access the new design by enabling the commenting Beta. 
>Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new updating experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

您可以在更新部分中向Adobe Workfront中的大多数对象添加注释。 有关哪些对象显示“更新”(Updates)部分的详细信息，请参阅 [更新部分概述](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

您可以在对对象进行注释时，对Workfront对象（项目、任务或问题）添加更新，以告知该对象的进度。 为对象分配或订阅了该对象的用户可以查看您的更新。 您还可以标记用户以引起用户对更新的注意。 标记用户将收到有关您更新的应用程序内通知和电子邮件。

本页中的信息介绍了如何对Workfront对象进行注释，以及如何更新项目、任务和问题。 有关对目标进行评论的信息，请参阅 [在Adobe Workfront目标中管理目标注释](../../workfront-goals/goal-management/manage-goal-comments.md). 您必须拥有其他许可证才能访问Workfront Goals。


您可以从Workfront的以下区域添加对项目、任务和问题的更新：

* 从Workfront对象的Updates部分中
* 从“主页”区域（针对任务和问题）
* 从对象列表的“摘要”面板（针对任务和问题）
* 从时间表（任务和问题）

## 访问要求

<!--
drafted for P&P release:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Current license: Contributor or higher for issues and documents: Light or higher for all other objects</p> 
   Or
   <p>Legacy  license: Request or higher for issues and documents; Review or higher for all other objects</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>（二）对问题和文件提出要求或更高要求；对所有其他对象进行审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>查看或编辑更新所在对象的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>查看对对象的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 向工作项添加更新

<!--drafted for the commenting experience - change the NOTE at the top of the following section with every new release to other objects

Adding an update to a work item differs depending on what version of the Updates section and what object you choose. 

### Add an update to a work item in the current Updates section

>[!NOTE]
>
>The following functionality is available for all objects except for goals. You must have an additional license to access Workfront Goals. For information about commenting on goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md)

-->

1. 转到要为其提供更新的工作项（例如项目、任务或问题）。
1. 单击 **更新** 中。
1. 单击 **开始新更新，** 然后键入更新。
1. （可选）使用富文本，或向更新中添加表情符号、链接或图像，以增强您的内容。 有关更多信息，请参阅本文中的“在Workfront更新中使用富文本”部分
1. （可选）更新有关工作项的以下任何信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>通知</strong></td> 
      <td>确定需要收到更新通知的用户。 为对象分配或订阅的用户在进行更新时会自动接收通知。<br><p>有关如何在更新中包含其他用户的信息，请参阅 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">更新时标记其他人</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>提交日期</strong></td> 
      <td>在日期选取器中，选择完成工作项的提交日期。 有关提交日期的信息，请参阅 <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">提交日期概述</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>完成情况</strong></td> 
      <td>为任务或问题选择新条件。 有关选择条件的信息，请参阅 <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">任务和问题的更新条件</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>状态</strong></td> 
      <td>单击当前状态旁边的箭头，然后从下拉菜单中选择所需的状态。 有关设置状态的信息，请参阅 <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">更新任务状态</a>.<p>更新工作项的状态不会自动更改项目的状态。 根据项目的设置方式，您可能需要分别对项目状态进行更新。 有关各种项目更新类型的更多信息，请参阅 <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">选择项目更新类型 </a>.</p><p><b>注释</b>

   当工作项目处于“待批准”状态时，您无法更改其状态。</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>完成栏</strong></td> 
      <td>（仅适用于任务）通过将进度条滑动到所需百分比来指示已完成的工作百分比。 您还可以双击完成栏并输入完成百分比。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>我的公司私有</strong></td> 
      <td> <p>禁用此选项，可阻止公司外的用户有权查看此更新。</p> 
      <p><b>注释</b></p>
      <p>仅当用户与公司关联时，才会显示此选项。</p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **更新** 将更新添加到Workfront对象。

   >[!NOTE]
   >
   >单击后，将显示一个小弹出窗口7秒 **更新**，允许您在发布更新之前撤消更新并返回到编辑窗格。 如果您关闭撤消弹出窗口，等待其消失或导航离开页面，则将发布更新。
   >
   >如果Workfront管理员在您的访问级别中选择了“绝不允许用户删除评论”设置，则无法撤消评论。 有关更多信息，请参阅 [创建和修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. 要回复更新，请参阅 [更新回复](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

<!--

### Add an update to a work item using the commenting Beta experience


>[!NOTE]
>
>The functionality described in this section is available for the following objects:
>
>* <span class="preview">Issues, when you enable the commenting Beta experience.</span>
>
>   <span class="preview">This functionality is available only for the Updates section of issues, and it is not available for the following areas:</span>
>
>   * <span class="preview">Home</span>
>   * <span class="preview">Summary panel in lists</span>
>   * <span class="preview">Summary panel in timesheets</span>
>* Goals
>
>   The commenting experience Beta is the default current experience for goals.
>   You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


1. Locate the object you want to update, then click its name to open the object's page.
1. Click  **Updates** in the left panel. 
1. Click **Try out the commenting Beta** button in the lower-right corner of the Updates area, then click **Agree** on the Beta agreement. This switches the Updates area to the commenting Beta experience. 
   The **Comments** tab is selected by default. 
1. Start entering a comment in the **New comment** box. 
   
   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Navigating away from the Updates section before you finish typing and submitting a comment keeps the comment on the page in draft mode even after you log off and log back on. Drafted comments are only visible to the user entering them.

1. (Optional) In the **Tag people or teams** area, start typing the name or the email of a user, or a team that you would like to include in this comment, then select it when it displays in the list. 
1. (Optional) To add rich text formatting to your update, use any of the following options from the **Rich Text** toolbar to enhance your text: 

   * Bold
   * Italics
   * Underline
   * Link
   * Bulleted List
   * Numbered List
   * Add attachment (mark this parenthesis as draft: ************ this might be renamed)
   
   For more information, see the "Use Rich Text in a Workfront update" section in this article.

   >[!TIP]
   >
   >   If another user submits a comment to the same item you are updating, there will be a red line with a "New" indicator to inform you of the newer comments. The indicator only displays only after the comment was submitted on the item, and not when the comment is still composed. 
   >
   > ![](assets/real-time-new-red-indicator-unified-commenting.png)



1. Click **Submit** to add the update to the Workfront object. 
1. (Optional) To edit a comment, click the **More** menu ![](assets/more-menu.png) to the right of the Like icon, then click **Edit**. 
1. Edit the information in the comment, or remove any of the tagged users. 
   You can edit your comment within 15 from submitting it. An "Edited" indicator is added to the left of the date stamp that displays when the comment was updated. 

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >   An email is generated to notify users of your update only when you submit the original update. No email is generated after you edited your update.
1. (Optional) Click **Reply** to reply to an existing comment, then follow the steps 5-7 above. (**************insure this stays accurate***********). For information about replying to an update, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
1. (Optional) Click the **Like** icon![](assets/like-icon.png). The icon updates with the number of likes.
1. (Conditional and Optional) If you included additional people in your comment, click the number of members included in the update to display a list of entities that the comment you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)
1. (Optional) Click the **System Activity** tab to view updates logged by the system. When the object or any of its children are updated, Workfront generates a note about that update and displays it in the System Activity tab. 

   For more information see [Updates section  overview](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >You cannot add a comment to a system update.
-->


## 在Workfront更新中使用富文本

<!--remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.

>[!NOTE]
>
>Some of the options in the Rich Text toolbar are not available for the commenting Beta experience.-->


您可以使用富文本或向其添加各种项目（如表情符号、链接或图像）来增强更新。

1. 转到更新区域，然后开始键入评论。
1. （可选）要向更新添加富文本格式，请在 **富文本** 工具栏。

   | **属性** | **工具栏按钮** | **Mac快捷键** | **PC快捷键** |
   |---|---|---|---|
   | 粗体 | ![mceclip10.png](assets/mceclip10.png) | ⌘+b | Ctrl+B |
   | 斜体 | ![mceclip9.png](assets/mceclip9.png) | ⌘+i | Ctrl+I |
   | 下划线 | ![mceclip8.png](assets/mceclip8.png) | ⌘+u | Ctrl+U |
   | 超链接 | ![mceclip7.png](assets/mceclip7.png) | ⌘+K | Ctrl+K |
   | 项目符号列表 | ![mceclip6.png](assets/mceclip6.png) | ⌘+Shift+8 | Ctrl+Shift+8 |
   | 编号列表 | ![mceclip5.png](assets/mceclip5.png) | ⌘+Shift+7 | Ctrl+Shift+7 |
   | 块引用 | ![](assets/block-quote-icon-large.png) | ⌘+Shift+9 | Ctrl+Shift+9 |

   要停止格式化文本，请取消选择 **富文本** 工具栏。

   >[!NOTE]
   >
   >* 格式设置还会显示在用户收到的包含您更新的任何电子邮件通知中。
   >* 在“更新”选项卡中查看更新时，应用于电子邮件中更新的富文本格式不会显示在更新中。
   >* 如果贵组织将Workfront与Internet Explorer结合使用，则粘贴到更新中的任何带格式的文本都将丢失其富文本格式，并显示为纯文本。 您可以使用富文本工具栏上的属性重新设置文本格式。
   >* 对于在“时间表”区域进行的更新，或在报表中查看的“备注”和“最后条件”对象，富文本格式不可用。


1. （可选）如果要包含来自先前更新或来自其他来源的文本，并将其与您自己的更新区分开，则可将其标记为“块引用”。 单击 **块报价** 图标 ![](assets/block-quote-small.png) 然后键入要引用的文本。 带引号的文本显示为垂直灰线。 单击 **块报价** 图标，以恢复正常格式。

   ![](assets/block-quote-marked-350x144.png)

1. （可选）将表情符号添加到更新中。

   >[!NOTE]
   >
   >* Workfront不会将标点符号（如：）替换为表情符号。
   >* 对于在“时间表”区域进行的更新，或在报表中查看的“备注”和“最后条件”对象，不提供表情符号。
   >* Workfront中的表情符号功能利用Unicode字符，因此，仅在支持Unicode代码点的浏览器和操作系统上显示。 与您的平台、浏览器或操作系统版本不同的用户可能无法访问相同的表情符号。
   >* 不支持的表情符号由黑框或白框表示。
   >* Windows 7仅支持黑白表情符号。
   >* 在“更新”区域查看更新时，应用于通过电子邮件进行的更新的表情符号不会显示在更新中。


1. （可选）要添加指向其他信息源的URL链接，请执行以下操作：

   1. 在要插入链接的更新中单击。
   1. 在 **富文本** 工具栏，单击 **超链接** 图标。 ![](assets/link-icon.png)

   1. 在 **创建链接** 框，位于 **URL**，键入或粘贴要链接的源的URL。

   1. 在 **要显示的文本**，请键入或粘贴链接文本。
   1. 单击&#x200B;**保存**。

1. （可选）要将图像附加到更新，请单击 **图像** 图标 ![](assets/addimageicon-35x32.png) 浏览到您计算机上的图像。\
   或\
   将图像拖入更新区域。

   >[!NOTE]
   >
   >* 您的Workfront管理员必须先启用添加图像功能，然后才能看到图像图标。
   >* 最大图像文件大小为7 MB。 支持的图像文件类型有.jpg、.gif和.png。
   >* 图像只能从对象的“更新”(Updates)选项卡访问，而无法在“文档”(Documents)选项卡中使用。
   >* 您可以发送包含图像的更新，而不发送任何文本。

1. 单击 **更新**  <!--<span class="preview">or **Submit**</span>, in the commenting Beta experience-->.


## 复制更新信息

<!--drafted for beta release toggle - remove when copying an update will be available: 

>[!NOTE]
>
>Copying an update is not possible when using the Beta commenting experience.
-->

您可以通过多种方式复制更新。 复制链接后，您可以与他人共享该链接，以将他们定向到更新。

* [复制更新](#copy-the-update)
* [复制线程链接](#copy-the-thread-link)
* [复制更新链接](#copy-the-update-link)

### 复制更新 {#copy-the-update}

此选项将文本从特定更新复制到剪贴板。

1. 转到要复制的更新或回复。
1. 单击 **更多** 菜单，然后单击 **复制正文文本**.

   ![选择复制正文文本](assets/update-stream-copy-body-text-350x152.png)

### 复制线程链接 {#copy-the-thread-link}

此选项会将整个线程链接复制到剪贴板，以便您可以与其他用户共享该线程。

1. 转到要复制的更新线程。
1. 单击 **更多** 菜单，然后单击 **复制线程链接**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

### 复制更新链接 {#copy-the-update-link}

此选项将特定更新链接复制到剪贴板。 当您共享更新链接时，跟踪该链接的用户会看到更新周围的边框。

1. 转到要复制的更新或回复。
1. 单击 **更多** 菜单，然后单击 **复制更新链接**.

   ![](assets/update-stream-reply-menu-marked-350x182.png)

## 删除更新或回复

根据Workfront管理员授予您的访问权限，您可能能够删除您在对象的Updates选项卡中添加的更新。 有关更多信息，请参阅 [创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) 在文章中 [创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

任何Workfront用户(包括Workfront管理员)都无法删除其他用户进行的更新。 但是，如果用户的访问级别允许他们删除自己的更新，则Workfront管理员可以以该用户身份登录并删除他们所做的更新。 有关更多信息，请参阅 [创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) 和 [以其他用户身份登录](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. 转到要删除的更新或回复。
1. 单击 **更多** 要删除的更新或回复旁边的菜单，然后单击 **删除**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. 在显示的消息中，单击 **确认** <!--<span class="preview">or **Delete**</span>, in the commenting Beta experience-->.

>[!NOTE]
>
>删除附加图像的更新会同时删除注释和图像。

## 添加时间表更新

1. 转到要更新的时间表。
1. 单击时间表以将其打开。
1. 在工时表底部，单击 **包含评论**.
1. 在“时间表”(Timeske)底部显示的框中，键入更新。

   ![timetime_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. （视情况而定）要保存更新而不提交时间表以供审批，请单击 **保存以备以后使用**.

   或

   要保存更新并提交时间表以供审批，请单击 **提交以供审批**.

   或

   如果未通过审批者设置工时单，请单击 **保存并关闭时间表** 以保存更新。

## 启用或禁用系统更新

<!--remove preview with 23.2 production: 

<div class="preview">
>[!NOTE]
>
>It is not possible to disable system updates when using the Beta commenting experience. 
>The information in this section refers only to functionality available in the current Updtes section. 
>For more information about system updates in the Beta version, see [Updates section overview](../updating-work-items-and-viewing-updates/updates-tab-overview.md) 
</div>
-->

Workfront对象的“更新”部分显示两种类型的信息：

* **用户更新：** 用户更新是您和系统中的其他用户输入的注释。

   ![](assets/user-update-cl-350x277.png)

* **系统更新：** 系统更新删除资产、添加或删除版本、附加或删除批准请求以及对对象上的文档所做的任何编辑或更改的记录。

   ![](assets/system-updates-cl-350x277.png)

根据您的Workfront许可证，系统更新可能默认启用。 Workfront管理员可以确定系统更新中跟踪的内容，如 [系统跟踪的更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). 您还可以过滤掉系统更新或活动，以便仅查看所有对象的用户更新。

有关用户和系统更新之间差异的详细信息，请参阅 [系统跟踪的更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

要启用或禁用系统更新，请执行以下操作：

1. 单击 **更新** 选项卡。
1. 单击 **显示系统更新** 向左（禁用）或向右（启用）滑动开关。

   ![](assets/show-system-updates-qs-350x55.png)

   此选项在整个Workfront中的所有对象中都是永久性的，并且会保持在您选择的位置，即使您从Workfront中注销也是如此。

