---
product-area: requests
navigation-topic: create-requests
title: 允许用户通过电子邮件将问题发送到请求队列项目
description: 允许用户通过电子邮件将问题发送到请求队列项目
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: 9cda6fd41ba7fcb9b9f412a7c2b7ffd39f3fe189
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# 允许用户通过电子邮件将问题发送到请求队列项目

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

您可以配置项目以允许用户通过电子邮件将问题添加到项目。 仅当项目被指定为请求队列时，您才可以允许通过电子邮件将问题发送到项目中。 有关创建“请求队列”项目的详细信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br></p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

配置项目需要以下先决条件，以允许用户通过电子邮件将问题添加到项目。

在启用此功能之前，必须满足以下条件：

* 通过电子邮件将问题发送到此帐户的用户必须是具有Workfront许可证的活动用户。
* 通过电子邮件将问题发送到此帐户的用户必须具有项目的“添加问题”权限。
* 外部用户无法将问题通过电子邮件发送到请求队列，因为他们无权创建问题。
* 只有来自与活动Workfront用户关联的电子邮件地址的电子邮件才允许将问题发送到项目。 从与Workfront帐户无关联的电子邮件转发到活动Workfront用户电子邮件的电子邮件无法在项目下创建问题，因为需要将原始发件人的电子邮件地址与活动Workfront帐户关联。
* 项目设置为请求队列。
* 与项目关联的电子邮件帐户未链接到Workfront用户帐户。

## 在Workfront中配置项目

>[!NOTE]
>
>启用电子邮件队列设置时，请牢记以下几点：
>
>* Workfront允许在所有集群中为每个请求队列发送一封唯一的电子邮件。 如果选择禁用请求队列，则只要您创建的电子邮件地址仍在“接收电子邮件地址”框中，该电子邮件地址就会保留。 如果选择停止使用接收电子邮件，则必须从“接收电子邮件”字段中将其删除，以便将来可以使用该电子邮件。
>
>* 如果请求队列具有多个队列主题或主题组，Workfront将随机选择通过电子邮件发送的请求将转到的队列主题，从而使通过电子邮件发送的请求难以管理。
>我们建议，您设置为通过电子邮件接收请求的项目不应有多个队列主题。 如果提交的请求针对不同的资源或项目，则在提交请求后应手动路由或移动它们。

1. 转到要启用以通过电子邮件接收问题的项目。
1. 单击 **队列详细信息** 在左侧面板中。 您可能需要单击 **显示更多** 首先。
1. 在 **队列类型** 区域，选择 **Publish作为帮助请求队列**.

1. 向下滚动到 **电子邮件队列设置** 区域，然后选择 **通过电子邮件启用请求接收**.

1. 在中输入电子邮件地址的开头 **接收电子邮件地址** 盒子。

   您必须创建一个唯一的电子邮件地址。 我们建议将您的公司名称用作接收电子邮件地址的一部分。

   >[!CAUTION]
   >
   >* 如果删除了包含请求队列的项目，则无法从回收站恢复此电子邮件地址。
   >
   >* 由于此电子邮件地址必须是唯一的，因此如果将其删除，则将来可能不可用。
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. （可选）选择 **通过电子邮件转发所有无法提交的问题**，然后在下面的框中输入转发电子邮件地址。

   此电子邮件地址会接收有关未能提交到项目的电子邮件的信息。

1. 单击 **保存**. 现在，当具有活动Workfront帐户的用户向此电子邮件地址发送电子邮件时，会在Workfront项目中创建问题。

   >[!NOTE]
   >
   >用户必须有权在项目中创建问题，才能通过电子邮件提交。 您可以在“高级设置”下的“共享”对话框中授予此访问权限。
   >
   >外部用户无法将问题通过电子邮件发送到请求队列，因为他们无权创建问题。

## 在Workfront中接收问题

当Workfront用户向Workfront发送电子邮件时，会发生以下情况：

* 电子邮件的“主题”行会变为“问题名称”。
* 电子邮件的正文将变为问题的描述。
* 如果有任何文档附加到电子邮件，这些文档将附加到Workfront中的问题。
* 在Workfront中，发送电子邮件的用户会成为新问题的主要联系人。
* 电子邮件的正文不能超过4,000个字符。
* 电子邮件附件总数不能超过7 MB。
