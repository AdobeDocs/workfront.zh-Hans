---
title: 以其他用户身份登录
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作为Adobe Workfront管理员，您有时可能需要代表其他用户访问Workfront。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

# 以其他用户身份登录

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>本页所述的程序仅适用于尚未载入Adobe Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则此操作不可用。
>
>有关根据贵组织是否已载入Adobe Admin Console而有所不同的步骤列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

作为Adobe Workfront管理员，您有时可能需要代表其他用户访问Workfront。

或者，作为组管理员，您可能需要代表您所管理组的成员用户访问Workfront。

例如，如果在休假用户执行某项操作之前任务无法继续，则您可以以该用户身份登录，然后改为执行该操作。

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
>由于文档集成可能会连接到私人个人文件，因此管理员在以其他用户身份登录时无法访问文档集成。
>
>有关文档集成的更多信息，请参阅 [配置文档集成](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>使用系统管理员访问级别，您可以以任何人身份登录。 有关此访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>. </p> <p>使用计划员访问级别，您可以以具有较低许可证级别的用户身份登录，如果 <b>用户</b> 在访问级别中的设置配置为 <b>编辑</b> 访问，使用 <b>创建</b> 至少两个中的一个 <b>用户管理员</b> 在 <b>优化设置</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>注意</b>:在这两个选项中，如果用户 <b>管理员（群组用户）</b> 启用后，您必须是用户所属的组的组管理员。</p> 
   <p>有关 <b>用户</b> 在访问级别中设置，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 以其他用户身份登录并执行操作

1. 以Workfront管理员或群组管理员身份登录Workfront。

   >[!NOTE]
   >
   >* 如果您是群组管理员，则只能以您管理的群组中的用户身份登录。 此外，必须在您的访问级别启用用户管理员（群组用户）权限：
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  默认情况下，此设置处于禁用状态。 有关更多信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* 无法重置Workfront管理员的密码。


1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **登录方式**.

1. 在 **用户** 框 **登录方式** 选项卡，开始键入用户的名称，然后在下拉列表中显示该名称时单击该名称。

   用户必须在Workfront中定义访问级别。 您无法以无权登录的用户身份登录Workfront系统。

   >[!NOTE]
   >
   >群组管理员只能作为其所管理群组的成员用户登录。 他们无法以Workfront管理员身份登录。

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

   当您以其他用户身份登录时，屏幕顶部会显示一条通知以指示此情况。

1. 作为用户执行了必要的操作后，单击 **注销。**

## 管理员以其他用户身份登录时跟踪和审核活动

Workfront提供了用于跟踪和审核管理员以其他用户身份登录期间发生的活动的机制。

当您以其他用户身份登录时，该用户的上次登录日期将被修改，直至系统或组管理员以该用户身份登录的日期。

* [查看项目指标](#view-indicators-on-items)
* [查看审核信息](#view-audit-information)

### 查看项目指标 {#view-indicators-on-items}

当您以其他用户身份登录Workfront并执行某项操作时，Workfront会明确指示您所执行的任何操作都是由您代表以身份登录的用户执行的。

例如，如果您以其他用户身份登录时对某个项目进行评论，则会有一条语句指示该评论是由您代表该用户做出的。

### 查看审核信息 {#view-audit-information}

1. 以Workfront管理员或组管理员身份登录Workfront。
1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **登录为，** 然后单击 **访问日志** 选项卡。

   每当系统或组管理员以其他用户身份登录Workfront时，该事件都会记录在审核跟踪中。 此外，管理员以其他用户身份登录时发生的任何可审核操作都将记录在审核跟踪中。

1. （可选）您可以通过以下方式过滤审核跟踪中显示的结果：

   * 按已登录的用户
   * 按已登录为
   * 按日期
