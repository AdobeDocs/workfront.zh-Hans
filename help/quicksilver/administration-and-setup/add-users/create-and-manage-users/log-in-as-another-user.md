---
title: 以其他用户身份登录
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作为Adobe Workfront管理员，有时您可能需要代表其他用户访问Workfront。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 8be7534dfc0a1227bd2274ad093a88ae19b4691d
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 0%

---

# 以其他用户身份登录


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>本页中介绍的过程仅适用于尚未载入Adobe Admin Console的组织。 如果您的组织已载入到Adobe Admin Console，则此操作不可用。
>
>有关因您的组织是否已登记到Adobe Admin Console而不同的过程列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

作为Adobe Workfront管理员，有时您可能需要代表其他用户访问Workfront。

或者，作为组管理员，您可能需要代表您管理组的成员用户访问Workfront。

例如，如果任务在休假用户执行某项操作之前无法进度，您可以以该用户身份登录并执行该操作。

<!--
<note type="note">
Some users, such as executives, need to be able to control which administrators can log in to their accounts, and for how long. Working with your organization, Workfront configures settings that allow this control for these users. When a Workfront administrator or group administrator (associated with one of the user's groups) tries to log in as one of these users, an on-screen message prompts the administrator to contact the user for access. From the user profile area, the user can then grant access to the administrator and specify an expiration time for it. For more information on how the user does this, see
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#access" class="MCXref xref">Access</a> in
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.
<span class="PinkDraftNote">[Add a note about this being only for the Enterprise package if they decide to do it that way]</span>
</note>
-->

>[!NOTE]
>
>由于文档集成可能会连接到个人专用文件，因此管理员在以其他用户身份登录时无法访问文档集成。
>
>有关文档集成的详细信息，请参阅 [配置文档集成](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>使用“系统管理员”访问级别，您可以作为任何人都登录。 有关此访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理权限</a>. </p> <p>使用Planner访问级别，您可以作为较低许可证级别的用户登录，如果 <b>用户</b> 访问级别中的设置配置为 <b>编辑</b> 访问，使用 <b>创建</b> 而且至少两者 <b>用户管理员</b> 下启用的选项 <b>微调您的设置</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>注意</b>：如果用户，则为这两个选项中的一个 <b>管理员（组用户）</b> 启用，您必须是用户所属的组的组管理员。</p> 
   <p>欲知关于 <b>用户</b> 在访问级别中设置，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 以其他用户身份登录并执行操作

1. 以Workfront管理员或组管理员身份登录到Workfront。

   >[!NOTE]
   >
   >* 如果您是组管理员，则只能以所管理组中的用户身份登录。 此外，必须在您的访问级别中启用“用户管理员（组用户）”权限：
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  默认情况下禁用此设置。 有关更多信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* 您无法重置Workfront管理员的密码。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **登录身份**.

1. 在 **用户** 上的框 **登录身份** 选项卡，开始键入用户的名称，然后在名称出现在下拉列表中时单击该名称。

   用户必须具有在Workfront中定义的访问级别。 您无法以无权登录的用户身份登录Workfront系统。

   >[!NOTE]
   >
   >组管理员只能以他们管理的组的成员用户身份登录。 他们无法以Workfront管理员身份登录。

1. 单击 **登录。**

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Might come in a future story:</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">click an Access period and then click Request to ask the user for access to log as him or her for the specified period of time. Continue these steps after the user grants access. Specify somewhere here that this is only for the Enterprise package if they decide on that</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Or </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a prompt appears indicating that the user has restricted access to their account, contact the user to request access.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The user can then can grant you "Log in as" access in their user profile. They can also specify an expiration date and time for the access period. </p>
   -->

   <!--
   This triggers an email to let you know that you have access to log in as the user, depending on how your event notifications are enabled. For more information, see <a href="../../../workfront-basics/using-notifications/event-notifications.md" class="MCXref xref">Event notifications</a>.
   </div>
   -->

   当您以其他用户身份登录时，屏幕顶部会显示一条通知来指示此情况。

1. 以用户身份执行必要的操作后，单击 **注销。**

## 在管理员以其他用户身份登录时跟踪和审核活动

Workfront提供多种机制，用于跟踪和审核管理员以其他用户身份登录时发生的活动。

以其他用户身份登录时，该用户的最后登录日期会被修改为系统或组管理员以该用户身份登录的日期。

* [查看项目指示器](#view-indicators-on-items)
* [查看审核信息](#view-audit-information)

### 查看项目指示器 {#view-indicators-on-items}

当您以其他用户身份登录Workfront并执行某个操作时，Workfront明确指示您执行的任何操作都是由您代表您以身份登录的用户执行的。

例如，如果您在以其他用户身份登录时对某个项目进行注释，则会显示一条语句，指示您代表该用户发表了注释。

<!--remove the note below when we bring this back to Prod: -->

>[!NOTE]
>
>使用新的评论体验时，评论会添加为以其他用户身份登录的用户，而不会指示他们代表其他人添加评论。
>
>例如，如果Workfront管理员以其他用户身份登录，则与评论关联的用户是Workfront管理员。 有关更多信息，请参阅 [新的评论体验](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


### 查看审核信息 {#view-audit-information}

1. 以Workfront管理员或组管理员身份登录到Workfront。
1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **登录身份，** 然后单击 **访问日志** 选项卡。

   每当系统或组管理员以其他用户身份登录到Workfront时，该事件即被记录到审核记录中。 此外，当管理员以其他用户身份登录时，发生的任何可审核操作都会记录到审核跟踪中。

1. （可选）您可以通过以下方式筛选审计跟踪中显示的结果：

   * 按已登录的用户
   * 按已登录的用户
   * 按日期
