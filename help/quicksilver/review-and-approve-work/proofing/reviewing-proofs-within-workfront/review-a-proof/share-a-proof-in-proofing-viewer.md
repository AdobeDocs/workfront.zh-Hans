---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 从验证查看者共享验证
description: 如果校对所有者或创建者启用了共享，则可以从校对查看者共享校对。
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 0%

---

# 从验证查看者共享验证

如果校对所有者或创建者启用了共享，则可以从校对查看者共享校对。

>[!IMPORTANT]
>
>必须启用允许通过公共URL或嵌入代码共享验证设置。

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
   <td> <p>编辑对文档的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、角色或验证权限配置文件，请联系您的Workfront或Workfront Proof管理员。

+++

## 共享URL

如果所有者已将验证配置为共享，则可以通过URL共享验证。 校对所有者可随时更新共享设置。 有关详细信息，请参阅[编辑校对设置](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md)。

1. 如果未显示左侧图标菜单，请单击验证查看器左上角的&#x200B;**菜单**&#x200B;图标。

   ![菜单图标](assets/menu-icon-in-proofing-viewer-350x188.png)

1. 在校对查看器的左侧图标菜单中，单击&#x200B;**共享**&#x200B;图标。

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. 在显示的&#x200B;**共享校对**&#x200B;选项中，确保选中&#x200B;**获取可共享链接**。

1.  执行以下任一操作：

   * 要将链接复制到剪贴板，请单击&#x200B;**复制链接**。

     您现在可以通过第三方工具（如聊天或电子邮件应用程序）分发链接。

   * 要通过电子邮件直接从Adobe Workfront发送链接，请执行以下操作：

      1. 在&#x200B;**或指向**&#x200B;的电子邮件链接字段中，开始键入并选择收件人的姓名。 或者指定要与之共享的外部用户的电子邮件地址。

         >[!NOTE]
         >
         >如果在共享验证时看到别名电子邮件，则在存在相应的别名电子邮件时，不要通过输入原始电子邮件来创建新的访客用户。

      1. 从以下选项中选择：

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">发送公共链接</td>
            <td><p>电子邮件通知中包含一个按钮，可将用户定向到他们正在使用的验证查看者中的验证，并授予查看权限。</p><p>如果<strong>通过公共URL或嵌入代码订阅验证</strong>对验证关闭，则用户可以使用其Workfront登录凭据登录以向验证添加评论。 如果启用，则提供其电子邮件地址和名称（无需密码）的任何人都可以签名并向验证中添加注释。</p></td>
           </tr>
           <tr>
            <td role="rowheader">发送下载链接</td>
            <td>电子邮件通知中包含一个按钮，可将用户定向到下载页面，其中提供文件详细信息、文件名和文件大小，并内联显示文件。 用户可以单击下载页面中的下载链接以下载文件。</td>
           </tr>
           <tr>
            <td role="rowheader">添加自定义消息</td>
            <td>允许您为电子邮件通知指定自定义主题和正文。</td>
           </tr>
          </tbody>
         </table>

      1. 单击&#x200B;**发送**。

         收件人会收到电子邮件通知，其中包含有关验证和您选择包含的按钮的信息。

         ![](assets/proof-share-email-350x87.png)

## 共享嵌入代码

如果验证所有者为此配置了验证，则您可以通过嵌入代码共享验证。

要通过嵌入代码共享验证，请执行以下操作：

1. 在验证查看器左侧的工具栏中，单击&#x200B;**共享**&#x200B;图标。

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. 在显示的&#x200B;**共享验证**&#x200B;选项中，单击&#x200B;**获取嵌入代码**，然后单击&#x200B;**复制**。

## 通过添加用户来共享验证

如果您具有以下任何权限，您可以在查看验证时将用户添加到验证：

* 主管或管理员权限
* 经理权限且您是验证创建者或所有者
* 具有作者或审查方验证角色的经理权限

如果验证具有自动工作流，则可以将用户添加到单个阶段。 有关详细信息，请参阅[自动化工作流概述](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)。

默认情况下，您添加到验证中的用户：

* 接收包含证明链接的电子邮件通知。
* 可以根据[批准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)中所述，从主页区域对验证做出批准决定。
* 无需启用验证即可查看验证。

如果启用了自动工作流，并且您向验证中添加了未在Workfront中启用验证的用户，则会在自动工作流中创建一个新阶段。 首次查看验证时，您添加的用户会自动添加到此新阶段。 有关详细信息，请参阅[自动化工作流概述](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)。

要与个人用户共享验证，请执行以下操作：

1. 在验证查看器左侧的工具栏中，单击&#x200B;**共享**&#x200B;图标。

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. 单击左侧列表中的&#x200B;**添加收件人**。
1. 在&#x200B;**新验证收件人**&#x200B;下，开始键入要与其共享验证的用户名，然后在该名称出现在下拉列表中时单击该名称。
1. （可选）更改人员姓名右侧的任何审阅人选项：

   * **验证角色**：有关详细信息，请参阅[在Workfront Proof中管理验证角色](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)。

   * **阶段**： （仅当验证具有自动工作流时可用）。 有关更多信息，请参阅  [自动工作流暂存概述](../../../../review-and-approve-work/proofing/proofing-overview/stages.md)。

   * **电子邮件提醒**：选择以下选项之一，以指定在验证活动时如何通知用户。

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
        <td>只有当某人明确回复其评论时，才会向审阅人发送电子邮件（这不包括他们自己对评论的回复）。 这意味着如果验证中的某人发表新评论，则不会通知查看者。<p>建议向验证上的客户使用此设置，以便他们不会收到有关验证的任何其他评论的通知，并且只会在回复他们自己的评论时收到通知。</p><p>虽然具有此电子邮件警报设置的查看者不会收到有关其他新评论的通知，但他们仍然可以在验证查看器中查看有关验证的所有评论。</p><p>有关评论的信息，请参阅<a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">查看和回复校对评论</a>。</p></td> 
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
        <td>Workfront会发送一封电子邮件，其中包含仅在有您自己的活动之外的活动时列出的所有评论、回复和决策。<p>此警报非常适合用于查看项目摘要，而不会在一天之内出现多次更新。</p><p>此摘要的示例用例是一个部门领导，他想要监控项目的整体进度。</p><p>有关详细信息，请参阅<a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理证明评论和决策的通知</a>。</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">无电子邮件</td> 
        <td>Workfront不发送任何电子邮件警报。<br>这对于仅供参考而添加到验证中且不需要收到任何更改通知的人员非常有用。<p>系统默认值为“Daily summary（每日摘要）”(也视为“Not Set（未设置）”)。 如果您或您的审阅人没有进行任何其他更改，则您的所有验证均具有此设置。</p></td> 
       </tr> 
      </tbody> 
     </table>

1. （可选）重复前两个步骤以将多个用户添加到验证。 
1. （可选）为审阅人设置&#x200B;**截止日期**（仅在验证没有自动工作流时可用）。
1. （可选）选择&#x200B;**向新收件人发送电子邮件通知**，告知他们您已将其添加到验证中。
1. 完成向验证添加用户后，单击&#x200B;**完成。**
