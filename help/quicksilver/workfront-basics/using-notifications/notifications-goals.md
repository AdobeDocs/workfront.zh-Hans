---
content-type: reference
navigation-topic: notifications
title: '通知：目标'
description: '通知：目标'
author: Lisa
feature: Get Started with Workfront
exl-id: 12e66711-4438-4fcf-af79-7fcc2c3b1522
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 6%

---

# 通知：目标

您可以为中发生的事件启用电子邮件通知 [!DNL Adobe Workfront Goals] 在您的个人资料中。 用户具有 [!UICONTROL 计划] 许可证还可以为其他用户启用它们。 有关信息，请参阅 [[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md).

## 访问要求

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: because there are conditions for who sees this, I added this from the How To articles/ template although this is not a How To. But I like the format, so I thought keeping it consistent might help users. We may decide to update this when we have access and prereq for overview-type articles)</p>
-->

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>产品</strong></td> 
   <td>[!DNL Workfront Goals] <p>有关信息 [!DNL Workfront Goals]，请参见 <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] 概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[！UICONTROL View]访问 [!DNL Goals] 或更高</p> <p>注意：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参见 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed]</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 先决条件

用户，其 [!DNL Goals] 更新后的通知必须满足以下条件：

* 布局模板，其中包括 [!DNL Goals] 中的区域 [!UICONTROL 主菜单].
* 访问新 [!DNL Adobe Workfront] 体验。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: we need this here because you can see these notifications from Classic)
  </MadCap:conditionalText>
  -->

## [!DNL Goals] 中的通知 [!UICONTROL 用户配置文件] 区域

下表列出的通知会提醒您在中发生的事件 [!DNL Workfront Goals]，例如有人为您分配目标、结果或活动，或者有人对您拥有的目标、结果或活动进行更新。 有关配置接收哪些通知的信息，请参阅 [修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/goals-notifications-preferences-350x114.png)

>[!NOTE]
>
>的即时通知 [!DNL Goals] 默认情况下处于禁用状态。 您无法启用或禁用每日通知，并且不会收到此类别中事件的每日摘要电子邮件。 您可以为启用或禁用单个即时通知 [!DNL Goals] 类别。

另请参阅 [事件通知](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>通知</strong></td> 
   <td> <p><strong>包含的字段</strong> </p> <p><strong>*仅即时通知</strong></p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人已将“结果”/“活动”分派给我</strong></td> 
   <td> <p>将结果或活动分配给您的人员的姓名</p> <p>结果或活动的目标时段</p> <p>结果或活动的名称</p> <p>此 <strong>[！UICONTROL在Web应用程序中打开]</strong> 按钮打开[！UICONTROL目标详细信息]面板</p> <p>此 <strong>[！UICONTROL更改通知设置]</strong> 按钮，用于管理通知。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人已为我创建新的个人“目标”</strong> </td> 
   <td> <p>分配目标的人员的姓名</p> <p>目标的周期</p> <p>目标的名称</p> <p>此 <strong>[！UICONTROL在Web应用程序中打开]</strong> 按钮打开[！UICONTROL目标详细信息]面板</p> <p>此 <strong>[！UICONTROL更改通知设置]</strong> 按钮，用于管理通知。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人在我的“目标”中留言了</strong></td> 
   <td> <p>留下评论的人员的姓名</p> <p>目标的周期 </p> <p>目标的名称</p> <p>评论的文本</p> <p>此 <strong>[！UICONTROL在Web应用程序中打开]</strong> 按钮打开[！UICONTROL目标详细信息]面板</p> <p>此 <strong>[！UICONTROL更改通知设置]</strong> 按钮，用于管理通知。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人赞了我的“目标”评论</strong></td> 
   <td> <p>喜欢评论的人员姓名</p> <p>目标的周期 </p> <p>目标的名称</p> <p>评论的文本 </p> <p>此 <strong>[！UICONTROL在Web应用程序中打开]</strong> 按钮打开[！UICONTROL目标详细信息]面板</p> <p>此 <strong>[！UICONTROL更改通知设置]</strong> 按钮，用于管理通知。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人赞了我的“目标”更新</strong></td> 
   <td> <p>当有人喜欢您对目标发表的评论或者您更新目标上的结果或活动的进度时，您会收到一封电子邮件。 </p> <p>喜欢此更新的人员的姓名</p> <p>目标的周期 </p> <p>目标的名称</p> <p>此 <strong>[！UICONTROL在Web应用程序中打开]</strong> 按钮打开[！UICONTROL目标详细信息]面板</p> <p>此 <strong>[！UICONTROL更改通知设置]</strong> 按钮，用于管理通知。</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
NOTE FOR NAME OF GOAL IN LAST TABLE CELL: check this. Is this true? Didn't triggger when this was written; add anything else? Maybe the type of the update is mentioned?!
-->
