---
navigation-topic: notifications
title: 自定义事件通知的电子邮件主体
description: 您可以自定义由事件通知触发的电子邮件的主题行。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 4%

---

# 自定义事件通知的电子邮件主体

您可以自定义由事件通知触发的电子邮件的主题行：

更改主题行会影响系统中的所有用户，而无论收件人的访问级别如何。 用户会看到电子邮件主题中包含的所有对象和字段。

某些事件通知具有多个主题行，这意味着这些事件通知可以根据其功能具有多个电子邮件主题。

>[!IMPORTANT]
>
>对于主题行引用多个对象时，在删除默认字段时要小心。 以下是包含此类主题行的事件通知列表：
>
>* 有人将我列入定向更新
>* 有人将我的团队列入定向更新
>* 对跟帖参与者的工作项备注
>* 对工作项分派人的工作项备注
>


## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>计划员或更高级别，具有提醒通知的管理访问权限</p> <p>有关授予计划用户管理访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 为事件通知自定义电子邮件主题行 {#customize-email-subject-lines-for-event-notifications}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **电子邮件** > **通知**.

1. 单击 **事件通知** 选项卡。
1. 单击要自定义的事件通知的名称以打开 **事件通知** 框中。
1. 在 **电子邮件主题行** 框中，更改电子邮件主题中的文本和字段（包括自定义字段）。

   添加的字段名称必须与数据库结构的驼峰式语法匹配。 <!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. 单击 **更新** 以保存电子邮件的新主题行。

## 为多对象电子邮件自定义电子邮件主题行

某些事件通知具有多个主题行，具体取决于它们触发的对象。

例如，“有人在定向更新中包含我”有两个不同的主题行：第一个是任务、问题、模板任务和文档（也称为“referenceObject”），第二个是允许用户进行注释的对象，如组合、程序等（也称为“topReferenceObject”）。

![](assets/Ev-not-mult-subj-lines.png)

如果用户包含在有关任务、问题、模板任务或文档的对话中，则将使用第一个主题行生成电子邮件。 主题行包含“referenceObject:name”，系统定义对象并在主题字段中显示相应的名称。 电子邮件主题行应类似于以下内容：&quot;对项目ABC上的任务123的评论。&quot;

如果将添加到项目对话，则将生成与第二个主题有关的电子邮件。 此处，主题行包含“topReferenceObject:name”，Workfront再次标识引用的对象，并将返回该对象名称，而不是主题中的“topReferenceObject:name”。 电子邮件主题行应类似于以下内容：“对项目ABC的评论。”

要编辑电子邮件主题行并将其他字段添加到任一主题行，请参阅 [为事件通知自定义电子邮件主题行](#customize-email-subject-lines-for-event-notifications) 在本文中。

## 为多操作电子邮件自定义电子邮件主题行

某些事件通知还具有多个电子邮件主体，用于概述对对象采取的不同操作。

例如，请求文档添加到问题中是可触发两封不同电子邮件的事件：一个用于添加文档的时间，另一个用于编辑文档的时间。

![](assets/ev-not-mult-subj-lines-diff-actions.png)

要编辑电子邮件主题行并将其他字段添加到任一主题行，请参阅 [为事件通知自定义电子邮件主题行](#customize-email-subject-lines-for-event-notifications) 在本文中。
