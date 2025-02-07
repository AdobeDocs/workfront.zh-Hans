---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 管理发送给新用户的电子邮件邀请
description: 作为Adobe Workfront管理员，您可以使用电子邮件邀请将用户添加到Workfront并通知他们已添加。
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# 管理对新用户的电子邮件邀请

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>本页中介绍的过程仅适用于尚未加入该Admin Console的组织。 如果贵组织已载入到Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>有关因贵组织是否已登记到Adobe Admin Console而不同的过程列表，请参阅[基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

作为Adobe Workfront管理员，您可以使用电子邮件邀请将用户添加到Workfront并通知他们已添加。

电子邮件邀请允许新用户访问一个链接，从中可为其Workfront帐户选择密码。 然后，他们可以完成帐户的设置。

为确保新帐户的安全，我们建议您为新用户使用电子邮件邀请，以便他们可以选择自己的密码。 或者，您也可以在创建新用户的帐户时为其选择密码。 有关向Workfront添加新用户的详细信息，请参阅[添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

您可以配置新用户电子邮件：

* 添加到Workfront的任何新用户
* 使用请求者许可证添加到Workfront的用户

发送电子邮件邀请时，所有新用户都会看到相同的电子邮件。

有关接收电子邮件邀请的信息，请参阅[接收电子邮件邀请并创建Adobe Workfront的密码](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

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
   <td> <p>系统管理员</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 生成电子邮件邀请 {#generate-email-invitations}

在以下情况下会生成电子邮件邀请：

* 当您创建新用户并在&#x200B;**新建用户**&#x200B;表单上选择&#x200B;**向此人发送邀请电子邮件**&#x200B;时。 有关创建新用户的详细信息，请参阅[添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。
* 导入多个新用户并选择&#x200B;**向这些用户发送邀请电子邮件**&#x200B;选项时。 有关导入多个新用户的详细信息，请参阅[导入用户](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md)。
* 创建用户后，您可以为尚未在Workfront中注册帐户且尚未建立Workfront密码的用户手动生成邀请。\
  在Workfront中，已创建帐户但尚未注册帐户的用户将被标记为&#x200B;**已取消注册**。

  >[!NOTE]
  >
  >如果在创建用户时取消选中&#x200B;**向此人发送电子邮件邀请**&#x200B;框，则无法手动生成电子邮件邀请。 仅当创建帐户时已发送原始电子邮件邀请的用户才可以手动重新发送电子邮件邀请。 有关创建新用户的详细信息，请参阅[添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

要手动生成发送给现有未注册用户的电子邮件邀请，请执行以下操作：

{{step-1-to-users}}

1. 选择在其名称后显示&#x200B;**已取消注册**&#x200B;标签的用户。

   ![已取消注册](assets/unreg-user-qs-350x221.png)

1. 单击“更多”图标![更多图标](assets/more-icon.png)，然后单击&#x200B;**提醒用户注册**。

   系统会向新用户发送电子邮件邀请，其中包含他们可用来创建Workfront密码的新链接。

   >[!NOTE]
   >
   >如果贵组织已登记到Admin Console，并通过Workfront添加用户，则无法向新用户发送电子邮件邀请。
   >
   >新的Adobe用户将添加到Admin Console，Admin Console会发送电子邮件邀请他们完成注册流程。 所有用户都必须完成注册过程才能访问任何Adobe系统。
   >
   >对于现有Adobe用户，用户可能会收到也可能不会收到有关Workfront可用性的电子邮件。 这是由Adobe管理员控制的产品首选项。

## 配置电子邮件邀请 {#configure-email-invitations}

作为Workfront管理员，您可以为新用户配置包含在新用户电子邮件邀请中的消息。

{{step-1-to-setup}}

1. 在左侧的列表中，单击&#x200B;**电子邮件** > **邀请**。

1. 在&#x200B;**常规选项**&#x200B;部分中，进行以下任一修改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>在……天后停用邀请链接</strong> </td> 
      <td> <p>选择电子邮件邀请不再包含指向Workfront的有效链接的时间。 默认天数是45。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>包含消息和/或服务期限</strong> </td> 
      <td> <p>如果要修改添加到Workfront的所有新用户的电子邮件邀请，请选择此选项。 这不包括拥有请求者许可证的用户。</p> 
       <ul> 
        <li><strong>消息</strong>：如果选择修改所有新用户的电子邮件邀请，请指定要包含在电子邮件邀请中的文本作为电子邮件正文。</li> 
        <li><strong>条款和条件</strong>：如果您选择修改所有新用户的电子邮件邀请，请指定要包含在电子邮件邀请中的文本作为条款和条件。<br></li> 
        <li><strong>包括帮助台用户的消息和/或服务期限</strong>：如果要修改添加到Workfront的所有新用户的电子邮件邀请（这些用户具有请求者许可证），请选择此选项。</li> 
        <li><strong>消息</strong>：如果您选择修改所有具有请求者许可证的新用户的电子邮件邀请，请指定要包含在电子邮件邀请中的文本作为电子邮件正文。</li> 
        <li><strong>条款和条件</strong>：如果您选择修改所有拥有请求者许可证的新用户的电子邮件邀请，请指定要包含在电子邮件邀请中的文本作为条款和条件。<br></li> 
        <li> <p>在<strong>邀请预览</strong>部分中，您可以看到电子邮件邀请的预览。 如果您选择在电子邮件邀请中包含自定义消息，则自定义消息将显示在此区域中。</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。
