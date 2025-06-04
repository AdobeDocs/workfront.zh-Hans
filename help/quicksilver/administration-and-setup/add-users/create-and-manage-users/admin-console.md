---
title: 在Adobe Admin Console中管理用户
description: Adobe管理员可以使用Adobe Admin Console创建Adobe Workfront用户和系统管理员。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: 14e47364f88b756a2fa25d66ee9f2d85a57c8161
workflow-type: tm+mt
source-wordcount: '1520'
ht-degree: 0%

---

# 在Adobe Admin Console中管理用户

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>本文中的功能仅在贵组织的Workfront实例已载入到Adobe Business Platform时才可用。
>
>有关因贵组织是否已登记到Adobe业务平台而不同的过程列表，请参阅[基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

Adobe管理员可以使用Adobe Admin Console创建Adobe Workfront系统管理员。 该控制台是管理整个组织中的Adobe权利的中心位置。 有关详细信息，请参阅[Admin Console概述](https://helpx.adobe.com/cn/enterprise/using/admin-console.html)。

>[!NOTE]
>
>* 必须在Adobe Admin Console中配置&#x200B;**Workfront管理员。**&#x200B;有关信息和说明，请参阅本文中的[使用Adobe Admin Console在Workfront中创建系统管理员](#create-system-administrators-in-workfront-with-the-adobe-admin-console)。
>* **如果您的组织使用单点登录(SSO)**，我们建议您在Adobe Admin Console中创建用户并将他们分配到Workfront。 可以在Workfront中创建这些用户，但根据贵组织的Admin Console的配置方式，将该信息传输到Adobe Admin Console时可能会出现问题。
>  &#x200B;>   在Adobe Admin Console中创建用户后，您可以在Workfront中配置用户信息，例如分配角色、组、团队和访问级别。
>* **如果您的组织不使用单点登录(SSO)**，则可以直接在Workfront中添加非系统管理员用户。 您可以在Adobe Admin Console中添加用户，但通过在Workfront中添加用户，您可以在创建用户时设置其访问级别，这可以节省您的时间。

从Admin Console更改用户配置文件时，更新将添加到Workfront中用户的系统活动选项卡中。 更新显示为“System”（系统）。 这是指Adobe Admin Console管理员，而非Workfront主管理员。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe管理员权限</td> 
   <td> <p>您必须是贵组织的Adobe产品的产品配置文件管理员</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在使用Admin Console for Workfront之前，您应该会收到一封电子邮件，邀请您进入控制台。

1. 如果您是初次使用Adobe，并且已收到一封电子邮件，告知您现在拥有管理贵组织的Adobe软件和服务的管理权限，请单击电子邮件中的按钮以创建Adobe帐户并打开Admin Console。

   或

   如果您已经拥有Adobe帐户，请转到[Adobe Admin Console页面](https://adminconsole.adobe.com/)。

## 有关Adobe Admin Console的其他详细信息

* Workfront系统管理员可以从Workfront中停用Workfront用户，但这不会在Admin Console中停用该用户。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* 根据创建用户&#x200B;**主组**&#x200B;的用户确定用户。 这不能从Admin Console中进行自定义。
* 只能从Adobe Admin Console中编辑Workfront系统管理员访问级别。

  <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* 将用户访问权限从系统管理员更改为任何其他访问级别，必须首先通过Admin Console完成。

  <!--
   This is not clear
  -->

* 要从Workfront中的用户删除系统管理员访问权限，您必须使用Adobe Admin Console以产品配置文件管理员身份删除该用户。 这会将用户的Workfront访问级别从系统管理员更改为请求者。

  >[!IMPORTANT]
  >
  >请勿对产品配置文件本身进行任何更改。

* Adobe Admin Console管理员可以设置自动分配规则，以自动将Adobe产品分配给组织中的用户。 您的组织必须迁移到Adobe Unified Experience才能使用此功能。 有关更多信息和说明，请参阅Adobe文档中的[管理自动分配规则](https://helpx.adobe.com/enterprise/using/automatic-assignment-rules.html)。

  >[!NOTE]
  >
  >如果在配置自动分配时选择受信任的组织，则可在“所选目录或域中的用户”区域中找到该组织。 单击&#x200B;**选择目录**&#x200B;字段旁边的下拉箭头并选择组织。 受信任的组织标有“受信任”徽章。

## 访问Workfront生产实例的用户和管理区域 {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. 从[Adobe Admin Console页面](https://adminconsole.adobe.com/)中，选择顶部导航栏中的&#x200B;**产品**&#x200B;选项卡，然后选择&#x200B;**Workfront**。

   <!--![Admin Console product](assets/admin-product-1.png)-->

1. 在显示的列表中，选择顶部的链接。

   这是用户工作的生产实例。

   <!--![Admin Console instances](assets/instances-1.png)-->

   >[!TIP]
   >
   >列表中的第二个链接，即预览实例，是一个复制实时生产环境的测试环境。 有关详细信息，请参阅[Adobe Workfront预览沙盒环境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)。
   >
   >
   >您还可能在列表中看到指向沙盒环境的链接。 有关详细信息，请参阅[Adobe Workfront预览沙盒环境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)。

1. 在显示的列表中选择&#x200B;**产品配置文件**&#x200B;选项卡后，单击Workfront产品配置文件链接的名称。

   ![产品配置文件](assets/prod-profile-1.png)

   此列表包含已分配给您的Workfront生产实例的所有用户。

   >[!IMPORTANT]
   >
   >请勿对产品配置文件本身进行任何更改。

1. 继续阅读本文中的以下章节之一：

   * [使用Adobe Admin Console在Workfront中创建用户](#create-users-in-workfront-with-the-adobe-admin-console)
   * [在Workfront中使用Adobe Admin Console创建系统管理员](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## 在Workfront中使用Adobe Admin Console创建系统管理员 {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

<!--Audited: 12/2023-->

仅在Adobe Admin Console上授予系统管理员访问级别。 您无法在Workfront中授予或删除管理员访问权限。

您必须先将用户添加到Workfront的生产实例，然后才能将用户设为Workfront系统管理员。

1. 按照本文中[访问Workfront生产实例的用户和管理区域](#access-the-user-and-admin-area-for-your-production-instance-of-workfront)一节中的说明，转到Admin Console中的用户和管理区域。
1. 选择用户列表上方的&#x200B;**管理员**&#x200B;选项卡。
1. 选择&#x200B;**添加管理员**。
1. 在&#x200B;**添加产品配置文件管理员**&#x200B;框中，输入要添加的管理员的电子邮件地址或名称，然后选择&#x200B;**保存**。

   ![添加管理员](assets/add-admin-1.png)

   在Workfront中创建系统管理员。

   >[!IMPORTANT]
   >
   >请勿对产品配置文件本身进行任何更改。


## 在Workfront中使用Adobe Admin Console创建用户 {#create-users-in-workfront-with-the-adobe-admin-console}

>[!NOTE]
>
>我们建议直接在Workfront中添加非系统管理员用户。 您可以在Adobe Admin Console中添加用户，但通过在Workfront中添加用户，您可以在创建用户时设置其访问级别，这可以节省您的时间。

* [直接在Adobe Admin Console的Workfront中创建用户](#create-users-in-workfront-directly-in-the-adobe-admin-console)
* [在Workfront中创建用户并批准他们用于Adobe Admin Console](#create-users-in-workfront-and-approve-them-for-the-adobe-admin-console)

### 直接在Adobe Admin Console的Workfront中创建用户

1. 按照本文中[访问Workfront生产实例的用户和管理区域](#access-the-user-and-admin-area-for-your-production-instance-of-workfront)一节中的说明，转到Admin Console中的用户和管理区域。
1. 选择列表上方的&#x200B;**用户**&#x200B;选项卡，选择&#x200B;**添加用户**。
1. 在&#x200B;**将用户添加到此产品配置文件**&#x200B;框中，输入要添加的用户的电子邮件地址或名称，然后选择&#x200B;**保存**。

   将使用请求者访问级别在Workfront中创建用户。

   >[!IMPORTANT]
   >
   >请勿对产品配置文件本身进行任何更改。

1. 在Workfront中，更改用户的访问级别。

   有关Workfront管理员如何更改用户访问级别的说明，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

1. 重复步骤3和4以添加更多用户。

   >[!NOTE]
   >
   >对于新的Adobe用户，Admin Console会发送一封电子邮件，邀请他们完成注册流程。 所有用户都必须完成注册过程才能访问任何Adobe应用程序。
   >
   >对于现有Adobe用户，用户可能会收到也可能不会收到有关Workfront可用性的电子邮件。 这是由Adobe管理员控制的产品首选项。 您的Adobe管理员可能与Workfront管理员不同。

### 在Workfront中创建用户并批准他们用于Adobe Admin Console

此工作流允许无权访问Adobe Admin Console的组管理员创建用户。

首先，组管理员在Workfront中创建用户。 这将创建处于已停用和未决批准状态的用户。

之后，Workfront管理员会批准用户。 这会在Workfront中激活用户并将他们添加到Adobe Admin Console。

#### 在Workfront中创建用户（组管理员）

有关在Workfront中创建用户的说明，请参阅[添加用户](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/add-users.md)。

#### 批准用户(Workfront管理员)

批准用户：

{{step-1-to-users}}

1. 选择用户，然后单击&#x200B;**更多**&#x200B;图标![更多图标](assets/more-icon.png)。

1. 要批准用户，请单击&#x200B;**批准**，然后单击&#x200B;**提交**。

   或

   要拒绝用户并从Workfront中删除用户，请单击&#x200B;**拒绝**，然后单击&#x200B;**提交**。

   批准的用户会自动添加到Adobe Admin Console。

   被拒绝的用户会自动从Workfront中删除。


## 在Adobe Admin Console中编辑现有用户

您可以在Adobe Admin Console中编辑以下用户详细信息：

* 用户组以及与用户关联的产品
* 管理权限
* 国家/地区

有关在Adobe Admin Console中编辑单个用户的信息，请参阅Adobe文档中的单独管理用户一文中的[编辑用户详细信息](https://helpx.adobe.com/enterprise/using/manage-users-individually.html#edit-user-details)。

有关在Adobe Admin Console中批量编辑用户的信息，请参阅
在Adobe的“管理多个用户”一文中，[编辑用户详细信息](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html#edit-user-details)。
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>You can create Adobe Workfront users and system administrators with the <a href="https://adminconsole.adobe.com/" alt="Admin Console link">Adobe Admin Console</a>. The console is a central location for managing the Adobe entitlements across your organization. For more information, see the <a href="https://helpx.adobe.com/enterprise/using/admin-console.html" alt="Admin Console Overview">Admin Console Overview</a>.</p>
<p>Before using the Admin Console for Workfront, you should receive a receive an email inviting you to the console. Click in the invitation to accept it and create an account. You can also use an existing account, if already available.</p>
<h2>Create users</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Create users in WF with the Adobe admin console</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">May need to add something about oging throug WF -- check with Jonah</p>

<p>To create users in Workfront with the Admin Console:</p>
<ol>
<li value="1"> <p>From the <a href="https://adminconsole.adobe.com/">Admin Console page</a>, select the <b>Products</b> tab and then select the <b>Workfront</b> product tile.</p> </li>
<li value="2"> <p>Select the link to the Workfront instance you want to change.</p> </li>
<li value="3"> <p>Select the Product profile link. This shows a list of the currently-assigned users. If the list is very long, you can also search for users in the search field above the list.</p> </li>
<li value="4"> <p>Select the <b>Add User</b> button.</p> </li>
<li value="5"> <p>In the <b>Add users</b> box, enter the email address or name of the user you want to add. Select <b>Save</b>. The administrator is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Create system administrators</h2>
<p>To create system administrators:</p>
<ol>
<li value="1"> <p>Make product profile assignments first. To be a Workfront System Administrator, the user must be assigned the Workfront product profile and be an admin for that product profile.</p> </li>
<li value="2"> <p>From the console, select the <b>Products</b> tab and then select the <b>Admins</b> tab. </p> </li>
<li value="3"> <p>Select <b>Add Admin</b>.</p> </li>
<li value="4"> <p>In the <b>Add product profile administrators</b> box, enter the email address or name of the administrator you want to add. Select <b>Save</b>. The user is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Additional details for the Admin Console</h2>
<ul>
<li> <p>System Administrator access level is granted only on the Admin Console. You cannot grant or remove admin access from within Workfront.</p> </li>
</ul>
<ul>
<li> <p>Creating and deleting users inside Workfront is only possible through the Admin Console.</p> </li>
<li> <p>Workfront System Administrators can deactivate Workfront users from within Workfront, but this does not deactivate the user in the Admin Console.</p> </li>
<li> <p>All new users are are assigned <b>Requestor</b> access level upon creation. Also, the user <b>Home Group</b> is determined based on the user who created them. This is currently not customizable from within the Admin Console.</p> </li>
<li> <p>The Workfront System Administrator access level can only be edited from within the Adobe Admin Console.</p> </li>
<li> <p>Editing a user who is a system admin to any other access level must be done through the Admin Console first.</p> </li>
<li> <p>To remove Workfront system admin access, remove users as Product Profile Administrators. This action changes the user access level in Workfront from a system admin to a <b>Requestor</b>.</p> </li>
</ul>
</div>
-->
