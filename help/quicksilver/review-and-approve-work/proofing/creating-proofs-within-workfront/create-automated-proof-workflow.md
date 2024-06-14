---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: 使用自动化工作流创建高级验证
description: 如果您的流程比较复杂，或者您定期将内容发送给同一人进行审阅，则使用自动工作流可以更轻松地管理审阅流程。 验证从一个阶段转移到另一个阶段，当每个用户需要审核时，Adobe Workfront会通知他们。 有关自动化工作流的详细信息，请参阅自动化工作流概述。
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 0%

---

# 使用自动化工作流创建高级验证

<!-- Audited: 2/2024 -->

如果您的流程比较复杂，或者您定期将内容发送给同一人进行审阅，则使用自动工作流可以更轻松地管理审阅流程。 验证从一个阶段转移到另一个阶段，当每个用户需要审核时，Adobe Workfront会通知他们。 有关自动化工作流的详细信息，请参阅 [自动化工作流概述](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>新建：任何</p><p>当前计划：专业版或更高版本</p><p>旧版计划：选择或更高版本</p> <p>有关验证不同计划的访问权限的详细信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>新增：标准</p><p>当前计划：工作或计划</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 使用自动化工作流创建高级验证

1. 转到要验证的项目、任务或问题，然后单击 **文档** 选项卡。
1. 单击 **新增** >验证，上传内容，然后完成以下列出的部分。

   或

   将鼠标悬停在现有文档上，然后单击 **创建校对** > **高级校对** 并完成下面列出的部分。

## 配置验证阶段

1. 在工作流类型部分，选择 **自动**.
1. （可选）如果要使用Workfront管理员创建并与您共享的自动化工作流模板，请单击 **添加模板**，在显示的框中选择模板，然后单击 **添加模板**.

   >[!NOTE]
   >
   >使用自动工作流模板时，请考虑以下事项：
   >   
   >* 自动工作流模板的设置确定您可以使用自动工作流执行哪些操作以进行验证。 例如，如果在模板中禁用了添加暂存按钮，则当您使用验证的自动工作流设置时，该按钮将不可见。
   >* 当有人在自动工作流模板中被添加到阶段，但也以审阅者身份出现在验证中时，应用模板会将审阅者从阶段中删除。 如果不将其他审阅人添加到阶段，则会显示一条消息，提示您添加审阅人。
   >* 能否修改自动工作流模板取决于Workfront管理员配置的模板设置，如中所述。 如果禁用了修改模板的功能，则只有模板所有者可以修改模板。

1. 配置自动工作流的第一个阶段：

   1. （可选）如果要为第一个阶段创建名称，请单击 **阶段1**，然后键入名称。
   1. 在 **收件人** 部分，将审阅人添加到舞台。

      >[!NOTE]
      >
      >将审阅者添加到阶段时，请考虑以下事项：
      >   
      >* 您可以使用电子邮件地址将外部用户添加到阶段。
      >* 将用户添加到阶段后，您可以在验证上为该用户配置设置。
      >* 您可以将用户直接拖到另一个阶段，也可以将用户拖到上的阶段 **暂存** 图表。 要选择多个用户，请按Shift+Ctrl键（在Windows上）或Shift+Command键(在Mac上)。
      >* 您只能将查看者添加到验证一次，这意味着您无法将同一人员添加到验证上的多个阶段。
      >* 未添加到专用阶段的审阅人无法在验证上看到该阶段，也无法在该阶段中做出评论。
      >* 默认情况下，将用户添加到阶段会授予该用户从创建验证之时起查看验证的权限。 在工作流进入添加用户的阶段之前，Workfront管理员可以限制用户访问验证。

   1. 单击 **暂存设置**.
   1. 单击 **激活阶段** 用于指示您希望如何激活暂存的选项。

      对于第一个阶段，您只能选择 **创建验证时**， **在特定日期和时间**，或 **手动**.

   1. （视情况而定）如果您选择 **在特定日期和时间** 在上一步中，选择要在中激活舞台的日期和时间 **激活日期** 框。

   1. 使用以下任意选项进一步配置舞台。

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">设置阶段截止日期</td>
         <td><p>要设置阶段的截止日期，请单击 <strong>截止日期选项</strong> 下拉列表。 然后，在下 <strong>截止日期</strong>，请执行下列操作之一：</p>
          <ul>
           <li>如果您选择 <strong>设置特定日期</strong>：选择所需的截止日期和时间。</li>
           <li>如果您选择 <strong>根据阶段激活日期计算</strong>：选择要添加到阶段激活日期的工作日数以确定截止日期。</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">锁定阶段</td>
         <td>指定可以锁定舞台的时间。 </td>
        </tr>
        <tr>
         <td role="rowheader">将主要决策权限转移到</td>
         <td><p>选择阶段上的主要决策者（仅在您将至少一名具有“审批者”或更高验证角色的人员添加到阶段后可用）。 如果选择主要决策者， <strong>只需一个决策</strong> 选项在此阶段被禁用。</p></td>
        </tr>
        <tr>
         <td role="rowheader">此阶段只需要一个决策</td>
         <td>当决策者做出决策时，结束整个审核过程。<p>如果您在中指定了用户，则此选项不可用 <strong>主要决策者</strong>下拉菜单。</p></td>
        </tr>
        <tr>
         <td role="rowheader">将此阶段设为私有</td>
         <td>仅允许以下人员查看在此阶段所做的评论和决策：主管、Workfront管理员和Workfront Proof管理员</td>
        </tr>
       </tbody>
      </table>

1. 添加和配置另一个阶段：

   1. 单击 **新阶段**.
   1. （可选）如果要为第一个阶段创建名称，请单击 **阶段2** (或 **阶段3**， **阶段4**，等等)，然后键入名称。

   1. 单击 **激活阶段**，然后选择一个选项以指定是自动激活舞台还是手动激活舞台。

      除了选项 **创建验证时**， **在特定日期和时间**，或 **手动**&#x200B;中，您可以选择取决于上一步骤中执行的操作的选项：

      ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. 如果您选择了取决于上一步中所发生情况的激活阶段选项，请使用显示的选项来配置激活设置。

      例如，如果您选择 **当上一个阶段的状态发生变化时**，选择 **上一阶段**，然后在中选择状态 **状态已更改为** 盒子。

1. 根据需要重复上一步添加更多阶段。

   将阶段添加到自动工作流时，屏幕上会出现一个图表来表示这些阶段：

   ![](assets/stages-diagram-350x213.png)

1. 继续 [配置验证的电子邮件设置](#configure-email-settings-for-the-proof) 下。

## 配置验证的电子邮件设置 {#configure-email-settings-for-the-proof}

1. 在 **电子邮件通知** 部分，选择是否向您在中选择的用户发送电子邮件通知和自定义消息 [使用自动化工作流创建高级验证](#workflow) 本文前文：

   <table>
      <tbody>
      <tr>
      <td>将此证明通知收件人</td>
      <td>选择此选项可向用户发送电子邮件通知。 时间 <strong>基本共享</strong> 在 <strong>工作流</strong> 部分，在创建验证时发送电子邮件通知。 时间 <strong>自动化工作流</strong> 在 <strong>工作流</strong> 部分，当验证进入用户关联的自动工作流阶段时会发送电子邮件通知。</td>
      </tr>
      <tr>
      <td>添加自定义消息</td>
      <td>选择此选项可在通知中包含自定义消息。 您可以指定主题和消息正文。 消息正文可以包括富文本格式，例如粗体、项目符号和超链接。</td>
      </tr>
      </tbody>
      </table>


1. 继续 [配置校对设置](#configure-proof-settings) 下。

## 配置校对设置 {#configure-proof-settings}

1. 在 **验证设置** 部分，选择以下任一选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">需要登录 — 验证只能与其他用户共享</td> 
      <td>禁用此选项（默认）后，具有URL的任何人都可以查看验证。 <br>选中此选项时：
       <ul>
        <li>只有Workfront Proof用户能够查看验证。</li>
        <li>用户无法登录到验证，除非他们已添加到验证中。</li>
        <li>无法启用订阅。</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">此证明只需一个决定</td> 
      <td>如果选择该选项，则审阅会在决策者之一做出决定后完成。<br>此选项默认处于禁用状态。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">要求对决策进行电子签名</td> 
      <td>用户必须在做出验证决策时指定用户名和密码。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">作出所有必需的决策时锁定验证</td> 
      <td>启用此设置后，将在做出所有决策后锁定验证状态。 当最终批准者做出决定时，状态会自动从已解锁更改为已锁定。<br>此选项默认处于禁用状态。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">下载原始文件</td> 
      <td>选择此选项后，审阅人将能够下载从中创建验证的原始文件。<br>取消选择此选项时，“下载”图标不再可见。<br>此选项默认处于启用状态。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">通过公共URL或嵌入代码共享验证</td> 
      <td>选择此选项后，可以通过公共URL或嵌入代码共享验证。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">通过公共URL或嵌入代码订阅验证</td> 
      <td>选择此选项时，未明确添加到验证的用户可以订阅验证。 订阅验证的用户将获得您在以下设置中定义的角色和电子邮件：
       <ul>
        <li><strong>订阅者角色：</strong> 分配给订阅了验证的所有审阅人的默认验证角色。</li>
        <li><strong>订阅者的电子邮件警报设置：</strong> 分配给订阅了验证的所有审阅人的默认电子邮件警报。</li>
       </ul><p>
        <ul>
         <li><strong>以下各项需要通过电子邮件链接访问证明：</strong> 配置订阅者是否收到一封包含证明链接的电子邮件。 您可以选择 <strong>无电子邮件</strong> （访问验证不需要电子邮件链接）， <strong>仅验证通知电子邮件</strong> （订阅者通过电子邮件接收指向验证的链接，无需任何验证），或 <strong>验证和验证通知电子邮件</strong> （订阅者通过电子邮件收到校样的链接，必须单击该链接才能访问校样，此选项旨在确保人员输入了他们有权访问的正确电子邮件地址）。</li>
        </ul><p><strong>注意：</strong> 如果验证已附加自动工作流，则所有订阅都将向验证所有者生成确认电子邮件，以便他们决定应将人员添加到哪个阶段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **创建校对**.

   Workfront开始生成选定文档或网站的验证。 根据文件大小和类型，文档上传的滞后时间可能有所不同。 请耐心等待，因为生成更大的文件需要更长的时间。 您可以离开页面，Workfront将继续生成您的文件。 最大文件上传大小为4GB。

1. 生成验证后，单击 **打开校对** 以启动验证查看器。

   ![](assets/open-proof-350x132.png)

   帐户未启用验证的用户仍然可以查看文档并对验证进行评论 [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
