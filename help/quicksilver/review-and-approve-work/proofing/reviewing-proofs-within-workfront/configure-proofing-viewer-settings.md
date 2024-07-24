---
product-area: documents;setup
navigation-topic: review-a-proof
title: 配置校对查看器设置
description: 您可以配置Web验证查看器和桌面验证查看器的设置。
author: Courtney
feature: Digital Content and Documents
exl-id: 3993cd67-90a9-4d7e-bbc0-7b9bd1057f54
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '1417'
ht-degree: 0%

---

# 配置校对查看器设置

您可以为Web验证查看器和桌面验证查看器配置以下设置：

* 注释标记和图钉是否显示在验证上。
* 标记工具是显示在校样查看器的顶部还是下拉菜单中。
* 您作为查看者会在打开的验证中收到哪些电子邮件通知。

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For comparative information about the Web Proofing Viewer and the Desktop Proofing Viewer, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p>
-->

您可以为桌面校对查看器配置以下设置：

* 希望在查看器中打开网站内容中的链接的方式。

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.</li>
  -->

* 当您单击设置为在新的浏览器选项卡或窗口中打开的链接时，会发生什么情况。
* 清除可能随您查看的验证一起保存的缓存数据，以使弹出窗口（可由浏览器缓存数据阻止）等内容显示在查看器中。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：专业版或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关使用其他计划进行验证访问的更多信息，请参阅<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、角色或验证权限配置文件，请联系您的Workfront或Workfront Proof管理员。

+++

## 配置校对查看器设置

要配置校对查看器设置，请执行以下操作：

1. 通过以下方式之一打开Web验证查看器或桌面验证查看器：

   * 如果您在Adobe Workfront中验证，请转到包含要查看的验证的文档列表，将鼠标悬停在文档上，然后单击&#x200B;**打开验证**。
   * 如果使用Workfront Proof，请单击仪表板或视图列表![](assets/go-to-proof-blue-icon.png)中验证的&#x200B;**转到验证**&#x200B;图标。

1. 如果未显示左侧工具栏，请单击Web验证查看器左上角的&#x200B;**菜单**&#x200B;图标。

   ![](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 在左侧工具栏中，单击&#x200B;**设置**&#x200B;图标![](assets/settings-icon-in-pv.png)。

1. 配置以下任何显示的&#x200B;**设置**。

   可用的设置可能因您打开的校样类型而异。

   * **显示标记** （始终在Web验证查看器和桌面验证查看器中可用）：这些是查看者在使用标记工具时添加到验证的注释标记。 如果禁用这些注释，则单击注释列表中的注释时，仍可以看到这些注释。

     此设置会影响您打开的所有校样。

   * **显示pin**（始终在Web验证查看器和桌面验证查看器中可用）：这些是查看者在使用标记工具时添加到验证中的编号的pin。 它们指示审阅人添加注释的位置和顺序。 如果禁用这些注释，则单击注释列表中的注释时，仍可以看到这些注释。

     此设置会影响您打开的所有校样。

   * **使用扩展的标记工具** （始终在Web验证查看器和桌面验证查看器中可用）：默认情况下，标记工具选项显示在验证查看器的顶部。 您可以将它们配置为在垂直菜单中显示，此垂直菜单仅在单击时打开。

     此设置对您打开的所有验证有效。

   * **向我发送有关**&#x200B;的电子邮件通知（始终在Web验证查看器和桌面验证查看器中可用）：单击以下选项之一。 此设置仅影响您已打开的校对。 有关详细信息，请参阅[校对评论和决策概述](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md)的通知。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">所有活动</td> 
        <td>每次验证上存在任何活动（如新评论、回复或决策）时，Workfront都会向查看者发送电子邮件。 <p>这是管理校对流程的人员的最佳选项，因为它允许他们查看活动发生的情况。 </p><p>用户不会收到有关其活动的电子邮件警报。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">回复我的评论</td> 
        <td>只有当某人明确回复其评论时，才会向审阅人发送电子邮件（这不包括他们自己对评论的回复）。 这意味着如果验证中的某人发表新评论，则不会通知查看者。<p>建议向验证上的客户使用此设置，以便他们不会收到有关验证的任何其他评论的通知，并且只会在回复他们自己的评论时收到通知。</p><p>虽然具有此电子邮件警报设置的查看者不会收到有关其他新评论的通知，但他们仍然可以在验证查看器中查看有关验证的所有评论。</p><p>有关评论的信息，请参阅<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">查看和回复校对评论</a>。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">决策</td> 
        <td>Workfront仅在有人做出决定时向审核者发送电子邮件。<p>这对于管理审批流程的人员（如项目经理）非常有用，他们需要监控验证进度并查看哪些用户做出了决定。</p><p>除非您在提交决策时选择了电子邮件确认选项，否则不会通知您自己的决策。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">最终决定</td> 
        <td>当验证的最后一位审批者做出决定时，Workfront会发送电子邮件。<p>此警报通常由设计人员使用，他们通常不需要参加实际的审核讨论。 当做出最终决定时，设计人员会收到通知，然后可以对任何必要的更改执行操作。</p><p>此警报对于需要仅在审核流程完成后才收到通知的部门领导也很有用。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">每小时摘要</td> 
        <td>Workfront每小时会向查看者发送一封电子邮件，其中包含该小时发生的所有评论、回复和决策的摘要。<p>仅当过去一小时内发生除您自己的活动以外的活动时，才会发送电子邮件。 </p><p>此警报非常适合用于查看项目概述。</p><p>此摘要的示例用例是高级查看者，他需要项目概述，但不需要立即收到有关验证中所有活动的通知。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">每日摘要</td> 
        <td>Workfront会发送一封电子邮件，其中包含仅在有您自己的活动之外的活动时列出的所有评论、回复和决策。<p>此警报非常适合用于查看项目摘要，而不会在一天之内出现多次更新。</p><p>此摘要的示例用例是一个部门领导，他想要监控项目的整体进度。</p><p>有关详细信息，请参阅<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理证明评论和决策的通知</a>。</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">无电子邮件</td> 
        <td>Workfront不发送任何电子邮件警报。<br>这对于仅供参考而添加到验证中且不需要收到任何更改通知的人员非常有用。<p>系统默认值为“Daily summary（每日摘要）”(也视为“Not Set（未设置）”)。 如果您或您的审阅人没有进行任何其他更改，则您的所有验证均具有此设置。</p></td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Use desktop app as default</strong>: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see in the article . For comparative information about the two viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </li>   
     -->

   * **在验证中单击超链接时**（仅在桌面验证查看器中可用）：选择一个选项，以指定当您单击设置为在新浏览器选项卡或窗口中打开的链接时，在桌面验证查看器中发生的情况。

     此设置对您打开的所有交互式验证有效。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">在验证查看器中打开</td> 
        <td>链接始终在桌面校对查看器中打开，您可以校对链接的内容。 </td> 
       </tr> 
       <tr> 
        <td role="rowheader">在浏览器中打开</td> 
        <td>链接始终在浏览器中打开，而不是在验证查看器中打开。 您无法校对链接的内容。</td> 
       </tr> 
       <tr> 
        <td role="rowheader">每次都询问我</td> 
        <td> <p>每次要在桌面验证查看器或浏览器中打开链接时，系统都会提示您进行选择。 如果在桌面校对查看器中打开链接，则可以校对链接的内容。 如果您在浏览器中打开链接，则无法验证链接的内容。</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_alwaysask.png" style="width: 350;height: 243;"> </p> <p>此设置仅影响您已打开的校对。</p> </td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Background color</strong> (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.</li>   
     -->

   * **清除缓存**：清除可能随您正在查看的交互式验证一起保存的浏览器缓存数据。 这样可使弹出窗口（可由浏览器缓存数据阻止）等内容显示在桌面验证查看器中。

     清除的数据包括HTTP缓存（如要在下一页刷新后重用的图像）和Web存储数据缓存（如Cookie和标识用户的数据）。

     此设置仅影响您已打开的校对。
