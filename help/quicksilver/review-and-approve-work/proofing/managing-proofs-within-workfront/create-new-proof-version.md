---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 创建新版本的验证
description: 跨工作项的多个版本或修订版本管理反馈可能是一项巨大的挑战。 Workfront通过允许您创建和比较验证的多个版本来简化此过程。
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 7477b62cf0e2e61966f8e74cf268217e2ceb67ef
workflow-type: tm+mt
source-wordcount: '1734'
ht-degree: 0%

---

# 创建新版本的验证

跨工作项的多个版本或修订版本管理反馈可能是一项巨大的挑战。 Workfront通过允许您创建和比较验证的多个版本来简化此过程。

创建新版本的验证时，请考虑以下信息：

* 您可以授予用户查看一个版本的权限，但不能授予用户查看另一个版本的权限。 相反，如果您与某个用户共享较新的版本，则该用户将无法查看较早版本，除非您返回并明确授予用户访问这些较早版本的权限。
* 要创建新版本的验证，您必须具有对验证的编辑权限。

  请参阅[在Workfront Proof中管理验证角色](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)和[在Workfront Proof中管理验证权限配置文件](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)，以了解有关谁具有验证编辑权限的更多信息。

  有关共享校样版本的信息，请参阅  [在Workfront Proof中共享校对](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)。

>[!IMPORTANT]
>
>如果在Adobe Workfront中创建验证，则还必须在Workfront中创建针对该验证创建的任何新版本。 如果校对是在Workfront Proof中创建的，则无法在Workfront中创建该校对的新版本。

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

## 在Workfront中创建验证的新版本

可通过多种方式在Workfront中上传新验证版本。 默认验证设置可能会也可能不会延续到以前的版本，具体取决于您选择的方法：

* **在上传文档时自动生成验证**：默认验证设置不会延续。 如果您在用户配置文件中启用了此设置，则在拖放新版本时默认验证设置不会延续。
* **创建验证>简单**：默认验证设置不会延续。 如果您在创建新验证版本时选择简单，则默认验证设置不会延续到以前的版本。
* **新增>版本>验证**：默认验证设置延续自以前的版本。
* **创建校对>高级**：默认校对设置继承自以前的版本。

  <table>
  <tbody>
  <tr>
  <td>上传文档时自动生成证明</td>
  <td>默认验证设置不会延续。 如果您在用户配置文件中启用了此设置，则在拖放新版本时默认验证设置不会延续。</td>
  </tr>
  <tr>
  <td>创建验证&gt;简单</td>
  <td>默认验证设置不会延续。 如果您在创建新验证版本时选择简单，则默认验证设置不会延续到以前的版本。</td>
  </tr>
  <tr>
  <td>新增&gt;版本&gt;验证</td>
  <td>默认验证设置延续自以前的版本。</td>
  </tr>
  <tr>
  <td>创建验证&gt;高级</td>
  <td>默认验证设置延续自以前的版本。</td>
  </tr>
  </tbody>
  </table>




要创建新版本的验证，请执行以下操作：

1. 打开包含校对的文档列表。
1. 从计算机的文件系统中，将新文件拖放到验证上。

   或

   选择列出校对的行，单击&#x200B;**新增** > **版本**，然后单击要用于添加新版本的校对的选项。

   ![](assets/add-new-version-350x185.png)

## 从验证查看者创建新版本的验证(仅限Workfront Proof)

如果您使用的是独立的Workfront Proof，则可以创建包含单个文件或Web捕获的新版本验证。 

>[!NOTE]
>
>如果您的帐户是企业计划，并且您上传了多个文件或Web捕获，则这些文件或捕获会自动合并到单个新版本中。 有关详细信息，请参阅[创建多页校对](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)。

要在Workfront Proof中创建新版本的验证，请执行以下操作：

1. 打开证明。
1. 单击左上角的&#x200B;**版本**&#x200B;下拉菜单，然后在显示的框中单击&#x200B;**+新版本**。

   在显示的&#x200B;**新验证版本的**&#x200B;页面上，您可以看到所有以前版本的审阅者，包括他们的角色和电子邮件通知设置。 您可以轻松地编辑现有审阅人的角色和通知，或从此页面上的新版本中删除现有审阅人。

1. 在&#x200B;**添加文件**&#x200B;下，通过从您的计算机中拖放文件或者单击&#x200B;**浏览**&#x200B;并选择所需的文件，将文件作为新版本的验证上传。 您可以键入版本的&#x200B;**校对名称**，或将此框留空以使用在末尾添加版本号的相同文件名。

   或

   通过键入URL将网页捕获为验证的新版本。

   >[!NOTE]
   >
   >只有完全支持HTML5的浏览器才提供拖放功能。 这不包括Internet Explorer 7至9和Safari。

1. 在&#x200B;**工作流**&#x200B;下，进行以下任何更改以指定此版本校对的审阅人。

   先前版本的审阅人将由您添加的审阅人替换。

   * 将该版本的&#x200B;**所有者**&#x200B;更改为帐户中的其他用户。\
     有关所有者权限的信息，请参阅Workfront Proof中的[验证权限配置文件](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)。

   * 使用&#x200B;**键入联系人姓名或电子邮件地址以添加收件人框**，将审阅人添加到该版本。 您可以为每个收件人指定&#x200B;**验证角色**&#x200B;和&#x200B;**电子邮件警报**&#x200B;类型。

     有关将组添加到验证的信息，请参阅  [将组添加到验证](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md)。 有关角色的信息，请参阅[在Workfront Proof中管理验证角色](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)。

     >[!NOTE]
     >
     >如果创建者或所有者  校对默认情况下已禁用[校对电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md)（在其个人设置中），即使在“新校对”页面上选中通过电子邮件通知人员框，他们也不会收到任何校对或新校对电子邮件。 有关电子邮件通知的信息，请参阅[ Workfront Proof中的配置电子邮件通知设置](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)。 另请参阅[校对电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md)和[新校对电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md)。

   * 设置版本的验证截止日期。
   * 将鼠标悬停在审阅人的姓名上，可查看审阅人在以前的版本上做出的任何决策。

1. 在&#x200B;**电子邮件通知**&#x200B;下，执行以下任一操作：

   * 指定是否要通知审阅者新版本。\
     您的选择将记录到验证详细信息页面的活动部分。 有关详细信息，请参阅[在Workfront Proof中管理校对详细信息](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)。

   * 添加自定义主题和消息。

1. 在&#x200B;**组织**&#x200B;部分中，执行以下任一操作： 

   * 将一个或多个标记应用于验证。 有关详细信息，请参阅[在Workfront Proof中创建和管理标签](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md)。\
     请注意，标记也继承自该验证的先前版本。 如果向新版本添加新标记，则也会标记以前的版本。

   * 将版本添加到文件夹。 有关详细信息，请参阅[在Workfront Proof中管理文件夹](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)。 将从该验证的先前版本复制该文件夹。 如果选择其他文件夹，则将移动整个验证（所有版本）。

   * 帐单管理员和管理员可以在“设置”选项卡上将该文件夹字段设为整个帐户的必填字段。 有关详细信息，请参阅。

1. 在验证设置下，进行以下任何更改：

   * 需要登录验证
   * 需要在证明上提供电子签名（仅限企业计划）
   * 作出所有决定时锁定验证
   * 允许或阻止下载原始文件
   * 公开共享证明，包括公开共享设置
   * 订阅证明\
     在此部分中所做的选择将显示在验证详细信息页面（可以编辑某些字段）中。 有关详细信息，请参阅[在Workfront Proof中管理校对详细信息](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Create a new version of a proof from the proofing viewer</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create a new version from the proofing viewer</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof.</li>
<li value="2"> <p>Click the <strong>Version</strong> drop-down menu in the upper-left corner, then click <strong>+ New version</strong> in the box that appears.</p> <p>On the <strong>New proof version of</strong> page that appears, you can see all the reviewers from the previous version, including their roles and email notification settings. You can easily edit the roles and notifications of existing reviewers or remove existing reviewers from the new version on this page.</p> </li>
<li value="3"> <p>Under <strong>Add files</strong>, upload a file as a new version of the proof by dragging and dropping from your computer or by clicking <strong>browse</strong> and selecting the file you want. You can type a&nbsp;<strong>Proof name</strong>&nbsp;for the version or leave this box blank to&nbsp;use the same filename with a version number added on the end.</p> <p>Or<br></p> <p>Capture a web page as a new version of the proof by typing a URL</p> <note type="note">
Drag and drop is available only with browsers that fully support HTML5. This excludes Internet Explorer 7 through 9 and Safari.
<br>
</note> </li>
<li value="4"> <p>Under <strong>Workflow</strong>, make any of the following changes to specify the reviewers for this version of the proof.</p> <p>Reviewers from the previous version are replaced by the reviewers you add.</p>
<ul>
<li>Change the <strong>Owner</strong> of the version to another user in your account.<br>For information about owner permissions, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md" class="MCXref xref">Proof Permissions Profiles in Workfront Proof</a>.</li>
<li> <p>Using the <strong>Type contact name or email address to add a recipient box</strong>, add reviewers to the version. You can specify a <strong>Proof role</strong> and an <strong>Email alerts</strong> type for each recipient.</p> <p>For information about adding groups to the proof, see&nbsp;<a href="../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md" class="MCXref xref">Add Groups to a Proof</a>.&nbsp;For information about roles, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p> <note type="note">
If the creator or owner of&nbsp;&nbsp;the proof has
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> disabled by default (in their personal settings), they won't receive any Proof made or New proof emails even if the Notify people by email box is checked on the New proof page. For information about email notifications, see
<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.&nbsp;See also
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> and
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">New proof email</a>.
<br>
</note> </li>
<li>Set a proof deadline for the version.</li>
<li>Hover over a reviewer's name to see any decisions he or she made on a previous version.</li>
</ul> </li>
<li value="5">Under <strong>Email notification</strong>, do any of the following:
<ul>
<li>Specify whether you want to notify the reviewers of the new version.<br>Your selection will be logged in the Proof activity section on the Proof details page.</li>
<li>Add a custom subject and message.</li>
</ul></li>
<li value="6">Under Proof settings, make any of the changes below:
<ul>
<li>Require login on the proof</li>
<li>Require electronic signatures on the proof (Enterprise plan only)</li>
<li>Lock the proof when all decisions are made</li>
<li>Allow or block download of original file</li>
<li>Public sharing of the proof,&nbsp;including public sharing settings</li>
<li>Subscription to the proof<br>The selections made in this section will be shown in the Proof details page.</li>
</ul></li>
</ol>
-->

## 关于新版本消息

如果先前版本的验证中包含自定义主题/消息，则默认情况下将显示在新版本页面上。 您可以：

* 编辑主题和消息。
* 取消选中通过电子邮件通知人员框，这意味着不会向审阅人发送电子邮件，通知他们他们要审阅的新版本。

  >[!NOTE]
  >
  >这不受您个人设置中保存的任何默认自定义主题/消息的影响。

如果您在个人设置中保存了默认主题和消息，这将影响新版本页面上默认显示的消息：

* 如果您选择使用标准电子邮件（例如，无自定义主题/消息）通过电子邮件向审阅人通知早期版本的验证，则您的默认自定义主题/消息（您的个人设置）将显示在新版本页面上。 然后，您可以编辑自定义主题和消息，或取消选中通过电子邮件通知人员框（这意味着不会向审阅人发送电子邮件，通知他们有要审阅的新版本）。
* 如果您选择不通过电子邮件通知审阅人以前版本的验证（例如，没有标准或自定义电子邮件），则默认情况下，“新版本”页面不会包含任何消息。 要向审阅人通知新版本，请单击“发送邮件”链接，该链接将显示您的默认自定义主题/邮件（根据您的个人设置）。 之后，您可以根据需要编辑自定义主题和消息。

如果您的个人设置中未保存默认主题和消息，则新版本页面上将显示以下内容：

* 如果您选择使用标准电子邮件（例如，无自定义主题/消息）通过电子邮件通知您以前版本的验证审阅人，则默认情况下将选中“新版本”页面上的“通过电子邮件通知人员”选项。 要添加自定义消息，请单击链接。
* 如果您选择不通过电子邮件通知审阅人以前版本的验证（例如，没有标准或自定义电子邮件），则默认情况下，“新版本”页面不会包含任何消息。 要通知审阅者新版本，请单击发送消息链接。 然后，您可以通过单击“添加自定义消息”链接来添加自定义主题和消息。
