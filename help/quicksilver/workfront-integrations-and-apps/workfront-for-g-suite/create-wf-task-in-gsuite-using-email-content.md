---
product-area: workfront-integrations;projects
keywords: google，doc，文档，工作表，幻灯片
navigation-topic: workfront-for-g-suite
title: 使用电子邮件内容在Google Workspace中创建 [!DNL Adobe Workfront] 任务
description: 您可以将外部电子邮件(非Adobe [!DNL Workfront]生成)转换为Workfront任务。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 0%

---

# 使用电子邮件内容在[!DNL Adobe Workfront]中创建[!DNL Google Workspace]任务

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

您可以将外部电子邮件（不是由[!DNL Adobe Workfront]生成）转换为[!DNL Workfront]任务。

您还可以将外部电子邮件转换为现有任务上的更新。 有关详细信息，请参阅[使用电子邮件内容 [!DNL Adobe Workfront] 更新 [!DNL Google Workspace] 中的](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md)项。

有关使用[!DNL Google Workspace]处理[!DNL Workfront]发送的通知电子邮件的信息，请参阅[管理 [!DNL Adobe Workfront] 中的 [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md)通知详细信息。

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
   <td> <p>[！UICONTROL工作]，[！UICONTROL计划]</p> </td> 
  </tr> 
   </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 先决条件

在[!DNL Workfront]中创建[!DNL Google Workspace]任务之前，您必须

* 安装[!DNL Workfront for Google Workspace]\
   有关说明，请参阅[安装 [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)。

## 使用电子邮件内容在[!DNL Adobe Workfront]中创建[!DNL Google Workspace]任务

1. 如果未显示[!UICONTROL Workfront for Google Workspace]面板，请单击页面最右侧[!DNL Workfront]加载项侧边栏中的![图标](assets/wf-lion-icon.png)Workfront图标[!DNL Google Workspace]。
1. 在[!DNL Google Workspace]中打开电子邮件后，单击[!DNL Workfront for Google Workspace]中的选项以将电子邮件转换为新的[!DNL Workfront]任务。

1. 选择&#x200B;**[!UICONTROL 新建]**&#x200B;选项以指示该任务将成为项目的一部分，还是独立于项目的个人任务。
1. 如果要将任务附加到父项目，请单击“**[!UICONTROL 项目名称]**”，开始输入任务所在项目的名称，然后在项目名称出现在以下列表中时单击该名称。
1. 进行以下任何更改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL任务名称]</td> 
      <td>编辑此文本的任何部分，这部分内容取自电子邮件的主题行。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL描述]</td> 
      <td>编辑此文本的任何部分，这部分内容取自电子邮件的正文。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL分配给]</td> 
      <td>单击<strong>[！UICONTROL分配给]</strong>，单击显示的<strong>[！UICONTROL将此分配给]</strong>选项，然后开始键入人员姓名，并在人员姓名出现在以下列表中时单击该姓名。 对要添加的每个人重复此操作，然后单击<strong>[！UICONTROL保存]</strong>。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL计划持续时间]</td> 
      <td> <p>单击<strong>[！UICONTROL计划持续时间]</strong>，然后键入您希望任务花费的天数。 </p> <p>注意：可以通过不同的方式为您的组织配置此选项。 例如，对于您的组织，您可能需要键入小时数而不是天数。 如果您需要更多信息，请咨询您的[!DNL Workfront]管理员。 如果您要指定配置的默认时间段以外的其他时间段，请在数字后键入<strong>m</strong>、<strong>h</strong>、<strong>d</strong>、<strong>w</strong>或<strong>mo</strong>，以表示分钟、小时、天、周或月。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL优先级]</td> 
      <td>单击下拉箭头，然后单击任务所需的优先级。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL Include e-mail attachments]</td> 
      <td> <p>（仅当电子邮件至少包含一个附件时才可用。） 单击此选项可将电子邮件中的附件保存到任务的[！UICONTROL文档]区域。 </p> <p>如果不想保存附件，请单击附件名称右侧的X。 </p> <p>如果电子邮件包含指向[!DNL Google Drive]中文档的链接，则这些链接将保存到您正在创建的任务的[！UICONTROL概述]选项卡中。 </p> <p>重要提示：为了使其正常工作，您的[!DNL Workfront]管理员必须授权[!DNL Google Drive]使用[!DNL Workfront]中的文档，如<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">配置文档集成</a>中的<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">配置集成以管理文档</a>部分所述。</p> <p>如果启用此选项，则对于您转换为任务、问题和更新的其他电子邮件，此选项将保持启用状态。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL包含电子邮件文件]</td> 
      <td> <p>单击此选项可将原始电子邮件作为电子邮件(EML)文件<span>保存到任务的[！UICONTROL文档]区域</span>。 从该位置，您可以双击文件以在电子邮件应用程序中打开电子邮件。</p> <p>如果启用此选项，则对于您转换为任务、问题和更新的其他电子邮件，此选项将保持启用状态。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 创建任务]**。

   新任务的&#x200B;**[!UICONTROL 详细信息]**&#x200B;选项卡显示在[!DNL Workfront for Google Workspace]面板中。 您可以单击&#x200B;**[!UICONTROL 更新]**&#x200B;并立即开始与协作者通信，而无需离开您的收件箱。

   在&#x200B;**[!UICONTROL 详细信息]**&#x200B;选项卡的底部，您还可以单击&#x200B;**[!UICONTROL 在[!DNL Workfront]]**&#x200B;中查看，以转到Workfront中的新任务。

   当您刷新浏览器时，[!DNL Workfront for Google Workspace]面板底部会显示一条消息，其中包含链接，用于确认您已将电子邮件转换为任务：

   您可以单击该链接以转到您已创建的任务的[!DNL Workfront for Google Workspace]面板内的“详细信息”视图。

   您可以重复这些步骤，将同一电子邮件转换为多个任务。 当您刷新浏览器或在下次返回电子邮件时，您为该电子邮件创建的所有链接都列在[!UICONTROL Workfront for Google Workspace]面板的底部。

1. （可选）通过执行以下任一操作继续处理[!DNL Workfront for Google Workspace]面板中的任务：

   * 若要在&#x200B;**[!UICONTROL 更新]**&#x200B;选项卡中添加更新，请单击&#x200B;**[!UICONTROL 开始新的更新]**&#x200B;并键入更新。

   * 若要回复&#x200B;**[!UICONTROL 更新]**&#x200B;选项卡上的更新，请单击&#x200B;**[!UICONTROL 回复]**，然后键入您的回复。

     对于上述两个操作，您可以通知特定用户您的评论。 单击&#x200B;**[!UICONTROL 通知]**，开始键入用户的名称，然后在名称出现在下拉列表中时单击该名称。 对要通知的其他用户重复此过程，然后单击&#x200B;**[!UICONTROL 发布]**。

   * 单击&#x200B;**[!UICONTROL 文档]**&#x200B;选项卡以查看随任务保存的任何文档。

您可以重复这些步骤，将同一电子邮件转换为多个任务。 当您刷新浏览器或在下次返回电子邮件时，您为该电子邮件创建的所有链接都会列在[!DNL Workfront for Google Workspace]面板的底部。
