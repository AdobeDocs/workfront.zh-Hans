---
content-type: reference
navigation-topic: notifications
title: 通知：目标
description: 通知：目标
author: Lisa
feature: Get Started with Workfront
exl-id: 12e66711-4438-4fcf-af79-7fcc2c3b1522
source-git-commit: 585a65c497211c84cffafeeaa5016218fd66acd2
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 2%

---

# 通知：目标

您可以为配置文件中发生[!DNL Adobe Workfront Goals]的事件启用电子邮件通知。 具有[!UICONTROL 计划]许可证的用户还可以为其他用户启用它们。 有关信息，请参阅[[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md)。

## 访问要求

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: because there are conditions for who sees this, I added this from the How To articles/ template although this is not a How To. But I like the format, so I thought keeping it consistent might help users. We may decide to update this when we have access and prereq for overview-type articles)</p>
-->

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL Request]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>产品</strong></td> 
   <td>[!DNL Workfront Goals] <p>有关[!DNL Workfront Goals]的信息，请参阅<a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals]概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[!UICONTROL View]对[!DNL Goals]或更高版本的访问权限</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何更改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed]</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

+++

## 先决条件

* 您要更新其[!DNL Goals]通知的用户必须具有布局模板，该模板包括[!UICONTROL 主菜单]中的[!DNL Goals]区域。


## [!UICONTROL 用户配置文件]区域中的[!DNL Goals]通知

下表列出的通知会提醒您有关[!DNL Workfront Goals]中发生的事件，例如有人为您分配目标、结果或活动，或者有人对您拥有的目标、结果或活动进行更新。 有关配置您收到的通知的信息，请参阅[修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

![通知首选项](assets/goals-notifications-preferences-350x114.png)

>[!NOTE]
>
>默认情况下，[!DNL Goals]的即时通知处于禁用状态。 您无法启用或禁用每日通知，并且不会收到此类别中事件的每日摘要电子邮件。 您可以启用或禁用[!DNL Goals]类别的单个即时通知。

另请参阅[事件通知](../../workfront-basics/using-notifications/event-notifications.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>通知</strong></td> 
   <td> <p><strong>字段已包含</strong> </p> <p><strong>*仅即时通知</strong></p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人已将“结果”/“活动”分派给我</strong></td> 
   <td> <p>将结果或活动分配给您的人员的姓名</p> <p>结果或活动的目标时段</p> <p>结果或活动的名称</p> <p>打开[!UICONTROL 目标详细信息]面板的<strong>[!UICONTROL 在Web应用程序中打开]</strong>按钮</p> <p>允许您管理通知的<strong>[!UICONTROL 更改通知设置]</strong>按钮。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人为我创建了新的个人目标</strong> </td> 
   <td> <p>分配目标的人员的姓名</p> <p>目标的周期</p> <p>目标的名称</p> <p>打开[!UICONTROL 目标详细信息]面板的<strong>[!UICONTROL 在Web应用程序中打开]</strong>按钮</p> <p>允许您管理通知的<strong>[!UICONTROL 更改通知设置]</strong>按钮。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人在我的“目标”中留言了</strong></td> 
   <td> <p>留下评论的人员的姓名</p> <p>目标的周期 </p> <p>目标的名称</p> <p>评论的文本</p> <p>打开[!UICONTROL 目标详细信息]面板的<strong>[!UICONTROL 在Web应用程序中打开]</strong>按钮</p> <p>允许您管理通知的<strong>[!UICONTROL 更改通知设置]</strong>按钮。</p> </td> 
  </tr> 
  <tr> 
  </tbody> 
</table>

<!--these were removed at some point: 

   <td><strong>Someone liked my comment on a Goal</strong></td> 
   <td> <p>The name of the person who liked the comment</p> <p>The Period of the goal </p> <p>The name of the goal</p> <p>The text of the comment </p> <p>The <strong>[!UICONTROL Open in web app]</strong> button which opens the [!UICONTROL Goal Details] panel</p> <p>The <strong>[!UICONTROL Change Notifications Settings]</strong> button which allows you to manage your notifications.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Someone liked an update on my Goal</strong></td> 
   <td> <p>You receive an email when someone likes a comment you made on a goal or when you update the progress of your results or activities on the goal. </p> <p>The name of the person who liked the update</p> <p>The Period of the goal </p> <p>The name of the goal</p> <p>The <strong>[!UICONTROL Open in web app]</strong> button which opens the [!UICONTROL Goal Details] panel</p> <p>The <strong>[!UICONTROL Change Notifications Settings]</strong> button which allows you to manage your notifications.</p> </td> 
  </tr> 
 -->

<!--
NOTE FOR NAME OF GOAL IN LAST TABLE CELL: check this. Is this true? Didn't triggger when this was written; add anything else? Maybe the type of the update is mentioned?!
-->
