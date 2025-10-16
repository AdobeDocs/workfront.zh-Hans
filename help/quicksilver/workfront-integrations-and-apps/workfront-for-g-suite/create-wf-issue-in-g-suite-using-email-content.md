---
product-area: workfront-integrations;projects
keywords: google，doc，文档，工作表，幻灯片
navigation-topic: workfront-for-g-suite
title: 使用电子邮件内容在Google Workspace中创建 [!DNL Adobe Workfront] 问题
description: 您可以将 [!DNL Adobe Workfront)] 未生成的外部电子邮件转换为 [!DNL Workfront] 问题。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 0%

---

# 使用电子邮件内容在[!DNL Adobe Workfront]中创建[!DNL Google Workspace]问题

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

您可以将外部电子邮件（非[!DNL Adobe Workfront]生成）转换为[!DNL Workfront]问题。

您还可以将外部电子邮件转换为现有问题的更新。 有关详细信息，请参阅[使用电子邮件内容 [!DNL Adobe Workfront] 更新 [!DNL Google Workspace] 中的](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md)项。

有关使用[!DNL Google Workspace]处理[!DNL Workfront]发送的通知电子邮件的信息，请参阅[管理 [!DNL Adobe Workfront] 中的 [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md)通知详细信息。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p><p>工作或更高</p>
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在从[!DNL Google Workspace]创建问题之前，您必须

* 安装[!DNL Workfront for Google Workspace]\
   有关说明，请参阅[安装 [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)。

## 使用电子邮件内容在[!DNL Adobe Workfront]中创建[!DNL Google Workspace]问题

1. 如果未显示[!UICONTROL Workfront for Google Workspace]面板，请单击页面最右侧[!DNL Workfront]加载项侧边栏中的![图标](assets/wf-lion-icon.png)Workfront图标[!DNL Google Workspace]。
1. 在[!DNL Google Workspace]中打开电子邮件后，单击[!DNL Workfront for Google Workspace]中的选项以将电子邮件转换为新的[!DNL Workfront]问题。

   ![转换电子邮件](assets/convert-email-task-issue-update.png)

1. 如果要将问题附加到父项目，请单击“**[!UICONTROL 项目名称]**”，开始键入要附加问题的项目名称，然后在该项目出现在以下列表中时单击该项目名称。
1. 进行以下任何更改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 问题名称]</td> 
      <td>编辑此文本的任何部分，这部分内容取自电子邮件的主题行。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 描述]</td> 
      <td>编辑此文本的任何部分，这部分内容取自电子邮件的正文。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 分配给]</td> 
      <td>单击<strong>[!UICONTROL 分配给]</strong>，单击显示的<strong>[!UICONTROL 将此分配给]</strong>选项，然后开始键入人员姓名，并在人员姓名出现在以下列表中时单击该姓名。 对要添加的每个人重复此操作，然后单击<strong>[!UICONTROL 保存]</strong>。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 优先级]</td> 
      <td>单击下拉箭头，然后单击问题的优先级。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include e-mail attachments]</td> 
      <td> <p>（仅当电子邮件至少包含一个附件时才可用。） 单击此选项可将电子邮件中的附件保存到问题的[!UICONTROL 文档]区域。 </p> <p>如果不想保存附件，请单击附件名称右侧的X。 </p> <p>如果电子邮件包含指向[!DNL Google Drive]中文档的链接，则这些链接将保存到您正在创建的问题的[!UICONTROL 概述]选项卡中。 </p> <p>重要提示：为了使其正常工作，您的[!DNL Workfront]管理员必须授权[!DNL Google Drive]使用[!DNL Workfront]中的文档，如<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">配置文档集成</a>中的<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">配置集成以管理文档</a>部分所述。</p> <p>如果启用此选项，则对于您转换为任务、问题和更新的其他电子邮件，此选项将保持启用状态。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">包括电子邮件文件</td> 
      <td> <p>单击此选项可将原始电子邮件作为电子邮件(EML) （电子邮件）文件<span>保存到问题的[!UICONTROL 文档]区域</span>。 从该位置，您可以双击文件以在电子邮件应用程序中打开电子邮件。</p> <p>如果启用此选项，则对于您转换为任务、问题和更新的其他电子邮件，此选项将保持启用状态。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 创建问题]**。

   新问题的&#x200B;**[!UICONTROL 详细信息]**&#x200B;选项卡显示在[!DNL Workfront for Google Workspace]面板中。 您可以单击&#x200B;**[!UICONTROL 更新]**&#x200B;并立即开始与协作者通信，而无需离开您的收件箱。

   在&#x200B;**[!UICONTROL 详细信息]**&#x200B;选项卡的底部，您还可以单击&#x200B;**[!UICONTROL 在Workfront中查看]**&#x200B;以转到Workfront中的新问题。

   当您刷新浏览器时，将显示一则消息，其中的[!UICONTROL Workfront for Google Workspace]面板底部有一个链接，用于确认您已将电子邮件转换为问题：

   您可以单击该链接以转到您已创建的问题在[!DNL Workfront for Google Workspace]面板中的“详细信息”视图。

   您可以重复这些步骤，将同一电子邮件转换为多个问题。 当您刷新浏览器或在下次返回电子邮件时，您为该电子邮件创建的所有链接都列在[!UICONTROL Workfront for Google Workspace]面板的底部。

1. （可选）通过执行以下任一操作继续处理[!DNL Workfront for Google Workspace]面板中的问题：

   * 若要在&#x200B;**[!UICONTROL 更新]**&#x200B;选项卡中添加更新，请单击&#x200B;**[!UICONTROL 开始新的更新]**&#x200B;并键入更新。

   * 若要回复&#x200B;**[!UICONTROL 更新]**&#x200B;选项卡上的更新，请单击&#x200B;**[!UICONTROL 回复]**，然后键入您的回复。

     对于上述两个操作，您可以通知特定用户您的评论。 单击&#x200B;**[!UICONTROL 通知]**，开始键入用户的名称，然后在名称出现在下拉列表中时单击该名称。 对要通知的其他用户重复此过程，然后单击&#x200B;**[!UICONTROL 发布]**。

   * 单击&#x200B;**[!UICONTROL 文档]**&#x200B;选项卡以查看与问题一起保存的任何文档。
