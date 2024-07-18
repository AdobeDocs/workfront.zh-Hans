---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: 从Slack管理您的工作和批准
description: 您可以访问主页工作列表，查看和同意处理任务和问题，并直接从Slack查看或作出批准决策。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 1%

---

# 从[!DNL Slack]管理您的工作和批准

安装[!DNL Adobe Workfront for Slack]后，您可以执行以下操作：

* 从[!DNL Slack]访问[!UICONTROL 主页]项目的列表
* 审阅并接受以处理[!DNL Slack]中的任务和问题
* 审阅并决定来自[!DNL Slack]的审批

有关使用[!DNL Slack]配置[!DNL Workfront]的详细信息，请参阅[配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront]计划</a>*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 先决条件

在从[!DNL Slack]管理您的工作和审批之前，您必须

* 配置[!DNL Workfront for Slack]\
  有关配置[!DNL Workfront for Slack]的说明，请参阅[配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 从[!DNL Slack]管理您的工作

1. 从[!DNL Slack]登录到[!DNL Slack]实例并登录到[!DNL Workfront]。\
   有关从[!DNL Slack]登录到[!DNL Workfront]的详细信息，请参阅[访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的“从[!DNL Slack]登录到[!DNL Workfront]”部分。

1. 从任何渠道中，开始在消息字段中键入以下命令：

   `/workfront home`

   >[!NOTE]
   >
   >* 命令区分大小写。
   >* 您可以使用`/wf`而不是`/workfront`来启动命令。

   显示可用于访问任务、问题和批准列表的按钮。 单击其中一个按钮将显示[!DNL Slack]中每个列表的前20项。

1. （可选）单击&#x200B;**[!UICONTROL 任务]**&#x200B;以显示您的所有任务。

   有关在[!DNL Slack]中管理任务的详细信息，请参阅[从 [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack)管理您的任务。

1. （可选）单击&#x200B;**[!UICONTROL 问题]**&#x200B;以显示您的所有问题。

   有关在[!DNL Slack]中管理问题的更多信息，请参阅[从 [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack)管理您的问题。

1. （可选）单击&#x200B;**[!UICONTROL 批准]**&#x200B;以显示等待您决策的所有批准。\
   有关在[!DNL Slack]中管理您的审批的详细信息，请参阅[从 [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack)管理您的审批。

## 从[!DNL Slack]管理您的任务 {#manage-your-tasks-from-slack}

1. 从[!DNL Slack]登录到[!DNL Slack]实例并登录到[!DNL Workfront]。\
   有关从[!DNL Slack]登录到[!DNL Workfront]的信息，请参阅[访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的“从[!DNL Slack]登录到[!DNL Workfront]”部分。

1. 从任何渠道中，开始在消息字段中键入以下任一命令：

   `/workfront home`，然后单击&#x200B;**[!UICONTROL 任务]**

   或

   `/workfront tasks`

   >[!NOTE]
   >
   >* 命令区分大小写。
   >* 您可以使用`/wf`而不是`/workfront`来启动命令。

   此时将显示列表上的前20个任务。

1. 单击&#x200B;**[!UICONTROL +`<remaining number>`更多]**&#x200B;以显示其他任务。
1. 考虑查看有关工作项的以下信息：

   * **[!UICONTROL 名称]**
   * **[!UICONTROL 项目名称]**&#x200B;或&#x200B;**[!DNL Parent Object Name]**

   * 工作项的&#x200B;**[!DNL Planned Completion Date]**。
   * **[!DNL Assigned By Name]**：这是将任务分配给您的用户的名称。
   * **[!UICONTROL 状态]**

1. （可选）单击项目的名称，以便在Workfront中的单独浏览器选项卡中打开该项目。
1. （可选）在&#x200B;**[!UICONTROL 状态]**&#x200B;字段中，选择一个新状态。
1. （可选）单击&#x200B;**[!UICONTROL 记录时间]**，然后选择&#x200B;**[!UICONTROL 小时类型]**&#x200B;和小时数量以记录项目上的时间。

   >[!NOTE]
   >
   >* 您只能以一小时或半小时的增量记录小时，最长12小时30分钟。
   >* 您记录的小时的“输入日期”为今天。 您无法记录来自[!DNL Slack]的过去或未来日期的时间。

   您会收到一个确认消息，确认该时间已被记录。

1. （可选）单击&#x200B;**[!UICONTROL 处理它]**&#x200B;接受处理任务。 [!UICONTROL 处理此项工作]按钮消失。

## 从[!DNL Slack]管理您的问题 {#manage-your-issues-from-slack}

1. 从[!DNL Slack]登录到[!DNL Slack]实例并登录到[!DNL Workfront]。\
   有关从[!DNL Slack]登录到[!DNL Workfront]的详细信息，请参阅[从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] 登录到 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)。 [!DNL Workfront] 

1. 从任何渠道中，开始在消息字段中键入以下任一命令：

   `/workfront home`，然后单击&#x200B;**[!UICONTROL 问题]**

   或

   `/workfront issues`

   >[!NOTE]
   >
   >* 命令区分大小写。
   >* 您可以使用`/wf`而不是`/workfront`来启动命令。

   将显示列表中的前20个问题。

1. 单击&#x200B;**[!UICONTROL +剩余`<number>`个以上]**&#x200B;以显示其他项目。
1. 考虑查看有关工作项的以下信息：

   * **[!UICONTROL 名称]**
   * **[!UICONTROL 项目]**&#x200B;名称或父对象名称
   * **[!UICONTROL 到期日期为]**&#x200B;日期：这是工作项的计划完成日期。
   * **[!DNL Requested by]**&#x200B;姓名：这是主要联系人（针对问题）或分派用户（针对任务）。

1. （可选）单击问题的名称，以在Workfront中的单独浏览器选项卡中将其打开。
1. （可选）单击&#x200B;**[!DNL Work on it]**&#x200B;以开始处理您尚未接受的问题。

   [!UICONTROL 处理此项工作]按钮消失。

## 从[!DNL Slack]管理您的审批 {#manage-your-approvals-from-slack}

1. 从[!DNL Slack]登录到[!DNL Slack]实例并登录到[!DNL Workfront]。\
   有关从[!DNL Slack]登录到[!DNL Workfront]的详细信息，请参阅[访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的“从[!DNL Slack]登录到[!DNL Workfront]”部分。

1. 从任何渠道中，开始在消息字段中键入以下任一命令：

   `/workfront home`，然后单击&#x200B;**[!UICONTROL 审批]**

   或

   `/workfront approvals`

   >[!NOTE]
   >
   >* 命令区分大小写。
   >* 您可以使用`/wf`而不是`/workfront`来启动命令。

   **[!UICONTROL 审批]**&#x200B;列表上的前20项显示。 还会显示有关这些项目的其他信息，例如请求这些项目的用户的名称或项目所属的项目名称。

1. 单击&#x200B;**[!UICONTROL +剩余`<number>`个以上]**&#x200B;以显示其他项目。

1. 考虑管理以下对象的批准：

   * **项目**

     单击&#x200B;**[!UICONTROL 批准]**&#x200B;或&#x200B;**[!UICONTROL 拒绝]**&#x200B;接受或拒绝项目的状态更改。

   * **任务**

     单击&#x200B;**[!UICONTROL 批准]**&#x200B;或&#x200B;**[!UICONTROL 拒绝]**&#x200B;接受或拒绝任务的状态更改。

   * **问题**

     单击&#x200B;**[!UICONTROL 批准]**&#x200B;或&#x200B;**[!DNL Reject]**&#x200B;接受或拒绝问题的状态更改。

   * **文档**

     单击&#x200B;**[!UICONTROL 批准]**&#x200B;以批准文档，**[!UICONTROL 拒绝]**&#x200B;以拒绝文档，或单击&#x200B;**[!UICONTROL 更改]**&#x200B;以指示您批准文档，但文档需要其他更改。\
     （可选）将鼠标悬停在文档缩略图上以单击放大镜并预览文档。

   * **验证**&#x200B;单击验证名称以在[!DNL Workfront]中在单独的选项卡中打开并管理审批。
   * **访问请求**

     单击&#x200B;**[!UICONTROL 授予访问权限]**&#x200B;以授予所请求对象的增强权限，或单击&#x200B;**[!UICONTROL 忽略]**&#x200B;以忽略请求以获取更多访问权限。

1. （可选）单击提交审批的对象的名称，以在新浏览器选项卡的[!DNL Workfront]中打开该对象。
