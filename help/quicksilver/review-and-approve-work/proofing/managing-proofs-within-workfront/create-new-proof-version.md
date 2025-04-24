---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 创建新版本的验证
description: 跨工作项的多个版本或修订版本管理反馈可能是一项巨大的挑战。 Workfront通过允许您创建和比较验证的多个版本来简化此过程。
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '1523'
ht-degree: 0%

---

# 创建新版本的验证

<!-- Audited: 4/2025 -->

跨工作项的多个版本或修订版本管理反馈可能是一项挑战。 Adobe Workfront通过允许您创建和比较验证的多个版本来简化此过程。

创建新版本的验证时，请考虑以下信息：

* 您可以授予用户查看一个版本的权限，但不能授予用户查看另一个版本的权限。 相反，如果您与某个用户共享较新的版本，则该用户将无法查看较早版本，除非您返回并向他们授予对这些早期版本的访问权限。
* 您必须对验证具有“编辑”权限才能创建新版本。

  有关详细信息，请参阅[在Workfront Proof中管理验证角色](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)和[在Workfront Proof中管理验证权限配置文件](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)。

  有关共享校样版本的信息，请参阅  [在Workfront Proof中共享校对](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)。

>[!IMPORTANT]
>
>如果在Adobe Workfront中创建验证，则还必须在Workfront中创建该验证的任何新版本。 如果验证是在Workfront Proof中创建的，则无法在Workfront中创建该验证的新版本。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>当前： Pro或更高版本</p> <p>或</p> <p>旧版：选择或Premium</p> <p>有关使用其他计划进行验证访问的更多信息，请参阅<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>当前：标准</p> 
   <p>或</p>
   <p>旧版：工作或计划（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在Workfront中创建新验证版本

可通过多种方式在Workfront中上传新验证版本。 默认验证设置可能会也可能不会延续到以前的版本，具体取决于您选择的方法：

* **上载文档时自动生成验证**：如果您在用户配置文件中启用了此设置，则在拖放新版本时默认验证设置不会延续。
* **创建校对>简单**：如果选择此选项，则默认校对设置不会延续到以前的版本。
* **新增>版本>验证**：如果选择此选项，则默认验证设置会从以前的版本延续。
* **创建校对>高级**：如果选择此选项，则默认校对设置会延续到以前的版本。

要创建新版本的验证，请执行以下操作：

1. 打开包含校对的文档列表。
1. 从计算机的文件系统中，将新文件拖放到验证上。

   或

   选择列出校对的行，单击&#x200B;**新增** > **版本**，然后单击要用于添加新版本的校对的选项。

   ![添加新版本](assets/add-new-proof-version.png)

## 从验证查看器创建新验证版本(仅限Workfront Proof)

如果您使用的是独立的Workfront Proof，则可以创建包含单个文件或Web捕获的新版本验证。 

>[!NOTE]
>
>如果您的帐户是企业计划，并且您上传了多个文件或Web捕获，则这些文件或捕获会自动合并到单个新版本中。 有关详细信息，请参阅[创建多页校对](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)。

要在Workfront Proof中创建新版本的验证，请执行以下操作：

1. 打开证明。
1. 在左上角，单击&#x200B;**版本**&#x200B;下拉菜单，然后在出现的框中单击&#x200B;**+新版本**。 新验证版本页面将打开。

   ![添加新版本](assets/new-version-button.png)

1. 在&#x200B;**添加文件**&#x200B;部分中，通过从计算机拖放文件或单击&#x200B;**浏览**&#x200B;并选择文件来将文件作为新验证版本上载。

   或

   通过输入URL将网页捕获为验证的新版本。

   >[!NOTE]
   >
   >只有完全支持HTML5的浏览器才提供拖放功能。 这不包括Internet Explorer 7至9和Safari。

1. （可选）选择验证标题并为版本输入新的&#x200B;**验证名称**。

1. 在&#x200B;**工作流**&#x200B;部分中，进行以下任何更改以为此校对版本添加审阅人（这将替换以前版本的审阅人）：

   * （可选）将版本的&#x200B;**所有者**&#x200B;更改为帐户中的其他用户。

     有关信息，请参阅Workfront Proof中的[校对权限配置文件](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)。

   * （可选）使用&#x200B;**键入联系人姓名或电子邮件地址来添加收件人**&#x200B;框，将审阅者添加到该版本。 然后，您可以为每个收件人选择&#x200B;**验证角色**&#x200B;和&#x200B;**电子邮件警报**&#x200B;类型。

     有关信息，请参阅[将组添加到验证](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md)和[在Workfront Proof中管理验证角色](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)。

     >[!NOTE]
     >
     >如果验证创建者或所有者的个人设置中默认禁用了已制作验证的电子邮件，则即使在新验证页面上选中了&#x200B;**将此验证通知收件人**&#x200B;框，他们也不会收到任何已制作验证或新验证电子邮件。 有关信息，请参阅[在Workfront Proof中配置电子邮件通知设置](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)、[校对电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md)和[新校对电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md)。

   * （可选）设置验证截止日期。

   * （可选且视情况而定）在&#x200B;**将主要决策权限转移到**&#x200B;下拉列表中选择一个新的主要决策者。

   * （可选）选中&#x200B;**仅需要此阶段**&#x200B;的一个决策框可删除将用户设置为新的主要决策者的选项。

1. 在&#x200B;**电子邮件通知**&#x200B;部分中，选择以下任意设置：

   * （可选） **将此校对通知收件人**：选择此选项可通知新版本的审阅人。 您的选择将记录在&#x200B;**验证详细信息**&#x200B;页面的&#x200B;**活动**&#x200B;部分。 有关详细信息，请参阅[在Workfront Proof中管理校对详细信息](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)。

   * （有条件，可选）**添加自定义主题和消息**：选择此选项可向电子邮件通知添加自定义主题行和消息。

1. 在&#x200B;**组织**&#x200B;部分中，选择以下任意设置：

   * 将一个或多个标记应用于验证。 有关详细信息，请参阅[在Workfront Proof中创建和管理标签](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md)。

   * 将版本添加到文件夹。 将从该验证的先前版本复制该文件夹。 如果选择其他文件夹，则将移动整个校对（包括所有版本）。 有关详细信息，请参阅[在Workfront Proof中管理文件夹](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)。

   * 帐单管理员和管理员可以在&#x200B;**设置**&#x200B;选项卡中将文件夹字段设为整个帐户的必填字段。

1. 在&#x200B;**校对设置**&#x200B;部分中，选择以下任意设置：

   * 要求用户登录以查看验证。
   * 需要在证明上提供电子签名（仅限企业计划）。
   * 作出所有决定时锁定校对。
   * 允许下载原始文件。
   * 允许公开共享证明。
   * 允许订阅验证。

     在此部分中所做的选择将显示在&#x200B;**校对详细信息**&#x200B;页面（可以编辑某些字段）中。 有关详细信息，请参阅[在Workfront Proof中管理校对详细信息](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)。

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

如果您的个人设置中保存了默认主题和消息，这将决定新版本页面上默认显示的消息：

* 如果您使用标准电子邮件（例如，无自定义主题/消息）通知查看者以前的验证版本，则您的默认自定义主题/消息（您的个人设置）将显示在新版本页面上。 然后，您可以编辑自定义主题和消息，或取消选中通过电子邮件通知人员框，这意味着不会向审阅人发送电子邮件，通知他们有要审阅的新版本。
* 如果您未将以前的校样版本通知给审阅人（例如，没有标准或自定义电子邮件），则默认情况下，“新版本”页面不会包含消息。 要向审阅人通知新版本，请单击“发送邮件”链接，该链接将显示您的默认自定义主题/邮件（根据您的个人设置）。 然后，您可以根据需要编辑自定义主题和消息。

如果您的个人设置中未保存默认主题和消息，则新版本页面上将显示以下内容：

* 如果您使用标准电子邮件（例如无自定义主题/消息）通知查看者以前的验证版本，则默认情况下将在新版本页面上选择通过电子邮件通知人员选项。 要添加自定义消息，请单击链接。
* 如果您没有通过电子邮件通知审阅人以前的验证版本（例如没有标准或自定义电子邮件），则默认情况下，“新版本”页面不会包含任何消息。 要通知审阅者新版本，请单击发送消息链接。 然后，您可以通过单击“添加自定义消息”链接来添加自定义主题和消息。
