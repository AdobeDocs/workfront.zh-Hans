---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 管理向新用户发送的电子邮件邀请
description: 作为Adobe Workfront管理员，您可以将用户添加到Workfront，并通过电子邮件邀请通知他们已添加用户。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---

# 管理向新用户发送的电子邮件邀请

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>此页面中描述的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>有关根据贵组织是否已载入Adobe Admin Console而有所不同的步骤列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

作为Adobe Workfront管理员，您可以将用户添加到Workfront，并通过电子邮件邀请通知他们已添加用户。

电子邮件邀请允许新用户关注一个链接，在该链接中，他们可以为其Workfront帐户选择密码。 然后，他们可以完成帐户设置。

为确保新帐户的安全性，我们建议您为新用户使用电子邮件邀请，以便他们可以选择自己的密码。 或者，您也可以在创建新用户帐户时为其选择密码。 有关将新用户添加到Workfront的更多信息，请参阅 [添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

您可以为以下对象配置新用户电子邮件：

* 任何新用户已添加到Workfront
* 已使用请求者许可证添加到Workfront的用户

发送电子邮件邀请后，所有新用户都会看到同一电子邮件。

有关接收电子邮件邀请的信息，请参阅 [接收电子邮件邀请并为Adobe Workfront创建密码](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

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
   <td> <p>系统管理员</p> </td> 
  </tr> 
 </tbody> 
</table>

## 生成电子邮件邀请 {#generate-email-invitations}

电子邮件邀请在以下情况下生成：

* 创建新用户并选择 **向此人发送邀请电子邮件** 在 **新用户** 表单。 有关创建新用户的更多信息，请参阅 [添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* 在导入多个新用户并选择 **向这些人员发送邀请电子邮件** 选项。 有关导入多个新用户的更多信息，请参阅 [导入用户](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* 创建用户后，您可以手动生成邀请，以发送给尚未在Workfront中注册其帐户且尚未建立Workfront密码的用户。\
   已创建帐户但尚未注册其帐户的用户将被标记为 **未注册** 在Workfront。

   >[!NOTE]
   >
   >如果取消选择 **向此人发送电子邮件邀请** 框中，无法手动生成电子邮件邀请。 只有在创建帐户时已发送原始电子邮件邀请的用户，才可以手动重新发送电子邮件邀请。 有关创建新用户的更多信息，请参阅 [添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

要手动为现有未注册用户生成电子邮件邀请，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **用户** ![](assets/users-icon-in-main-menu.png).
1. 选择显示 **未注册** 标签。

   ![](assets/unreg-user-qs-350x221.png)

1. 单击更多图标 ![](assets/more-icon.png)，然后单击 **提醒用户注册**.

   系统会向新用户发送一封电子邮件邀请，其中包含他们可用于创建Workfront密码的新链接。

   >[!NOTE]
   >
   >如果贵组织已载入Admin Console，并且您通过Workfront添加了用户，则无法选择向新用户发送电子邮件邀请。
   >
   >新的Adobe用户会添加到Admin Console,Admin Console会发送一封电子邮件邀请他们完成注册流程。 所有用户必须完成注册过程才能访问任何Adobe系统。
   >
   >对于现有Adobe用户，用户可能会（也可能不会）收到有关Workfront可用的电子邮件。 这是由Adobe管理员控制的产品首选项。

## 配置电子邮件邀请 {#configure-email-invitations}

作为Workfront管理员，您可以配置包含在新用户电子邮件邀请中的消息。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧的列表中，单击 **电子邮件** > **邀请**.

1. 在 **常规选项** 部分进行以下任何修改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>...天后停用邀请链接</strong> </td> 
      <td> <p>选择电子邮件邀请在多长时间后不再包含指向Workfront的有效链接。 默认天数为45天。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>包括消息和/或服务期限</strong> </td> 
      <td> <p>如果要修改添加到Workfront的所有新用户的电子邮件邀请，请选择此选项。 这不包括具有请求者许可证的用户。</p> 
       <ul> 
        <li><strong>消息</strong>:如果选择修改所有新用户的电子邮件邀请，请指定要作为电子邮件正文包含在电子邮件邀请中的文本。</li> 
        <li><strong>条款和条件</strong>:如果选择修改所有新用户的电子邮件邀请，请指定要作为条款和条件包含在电子邮件邀请中的文本。<br></li> 
        <li><strong>包括面向服务台用户的消息和/或服务期限</strong>:如果要修改添加到Workfront且具有请求者许可证的所有新用户的电子邮件邀请，请选择此选项。</li> 
        <li><strong>消息</strong>:如果您选择修改具有请求者许可证的所有新用户的电子邮件邀请，请指定要作为电子邮件正文包含在电子邮件邀请中的文本。</li> 
        <li><strong>条款和条件</strong>:如果您选择修改具有请求者许可证的所有新用户的电子邮件邀请，请指定要作为条款和条件包含在电子邮件邀请中的文本。<br></li> 
        <li> <p>在 <strong>邀请预览</strong> 部分，则可以查看电子邮件邀请的预览。 如果您选择在电子邮件邀请中包含自定义消息，则此区域会显示自定义消息。</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。
