---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 管理校样注释和决策通知
description: 在处理校样时(无论您是Adobe Workfront用户还是外部协作者)，您可以指定要接收有关校样的评论和决策的电子邮件通知。 有关更多信息，请参阅校样评论和决策通知概述。
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '983'
ht-degree: 0%

---

# 管理校样注释和决策通知

在处理校样时(无论您是Adobe Workfront用户还是外部协作者)，您可以指定要接收有关校样的评论和决策的电子邮件通知。 有关更多信息，请参阅 [校样注释和决策通知概述](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>这些通知与您收到的有关审阅人校样流程的电子邮件警报不同。 它们也与您在Workfront中配置的电子邮件警报设置不同。 

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

## 管理校样注释和决策通知

1. 打开要配置将收到的通知的校样。
1. 如果未显示左侧工具栏，请单击 **菜单** 图标（位于Web校样查看器的左上角）。

   ![Menu_icon_in_Poofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 在左侧工具栏中，单击 **设置** 图标。 ![Settings_icon.png](assets/settings-icon.png)

1. 在 **向我发送有关**，单击校样所需的设置。

   您选择的设置仅对已打开的校样有效。

   系统默认为 **每日摘要**. 如果您或您的审阅人没有进行任何其他更改，则所有校样都具有此设置。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">所有活动</td> 
      <td>每当校样有任何活动（如新评论、回复或决定）时，都会向审阅人发送电子邮件。<br><p>对于管理校对流程的人员而言，这是一个非常好的选项，因为它允许他们查看所发生的活动。 用户不会收到有关其自身活动的电子邮件警报（例如，评论、回复和做出的决定）。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">对我的评论的答复</td> 
      <td>仅当某人明确回复了其评论时，才会向审阅人发送电子邮件（这不包括他们自己对评论的回复）。 这意味着，如果校样上的某人做出新评论，则不会通知审阅人。<p>建议您的客户在验证时使用此设置，以便他们不会收到关于验证的任何其他评论的通知，并且仅会收到对其自己评论的回复通知。</p><p>虽然具有此电子邮件警报设置的审阅人不会收到有关其他新注释的通知，但审阅人仍然可以在校样查看器中查看校样上的所有注释。<br></p><p>有关信息，请参阅 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">查看和回复校样评论</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">决策</td> 
      <td>只有当某人作出决定时，才会向审阅人发送电子邮件。<br><p>此电子邮件警报对于管理批准流程的人员（例如项目经理）非常有用，因为它允许管理批准流程的人员监控校样进度并查看哪些用户做出了决策。<br></p><p>在提交您的决定时，您不会收到有关自己决定的通知，除非您选择了电子邮件确认选项。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">最终决定</td> 
      <td>当对校样做出最终决策时（当校样的最后审批者做出其决策时），将发送电子邮件。<br><p>此警报通常由设计人员使用，因为设计人员无需参加实际的审阅讨论。 当做出最终决策时，系统会通知设计人员，然后可以对任何必要的更改采取操作。<br></p><p>此警报对于只有在审核过程完成后才需要通知的部门负责人也非常有用。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">每小时概要</td> 
      <td>每小时向审阅人发送一封电子邮件，其中包含在最后一小时中发生的所有评论、回复和决策的摘要。<br><p>仅当您自己的活动之外的其他活动在过去一小时内发生时，才会发送电子邮件。 如果其他用户没有活动，则不会发送电子邮件。<br></p><p>此警报是查看项目概述的好方法。<br></p><p>本摘要的一个用例示例是高级审阅人，他需要项目概述，但不需要立即收到校样上所有活动的通知。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">每日摘要</td> 
      <td>（默认设置）：每天都会发送一封电子邮件，其中列出了所有评论、回复和决策。 仅当您自己的活动之外还有活动时，才会在天内发送电子邮件。<br><p>此警报是您查看项目摘要的好方法，不会在一天中出现多次更新。<br></p><p>此摘要的一个示例用例是部门负责人，他希望监控项目的整体进度。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">无电子邮件</td> 
      <td>不会发送电子邮件警报。<br><p>此设置对于仅出于参考目的而添加到校样，且无需收到任何更改通知的人员非常有用。</p><p>注释: <p>此选项仅关闭您能够收到有关校样评论和决策的电子邮件警报。 它不会关闭您可以收到的有关校样流程的电子邮件警报，例如New Proof或Late Proof电子邮件。 有关校样流程的电子邮件警报的更多信息，请参阅以下文章： </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">新校样电子邮件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">新版本电子邮件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">延迟校样电子邮件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">校样制作的电子邮件</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
