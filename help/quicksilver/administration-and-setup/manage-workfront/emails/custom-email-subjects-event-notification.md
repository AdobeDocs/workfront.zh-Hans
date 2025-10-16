---
navigation-topic: notifications
title: 自定义事件通知的电子邮件主题
description: 您可以自定义事件通知触发的电子邮件主题行。
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 5%

---

# 自定义事件通知的电子邮件主题

您可以自定义由事件通知触发的电子邮件主题行：

更改主题行会影响系统中的所有用户，而不管收件人的访问级别如何。 用户会看到电子邮件主题中包含的所有对象和字段。

某些事件通知具有多个主题行，这意味着这些事件通知根据其功能可以具有多个电子邮件主题。

>[!IMPORTANT]
>
>对于主题行引用多个对象的情况，在删除默认字段时请务必谨慎。 以下是包含此类主题行的事件通知列表：
>
>* 有人将我列入定向更新
>* 有人将我的团队列入定向更新
>* “工作项评论”到“主题参与者”
>* “工作项评论”到“工作项被分派人”
>

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>Planner或更高版本，具有提醒通知的管理访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 自定义事件通知的电子邮件主题行 {#customize-email-subject-lines-for-event-notifications}

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**电子邮件** > **通知**。

1. 单击&#x200B;**事件通知**&#x200B;选项卡。
1. 单击要自定义的事件通知的名称以打开&#x200B;**事件通知**&#x200B;框。
1. 在&#x200B;**电子邮件主题行**&#x200B;框中，更改电子邮件主题中的文本和字段，包括自定义字段。

   添加的字段名称必须与我们数据库结构的驼峰式大小写语法匹配。<!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. 单击&#x200B;**更新**&#x200B;以保存您电子邮件的新主题行。

## 自定义多对象电子邮件的电子邮件主题行

某些事件通知具有多个主题行，具体取决于它们触发的对象。

例如，“有人在定向更新中包含我”有两个不同的主题行：第一个主题行用于任务、问题、模板任务和文档（也称为“referenceObject”），第二个主题行用于允许用户进行注释的对象，如项目组合、项目群等（也称为“topReferenceObject”）。

![事件不是多个主题行](assets/ev-multiple-subject.png)

如果某个用户包含在关于任务、问题、模板任务或文档的对话中，则会生成包含第一个主题行的电子邮件。 主题行包含“referenceObject:name”，系统定义该对象并在主题字段中显示适当的名称。 电子邮件主题行将类似于以下内容：“对项目ABC中的任务123的评论”。

如果添加到项目对话，将生成一封包含第二个主题的电子邮件。 此处，主题行包含“topReferenceObject:name”，Workfront再次标识所引用的对象，并且将在主题中返回该对象名称而不是“topReferenceObject:name”。 电子邮件主题行类似于：“对项目ABC的评论”。

要编辑电子邮件主题行并向任一主题行添加其他字段，请参阅本文中的[自定义事件通知的电子邮件主题行](#customize-email-subject-lines-for-event-notifications)。

## 自定义多操作电子邮件的电子邮件主题行

某些事件通知还具有多个电子邮件主题，可概述对对象执行的不同操作。

例如，请求将文档添加到问题是一个事件，该事件会触发两个不同的电子邮件：一个用于添加文档时，另一个用于编辑文档时。



![事件不是多个主题行](assets/Ev-not-mult-subj-lines.png)

要编辑电子邮件主题行并向任一主题行添加其他字段，请参阅本文中的[自定义事件通知的电子邮件主题行](#customize-email-subject-lines-for-event-notifications)。
