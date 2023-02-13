---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: 从Slack创建任务和问题
description: 安装并配置后 [!DNL Adobe Workfront] 对于Slack，您可以从Slack创建任务和问题，并将它们与Workfront中的项目相关联。
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# 从创建任务和问题 [!DNL Slack]

安装并配置后 [!DNL Adobe Workfront for Slack]，则可以在 [!DNL Slack] 将它们与 [!DNL Workfront].

有关配置的更多信息 [!DNL Workfront] with [!DNL Slack]，请参阅 [配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

您必须有权在访问级别创建任务和问题，并且必须 [!UICONTROL Contribute] 与您关联的项目的权限。

有关访问级别的更多信息，请参阅 [访问级别概述](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). 有关对象权限的更多信息，请参阅 [对象共享权限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] 计划]</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员\

## 先决条件

在从 [!DNL Slack]，您必须

* 配置 [!DNL Workfront] Slack\
   有关配置的说明 [!DNL Workfront for Slack]，请参阅 [配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## 从创建任务 [!DNL Slack]

1. 登录到 [!DNL Slack] 实例和登录到 [!DNL Workfront] 从 [!DNL Slack].\
   有关从登录Workfront的更多信息 [!DNL Slack]，请参阅“登录到” [!DNL Workfront] 从 [!DNL Slack]“ ”部分 [访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 在任意渠道中，开始在消息字段中键入以下命令：

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >命令区分大小写。 您可以使用 `/wf` 而不是 `/workfront`.
   >  
   >必须输入任务名称，该名称将显示在 [!DNL Workfront] 界面（不带方括号或引号）。\
   >![add_task_to_project.png](assets/add-task-to-project-350x63.png)

1. （可选）开始键入要与新任务关联的项目名称，并在新任务显示在列表中时将其选中。\
   您会收到一条确认消息，指示该任务已添加到选定的项目。
1. （可选）单击确认消息中任务的名称以在中将其打开 [!DNL Workfront]，位于新的浏览器选项卡中。

## 从创建问题 [!DNL Slack]

1. 登录到 [!DNL Slack] 实例和登录到 [!DNL Workfront] 从 [!DNL Slack].\
   有关登录的更多信息，请参阅 [!DNL Workfront] 从 [!DNL Slack]，请参阅“登录到” [!DNL Workfront] 从 [!DNL Slack]“ ”部分 [访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 在任意渠道中，开始在消息字段中键入以下命令：

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >命令区分大小写。 可以使用“/wf”而不是“/workfront”启动命令。 \
   >必须输入问题名称，因为该名称将显示在 [!DNL Workfront] 界面（不带方括号或引号）。\
   >![slack_add_issue_to_project.png](assets/slack-add-issue-to-project-350x88.png)

1. （可选）开始键入要与新问题关联的项目名称，并在新问题显示在列表中时将其选中。\
   您会收到一则确认消息，指示问题已添加到选定的项目。
1. （可选）单击确认消息中问题的名称以在中将其打开 [!DNL Workfront]，位于新的浏览器选项卡中。
