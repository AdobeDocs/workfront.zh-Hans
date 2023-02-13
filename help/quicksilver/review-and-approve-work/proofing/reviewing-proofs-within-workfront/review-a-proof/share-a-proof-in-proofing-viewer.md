---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 从校对查看器共享校样
description: 如果校样所有者或创建者启用了共享，则可以从校样查看器共享校样。
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# 从校对查看器共享校样

如果校样所有者或创建者启用了共享，则可以从校样查看器共享校样。

>[!IMPORTANT]
>
>必须启用允许通过公共URL或嵌入代码共享校样设置。

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
   <td> <p>编辑对文档的访问</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 共享URL

如果所有者配置了校样以进行共享，则可以通过URL共享校样。 校样所有者可以随时更新共享设置。 有关更多信息，请参阅 [编辑校样设置](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. 如果未显示左侧图标菜单，请单击 **菜单** 图标。

   ![](assets/menu-icon-in-proofing-viewer-350x188.png)

1. 在校样查看器的左侧图标菜单中，单击 **共享** 图标。

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. 在 **共享校样** 显示的选项，确保 **获取可共享链接** 中。

1.  执行以下任一操作：

   * 要将链接复制到剪贴板，请单击 **复制链接**.

      您现在可以通过第三方工具（如聊天或电子邮件应用程序）分发链接。

   * 要直接从Adobe Workfront通过电子邮件发送链接，请执行以下操作：

      1. 在 **或通过电子邮件链接至** 字段，开始键入并选择收件人的名称。 或指定要与之共享的外部用户的电子邮件地址。

         >[!NOTE]
         >
         >如果在共享校样时看到别名电子邮件，则如果存在相应的别名电子邮件，则不要通过输入原始电子邮件来创建新的来宾用户。

      1. 从以下选项中进行选择：

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">发送公共链接</td>
            <td><p>在电子邮件通知中包含一个按钮，用于将用户引导至其所使用的校对查看器中的校样，并授予“查看”访问权限。</p><p>如果 <strong>通过公共URL或嵌入代码订阅校样</strong> 为校样关闭时，用户可以使用其Workfront登录凭据登录，以向校样添加注释。 如果启用了该设置，则提供其电子邮件地址和名称（无需密码）的任何人都可以签名并向校样添加注释。</p></td>
           </tr>
           <tr>
            <td role="rowheader">发送下载链接</td>
            <td>在电子邮件通知中包含一个按钮，可将用户引导至下载页面，该页面提供文件详细信息、文件名和文件大小，并且文件显示为内嵌。 用户可以单击下载页面中的下载链接以下载文件。</td>
           </tr>
           <tr>
            <td role="rowheader">添加自定义消息</td>
            <td>用于指定电子邮件通知的自定义主题和正文。</td>
           </tr>
          </tbody>
         </table>

      1. 单击 **发送**.

         收件人会收到一封电子邮件通知，其中包含有关您选择包含的校样和按钮的信息。

         ![](assets/proof-share-email-350x87.png)

## 共享嵌入代码

如果校样所有者为此配置了校样，则可以通过嵌入代码共享校样。

要通过嵌入代码共享校样，请执行以下操作：

1. 在校对查看器左侧的工具栏中，单击 **共享** 图标。

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. 在 **共享校样** 显示的选项，单击 **获取嵌入代码**，然后单击 **复制**.

## 通过向校样添加用户来共享校样

如果您具有以下任何权限，则可以在审核校样时向校样添加用户：

* 主管或管理员权限
* Manager权限，您是校样创建者或所有者
* 具有作者或审核者校样角色的经理权限

如果校样具有自动工作流，则可以将用户添加到单个阶段。 有关更多信息，请参阅 [自动化工作流概述](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

默认情况下，您会向校样中添加用户：

* 接收包含校样链接的电子邮件通知。
* 可以对来自“Home”（主页）或“My Work”（我的工作）区域的校样进行批准决策，如 [批准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* 无需启用校样即可查看校样。

启用自动工作流后，如果向校样中添加了未在Workfront中启用校样的用户，则会在自动工作流中创建一个新阶段。 您添加的用户在首次查看校样时会自动添加到此新阶段。 有关更多信息，请参阅 [自动化工作流概述](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

要与个人用户共享校样，请执行以下操作：

1. 在校对查看器左侧的工具栏中，单击 **共享** 图标。

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. 单击 **添加收件人** 在左边的列表里。
1. 在 **新校样收件人**，开始键入要与其共享校样的用户名称，然后在下拉列表中显示该名称时单击该名称。
1. （可选）在人员姓名右侧更改任何审阅人选项：

   * **校样角色**:有关更多信息，请参阅 [在Workfront校样中管理校样角色](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **阶段**:（仅当校样具有自动工作流时才可用）。 有关更多信息，请参阅  [自动化工作流阶段概述](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **电子邮件警报**：选择以下选项之一，以指定如何通知人员校样中的活动。

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
        <td>仅当某人明确回复了其评论时，才会向审阅人发送电子邮件（这不包括他们自己对评论的回复）。 这意味着，如果校样上的某人做出新评论，则不会通知审阅人。<p>建议您的客户在验证时使用此设置，以便他们不会收到关于验证的任何其他评论的通知，并且仅会收到对其自己评论的回复通知。</p><p>虽然具有此电子邮件警报设置的审阅人不会收到有关其他新注释的通知，但审阅人仍然可以在校样查看器中查看校样上的所有注释。</p><p>有关注释的信息，请参阅 <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">查看和回复校样评论</a>.</p></td> 
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
        <td>Workfront会发送一封电子邮件，其中列出的所有评论、回复和决策仅在您自己的活动之外的几天内列出。<p>此警报是您查看项目摘要的好方法，不会在一天中出现多次更新。</p><p>此摘要的一个示例用例是部门负责人，他希望监控项目的整体进度。</p><p>有关更多信息，请参阅 <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理校样注释和决策通知</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">无电子邮件</td> 
        <td>Workfront不会发送任何电子邮件警报。<br>对于仅出于参考目的而添加到校样且无需接收任何更改通知的人员，此功能非常有用。<p>系统默认为“每日摘要”（也称为“未设置”）。 如果您或您的审阅人没有进行任何其他更改，则所有校样都具有此设置。</p></td> 
       </tr> 
      </tbody> 
     </table>

1. （可选）重复上述两个步骤以向校样添加多个用户。 
1. （可选）设置 **截止时间** （仅当校样没有自动工作流时可用）。
1. （可选）选择 **向新收件人发送电子邮件通知** 让他们知道，你已经把他们加入了证据。
1. 完成向校样添加用户后，单击 **完成。**
