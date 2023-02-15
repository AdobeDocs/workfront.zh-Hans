---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: 使用自动工作流创建高级校样
description: 如果您的流程复杂，或者您定期向同一人员发送内容以供审阅，则通过自动化工作流可以更轻松地管理审阅流程。 校样会从舞台移动到舞台，Adobe Workfront会在每位用户需要进行审阅时通知他们。 有关自动化工作流的更多信息，请参阅自动化工作流概述。
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1856'
ht-degree: 0%

---

# 使用自动工作流创建高级校样

如果您的流程复杂，或者您定期向同一人员发送内容以供审阅，则通过自动化工作流可以更轻松地管理审阅流程。 校样会从舞台移动到舞台，Adobe Workfront会在每位用户需要进行审阅时通知他们。 有关自动化工作流的更多信息，请参阅 [自动化工作流概述](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

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

## 使用自动工作流创建高级校样

1. 转到要校样的项目、任务或问题，然后单击 **文档** 选项卡。
1. 单击 **新增** >校样，上传内容，然后完成下面列出的部分。

   或

   将鼠标悬停在现有文档上，然后单击 **创建校样** > **高级校样** 和阅读下面列出的部分。

## 配置校样阶段

1. 在工作流类型部分中，选择 **自动**.
1. （可选）如果要使用Workfront管理员创建并与您共享的自动工作流模板，请单击 **添加模板**，在显示的框中选择模板，然后单击 **添加模板**.

   >[!NOTE]
   >
   >使用自动化工作流模板时，请考虑以下事项：
   >   
   >* 自动工作流模板的设置决定了您可以使用自动工作流进行校样的操作。 例如，如果模板中禁用了添加阶段按钮，则当您使用校样的自动工作流设置时，该按钮将不可见。
   >* 当某人在自动工作流模板中添加到页面，但已作为校样的审阅人存在时，应用该模板会将审阅人从舞台中删除。 如果不将其他审阅人添加到舞台，则会显示一条消息，提示您添加一个审阅人。
   >* 您能否修改自动工作流模板取决于由Workfront管理员配置的模板设置，如中所述。 如果禁用了修改模板的功能，则只有模板的所有者才能修改模板。


1. 配置自动化工作流的第一阶段：

   1. （可选）如果要为第一个阶段创建名称，请单击 **阶段1**，然后键入名称。
   1. 在 **收件人** 部分，将审阅者添加到舞台。

      >[!NOTE]
      > 
      >在将审阅人添加到阶段时，请考虑以下事项：
      > 
      >* 您可以使用电子邮件地址将外部用户添加到舞台。
      >* 将用户添加到舞台后，您可以在校样中为该用户配置设置。
      >* 您可以将用户直接拖到另一个舞台，也可以将用户拖到 **阶段** 图表。 要选择多个用户，请按Shift+Ctrl（在Windows上）或Shift+Command(在Mac上)。
      >* 您只能向校样添加一次审阅人，这意味着您无法将同一人添加到校样的多个阶段。
      >* 未添加到专用舞台的审阅人无法在该舞台中进行校样或评论。
      >* 默认情况下，将用户添加到舞台会授予用户从创建校样开始查看校样的权限。\
      >  您的Workfront管理员可以限制用户访问校样，直到工作流进入添加用户的阶段。


   1. 单击 **舞台设置**.
   1. 单击 **激活阶段** 选项来指示您希望如何激活舞台。

      对于第一个阶段，您只能选择 **论校样创建**, **在特定的日期和时间**&#x200B;或 **手动**.

   1. （视情况而定）如果您选择 **在特定的日期和时间** 在上一步中，选择要在 **激活时间** 框中。

   1. 使用以下任意选项进一步配置舞台。

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">设置阶段截止时间</td>
         <td><p>要设置阶段的截止时间，请单击 <strong>截止日期选项</strong> 下拉列表。 然后，在 <strong>截止时间</strong>，执行下列操作之一：</p>
          <ul>
           <li>如果您选择 <strong>设置特定日期</strong>:选择所需的截止日期和时间。</li>
           <li>如果您选择 <strong>从阶段激活日期计算</strong>:选择要添加到阶段激活日期的工作天数，以确定截止日期。</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">锁台</td>
         <td>指定舞台可以锁定的时间。 </td>
        </tr>
        <tr>
         <td role="rowheader">将主要决策权转移到</td>
         <td><p>在舞台上选择主要决策者（只有在您向舞台中添加至少一名具有“审批者”或更高“校样”角色的人员后才可用）。 如果选择“主要决策者”，则 <strong>只需要一个决定</strong> 选项。</p></td>
        </tr>
        <tr>
         <td role="rowheader">此阶段只需要一个决策</td>
         <td>当某个决策者做出决策时，结束整个审查过程。<p>如果您在 <strong>主要决策者</strong>下拉菜单。</p></td>
        </tr>
        <tr>
         <td role="rowheader">将此阶段设为私有</td>
         <td>仅允许以下人员查看在此阶段做出的评论和决策：主管、Workfront管理员和Workfront校样管理员</td>
        </tr>
       </tbody>
      </table>

1. 添加和配置另一个阶段：

   1. 单击 **新阶段**.
   1. （可选）如果要为第一个阶段创建名称，请单击 **阶段2** (或 **阶段3**, **阶段4**&#x200B;等)，然后键入名称。

   1. 单击 **激活阶段**，然后选择一个选项以指定是自动激活还是手动激活舞台。

      除了 **论校样创建**, **在特定的日期和时间**&#x200B;或 **手动**，则可以选择与上一步骤中所发生情况相关的选项：

      ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. 如果您选择的激活阶段选项取决于上一步中发生的情况，请使用显示的选项来配置激活设置。

      例如，如果您选择 **上一阶段状态更改时**，选择 **上一阶段**，然后选择 **状态已更改为** 框中。

1. 根据需要重复上一步骤以添加更多阶段。

   在向自动化工作流中添加阶段时，屏幕上会显示一个用于表示这些阶段的图表表单：

   ![](assets/stages-diagram-350x213.png)

1. 继续 [配置校样的电子邮件设置](#configure-email-settings-for-the-proof) 下。

## 配置校样的电子邮件设置 {#configure-email-settings-for-the-proof}

1. 在 **电子邮件通知** 部分，选择是否向您在 [使用自动工作流创建高级校样](#workflow) 本文的前文：

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
        </ul><p><strong>注意：</strong> 如果校样附加了自动工作流，则所有订阅都会向校样所有者生成确认电子邮件，以便他们决定应将人员添加到哪个阶段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **创建校样**.

   Workfront开始生成所选文档或网站的校样。 根据文件大小和类型，文档上传的滞后时间可能会有所不同。 请耐心等待，因为生成较大的文件需要更长的时间。 您可以从页面导航到其他位置，Workfront将继续生成您的文件。 最大文件上传大小为4 GB。

1. 生成校样后，单击 **打开校样** 启动校对查看器。

   ![](assets/open-proof-350x132.png)

   帐户中未启用校样的用户仍可以查看文档并对校样进行评论 [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
