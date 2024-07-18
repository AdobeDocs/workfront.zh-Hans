---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 管理验证评论和决策的通知
description: 处理验证时，无论您是Adobe Workfront用户还是外部协作者，都可以指定您想要接收哪些有关对验证所做的评论和决策的电子邮件通知。 有关更多信息，请参阅验证评论和决策通知概述。
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '978'
ht-degree: 1%

---

# 管理验证评论和决策的通知

处理验证时，无论您是Adobe Workfront用户还是外部协作者，都可以指定您想要接收哪些有关对验证所做的评论和决策的电子邮件通知。 有关详细信息，请参阅[校对评论和决策概述](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md)的通知。

>[!NOTE]
>
>这些通知不同于您可以收到的有关审阅人之间验证流程的电子邮件警报。 它们也不同于您可以在Workfront中配置的电子邮件警报设置。 

## 访问要求

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

## 管理验证评论和决策的通知

1. 打开要配置接收通知的校对。
1. 如果未显示左侧工具栏，请单击Web验证查看器左上角的&#x200B;**菜单**&#x200B;图标。

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 在左侧工具栏中，单击&#x200B;**设置**&#x200B;图标。 ![Settings_icon.png](assets/settings-icon.png)

1. 在&#x200B;**向我发送有关**&#x200B;的电子邮件通知下，单击验证所需的设置。

   您选择的设置仅对已打开的校样有效。

   系统默认值为&#x200B;**每日摘要**。 如果您或您的审阅人没有进行任何其他更改，则您的所有验证均具有此设置。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">所有活动</td> 
      <td>每次验证上存在任何活动（如新评论、回复或决策）时，都会向查看者发送电子邮件。<br><p>这是管理校对流程的人员的最佳选项，因为它允许他们查看活动发生的情况。 用户不会收到有关其自身活动（例如，评论、回复和作出的决策）的电子邮件警报。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">回复我的评论</td> 
      <td>只有当某人明确回复其评论时，才会向审阅人发送电子邮件（这不包括他们自己对评论的回复）。 这意味着如果验证中的某人发表新评论，则不会通知查看者。<p>建议向验证上的客户使用此设置，以便他们不会收到有关验证的任何其他评论的通知，并且只会在回复他们自己的评论时收到通知。</p><p>虽然具有此电子邮件警报设置的查看者不会收到有关其他新评论的通知，但他们仍然可以在验证查看器中查看有关验证的所有评论。<br></p><p>有关信息，请参阅<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">查看并回复校对备注</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">决策</td> 
      <td>仅当有人做出决定时，才会向审阅人发送电子邮件。<br><p>此电子邮件警报对于管理审批流程的人员（如项目经理）非常有用，因为它允许管理审批流程的人员监控验证进度并查看哪些用户做出了其决策。<br></p><p>除非您在提交决策时选择了电子邮件确认选项，否则不会通知您自己的决策。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">最终决定</td> 
      <td>在对验证做出最终决定时（当验证的最后一个审批者做出决定时），将发送电子邮件。<br><p>此警报通常由设计人员使用，因为设计人员不需要参与实际的审阅讨论。 当做出最终决定时，设计人员会收到通知，然后可以对任何必要的更改执行操作。<br></p><p>此警报对于需要仅在审核流程完成后才收到通知的部门领导也很有用。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">每小时摘要</td> 
      <td>每小时会向查看者发送一封电子邮件，其中包含过去一小时内发生的所有评论、回复和决策的摘要。<br><p>仅当过去一小时内发生除您自己的活动以外的活动时，才会发送电子邮件。 如果其他用户没有活动，则不会发送电子邮件。<br></p><p>此警报非常适合用于查看项目概述。<br></p><p>此摘要的示例用例是高级查看者，他需要项目概述，但不需要立即收到有关验证中所有活动的通知。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">每日摘要</td> 
      <td>（默认设置）：每天都会发送一封电子邮件，其中列出了所有评论、回复和决策。 仅当您的活动之外有活动时，才会发送电子邮件。<br><p>此警报非常适合用于查看项目摘要，而不会在一天之内出现多次更新。<br></p><p>此摘要的示例用例是一个部门领导，他想要监控项目的整体进度。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">无电子邮件</td> 
      <td>不发送电子邮件提醒。<br><p>此设置对于仅出于参考目的添加到验证而无需通知任何更改的人员非常有用。</p><p>注意： <p>此选项仅关闭您可以收到的有关验证评论和决策的电子邮件警报。 它不会关闭您收到的有关验证流程的电子邮件警报，例如新验证或延迟验证电子邮件。 有关有关验证流程的电子邮件警报的更多信息，请参阅以下文章： </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">新验证电子邮件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">新版本电子邮件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">延迟验证电子邮件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">校对已发送电子邮件</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
