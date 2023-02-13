---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: 使用基本工作流创建高级校样
description: 使用基本的工作流，您可以让多个审阅人进行校样，但是这些审阅人并未分阶段进行组织。 您添加的所有审阅人都可以在创建校样后立即访问该校样。
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 1%

---

# 使用基本工作流创建高级校样

使用基本的工作流，您可以让多个审阅人进行校样，但是这些审阅人并未分阶段进行组织。 您添加的所有审阅人都可以在创建校样后立即访问该校样。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：选择或更高</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
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
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 使用基本工作流创建高级校样

1. 转到要校样的项目、任务或问题，然后单击 **文档** 选项卡。
1. 单击 **新增** >校样，上传内容，然后完成下面列出的部分。

   或

   将鼠标悬停在现有文档上，然后单击 **创建校样** > **高级校样** 和阅读下面列出的部分。

## 配置工作流并添加审阅人

1. 在工作流类型部分中，选择 **基本**.
1. 指定要添加的用户，然后选择校样角色。

   ![](assets/new-proof---roles-350x213.png)

1. 下表列出了每个角色以及与其关联的权限。

   <table border="1" cellspacing="15" cellpadding="1"> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p> </p> </th> 
      <th> <p><strong>查看校样</strong> </p> </th> 
      <th> <p><strong>添加标记</strong> </p> </th> 
      <th> <p><strong>添加注释</strong> </p> </th> 
      <th> <p><strong>如果没有回复，则编辑自己的评论</strong> </p> </th> 
      <th> <p><strong>做出决定</strong> </p> </th> 
      <th> <p><strong>删除他人的评论</strong> </p> </th> 
      <th>解决注释</th> 
      <th>将操作应用到注释</th> 
      <th> <p><strong>编辑校样</strong> </p> </th> 
      <th>与他人共享证据</th> 
      <th>创建新版本</th> 
      <th> <p><strong>在“主页”区域中查看批准请求</strong> </p> </th> 
      <th>添加新审阅人</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>只读</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>查看者</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>审批者</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>审核人和批准者</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>作者</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> </td> 
      <td>✓</td> 
     </tr> 
     <tr> 
      <td> <p><strong>审阅人</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p><strong>✓</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
     </tr> 
    </tbody> 
   </table>

1. 新Workfront计划的用户可以向系统中的任何用户授予作者或审核者角色。 旧版计划中的用户可以向系统中具有校样许可证的任何用户授予作者或审核者角色。
1. （可选）如果下拉菜单仍然打开，请选择位于菜单底部的任何其他权限：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">解决注释并应用操作 </td> 
      <td> <p>允许Workfront用户执行以下操作：</p> 
       <ul> 
        <li>在评论得到处理后解决，如 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">解决校样注释</a>.</li> 
        <li>将操作应用到注释，如 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">对校样注释使用操作</a>. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通过标记共享证明</td> 
      <td> <p>允许审阅人向校样中添加任何Workfront用户，如 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">标记用户以共享校样</a>.</p> <p>注释:  <p>如果这两个选项不可用（灰显），则用户已拥有权限配置文件，该配置文件允许解析注释、对注释应用操作以及标记任何用户。 </p> <p>如果未显示选项，则您添加的人员不是Workfront许可证持有者。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 对已添加到校样的任何其他用户重复步骤1-3。
1. 对于您与共享的每个用户， **电子邮件警报** 下拉列表中，选择用户在对校样做出评论和决策时收到的电子邮件警报类型：

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

1. 继续 [配置校样的电子邮件设置](#configure-email-settings-for-the-proof) 下。

## 配置校样的电子邮件设置 {#configure-email-settings-for-the-proof}

1. 在 **电子邮件通知** 部分，选择是否向您在 [使用基本工作流创建高级校样](#workflow) 本文的前文：

   <table>
   <tbody>
   <tr>
   <td>通知收件人此校样</td>
   <td>选择此选项可向用户发送电子邮件通知。 When <strong>基本共享</strong> 的 <strong>工作流</strong> 部分，则在创建校样时会发送电子邮件通知。 When <strong>自动化工作流</strong> 的 <strong>工作流</strong> 部分，则当校样进入用户关联的自动工作流的阶段时，会发送电子邮件通知。</td>
   </tr>
   <tr>
   <td>添加自定义消息</td>
   <td>选择此选项可在通知中包含自定义消息。 您可以指定主题和消息正文。 消息正文可以包含富文本格式，如粗体、项目符号和超链接。</td>
   </tr>
   </tbody>
   </table>


1. 继续 [配置校样设置](#configure-proof-settings) 下。

## 配置校样设置 {#configure-proof-settings}

1. 在 **校样设置** 选项，请选择以下任意选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">需要登录 — 校样只能与其他用户共享</td> 
      <td>禁用此选项（默认）后，任何具有URL的人都能查看校样。 <br>选择此选项时：
       <ul>
        <li>只有Workfront校样用户才能查看校样。</li>
        <li>用户无法登录到校样，除非已将他们添加到校样中。</li>
        <li>无法启用订阅。</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">只需要一个决定即可进行此证明</td> 
      <td>当选择此选项时，在其中一名决策者作出决定后完成审查。<br>默认情况下，此选项处于禁用状态。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">要求对决策进行电子签名</td> 
      <td>用户在决定校样时需要指定其用户名和密码。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在做出所有必需的决策时锁定验证</td> 
      <td>启用此设置后，在做出所有决策后，校样状态将被锁定。 当最终审批者做出决策时，状态会自动从已解锁更改为已锁定。<br>默认情况下，此选项处于禁用状态。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">下载原始文件</td> 
      <td>选择此选项后，审阅人可以下载创建校样的原始文件。<br>取消选择此选项后，“下载”图标将不再可见。<br>默认情况下，此选项处于启用状态。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">通过公共URL或嵌入代码共享校样</td> 
      <td>选择此选项后，可通过公共URL或嵌入代码共享校样。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">通过公共URL或嵌入代码订阅校样</td> 
      <td>选择此选项后，尚未明确添加到校样的人员可订阅校样。 在以下设置中，校样订阅者将获得您定义的角色和电子邮件：
       <ul>
        <li><strong>订阅者角色：</strong> 分配给所有订阅校样的审阅人的默认校样角色。 </li>
        <li><strong>订阅者的电子邮件警报设置：</strong> 分配给所有订阅校样的审阅人的默认电子邮件警报。</li>
       </ul><p>
        <ul>
         <li><strong>通过电子邮件链接进行校样访问时，需要满足以下条件：</strong> 配置订阅者是否收到包含校样链接的电子邮件。 您可以选择 <strong>无电子邮件</strong> （访问校样不需要电子邮件链接）、 <strong>仅校样通知电子邮件</strong> （订阅者通过电子邮件接收指向校样的链接，且未进行任何验证）或 <strong>验证和校样通知电子邮件</strong> （订阅者会通过电子邮件收到指向校样的链接，并且必须单击该链接才能访问校样，此选项旨在确保用户输入了他们有权访问的正确电子邮件地址）。</li>
        </ul><p>注意： 如果校样附加了自动工作流，则所有订阅都会向校样所有者生成确认电子邮件，以便他们决定应将人员添加到哪个阶段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **创建校样**.

   Workfront开始生成所选文档或网站的校样。 根据文件大小和类型，文档上传的滞后时间可能会有所不同。 请耐心等待，因为生成较大的文件需要更长的时间。 您可以从页面导航到其他位置，Workfront将继续生成您的文件。 最大文件上传大小为4 GB。

1. 生成校样后，单击 **打开校样** 启动校对查看器。

   ![](assets/open-proof-350x132.png)

   帐户中未启用校样的用户仍可以查看文档并对校样进行评论。