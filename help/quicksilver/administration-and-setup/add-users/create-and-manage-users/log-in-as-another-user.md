---
title: 以其他用户身份登录
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作为Adobe Workfront管理员，有时您可能需要代表其他用户访问Workfront。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: f8d04790caefd12c9811ea3ed94e1f892311d031
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# 以其他用户身份登录。

<!--Audited: 5/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

作为Adobe Workfront管理员，有时您可能需要代表其他用户访问Workfront。 或者，作为组管理员，您可能需要代表您管理组的成员用户访问Workfront。

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
>有关文档集成的详细信息，请参阅[配置文档集成](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td> 
  </tr>
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>您必须具备以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 这允许您以任何人的身份登录。</li> 
     <li> <p>访问级别中的<b>用户</b>设置配置为<b>编辑</b>访问，其中<b>创建</b>以及<b>微调设置</b> <b>下至少启用</b>用户管理员<img src="assets/gear-icon-in-access-levels.png">选项之一。 这允许您以较低许可证级别的用户身份登录。 </p> <p>在这两个选项中，如果启用了<b>用户管理员（组用户）</b>，您必须是该用户所属组的组管理员。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 以其他用户身份登录并执行操作

1. 以Workfront管理员或组管理员身份登录到Workfront。

   >[!NOTE]
   >
   >* 如果您是组管理员，则只能以所管理组中的用户身份登录。 此外，必须在您的访问级别中启用“用户管理员（组用户）”权限：
   >   
   >  ![组管理员用户](assets/group-admin-user.png)
   >   
   >  默认情况下禁用此设置。 有关详细信息，请参阅[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。
   >   
   >* 您无法重置Workfront管理员的密码。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**登录身份**。

1. 在&#x200B;**登录身份**&#x200B;选项卡的&#x200B;**开始键入名称……**&#x200B;框中，开始键入用户的名称，然后在名称出现在下拉列表中时单击该名称。


   >[!NOTE]
   >* 您选择的用户必须具有Workfront中定义的访问级别。 您无法以无权登录的用户身份登录Workfront系统。
   >* 组管理员只能以他们管理的组的成员用户身份登录。 他们无法以Workfront管理员身份登录。

1. 单击&#x200B;**登录**。 您以其他用户身份登录，屏幕顶部会显示一条通知来指示此信息。

   <!--
   <p> Might come in a future story:</p>
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



1. 以用户身份执行了必要的操作后，单击屏幕顶部的&#x200B;**注销**。

## 在管理员以其他用户身份登录时跟踪和审核活动

Workfront提供多种机制，用于跟踪和审核管理员以其他用户身份登录时发生的活动。

以其他用户身份登录时，该用户的最后登录日期将修改为系统或组管理员以该用户身份登录的日期。

* [查看项目指示器](#view-indicators-on-items)
* [查看审核信息](#view-audit-information)

### 查看项目指示器 {#view-indicators-on-items}

当您以其他用户身份登录Workfront并执行某个操作时，Workfront明确指示您执行的任何操作都是由您代表您以身份登录的用户执行的。

例如，如果您在以其他用户身份登录时对某个项目进行注释，则语句表示您在查看对象的Updates部分时代表该用户发表了注释。

### 查看审核信息 {#view-audit-information}

1. 以Workfront管理员或组管理员身份登录到Workfront。
   {{step-1-to-setup}}
   <!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

1. 在左侧面板中，单击&#x200B;**登录身份**，然后单击&#x200B;**访问日志**&#x200B;选项卡。

   >[!NOTE]
   >
   >每当系统或组管理员以其他用户身份登录到Workfront时，该事件即被记录到审核记录中。 此外，当管理员以其他用户身份登录时，发生的任何可审核操作都会记录到审核跟踪中。

1. （可选）您可以通过以下方式筛选审计跟踪中显示的结果：

   * 按已登录的用户
   * 按已登录的用户
   * 按日期和时间
