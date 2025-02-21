---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: 使用基本工作流创建高级验证
description: 使用基本工作流，您可以让多个审阅人查看验证，但他们不会归为多个阶段。 您添加的所有审阅人可以在您创建验证后立即访问该验证。
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 1%

---

# 使用基本工作流创建高级验证

<!-- Audited: 1/2024 -->

使用基本工作流，您可以让多个审阅人查看验证，但他们不会归为多个阶段。 您添加的所有审阅人可以在您创建验证后立即访问该验证。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td>
   <p>新建：任何</p>
    <p>当前计划：专业版或更高版本</p>
   <p>旧版计划：选择或更高版本</p> <p>有关使用其他计划进行验证访问的更多信息，请参阅<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>新增：标准</p>
    <p>当前：工作或计划</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、角色或验证权限配置文件，请联系您的Workfront或Workfront Proof管理员。

+++

## 使用基本工作流创建高级验证

1. 转到要验证的项目、任务或问题，然后单击&#x200B;**文档**&#x200B;选项卡。
1. 单击&#x200B;**新增** >校对，上传内容，然后完成下面列出的部分。

   或

   将鼠标悬停在现有文档上，然后单击&#x200B;**创建验证** > **高级验证**&#x200B;并处理下面列出的部分。

## 配置工作流并添加审阅者

1. 在“工作流类型”部分中，选择&#x200B;**基本**。
1. 指定要添加的用户，然后选择验证角色。

   ![新验证角色](assets/new-proof---roles-350x213.png)

1. 下表列出了每个角色及其关联的权限。

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
      <th> <p><strong>查看校对</strong> </p> </th> 
      <th> <p><strong>添加标记</strong> </p> </th> 
      <th> <p><strong>添加评论</strong> </p> </th> 
      <th> <p><strong>如果没有回复，则编辑自己的评论</strong> </p> </th> 
      <th> <p><strong>做出决定</strong> </p> </th> 
      <th> <p><strong>删除其他人的评论</strong> </p> </th> 
      <th>解决评论</th> 
      <th>将操作应用到注释</th> 
      <th> <p><strong>编辑校对</strong> </p> </th> 
      <th>与他人共享证明</th> 
      <th>创建新版本</th> 
      <th> <p><strong>在主页区域查看审批请求</strong> </p> </th> 
      <th>添加新审阅者</th> 
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
      <td> <p><strong>审阅者和批准者</strong> </p> </td> 
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

1. 新Workfront计划上的用户可以向系统中的任何用户授予创作或审查方角色。 旧版计划用户可以将作者或审查方角色授予系统中拥有验证许可证的任何用户。
1. （可选）在下拉菜单仍然打开的情况下，选择菜单底部可用的任何其他权限：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">解决注释并应用操作 </td> 
      <td> <p>允许Workfront用户执行以下操作：</p> 
       <ul> 
        <li>解决评论之后再解决它，如<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">解决校对评论</a>中所述。</li> 
        <li>将操作应用于评论，如<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">对验证评论使用操作</a>中所述。 </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通过标记共享校样</td> 
      <td> <p>允许查看者将任何Workfront用户添加到验证，如<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">标记共享验证的用户</a>中所述。</p> <p>注意：  <p>如果这两个选项不可用（灰显），则用户已有权限配置文件，该配置文件允许解析注释、将操作应用于注释以及标记任何用户。 </p> <p>如果选项未显示，则您添加的人不是Workfront许可证所有者。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 对已添加到验证的任何其他用户重复步骤1-3。
1. 对于与您共享的每个用户，在&#x200B;**电子邮件警报**&#x200B;下拉列表中，选择此用户在他人对验证做出评论和决策时收到的电子邮件警报类型：

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

1. 继续[为下面的校对配置电子邮件设置](#configure-email-settings-for-the-proof)。

## 配置验证的电子邮件设置 {#configure-email-settings-for-the-proof}

1. 在&#x200B;**电子邮件通知**&#x200B;部分中，选择是否向您在[使用本文前面的“基本”工作流创建高级验证](#workflow)中选择的用户发送电子邮件通知和自定义消息：

   <table>
   <tbody>
   <tr>
   <td>将此证明通知收件人</td>
   <td>选择此选项可向用户发送电子邮件通知。 在<strong>工作流</strong>部分中选择<strong>基本共享</strong>时，会在创建验证时发送电子邮件通知。 在<strong>工作流</strong>部分中选择<strong>自动工作流</strong>时，当验证进入用户关联的自动工作流阶段时，将发送电子邮件通知。</td>
   </tr>
   <tr>
   <td>添加自定义消息</td>
   <td>选择此选项可在通知中包含自定义消息。 您可以指定主题和消息正文。 消息正文可以包括富文本格式，例如粗体、项目符号和超链接。</td>
   </tr>
   </tbody>
   </table>


1. 继续[配置下面的校对设置](#configure-proof-settings)。

## 配置校对设置 {#configure-proof-settings}

1. 在&#x200B;**校对设置**&#x200B;部分中，选择以下任一选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">需要登录 — 验证只能与其他用户共享</td> 
      <td>禁用此选项（默认）后，具有URL的任何人都可以查看验证。 <br>选择此选项时：
       <ul>
        <li>只有Workfront Proof用户能够查看验证。</li>
        <li>用户无法登录到验证，除非他们已添加到验证中。</li>
        <li>无法启用订阅。</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">此证明只需一个决定</td> 
      <td>如果选择该选项，则审阅会在决策者之一做出决定后完成。<br>默认情况下已禁用此选项。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">要求对决策进行电子签名</td> 
      <td>用户必须在做出验证决策时指定用户名和密码。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">作出所有必需的决策时锁定验证</td> 
      <td>启用此设置后，将在做出所有决策后锁定验证状态。 当最终批准者做出决定时，状态会自动从已解锁更改为已锁定。<br>默认情况下已禁用此选项。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">下载原始文件</td> 
      <td>选择此选项后，审阅人将能够下载从中创建验证的原始文件。<br>取消选择此选项时，“下载”图标不再可见。<br>默认启用此选项。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">通过公共URL或嵌入代码共享验证</td> 
      <td>选择此选项后，可以通过公共URL或嵌入代码共享验证。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">通过公共URL或嵌入代码订阅验证</td> 
      <td>选择此选项时，未明确添加到验证的用户可以订阅验证。 订阅验证的用户将获得您在以下设置中定义的角色和电子邮件：
       <ul>
        <li><strong>订阅者角色：</strong>分配给订阅了验证的所有审阅人的默认验证角色。 </li>
        <li><strong>订阅者的电子邮件警报设置：</strong>分配给订阅了验证的所有审阅人的默认电子邮件警报。</li>
       </ul><p>
        <ul>
         <li><strong>通过电子邮件链接访问验证所需的链接：</strong>配置订阅者是否收到包含验证链接的电子邮件。 您可以选择<strong>无电子邮件</strong> （访问验证不需要电子邮件链接）、<strong>仅验证通知电子邮件</strong> （订阅者通过电子邮件接收验证链接，无需任何验证）或<strong>验证和验证通知电子邮件</strong> （订阅者通过电子邮件接收验证链接，必须单击该链接才能访问验证，此选项旨在确保此人输入了他们有权访问的正确电子邮件地址）。</li>
        </ul><p>注意：  如果验证已附加自动工作流，则所有订阅都将向验证所有者生成确认电子邮件，以便他们决定应将人员添加到哪个阶段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**创建校对**。

   Workfront开始生成选定文档或网站的验证。 根据文件大小和类型，文档上传的滞后时间可能有所不同。 请耐心等待，因为生成更大的文件需要更长的时间。 您可以离开页面，Workfront将继续生成您的文件。 最大文件上传大小为4GB。

1. 生成校对后，单击&#x200B;**打开校对**&#x200B;以启动校对查看器。

   ![打开校对](assets/open-proof-350x132.png)

   帐户未启用验证的用户仍可以查看文档并对验证进行评论。