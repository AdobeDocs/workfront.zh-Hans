---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: 管理 [!DNL Adobe Workfront] 通知 [!DNL Microsoft] 团队
description: 您可以从接收通知 [!DNL Adobe Workfront] 您需要批准的项目、已给您的分配，或您关联的项目的注释和更改。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 473a1fe3cb7e247749d9b540e3e5556cbe17a1dd
workflow-type: tm+mt
source-wordcount: '1280'
ht-degree: 0%

---

# 管理 [!DNL Adobe Workfront] 通知 [!DNL Microsoft Teams]

您可以从接收通知 [!DNL Adobe Workfront] 您需要批准的项目、已给您的分配，或您关联的项目的注释和更改。

这些通知包含 [!DNL Workfront] 可在中执行的操作 [!DNL Microsoft Teams] 不导航 [!DNL Microsoft Teams] 来完成他们。

>[!NOTE]
>
>[!DNL Microsoft Teams] 不再支持 [!DNL Internet Explorer]. 使用 [!DNL Adobe Workfront for Microsoft Teams integration]，则必须使用 [!DNL Internet Explorer].


## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Work]、[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 接收先决条件 [!DNL Workfront] 通知 [!DNL Microsoft Teams]

您可以 [!DNL Workfront] 通知 [!DNL Microsoft Teams] 满足下列条件时：

* 已安装并配置团队所有者 [!DNL Workfront for Microsoft Teams] 为你的团队。
* 您已登录 [!DNL Workfront] 从 [!DNL Microsoft Teams].
* 您已在 [!DNL Workfront]. 有关启用即时通知的信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

有关安装的信息 [!DNL Workfront for Microsoft Teams] 登录到 [!DNL Workfront from Microsoft Teams]，请参阅 [安装 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## 管理 [!DNL Workfront] 通知 [!DNL Microsoft Teams]

当 [!DNL Workfront for Microsoft Teams] 安装应用程序时， [!DNL Workfront] 在中创建聊天渠道 [!DNL Microsoft Teams] 为那个团队的每一个成员。 在中执行特定操作时 [!DNL Workfront]，则可以为 [!DNL Workfront for Microsoft Teams] 接收有关该操作的通知 [!DNL Workfront] 聊天渠道 [!DNL Microsoft Teams].

使用时请考虑以下事项 [!DNL Workfront] 通知来自 [!DNL Microsoft Teams]:

* 您无法接收全部，但只能接收选定数量的 [!DNL Workfront] 通知 [!DNL Microsoft Teams].
* 从接收的所有通知 [!DNL Workfront] 显示在 [!DNL Workfront] 机器人聊天渠道。

   有关安装的信息 [!DNL Workfront] 机器人渠道，请参阅 [登录到 [!DNL Workfront] 从 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) 部分 [安装 [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) 文章。

* 在中进行更新之后，最长可能会有5分钟的延迟 [!DNL Workfront] 当您在 [!DNL Microsoft Teams].
* 对于 [!DNL Microsoft Teams] 通知时，您还会收到电子邮件通知。

管理 [!DNL Workfront] 可在 [!DNL Microsoft Teams]:

1. 单击 **[!UICONTROL 已添加更多]** （三个圆点）应用程序图标 [!DNL Microsoft Teams].

1. 单击 [!DNL Workfront] 在显示的列表中。
1. 选择 **[!UICONTROL 设置]** 选项卡。

   ![](assets/ms-teams-settings-tab-350x552.png)

1. 禁用您不希望接收的任何通知。 您可以启用或禁用通知组（如信息或批准通知），也可以单独管理通知。

   默认情况下，所有通知都处于启用状态。

   的通知设置 [!DNL Workfront for Microsoft] 团队会自动保存。

   >[!NOTE]
   >
   >您无法向默认可用的通知添加更多通知。

## 响应 [!DNL Workfront] 中的通知和批准请求 [!DNL Microsoft Teams]

1. 登录到 [!DNL Workfront] 从 [!DNL Microsoft Teams].\
   有关登录到的信息 [!DNL Workfront]，请参阅 [安装 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. 转到 **[!UICONTROL 聊天]** ，然后单击 **[!DNL Workfront]** 机器人渠道。\
   此渠道用于与 [!DNL Workfront] 机器人。 全部 [!DNL Workfront] 此处将显示通知。
1. 根据您收到的通知类型，转到相关部分：

   * [批准通知](#approval-notifications-approval-notifications)
   * [分配通知](#assignment-notifications-assignment-notifications)
   * [注释通知](#comment-notifications-comment-notifications)
   * [更新通知](#update-notifications-update-notifications)
   * [日期更改通知](#date-change-notifications-date-change-notifications)

### 批准通知 {#approval-notifications}

当要求您批准对象（如任务、时间表或校样）时，您会收到批准通知。 但是，您仍可以对通知进行评论。在批准通知中，您可以执行以下操作：

* **[!UICONTROL 批准]**:单击以批准该项目。
* **[!UICONTROL 更改]**:单击以批准更改的项目。
* **[!UICONTROL 拒绝]**:单击以拒绝项目。
* **[!UICONTROL 注释]**:单击以进行评论。 您的评论也会显示在 [!DNL Workfront] 作为对通知所针对的对象的更新。
* **[!UICONTROL 转到校样]**:单击以打开校样。 然后，您可以直接在校样中做出决策。 有关更多信息，请参阅 [在校对查看器中对校样做出决策](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>做出批准决策后，便无法从通知中更改它。

#### 可在特定批准通知中执行的操作：

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
   <th>[!UICONTROL Reject]</th> 
   <th> <p>[!UICONTROL Change]</p> </th> 
   <th> <p>[!UICONTROL转到校样] </p> </th> 
   <th>[!UICONTROL注释]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您需要批准项目</td> 
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
   <td role="rowheader">您需要批准问题</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要批准文档</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要批准对对象的访问</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要批准时间表</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人要你批准这个证明</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的时间表被拒绝</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">重新打开您的时间表</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您请求的文档批准请求已获得批准</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您请求的文档批准请求已通过更改获得批准</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您请求的文档批准请求被拒绝</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的时间表已获得批准</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 分配通知 {#assignment-notifications}

当您或您所在的团队被分配到Workfront中的任务或问题时，您会收到分配通知。 在分配通知中，您可以执行以下操作：

* **[!UICONTROL 处理它]**:选择以提交以处理该项目。 此时会短暂显示一则通知，确认已将新项目添加到您的工作列表。
* **[!UICONTROL 查看[!DNL Workfront]]**:选择以在Workfront中查看分配的问题或任务，此时将打开一个新选项卡。
* **[!UICONTROL 开始]**:单击以开始处理该项目。 此时会短暂显示一则通知，确认已将新项目添加到您的工作列表。
* **[!UICONTROL 注释]**:单击以对项目进行评论。 您的评论也会显示在Workfront中该项目的更新流中。
* **[!UICONTROL 状态]**:单击，然后从下拉菜单中选择工作项的新状态。

#### 可用于特定分配通知的操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL开始]</th> 
   <th>[!UICONTROL注释]</th> 
   <th> <p>[!UICONTROL状态]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您被分配到任务</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您已分配到问题</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">被指派给的团队会收到任务的工作请求</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您所在的团队会收到问题的工作请求</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 注释通知 {#comment-notifications}

当某人对您关联的项目发表评论或将您包含在更新中时，您会收到通信通知。 在通信通知中，您可以执行以下操作：

* **代表ly**:单击以回复评论或 [!UICONTROL 更新]. 您的回复也会显示在更新流中，该评论会显示在Workfront中。
* **[!UICONTROL 在Workfront中查看]**:选择以在Workfront中查看评论和项目，该注释和项目将在新选项卡中打开。
* **[!UICONTROL 状态]**:单击，然后为评论或更新所涉及的工作项选择新状态。

#### 可在特定通信通知中执行的操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL状态]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您的请求中会发布评论</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的工作请求上发布了回复</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">某人对您所在的线程进行评论</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人对您的某个工作项目发表评论</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">某人对您批准的时间表进行评论</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">评论会添加到您的用户配置文件页面，或通过批量编辑多个用户来添加</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的某个更新中会添加评论</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">在您的时间表中添加注释</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 更新通知 {#update-notifications}

当您关联的某个项目发生更新时，您会收到一则信息通知，但您无需对该项目执行任何操作。 在信息通知中，您可以执行以下操作：

* **[!UICONTROL 回复]**:单击可回复 [!UICONTROL 更新]. 您的回复也会显示在Workfront中项目的更新流中。
* **在Workfront中查看**:选择以在Workfront中查看评论和项目，该注释和项目将在新选项卡中打开。
* **[!UICONTROL 状态]**:单击，然后从下拉菜单中选择项目的新状态。

#### 可用于特定信息通知的操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL状态]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">对您订阅的任务、发行或项目进行更新</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人在定向更新中包括您</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人会在[!UICONTROL定向更新]中包含您的团队</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 日期更改通知 {#date-change-notifications}

当您分配到的工作项上的日期更改时，您会收到日期更改通知。 在日期更改通知中，您可以执行以下操作。

* **[!UICONTROL 注释]**:单击以对项目进行评论。 您的评论也会显示在Workfront中该项目的更新流中。
* **[!UICONTROL 状态]**:单击，然后从下拉菜单中选择工作项的新状态。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>[!UICONTROL注释]</p> </th> 
   <th> <p>[!UICONTROL状态]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您被分配到的任务的到期日期更改</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
