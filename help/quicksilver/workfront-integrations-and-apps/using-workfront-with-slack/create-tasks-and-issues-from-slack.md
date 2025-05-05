---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: 从Slack创建任务和问题
description: 为Slack安装和配置 [!DNL Adobe Workfront] 后，您可以从Slack创建任务和问题，并将它们与Workfront中的项目关联。
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 从[!DNL Slack]创建任务和问题

安装和配置[!DNL Adobe Workfront for Slack]后，您可以从[!DNL Slack]创建任务和问题，并将它们与[!DNL Workfront]中的项目关联。

有关使用[!DNL Slack]配置[!DNL Workfront]的详细信息，请参阅[配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

您必须具有在访问级别创建任务和问题的访问权限，并且在要与它们关联的项目中必须具有[!UICONTROL Contribute]权限。

有关访问级别的详细信息，请参阅[访问级别概述](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)。 有关对象权限的详细信息，请参阅[对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront]计划]</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。\

## 先决条件

在从[!DNL Slack]创建任务和问题之前，您必须

* 为Slack配置[!DNL Workfront]\
   有关配置[!DNL Workfront for Slack]的说明，请参阅[配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 从[!DNL Slack]创建任务

1. 从[!DNL Slack]登录到[!DNL Slack]实例并登录到[!DNL Workfront]。\
   有关从[!DNL Slack]登录到Workfront的更多信息，请参阅[访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的“从[!DNL Slack]登录到[!DNL Workfront]”部分。

1. 从任何渠道中，开始在消息字段中键入以下命令：

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >命令区分大小写。 您可以使用`/wf`而不是`/workfront`来启动命令。
   >  
   >必须输入任务名称，因为它将显示在[!DNL Workfront]界面中，不带括号或引号。

1. （可选）开始键入要与新任务关联的项目的名称，并在项目出现在列表中时将其选定。\
   您将收到一条确认消息，指示任务已添加到选定项目。
1. （可选）单击确认消息中任务的名称，以在新的浏览器选项卡的[!DNL Workfront]中打开该任务。

## 从[!DNL Slack]创建问题

1. 从[!DNL Slack]登录到[!DNL Slack]实例并登录到[!DNL Workfront]。\
   有关从[!DNL Slack]登录到[!DNL Workfront]的详细信息，请参阅[访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的“从[!DNL Slack]登录到[!DNL Workfront]”部分。

1. 从任何渠道中，开始在消息字段中键入以下命令：

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >命令区分大小写。 可以使用“/wf”而不是“/workfront”启动命令。 \
   >必须输入问题名称，因为它将出现在[!DNL Workfront]界面中，不带括号或引号。

1. （可选）开始键入要与新问题关联的项目的名称，并在该问题出现在列表中时将其选定。\
   您将收到一条确认消息，指示该问题已添加到选定项目。
1. （可选）单击确认消息中问题的名称，以在新的浏览器选项卡的[!DNL Workfront]中将其打开。
