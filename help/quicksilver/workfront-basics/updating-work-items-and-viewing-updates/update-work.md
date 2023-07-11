---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新工作
description: 您可以对Adobe Workfront对象（项目、任务或问题）添加更新，以传达对象的进度。 已分配或订阅对象的用户可以查看您的更新。 您还可以标记用户，以引起他们对更新的注意。
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 4116cd1610cc5b8de0407a96a4bc67532d78a25e
workflow-type: tm+mt
source-wordcount: '3465'
ht-degree: 1%

---

# 更新工作

<!--take "Beta" references out when we remove the beta-->

<span class="preview">此页面上高亮显示的信息是指尚未公开发布的功能。 它仅适用于预览环境中的所有客户。</span>

>[!NOTE]
>
>我们目前正在重新设计Adobe Workfront中的评论体验。
>
>有关新评论体验的更多信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>您可以访问以下对象的新体验：
> * 问题， <span class="preview">项目、任务和文档</span>.
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

您可以在“更新”部分向Adobe Workfront中的大多数对象添加注释。 有关哪些对象显示“更新”部分的更多信息，请参阅 [更新部分概述](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

您可以对Workfront对象（项目、任务或问题）添加更新，以在对象上添加注释时传达对象的进度。 已分配或订阅对象的用户可以查看您的更新。 您还可以标记用户，以引起他们对更新的注意。 标记的用户会收到应用程序内通知和一封关于您更新的电子邮件。 有关更多信息，请参阅 [为其他人标记更新](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

您可以向可查看的对象添加注释，也可以以Workfront或组管理员身份登录并代表其他用户添加注释。 有关更多信息，请参阅 [以其他用户身份登录](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

本页上的信息介绍了如何评论Workfront对象以及如何更新项目、任务和问题。 有关对目标进行注释的信息，请参阅 [在Adobe Workfront目标中管理目标注释](../../workfront-goals/goal-management/manage-goal-comments.md). 您必须拥有其他许可证才能访问Workfront目标。


您可以从Workfront的以下区域向项目、任务和问题添加更新：

* 从Workfront对象，在更新部分
* 从主页区域（用于任务和问题）
* 从“摘要”面板中的对象列表（用于任务和问题）
* 从时间表（用于任务和问题）

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
您必须具有以下权限才能执行本文中的步骤：

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
   <td> <p>对于问题和文档，请求或更高版本；对于所有其他对象，审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>查看或编辑更新所在对象的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>查看对对象的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 向工作项添加更新

<!--drafted for the commenting experience - change the NOTE at the top of the following section with every new release to other objects -->

向工作项添加更新会因更新部分的版本以及您选择的对象而异。

### 在当前更新分区中为工作项添加更新

>[!NOTE]
>
>以下功能适用于除目标和信息卡之外的所有对象。 您必须拥有其他许可证才能访问Workfront目标。 有关对目标进行注释的信息，请参阅 [在Adobe Workfront目标中管理目标注释](../../workfront-goals/goal-management/manage-goal-comments.md).
>
>在信息卡上启用“注释”和“系统活动”部分时，您可以在“信息卡”区域中添加和查看信息卡的更新。 有关更多信息，请参阅 [向展示板添加临时信息卡](../../agile/get-started-with-boards/add-card-to-board.md).

1. 转到要为其提供更新的工作项（如项目、任务或问题）。
1. 单击 **更新** 部分。
1. 单击 **开始新的更新，** 然后键入您的更新。
1. （可选）使用富文本或在更新中添加表情符号、链接或图像来增强内容。 欲了解更多信息，请参见 [在Workfront更新中使用富文本](#use-rich-text-in-a-workfront-update) 章节
1. （可选）更新有关工作项的以下任何信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>通知</strong></td> 
      <td>确定必须收到更新通知的用户。 进行更新时，分配给或订阅对象的用户会自动收到通知。<br><p>有关如何将其他人包含在更新中的信息，请参阅 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">为其他人标记更新</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>提交日期</strong></td> 
      <td>在日期选取器中，选择您提交以完成工作项的日期。 有关提交日期的信息，请参见 <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">提交日期概述</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>完成情况</strong></td> 
      <td>为任务或问题选择新条件。 有关选择条件的信息，请参阅 <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">更新任务和问题的条件</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>状态</strong></td> 
      <td>单击当前状态旁边的箭头，然后从下拉菜单中选择所需的状态。 有关设置状态的信息，请参阅 <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">更新任务状态</a>.<p>更新工作项的状态不会自动更改项目的状态。 根据项目的设置方式，您可能必须单独更新项目状态。 有关各种项目更新类型的更多信息，请参阅 <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">选择项目更新类型 </a>.</p><p><b>注释</b>

   当工作项处于未决批准状态时，您无法更改其状态。</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>完成栏</strong></td> 
      <td>（仅在任务中可用）通过将进度条滑动到所需的百分比来指示已完成工作的百分比。 您还可以双击完成栏并输入完成百分比。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>我的公司私有</strong></td> 
      <td> <p>禁用此选项可阻止公司外部的用户查看此更新。</p> 
      <p><b>注释</b></p>
      <p>仅当用户与公司关联时，才会显示此选项。</p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **更新** 将更新添加到Workfront对象。

   >[!NOTE]
   >
   >单击后会显示一个小型弹出窗口，持续七秒 **更新**，允许您在发布更新之前撤消更新并返回编辑窗格。 如果您关闭撤消弹出窗口、等待其消失或导航离开页面，则会发布更新。
   >
   >如果您的Workfront管理员在访问级别选择“从不允许用户删除评论”设置，则无法撤消评论。 有关更多信息，请参阅 [创建和修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. 要回复更新，请参阅 [回复更新](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

### 使用备注测试版体验向工作项添加更新

有关哪些功能可用于新注释体验以及哪些对象的信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. 找到要更新的对象，然后单击其名称以打开该对象的页面。
1. 单击  **更新** （在左侧面板中）。
1. 启用 **评论Beta版** 在“更新”区域的右上角进行切换，然后单击 **同意** 在Beta版协议上。 这会将“更新”区域切换到备注测试版体验。
此 **注释** 选项卡默认处于选中状态。
1. 开始在 **新建评论** 盒子。

   <span class="preview">![](assets/comment-box-empty-unshimmed.png)</span>

   >[!TIP]
   >
   >在完成键入和提交评论之前导航离开更新部分，即使注销并重新登录后，页面上的评论仍会处于草稿模式。 添加到注释中的任何图像也会保存在草稿中。 草稿会保存7天，之后将丢弃它们并且无法恢复。 草稿注释仅对输入它们的用户可见。

1. （可选）要撤消或重做更改，请使用以下快捷键：
   * 按CTRL + Z(Mac按⌘ + z)可撤消更改
   * 按CTRL + Y(Mac按⌘ + y)可重做更改
1. （可选）在 **标记人员或团队** 区域，开始键入要包含在此评论中的用户或团队的名称或电子邮件，然后在此评论显示在列表中时将其选定。
1. （可选）要向更新添加富文本格式，请使用 **富文本** 工具栏来增强文本：

   * 粗体
   * 斜体
   * 下划线
   * 链接
   * 项目符号列表
   * 编号列表
   * 添加附件 <!--(mark this parenthesis as draft: ************ this might be renamed to "Add image")-->

   欲了解更多信息，请参见 [在Workfront更新中使用富文本](#use-rich-text-in-a-workfront-update) 章节。 <!--remove this list, above, when we get to parity for Rich Text-->

   >[!TIP]
   >
   >如果另一个用户向您正在更新的同一项目提交评论，则会显示一条带“新”指示器的红线，以告知您较新的评论。
   >
   >指示符仅在提交项目的评论之后显示，而不会在评论仍处于撰写状态时显示。
   >
   >“新”指示符仅在输入新更新的用户以及当前输入更新的用户都使用新注释体验时显示。
   >![](assets/real-time-new-red-indicator-unified-commenting.png)


1. 单击 **提交** 将更新添加到Workfront对象。
1. （可选）要编辑评论，请单击 **更多** 菜单 ![](assets/more-menu.png) 单击“赞”图标右侧，然后单击 **编辑**.
1. 编辑评论中的信息，添加或删除图像，或者删除任何已标记的用户。
您可以在15分钟内通过提交评论来编辑评论。 “已编辑”指示符将添加到更新评论时显示的日期戳的左侧。

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >* 仅当提交原始更新时，才会生成电子邮件通知用户您的更新。 编辑更新后不会生成电子邮件。
   >* 评论旁边的日期戳是原始评论的日期，而不是上次编辑的日期。

1. （可选）单击 **回复** 要回复现有评论，请按照上述步骤4至7操作。 <!--(**************insure this stays accurate***********)-->. 有关回复更新的信息，请参阅 [回复更新](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
1. （有条件和可选）如果其他用户添加了显示在更新部分的可见区域之外的注释，请单击 **视图** 蓝色内部 **新评论横幅** 在屏幕底部显示这些注释。

   ![](assets/blue-new-comments-banner-with-view-button.png)

   屏幕底部会显示其他注释。

   >[!NOTE]
   >
   >   “新注释”指示器和“查看”按钮仅在进入新更新的用户以及当前查看更新分区的用户都使用新注释体验时显示。


1. （可选）单击 **点赞** 图标![](assets/like-icon.png). 图标会随喜欢的数量而更新。
1. （有条件，可选）如果在注释中包括了其他人员，请单击更新中包括的成员数，以显示与所输入的注释共享的实体列表。

   ![](assets/members-icons-expanded-unshimmed.png)
1. （可选）单击 **系统活动** 选项卡以查看系统记录的更新。 更新对象或其任何子对象时，Workfront会生成有关该更新的注释，并将其显示在“系统活动”选项卡中。

   有关详细信息，请参阅 [更新部分概述](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >您无法将注释添加到系统更新。


## 在Workfront更新中使用富文本{#use-rich-text-in-a-workfront-update}

<!--remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.-->

>[!NOTE]
>
>富文本工具栏中的某些选项可能不适用于注释测试版体验。

您可以使用富文本或向其添加各种项目（如表情符号、链接或图像）来增强更新。

1. 转到更新区域并开始键入评论。
1. （可选）要向更新添加富文本格式，请使用 **富文本** 工具栏。

   | **属性** | **工具栏按钮** | **Mac快捷键** | **Windows快捷键** |
   |---|---|---|---|
   | 粗体 | ![mceclip10.png](assets/mceclip10.png) | ⌘+b | Ctrl+B |
   | 斜体 | ![mceclip9.png](assets/mceclip9.png) | ⌘+i | Ctrl+I |
   | 下划线 | ![mceclip8.png](assets/mceclip8.png) | ⌘+u | Ctrl+U |
   | 超链接 | ![mceclip7.png](assets/mceclip7.png) | <br>要打开“创建链接”或“添加链接”框，请执行以下操作：⌘+K</br> <br>在备注测试版体验中，将链接粘贴到所选文本上： ⌘+V</br> | <br>要打开“创建链接”或“添加链接”框，请执行以下操作：Ctrl+K</br> <br>在备注测试版体验中，将链接粘贴到所选文本上：Ctrl+V</br> |
   | 项目符号列表 | ![mceclip6.png](assets/mceclip6.png) | ⌘+Shift+8 | Ctrl+Shift+8 |
   | 编号列表 | ![mceclip5.png](assets/mceclip5.png) | ⌘+Shift+7 | Ctrl+Shift+7 |
   | 块引用 | ![](assets/block-quote-icon-large.png) | ⌘+Shift+9 | Ctrl+Shift+9 |

   要停止设置文本格式，请取消选择 **富文本** 工具栏。

   <!-- in the table above: take "Create Links" verbiage from the hyperlink when the old commenting is removed and the commenting beta is the only way to comment-->

   >[!NOTE]
   >
   >* 用户收到的任何包含您更新的电子邮件通知中也会显示格式。
   >* 在“更新”选项卡中查看更新时，应用于电子邮件中更新的富文本格式不会显示在更新上。
   >* 如果您的组织将Workfront与Internet Explorer结合使用，则粘贴到更新中的任何格式化文本都将丢失其富文本格式并显示为纯文本。 您可以使用“富文本”工具栏上的属性来重新设置文本格式。
   >* 富文本格式不适用于在时间表区域中所做的更新，也不适用于在报表中查看的注释和上一个条件对象。

1. （可选）如果要包含来自先前更新或其他来源的文本，并将其与您自己的更新区分开来，您可以将其标记为“块引用”。 单击 **块引用** 图标 ![](assets/block-quote-small.png) 并键入要引述的文本。 带引号的文本以垂直灰色线标记显示。 单击 **块引用** 图标，以返回正常格式。

   ![](assets/block-quote-marked-350x144.png)

1. （可选）将表情符号添加到您的更新中。

   >[!NOTE]
   >
   >* Workfront不会将标点符号表情符号（例如：）替换为表情符号。
   >* 表情符号不适用于时间表区域中所做的更新，也不适用于报告中查看的注释和上一个条件对象。
   >* Workfront中的表情符号功能利用Unicode字符，因此，仅在支持Unicode代码点的浏览器和操作系统上显示。 平台、浏览器或操作系统版本与您的版本不同的用户可能无法访问相同的表情符号。
   >* 不支持的emoji由黑白框表示。
   >* Windows 7仅支持黑白表情符号。
   >* 在更新区域查看时，应用到通过电子邮件进行的更新的表情符号不会显示在更新上。

1. （可选）要添加指向其他信息源的URL链接，请执行以下操作：

   1. 单击更新中要插入链接的位置。
   1. 在 **富文本** 工具栏上，单击 **超链接** 图标 ![](assets/link-icon.png).

   1. 在 **创建链接** 框，位于下 **URL**，键入或粘贴要链接到的源的URL。

   1. 下 **要显示的文本**，键入或粘贴链接文本。
   1. 单击&#x200B;**保存**。

1. （可选）要将图像附加到更新，请根据您使用的环境执行以下操作之一：

   * 单击 **图像** 图标 ![](assets/addimageicon-35x32.png) 使用当前的更新体验时，浏览到计算机上的图像或将图像拖到更新区域中

   或

   单击 **添加附件** 图标 ![](assets/add-image-paperclip-icon.png) 使用评论Beta版体验时，和浏览到计算机上的图像。 <!--the name of the icon and the icon for it might change-->

   >[!NOTE]
   >
   >* 您的Workfront管理员必须在Workfront界面区域的更新馈送首选项部分启用添加图像功能，然后才能看到图像或添加附件图标。 有关信息，请参阅 [配置用户更新的首选项](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
   >* 最大图像文件大小为7 MB。 支持的图像文件类型为.jpg、.gif和.png。
   >* 可以从对象的“更新”部分访问图像，并且这些图像也可在文档区域中使用。
   >* 您可以发送包含图像但不包含文本的更新。
   >* 删除包含图像的评论时，根据您选择的体验，会出现以下情况：
   >
   >     * 在当前备注体验中，图像保留在文档区域中，但在更新部分中不再可见。
   >     * 在新的注释体验中，图像会从更新部分以及文档区域中删除。 编辑评论和删除图像时，图像也会从“文档”区域删除。
   >* 当有人从“文档”区域删除附加到评论的图像时，该图像也会从评论中删除。

1. 单击 **更新**  或 **提交**，使用评论Beta体验时。


## 复制更新信息

有几种方法可以复制更新。 复制链接后，您可以与其他人共享该链接，以将他们定向到更新。

根据您使用的注释体验，复制更新会有所不同。

### 复制当前评论体验中的更新

* [复制更新](#copy-the-update)
* [复制跟帖链接](#copy-the-thread-link)
* [复制更新链接](#copy-the-update-link)

#### 复制更新 {#copy-the-update}

此选项将文本从特定更新复制到剪贴板。

1. 转到要复制的更新或回复。
1. 单击 **更多** 菜单，然后单击 **复制正文文本**.

   ![选择复制正文文本](assets/update-stream-copy-body-text-350x152.png)

#### 复制跟帖链接 {#copy-the-thread-link}

此选项将完整的线程链接复制到剪贴板，以便您可以与其他用户共享线程。

1. 转到要复制的更新线程。

1. 单击 **更多** 菜单，然后单击 **复制跟帖链接**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

#### 复制更新链接 {#copy-the-update-link}

此选项将特定的更新链接复制到剪贴板。 当您共享更新链接时，关注该链接的用户会看到更新周围的边框。

1. 转到要复制的更新或回复。
1. 单击 **更多** 单个更新旁边的菜单，然后单击 **复制更新链接**.

   ![](assets/update-stream-reply-menu-marked-350x182.png)


### 复制新评论体验中的更新

有关哪些功能可用于新注释体验以及哪些对象的信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--when we remove and deprecate the legacy stream, add screen shots in the secitons below-->

* [复制链接](#copy-link)
* [复制正文文本](#copy-body-text)

#### 复制链接

此选项将注释或线程链接复制到剪贴板，以便您可以与其他用户共享注释或整个线程。

1. 转到要复制其链接的更新。

1. 单击 **更多** 菜单，然后单击 **复制链接**.

#### 复制正文文本

此选项将文本从特定更新复制到剪贴板。

1. 转到要复制的更新或回复。
1. 单击 **更多** 菜单，然后单击 **复制正文文本**.

## 删除更新或回复

根据Workfront管理员赋予您的访问权限，您也许能够删除在对象的“更新”选项卡上添加的更新。 有关更多信息，请参阅 [创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) 在文章中 [创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

任何Workfront用户(包括Workfront管理员)都无法删除其他用户所做的更新。 但是，如果用户的访问级别允许他们删除自己的更新，Workfront管理员可以以该用户身份登录并删除他们所做的更新。 有关更多信息，请参阅 [创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) 和 [以其他用户身份登录](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. 转到要删除的更新或回复。
1. 单击 **更多** 菜单，然后单击要删除的更新或回复旁边的 **删除**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. 在显示的消息中，单击 **确认** 或单击 **删除**，使用评论Beta体验时。

   >[!NOTE]
   >
   >删除具有附加图像的更新会同时删除注释和图像。 欲了解更多信息，请参见 [在Workfront更新中使用富文本](#use-rich-text-in-a-workfront-update) 章节。

   当您删除的评论具有与其关联的回复时，将显示删除评论的指示以及删除评论的用户的名称。

   ![](assets/removed-comment-indicator-new-experience.png)

   使用备注测试版体验时，已删除的备注会立即从Workfront中删除。 使用“更新”部分的用户会看到评论被其他用户实时删除。

   <!--when we remove the beta, take out the first part of the sentence above about only when commenting in beta experience. Leave the rest though-->

## 在时间表上添加更新

1. 转到要更新的“时间表”。
1. 单击时间表以将其打开。
1. 在时间表底部，单击 **包括评论**.
1. 在时间表底部显示的框中，键入更新。

   ![timesheet_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. （视情况而定）要保存更新而不提交时间表以供审批，请单击 **保存供以后使用**.

   或

   要保存更新并提交时间表以供审批，请单击 **提交以供审批**.

   或

   如果您的时间表未由批准者设置，请单击 **保存并关闭工时表** 以保存您的更新。

## 启用或禁用系统更新

<!--remove the preview tag with 23.2 production, but keep the note till we remove Beta and it becomed the only exprience: -->

>[!NOTE]
>
>使用Beta版评论体验时，无法禁用系统更新。
>此部分中的信息仅引用了当前更新部分中可用的功能。
>有关Beta版系统更新的更多信息，请参阅 [更新部分概述](../updating-work-items-and-viewing-updates/updates-tab-overview.md).


Workfront对象的“更新”部分显示两种类型的信息：

* **用户更新：** 用户更新是您和系统中的其他用户输入的注释。

  ![](assets/user-update-cl-350x277.png)

* **系统更新：** 系统更新记录删除资产、添加或删除版本、附加或删除审批请求，以及对对象上的文档所做的任何编辑或更改。

  ![](assets/system-updates-cl-350x277.png)

根据您的Workfront许可证，默认情况下可能会启用系统更新。 Workfront管理员可以确定系统更新中跟踪的内容，如中所述 [系统跟踪的更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). 您还可以过滤掉系统更新或活动，以便只看到所有对象的用户更新。

有关用户更新和系统更新之间差异的更多信息，请参阅 [系统跟踪的更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

要启用或禁用系统更新：

1. 单击 **更新** 选项卡。
1. 单击 **显示系统更新** 向左（禁用）或向右（启用）滑动交换机。

   ![](assets/show-system-updates-qs-350x55.png)

   该选项在Workfront中的所有对象中都是持久的，并且会保留在您选择的位置，即使您从Workfront注销也是如此。

