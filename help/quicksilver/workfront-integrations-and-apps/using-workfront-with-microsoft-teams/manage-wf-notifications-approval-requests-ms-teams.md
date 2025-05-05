---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: 管理 [!DNL Microsoft] 团队中的 [!DNL Adobe Workfront] 通知
description: 您可以从 [!DNL Adobe Workfront] 接收有关需要批准的项目、已给予您的分配或您关联项目的注释和更改的通知。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 69fdb5c23bb501fc81e4ef3c3ab7c94e78e69d29
workflow-type: tm+mt
source-wordcount: '1338'
ht-degree: 0%

---

# 在[!DNL Microsoft Teams]中管理[!DNL Adobe Workfront]通知

<!--

>[!NOTE]
>
>As of July 1, 2025, Microsoft will remove support for the Classic Teams desktop app. As a result, the Workfront integration with Microsoft Teams will not be supported after the Classic Teams desktop app is no longer available.

-->

您可以从[!DNL Adobe Workfront]接收有关您需要审批的项目、已给予您的分配或您关联项目的注释和更改的通知。

这些通知包含您可以在[!DNL Microsoft Teams]内执行的[!DNL Workfront]操作，无需离开[!DNL Microsoft Teams]即可完成这些操作。

>[!NOTE]
>
>[!DNL Microsoft Teams]不再支持[!DNL Internet Explorer]。 要使用[!DNL Adobe Workfront for Microsoft Teams integration]，您必须使用[!DNL Internet Explorer]以外的Web浏览器。


## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL 工作]，[!UICONTROL 计划]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 在[!DNL Microsoft Teams]中接收[!DNL Workfront]通知的先决条件

如果满足以下条件，则可以在[!DNL Microsoft Teams]中接收[!DNL Workfront]通知：

* 团队所有者已为您的团队安装和配置[!DNL Workfront for Microsoft Teams]。
* 您已从[!DNL Microsoft Teams]登录[!DNL Workfront]。
* 您已在[!DNL Workfront]中启用即时通知。 有关启用即时通知的信息，请参阅[修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

有关安装[!DNL Workfront for Microsoft Teams]和登录到[!DNL Workfront from Microsoft Teams]的信息，请参阅[安装 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

## 管理[!DNL Microsoft Teams]中的[!DNL Workfront]通知

安装[!DNL Workfront for Microsoft Teams]应用后，将在[!DNL Microsoft Teams]中为该团队的每个成员创建[!DNL Workfront]聊天渠道。 在[!DNL Workfront]中执行特定操作时，您可以配置[!DNL Workfront for Microsoft Teams]的设置，以在[!DNL Microsoft Teams]的[!DNL Workfront]聊天频道中接收有关该操作的通知。

处理来自[!DNL Microsoft Teams]的[!DNL Workfront]通知时，请考虑以下事项：

* 您无法在[!DNL Microsoft Teams]中接收所有，但只能接收选定数量的[!DNL Workfront]个通知。
* 您从[!DNL Workfront]收到的所有通知都会显示在[!DNL Workfront]机器人聊天频道中。

  有关安装[!DNL Workfront]机器人通道的信息，请参阅[正在安装 [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)文章中的[从 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront)登录到 [!DNL Workfront] 部分。

* 从[!DNL Workfront]中进行更新到在[!DNL Microsoft Teams]中收到有关该更新的通知，最多可能有5分钟的延迟。
* 对于每个[!DNL Microsoft Teams]通知，您还会收到电子邮件通知。

要管理可在[!DNL Microsoft Teams]中收到的[!DNL Workfront]通知，请执行以下操作：

1. 单击[!DNL Microsoft Teams]左侧导航栏上的&#x200B;**[!UICONTROL 更多已添加]** （三点）应用图标。

1. 在显示的列表中单击[!DNL Workfront]。
1. 选择&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡。

   ![MS Teams设置选项卡](assets/ms-teams-settings-tab-350x552.png)

1. 禁用任何您不想接收的通知。 您可以启用或禁用通知组，如信息或批准通知，也可以单独管理通知。

   默认启用所有通知。

   将自动保存[!DNL Workfront for Microsoft]团队的通知设置。

   >[!NOTE]
   >
   >您无法向默认可用的通知中添加更多通知。

## 在[!DNL Microsoft Teams]中响应[!DNL Workfront]个通知和批准请求

1. 从[!DNL Microsoft Teams]登录到[!DNL Workfront]。\
   有关登录到[!DNL Workfront]的信息，请参阅[安装 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

1. 转到&#x200B;**[!UICONTROL 聊天]**&#x200B;区域并单击&#x200B;**[!DNL Workfront]**&#x200B;机器人频道。\
   此频道用于您与[!DNL Workfront]机器人的个人聊天。 此处显示所有[!DNL Workfront]通知。
1. 根据您收到的通知类型，转到相关部分：

   * [审批通知](#approval-notifications-approval-notifications)
   * [任务通知](#assignment-notifications-assignment-notifications)
   * [评论通知](#comment-notifications-comment-notifications)
   * [更新通知](#update-notifications-update-notifications)
   * [日期更改通知](#date-change-notifications-date-change-notifications)

### 审批通知 {#approval-notifications}

当要求您批准对象（如任务、时间表或验证）时，您会收到批准通知。 但是，您仍然可以对通知进行评论。通过审批通知，您可以执行以下操作：

* **[!UICONTROL 批准]**：单击以批准该项目。
* **[!UICONTROL 更改]**：单击以批准包含更改的项目。
* **[!UICONTROL 拒绝]**：单击可拒绝该项。
* **[!UICONTROL 评论]**：单击以发表评论。 您的注释也会在[!DNL Workfront]中显示为通知相关对象的更新。
* **[!UICONTROL 前往校对]**：单击以打开校对。 然后，您可以直接在验证中做出决定。 有关详细信息，请参阅[在校对查看者中做出校对决定](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)。

>[!NOTE]
>
>作出批准决策后，便无法从通知中更改该决策。

#### 特定审批通知上的可用操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL Approve]</th> 
   <th>[!UICONTROL 拒绝]</th> 
   <th> <p>[!UICONTROL 更改]</p> </th> 
   <th> <p>[!UICONTROL 转至验证] </p> </th> 
   <th>[!UICONTROL Comment]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您需要审批一个项目</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要批准任务</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要审批问题</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要审批文档</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要批准对对象的访问权限</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要审批工时表</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人希望您批准该证明</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的工时表已被拒绝</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的工时表已重新开立</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您请求的文档审批请求已审批</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您请求的文档审批请求已审批，但有更改</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您请求的文档审批请求被拒绝</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的工时表已审批</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 任务通知 {#assignment-notifications}

当您或您所在的团队分配到Workfront中的任务或问题时，您会收到分配通知。 从分配通知中，您可以执行以下操作：

* **[!UICONTROL 处理它]**：选择提交以处理该项。 系统会短暂显示通知，确认您已将新项目添加到工作列表。
* **[!UICONTROL 在[!DNL Workfront]]**&#x200B;中查看：选择此项可在Workfront中查看分配的问题或任务，这将打开一个新选项卡。
* **[!UICONTROL 开始]**：单击以开始处理该项目。 系统会短暂显示通知，确认您已将新项目添加到工作列表。
* **[!UICONTROL 评论]**：单击以评论该项目。 您的备注也会在Workfront的项目更新流中显示。
* **[!UICONTROL 状态]**：单击，然后从下拉菜单中选择工作项的新状态。

#### 特定分配通知中可用的操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL 开始]</th> 
   <th>[!UICONTROL Comment]</th> 
   <th> <p>[!UICONTROL 状态]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您被分派至一个任务</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您被分配到问题</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您分配到其中的团队会收到任务的工作请求</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您分配到的一个团队会收到问题的工作请求</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 评论通知 {#comment-notifications}

当某人备注与您关联的项目或将您包含在更新中时，您将收到通信通知。 在通信通知中，您可以执行以下操作：

* **代表ly**：单击以回复评论或[!UICONTROL 更新]。 您的回复也会出现在更新流中，评论会显示在Workfront中。
* **[!UICONTROL 在Workfront中查看]**：选择此项可查看评论以及在Workfront中打开的新选项卡中的项。
* **[!UICONTROL 状态]**：单击，然后为评论或更新相关的工作项选择新状态。

#### 对特定通信通知可用的操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL 回复]</th> 
   <th> <p>[!UICONTROL 状态]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您的请求上已张贴了一个评论</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">回复已发布在您的工作请求中</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">某人备注您所在的跟帖</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">某人备注您的工作项之一</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">某人备注您批准的工时表</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">评论会添加到您的用户配置文件页面上，或通过批量编辑多个用户的方式进行添加</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的一项更新中添加了一个评论</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的时间表中添加了评论</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 更新通知 {#update-notifications}

当与关联的项目有更新时，您会收到信息通知，但您无需对项目执行任何操作。 从信息通知中，您可以执行以下操作：

* **[!UICONTROL 回复]**：单击以回复[!UICONTROL 更新]。 您的回复也会在Workfront的项目更新流中显示。
* **在Workfront中查看**：选择此项可查看评论以及在Workfront中打开的新选项卡中的项。
* **[!UICONTROL 状态]**：单击，然后从下拉菜单中选择项目的新状态。

#### 可对特定信息通知执行的操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL 回复]</th> 
   <th> <p>[!UICONTROL 状态]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您订阅的任务、问题或项目已更新</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人将您列入定向更新</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人将您的团队包含在[!UICONTROL 定向更新]中</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 日期更改通知 {#date-change-notifications}

当日期更改分配给您的工作项时，您将收到日期更改通知。 从日期更改通知中，您可以执行以下操作。

* **[!UICONTROL 评论]**：单击以评论该项目。 您的备注也会在Workfront的项目更新流中显示。
* **[!UICONTROL 状态]**：单击，然后从下拉菜单中选择工作项的新状态。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>[!UICONTROL Comment]</p> </th> 
   <th> <p>[!UICONTROL 状态]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">当任务的截止日期改变时，向被分派的用户发送电子邮件</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
