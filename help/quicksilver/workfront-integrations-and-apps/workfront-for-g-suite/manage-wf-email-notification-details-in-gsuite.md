---
product-area: workfront-integrations
keywords: google，doc，文档，工作表，幻灯片
navigation-topic: workfront-for-g-suite
title: 从Google Workspace管理 [!DNL Adobe Workfront] 通知详细信息
description: 在Google Workspace中，打开Adobe [!DNL Workfront] 发送的通知电子邮件时，您可以查看相关工作项详细信息并在不离开收件箱的情况下做出回应。 如果可以使用操作（如批准请求），则可以直接从Workfront中为Google Workspace执行这些操作。
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 228fd22f1894689c0d256270350cc82954901641
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# 管理来自[!DNL Adobe Workfront]的[!DNL Google Workspace]通知详细信息

>[!IMPORTANT]
>
>为了提供更稳定、更可扩展的集成，我们已转为使用Workfront自动化与集成(Fusion)的现代、灵活集成方法。 在此过渡过程中，以下Workfront for Google Workspace功能&#x200B;**不再可用**：
>
>* 从Workfront访问Google Workspace功能
>
>* 从Gmail或Google日历网站面板查看和管理Workfront任务
>
>为了满足贵组织与Google Workspace的集成需求，我们建议使用Workfront自动化和集成。
>
>有关Workfront自动化和集成的概述，请参阅[Adobe Workfront Fusion概述](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>有关Google Workspace的Workfront自动化和集成模块的特定功能的信息，请参阅[Gmail模块](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)和[Google日历模块](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)。

<!--

In [!DNL Google Workspace], when you open a notification email [!DNL Adobe Workfront] has sent, you can view the associated work item details and respond without leaving your [!UICONTROL Inbox]. If actions are available, such as approving a request, you can perform those actions directly from [!DNL Workfront for Google Workspace].

>[!NOTE]
>
> [!DNL Workfront for Google Workspace] supports almost every type of email notification you can receive from [!DNL Workfront] (about 120 different types). [!UICONTROL Daily digest] emails sent from [!DNL Workfront] do not appear in [!DNL Workfront for Google Workspace]. For information about the [!DNL Workfront] email notification types, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p><p>Work or higher</p>
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you can manage notification details from [!DNL Google Workspace], you must

* Install [!DNL Workfront for Google Workspace]\
   For instructions, see [Install [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Manage [!DNL Adobe Workfront] notification details from [!DNL Google Workspace]

1. If the [!DNL Workfront for Google Workspace] panel is not displayed, click the [!DNL Workfront] icon ![Workfront icon](assets/wf-lion-icon.png) in the [!DNL Google Workspace] add-ons sidebar at the far-right of the page.
1. In [!DNL Google Workspace], open a [!DNL Workfront] notification email.
1. Click **[!UICONTROL View all updates]** if it is displayed near the top of the panel.
1. Click **[!UICONTROL Details]**.
1. Click any available options.

   The options that might display relate to the type of email notification you have opened. For example, if it's an email notification asking you to approve a task, you see **[!UICONTROL Approve]** and **[!UICONTROL Reject]** instead of options such as **[!UICONTROL Work on It]** or **[!UICONTROL Done]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Type of email notification</th> 
      <th>Action</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Task or issue</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, <strong>[!UICONTROL Ignore]</strong> a request for access to it, <strong>[!UICONTROL Work on it]</strong>, or click an option to indicate that you are <strong>[!UICONTROL Done]</strong> with it</td> 
     </tr> 
     <tr> 
      <td>Project</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, or <strong>[!UICONTROL Ignore]</strong> a request for access to it</td> 
     </tr> 
     <tr> 
      <td>Document</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, or <strong>[!UICONTROL Ignore]</strong> a request for access to it</td> 
     </tr> 
     <tr> 
      <td>Update </td> 
      <td> <p>View any part of the entire list of updates for the item so that you have the context you need to <strong>[!UICONTROL Post]</strong> a new update or a <strong>[!UICONTROL Reply]</strong>. You can click <strong>[!UICONTROL Notify]</strong> to alert particular users about your reply. </p> <p>For more information, see <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Reply to a [!DNL Adobe Workfront] update notification from [!DNL Google Workspace]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Approval request</td> 
      <td><strong>[!UICONTROL Approve]</strong> or <strong>[!UICONTROL Reject]</strong> it (you can change your mind by clicking the other option), download it, view its owner, or view its reference number</td> 
     </tr> 
     <tr> 
      <td>A change in a project's status</td> 
      <td> View all the current information about the project, including any custom forms. </td> 
     </tr> 
    </tbody> 
   </table>

   -->
