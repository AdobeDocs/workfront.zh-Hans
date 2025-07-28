---
product-area: workfront-integrations
keywords: google，doc，文档，工作表，幻灯片
navigation-topic: workfront-for-g-suite
title: 从Google Workspace管理 [!DNL Adobe Workfront] 通知详细信息
description: 在Google Workspace中，打开Adobe [!DNL Workfront] 发送的通知电子邮件时，您可以查看相关工作项详细信息并在不离开收件箱的情况下做出回应。 如果可以使用操作（如批准请求），则可以直接从Workfront中为Google Workspace执行这些操作。
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# 管理来自[!DNL Adobe Workfront]的[!DNL Google Workspace]通知详细信息

>[!IMPORTANT]
>
>为了提供更稳定和可扩展的集成，我们正在使用Workfront自动化与集成(Fusion)转向一种现代、灵活的集成方法。 在此过渡过程中，以下适用于Google Workspace的Workfront功能在&#x200B;**2026年2月28日**&#x200B;之后将不可用：
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

在[!DNL Google Workspace]中，当您打开已发送的通知电子邮件[!DNL Adobe Workfront]时，您可以查看相关工作项详细信息并在不离开[!UICONTROL 收件箱]的情况下做出回应。 如果操作可用（如批准请求），则可以直接从[!DNL Workfront for Google Workspace]执行这些操作。

>[!NOTE]
>
> [!DNL Workfront for Google Workspace]支持您从[!DNL Workfront]收到的几乎每种类型的电子邮件通知（大约120种不同的类型）。 从[!UICONTROL 发送的]每日摘要[!DNL Workfront]电子邮件未出现在[!DNL Workfront for Google Workspace]中。 有关[!DNL Workfront]电子邮件通知类型的信息，请参阅[修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

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

## 先决条件

在从[!DNL Google Workspace]管理通知详细信息之前，您必须

* 安装[!DNL Workfront for Google Workspace]\
   有关说明，请参阅[安装 [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)。

## 管理来自[!DNL Adobe Workfront]的[!DNL Google Workspace]通知详细信息

1. 如果未显示[!DNL Workfront for Google Workspace]面板，请单击页面最右侧[!DNL Workfront]加载项侧边栏中的![图标](assets/wf-lion-icon.png)Workfront图标[!DNL Google Workspace]。
1. 在[!DNL Google Workspace]中，打开[!DNL Workfront]通知电子邮件。
1. 如果显示在面板顶部附近，请单击&#x200B;**[!UICONTROL 查看所有更新]**。
1. 单击&#x200B;**[!UICONTROL 详细信息]**。
1. 单击任何可用选项。

   可能显示的选项与已打开的电子邮件通知类型相关。 例如，如果是要求您批准任务的电子邮件通知，您会看到&#x200B;**[!UICONTROL 批准]**&#x200B;和&#x200B;**[!UICONTROL 拒绝]**，而不是&#x200B;**[!UICONTROL 处理任务]**&#x200B;或&#x200B;**[!UICONTROL 完成]**&#x200B;等选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>电子邮件通知类型</th> 
      <th>操作</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>任务或问题</td> 
      <td><strong>[!UICONTROL 批准]</strong>它，<strong>[!UICONTROL 拒绝]</strong>它，<strong>[!UICONTROL 授予]</strong>访问权限，<strong>[!UICONTROL 忽略]</strong>访问它的请求，<strong>[!UICONTROL 处理它]</strong>，或单击某个选项以指示您使用它<strong>[!UICONTROL 完成]</strong></td> 
     </tr> 
     <tr> 
      <td>项目</td> 
      <td><strong>[!UICONTROL 批准]</strong>它，<strong>[!UICONTROL 拒绝]</strong>它，<strong>[!UICONTROL 授予]</strong>对它的访问权限，或<strong>[!UICONTROL 忽略]</strong>对它的访问请求</td> 
     </tr> 
     <tr> 
      <td>文档</td> 
      <td><strong>[!UICONTROL 批准]</strong>它，<strong>[!UICONTROL 拒绝]</strong>它，<strong>[!UICONTROL 授予]</strong>对它的访问权限，或<strong>[!UICONTROL 忽略]</strong>对它的访问请求</td> 
     </tr> 
     <tr> 
      <td>更新 </td> 
      <td> <p>查看项目更新完整列表的任何部分，以便您拥有<strong>[!UICONTROL Post]</strong>新更新或<strong>[!UICONTROL 回复]</strong>所需的上下文。 您可以单击<strong>[!UICONTROL Notify]</strong>以提醒特定用户您的回复。 </p> <p>有关详细信息，请参阅<a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">回复来自[!DNL Adobe Workfront]的[!DNL Google Workspace]</a>更新通知。</p> </td> 
     </tr> 
     <tr> 
      <td>审批请求</td> 
      <td><strong>[!UICONTROL Approve]</strong>或<strong>[!UICONTROL Reject]</strong> （您可以通过单击其他选项改变主意）、下载、查看其所有者或查看其参考编号</td> 
     </tr> 
     <tr> 
      <td>项目状态的更改</td> 
      <td> 查看有关项目的所有当前信息，包括任何自定义表单。 </td> 
     </tr> 
    </tbody> 
   </table>
