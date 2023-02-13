---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 创建校样的新版本
description: 管理作品的多个版本或修订版本之间的反馈可能是一项巨大的挑战。 Workfront通过允许您创建和比较多个版本的校样来简化此过程。
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1721'
ht-degree: 0%

---

# 创建校样的新版本

管理作品的多个版本或修订版本之间的反馈可能是一项巨大的挑战。 Workfront通过允许您创建和比较多个版本的校样来简化此过程。

创建校样的新版本时，请考虑以下信息：

* 您可以授予用户查看一个版本的权限，但不能查看另一个版本。 相反，如果您与某个用户共享较新版本，则该用户将无法查看较早版本，除非您返回并明确授予该用户访问这些先前版本的权限。
* 要创建校样的新版本，您必须对校样具有编辑权限。

   请参阅 [在Workfront校样中管理校样角色](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) 和 [在Workfront校样中校样权限配置文件](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 以获取有关谁对校样具有编辑权限的更多信息。

   有关共享校样版本的信息，请参阅  [在Workfront校样中共享校样](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>如果在Adobe Workfront中创建了校样，则还必须在Workfront中创建为该校样创建的任何新版本。 如果校样是在Workfront中创建的，则无法在Workfront中创建该校样的新版本。

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

## 在Workfront中创建校样的新版本

在Workfront中可以通过多种方法上传新的校样版本。 默认校样设置可能会（也可能不会）从以前的版本继承，具体取决于您选择的方法：

* **上传文档时自动生成校样**:默认校样设置不会继续。 如果您在用户配置文件中启用了此设置，则在拖放新版本时，默认校样设置不会继续执行。
* **创建校样>简单**:默认校样设置不会继续。 如果在创建新校样版本时选择“简单”，则默认校样设置不会继承之前版本的校样设置。
* **新增>版本>校样**:默认校样设置会与之前的版本进行比较。
* **创建校样>高级**:默认校样设置会与之前的版本进行比较。

   <table>
  <tbody>
  <tr>
  <td>上传文档时自动生成证明</td>
  <td>默认校样设置不会继续。 如果您在用户配置文件中启用了此设置，则在拖放新版本时，默认校样设置不会继续执行。</td>
  </tr>
  <tr>
  <td>创建校样&gt;简单</td>
  <td>默认校样设置不会继续。 如果在创建新校样版本时选择“简单”，则默认校样设置不会继承之前版本的校样设置。</td>
  </tr>
  <tr>
  <td>新增&gt;版本&gt;校样</td>
  <td>默认校样设置会与之前的版本进行比较。</td>
  </tr>
  <tr>
  <td>创建校样&gt;高级</td>
  <td>默认校样设置会与之前的版本进行比较。</td>
  </tr>
  </tbody>
  </table>




要创建校样的新版本，请执行以下操作：

1. 打开包含校样的文档列表。
1. 从您计算机的文件系统中，将新文件拖放到校样上。

   或

   选择列出校样的行，单击 **新增** > **版本**，然后单击要用于添加新版本校样的选项。

   ![](assets/add-new-version-350x185.png)

## 从校样查看器创建校样的新版本(仅限Workfront校样)

如果您使用的是独立的Workfront校样，则可以创建包含单个文件或Web捕获的校样的新版本。 

>[!NOTE]
>
>如果您的帐户位于企业计划中，并且您上传了多个文件或Web捕获，则这些文件或Web捕获会自动合并到单个新版本中。 请参阅 [创建多页校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) 以了解更多信息。

要在Workfront校样中创建校样的新版本，请执行以下操作：

1. 打开校样。
1. 单击 **版本** 下拉菜单，然后单击 **+新版本** 框中。

   在 **的新校样版本** 页面，您可以查看以前版本的所有审阅人，包括其角色和电子邮件通知设置。 您可以轻松编辑现有审阅人的角色和通知，或从本页的新版本中删除现有审阅人。

1. 在 **添加文件**，通过从计算机中拖放或通过单击 **浏览** 并选择所需的文件。 您可以键入 **校样名称** 对于版本，或将此框留空，以使用相同的文件名，并在末尾添加版本号。

   或

   通过键入URL捕获网页作为校样的新版本。

   >[!NOTE]
   >
   >拖放仅在完全支持HTML5的浏览器中可用。 这不包括Internet Explorer 7至9和Safari。

1. 在 **工作流**，请进行以下任何更改以指定此版本校样的审阅人。

   以前版本的审阅人将替换为您添加的审阅人。

   * 更改 **所有者** 的其他用户。\
      有关所有者权限的信息，请参阅 [在Workfront校样中校样权限配置文件](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * 使用 **键入联系人姓名或电子邮件地址以添加收件人框**，将审阅人添加到版本中。 您可以指定 **校样角色** 和 **电子邮件警报** 为每个收件人键入。

      有关向校样添加组的信息，请参阅  [将组添加到校样](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md). 有关角色的信息，请参阅 [在Workfront校样中管理校样角色](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      >[!NOTE]
      >
      >如果校样的创建者或所有者 [校样制作的电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) 默认情况下处于禁用状态（在其个人设置中），即使在“New proof”（新建校样）页面上选中“Notify poyel by email”（通过电子邮件通知人员）框，用户也不会收到任何校样或新校样电子邮件。 有关电子邮件通知的信息，请参阅 [在Workfront校样中配置电子邮件通知设置](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md). 另请参阅 [校样制作的电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) 和 [新校样电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * 为版本设置校样截止时间。
   * 将鼠标悬停在审阅人的姓名上，可查看他/她对之前版本做出的任何决策。

1. 在 **电子邮件通知**，执行以下任一操作：

   * 指定是否要通知审阅人新版本。\
      您的选择将记录在校样详细信息页面的活动部分。 有关更多信息，请参阅 [在Workfront校样中管理校样详细信息](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * 添加自定义主题和消息。

1. 在 **组织** ，请执行以下任一操作： 

   * 对校样应用一个或多个标记。 有关更多信息，请参阅 [在Workfront校样中创建和管理标记](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).\
      请注意，标记也从校样的先前版本继承。 如果向新版本添加新标记，则先前版本也会进行标记。

   * 将版本添加到文件夹。 请参阅 [在Workfront校样中管理文件夹](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) 以了解更多信息。 文件夹将从校样的先前版本复制。 如果您选择其他文件夹，则会移动整个校样（所有版本）。

   * 账单管理员和管理员可以在“设置”选项卡上将整个帐户中的文件夹字段设为必填字段。 有关更多信息，请参阅。

1. 在校样设置下，进行以下任何更改：

   * 需要在校样上登录
   * 需要验证电子签名（仅限企业计划）
   * 在做出所有决定时锁定证据
   * 允许或阻止下载原始文件
   * 公开共享校样，包括公开共享设置
   * 订阅校样\
      在此部分中所做的选择将显示在校样详细信息页面中（其中可以编辑一些字段）。 有关更多信息，请参阅 [在Workfront校样中管理校样详细信息](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

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

如果校样的先前版本中包含自定义主题/消息，则默认情况下会在新版本页面上显示该主题/消息。 您能够:

* 编辑主题和消息。
* 取消选中“通过电子邮件通知人员”框，这表示不会向审阅人发送电子邮件，以通知他们有待审阅的新版本。

   >[!NOTE]
    不受个人设置中保存的任何默认自定义主题/消息的影响。

如果您的个人设置中保存了默认主题和消息，则这将影响新版本页面上默认显示的消息内容：

* 如果您选择使用标准电子邮件（例如，无自定义主题/消息）通过电子邮件通知审阅人校样的先前版本，则您的默认自定义主题/消息（您的个人设置）将显示在新版本页面上。 然后，您可以编辑自定义主题和消息，或取消选中“通过电子邮件通知人员”框（这意味着不会向您的审阅人发送任何电子邮件以通知他们有待审阅的新版本）。
* 如果您选择不通过电子邮件通知审阅人校样的早期版本（例如，没有标准或自定义电子邮件），则新版本页面将默认不包含任何消息。 要通知您的审阅人新版本，请单击发送消息链接，该链接将显示默认的自定义主题/消息（根据您的个人设置）。 然后，您可以根据需要编辑自定义主题和消息。

如果您没有在个人设置中保存的默认主题和消息，则新版本页面上将显示以下内容：

* 如果您选择使用标准电子邮件（例如，无自定义主题/消息）通过电子邮件通知审阅人校样的先前版本，则“新版本”页面中将默认选中“通过电子邮件通知人员”选项。 要添加自定义消息，请单击链接。
* 如果您选择不通过电子邮件通知审阅人校样的早期版本（例如，没有标准或自定义电子邮件），则新版本页面将默认不包含任何消息。 要通知您的审阅人新版本，请单击发送消息链接。 然后，您可以通过单击添加自定义消息链接来添加自定义主题和消息。
