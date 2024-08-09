---
user-type: administrator
product-area: system-administration
navigation-topic: start-with-workfront-administration
title: 发送公告
description: 作为Adobe Workfront管理员，您可以使用公告页面向用户发送公告。
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 413e3051-fcb5-44d7-b6bd-6b05d39935e8
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# 发送公告

作为Adobe Workfront管理员，您可以使用公告页面向用户发送公告。

来自Workfront的公告消息通常包括关于新增功能和版本、流程更改等方面的信息。

有关查看公告的信息，请参阅[查看和管理应用程序内通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)。

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
   <td> <p>您必须是Workfront管理员。 有关详细信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 向用户发送公告

您可以使用&#x200B;**公告**&#x200B;页面通过转发从Workfront发送的公告和撰写新公告来与Workfront系统中的用户通信。 您可以向Workfront系统中的特定用户、组、团队或公司发送公告。

* [将Workfront公告转发给用户](#forward-workfront-announcements-to-users)
* [撰写新公告](#compose-new-announcements)

### 将Workfront公告转发给用户 {#forward-workfront-announcements-to-users}

您可以轻松地将从Workfront收到的消息转发给系统中的用户。

1. 单击Workfront界面右上角的&#x200B;**通知**&#x200B;图标，然后单击&#x200B;**所有公告**，以转到“公告”页面。

   ![](assets/announcement-access-350x212.png)

1. 在&#x200B;**公告**&#x200B;页面上，选择要转发的消息。
1. 单击&#x200B;**转发**。
1. 在“**发送至**”框中，开始键入您希望接收公告消息的用户、组、团队或公司的名称，然后在该名称出现在下拉列表中时单击该名称。 重复此过程以添加多个用户、组、团队或公司。

   或

   要将公告转发给系统中的所有用户，请开始键入&#x200B;**所有人**，然后当公告出现在下拉列表中时单击它。

1. 继续执行[撰写新公告](#compose-new-announcements)中的步骤3。

### 撰写新公告 {#compose-new-announcements}

1. 单击Workfront界面右上角的&#x200B;**通知**&#x200B;图标，然后单击&#x200B;**所有公告**，以转到“公告”页面。

   ![](assets/announcement-access-350x212.png)

1. 在&#x200B;**公告**&#x200B;页面上，单击&#x200B;**新建公告。**

1. 在“**发送至**”框中，开始键入您希望接收公告消息的用户、组、团队或公司的名称，然后在该名称出现在下拉列表中时单击该名称。 重复此过程以添加多个用户、组、团队或公司。

   默认情况下，在发送新公告消息时，**每个人**&#x200B;都会预填充到此字段中。 如果您不希望系统中的所有用户都收到公告消息，请从列表中删除&#x200B;**所有人**。

1. 指定以下附加信息：

   | 主题 | 指定公告的主题。 |
   |---|---|
   | 在此处键入消息 | 指定消息的内容。 消息编辑器允许您包含常用标记，包括粗体、斜体、下划线、项目符号和编号列表以及超链接。 |
   | 附件 | 单击&#x200B;**添加附件，**，然后浏览并选择要附加到邮件的文件。 |

   {style="table-layout:auto"}

1. （可选）单击&#x200B;**另存为草稿**&#x200B;以将邮件（包括收件人列表、主题和附件）另存为草稿。

1. （可选）要查看草稿，请在&#x200B;**公告**&#x200B;区域中单击&#x200B;**草稿**。

1. 单击&#x200B;**发送。**

   用户现在可以查看公告消息，如[查看和管理应用程序内通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)中所述。

## 限制您收到的Workfront公告类型

如果您是Workfront管理员，则可以取消订阅以停止接收某些类型的消息。

默认情况下，您会收到从Workfront发送的所有消息。 这是推荐的配置。

1. 在&#x200B;**公告**&#x200B;页面上，单击&#x200B;**设置。**
1. 选择您不再希望接收消息的主题。
1. 单击&#x200B;**保存设置。**
