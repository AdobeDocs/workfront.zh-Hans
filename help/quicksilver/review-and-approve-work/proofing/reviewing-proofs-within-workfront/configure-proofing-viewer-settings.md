---
product-area: documents;setup
navigation-topic: review-a-proof
title: 配置校对查看器设置
description: 您可以为Web校样查看器和桌面校样查看器 — 编辑我配置以下设置。
author: Courtney
feature: Digital Content and Documents
exl-id: 3993cd67-90a9-4d7e-bbc0-7b9bd1057f54
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1412'
ht-degree: 0%

---

# 配置校对查看器设置

您可以为Web校样查看器和桌面校样查看器配置以下设置：

* 注释标记和针脚是否显示在校样上。
* 标记工具是显示在校样查看器的顶部还是下拉菜单中。
* 作为已打开校样的审阅人，您会收到哪些电子邮件通知。

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For comparative information about the Web Proofing Viewer and the Desktop Proofing Viewer, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p>
-->

您可以为桌面校对查看器配置以下设置：

* 您希望如何在查看器中打开网站内容中的链接。

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.</li>
  -->

* 单击设置为在新浏览器选项卡或窗口中打开的链接时会发生什么情况。
* 清除可能与您正在查看的校样一起保存的缓存数据，以便使弹出窗口（浏览器缓存数据可能会阻止）等内容能够显示在查看器中。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>经理或更高级别</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 配置校对查看器设置

要配置校对查看器设置，请执行以下操作：

1. 通过以下方式之一打开Web校样查看器或桌面校样查看器：

   * 如果在Adobe Workfront中进行校样，请转到包含要查看的校样的文档列表，将鼠标悬停在该文档上，然后单击 **打开校样**.
   * 如果您使用Workfront校样，请单击 **转到校样** 图标（在功能板或视图列表中）进行校样 ![](assets/go-to-proof-blue-icon.png).

1. 如果未显示左侧工具栏，请单击 **菜单** 图标（位于Web校样查看器的左上角）。

   ![](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 在左侧工具栏中，单击 **设置** 图标 ![](assets/settings-icon-in-pv.png).

1. 配置以下任一项 **设置** 显示。

   可用的设置可能因您打开的校样类型而异。

   * **显示标记** （始终在Web校样查看器和桌面校样查看器中可用）：这些是审阅人在使用标记工具时添加到校样的注释标记。 如果禁用这些注释，则在单击注释列表中的注释时，仍可以看到这些注释。

      此设置会影响您打开的所有校样。

   * **显示针脚** （始终在Web校样查看器和桌面校样查看器中可用）：这些是审阅人在使用标记工具时添加到校样的编号针脚。 它们指示审阅人添加注释的位置和顺序。 如果禁用这些注释，则在单击注释列表中的注释时，仍可以看到这些注释。

      此设置会影响您打开的所有校样。

   * **使用扩展的标记工具** （始终在Web校样查看器和桌面校样查看器中可用）：默认情况下，校样查看器的顶部会显示标记工具选项。 您可以将它们配置为显示在垂直菜单中，该垂直菜单仅在单击时才打开。

      此设置对您打开的所有校样有效。

   * **向我发送有关** （始终在Web校样查看器和桌面校样查看器中可用）：单击下面的选项之一。 此设置仅影响您打开的校样。 有关更多信息，请参阅 [校样注释和决策通知概述](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">所有活动</td> 
        <td>每当校样有任何活动（如新评论、回复或决定）时，Workfront都会向审阅人发送电子邮件。 <p>对于管理校对流程的人员而言，这是一个非常好的选项，因为它允许他们查看所发生的活动。 </p><p>用户不会收到有关其自身活动的电子邮件警报。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">对我的评论的答复</td> 
        <td>仅当某人明确回复了其评论时，才会向审阅人发送电子邮件（这不包括他们自己对评论的回复）。 这意味着，如果校样上的某人做出新评论，则不会通知审阅人。<p>建议您的客户在验证时使用此设置，以便他们不会收到关于验证的任何其他评论的通知，并且仅会收到对其自己评论的回复通知。</p><p>虽然具有此电子邮件警报设置的审阅人不会收到有关其他新注释的通知，但审阅人仍然可以在校样查看器中查看校样上的所有注释。</p><p>有关注释的信息，请参阅 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">查看和回复校样评论</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">决策</td> 
        <td>Workfront仅在某人做出决策时向审阅人发送电子邮件。<p>这对于管理审批流程的人员（例如项目经理）和需要监控校样进度并查看哪些用户做出了决策的人员非常有用。</p><p>在提交您的决定时，您不会收到有关自己决定的通知，除非您选择了电子邮件确认选项。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">最终决定</td> 
        <td>Workfront在校样的最后审批者做出决定后发送电子邮件。<p>此警报通常由设计人员使用，他们通常不需要参加实际的审阅讨论。 当做出最终决策时，系统会通知设计人员，然后可以对任何必要的更改采取操作。</p><p>此警报对于只有在审核过程完成后才需要通知的部门负责人也非常有用。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">每小时概要</td> 
        <td>Workfront每小时向审阅人发送一封电子邮件，其中包含该小时内发生的所有评论、回复和决策的摘要。<p>仅当您自己的活动之外的其他活动在过去一小时内发生时，才会发送电子邮件。 </p><p>此警报是查看项目概述的好方法。</p><p>本摘要的一个用例示例是高级审阅人，他需要项目概述，但不需要立即收到校样上所有活动的通知。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">每日摘要</td> 
        <td>Workfront会发送一封电子邮件，其中列出的所有评论、回复和决策仅在您自己的活动之外的几天内列出。<p>此警报是您查看项目摘要的好方法，不会在一天中出现多次更新。</p><p>此摘要的一个示例用例是部门负责人，他希望监控项目的整体进度。</p><p>有关更多信息，请参阅 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理校样注释和决策通知</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">无电子邮件</td> 
        <td>Workfront不会发送任何电子邮件警报。<br>对于仅出于参考目的而添加到校样且无需接收任何更改通知的人员，此功能非常有用。<p>系统默认为“每日摘要”（也称为“未设置”）。 如果您或您的审阅人没有进行任何其他更改，则所有校样都具有此设置。</p></td> 
       </tr> 
      </tbody> 
     </table>

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Use desktop app as default</strong>: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see in the article . For comparative information about the two viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </li>   
     -->

   * **在校样中单击超链接时** （仅在桌面校对查看器中可用）：选择一个选项，以指定在单击设置为在新浏览器选项卡或窗口中打开的链接时，桌面校对查看器中发生的情况。

      此设置对您打开的所有交互式校样有效。

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">在校对查看器中打开</td> 
        <td>链接始终在桌面校样查看器中打开，您可以校样链接的内容。 </td> 
       </tr> 
       <tr> 
        <td role="rowheader">在浏览器中打开</td> 
        <td>链接始终在浏览器中打开，而不是在校样查看器中打开。 您无法校样链接的内容。</td> 
       </tr> 
       <tr> 
        <td role="rowheader">每次都问我</td> 
        <td> <p>每次要在桌面校对查看器中还是浏览器中打开链接时，系统都会提示您。 如果在桌面校对查看器中打开链接，则可以校样链接的内容。 如果您在浏览器中打开链接，则无法校样链接的内容。</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_alwaysask.png" style="width: 350;height: 243;"> </p> <p>此设置仅影响您打开的校样。</p> </td> 
       </tr> 
      </tbody> 
     </table>

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Background color</strong> (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.</li>   
     -->

   * **清除缓存**:清除可能使用您正在查看的交互式校样保存的浏览器缓存数据。 这样，诸如弹出窗口（浏览器缓存数据可能会阻止）之类的内容便可在桌面校样查看器中显示。

      被清除的数据包括HTTP缓存（例如，在下一页刷新后要重复使用的图像）和Web存储数据缓存（例如标识用户的Cookie和数据）。

      此设置仅影响您打开的校样。
