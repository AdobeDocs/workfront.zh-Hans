---
product-area: workfront-integrations;projects
keywords: google，doc，文档，工作表，幻灯片
navigation-topic: workfront-for-g-suite
title: 使用电子邮件内容从Google Workspace更新 [!DNL Adobe Workfront] 项目
description: 您可以使用非Adobe Workfront电子邮件中的信息更新现有项目、任务或问题。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# 使用电子邮件内容更新[!DNL Adobe Workfront]中的[!DNL Google Workspace]项

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

您可以使用非[!DNL Adobe Workfront]电子邮件中的信息更新现有项目、任务或问题。

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

在使用[!DNL Workfront]中的电子邮件内容更新[!DNL Google Workspace]项之前，您必须

* 安装[!DNL Workfront for Google Workspace]\
   有关说明，请参阅[安装 [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)。

## 使用来自[!DNL Workfront]的电子邮件内容更新[!DNL Google Workspace]项

1. 如果未显示[!UICONTROL Workfront for Google Workspace]面板，请单击页面最右侧的![加载项侧边栏中的Workfront图标](assets/wf-lion-icon.png)Workfront图标[!DNL Google Workspace]。
1. 在[!DNL Google Workspace]中打开电子邮件后，在&#x200B;**[!UICONTROL 面板中单击]**&#x200B;作为新更新发布[!DNL Google Workspace]。
1. 在&#x200B;**[!UICONTROL 类型]**&#x200B;下，单击下拉箭头，然后单击要添加更新的对象类型。
1. 单击“**[!UICONTROL 搜索]**”选项，开始键入要添加更新的对象的名称，然后在项目出现在下面的列表中时选择该项目。

   此选项因您在步骤3中选择的内容而异。 它可能是&#x200B;**[!UICONTROL 搜索项目]**、**[!UICONTROL 搜索任务]**&#x200B;或&#x200B;**[!UICONTROL 搜索问题]**。

   >[!NOTE]
   >
   >键入任务的名称时，个人临时任务将从下面显示的名称列表中排除。

1. 进行以下任何可选更改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 更新]</td> 
      <td>编辑此文本的任何部分，这些部分取自电子邮件的主题行和正文文本。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include e-mail attachments]</td> 
      <td><p>（仅当电子邮件至少包含一个附件时才可用。） 单击此选项可在任务或问题的[!UICONTROL 文档]选项卡中保存附件。 </p><p>如果不想保存附件，请单击附件名称右侧的X。 </p><p>如果电子邮件包含指向[!DNL Google Drive]中文档的链接，则这些链接将保存到您正在创建的任务或问题的[!UICONTROL 概述]选项卡中。 </p><p>重要信息： <span style="color: #ff1493;"><span style="color: #000000;">要使此功能正常工作，您的</span></span>[!DNL Workfront]管理员<span style="color: #ff1493;"><span style="color: #000000;">必须授权[!DNL Google Drive]与[!DNL Workfront]</span></span>协作</p>
      <p>如果启用此选项，则对于您转换为任务、问题和更新的其他电子邮件，此选项将保持启用状态。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">通知</td> 
      <td>单击<strong>[!UICONTROL 通知]</strong>，单击显示的<strong>[!UICONTROL 搜索用户或团队]</strong>选项，然后开始键入人员或团队的名称，并在该名称出现在以下列表中时单击它。 对要添加的每个人员和团队重复此操作，然后单击<strong>[!UICONTROL 保存]</strong>。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 更新]**。

   当您刷新浏览器时，将显示一则消息，其中在[!DNL Workfront for Google Workspace]面板底部有一个链接，用于确认您已将电子邮件转换为更新：

   您可以单击该链接以转到您在步骤4中指定的对象在[!UICONTROL 中的]更新[!DNL Workfront]选项卡。

   您可以重复这些步骤，将相同的电子邮件转换为更新、任务和问题(请参阅[在 [!DNL Google Workspace] 中使用电子邮件内容创建Adobe Workfront问题](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md))。 当您刷新浏览器或在下次返回电子邮件时，您为该电子邮件创建的所有链接都列在[!UICONTROL Workfront for Google Workspace]面板的底部。

1. （可选）通过执行以下任一操作，继续在[!DNL Workfront]加载项面板中使用更新：

   * 若要在&#x200B;**[!UICONTROL 更新]**&#x200B;选项卡中添加其他更新，请单击&#x200B;**[!UICONTROL 开始新的更新]**&#x200B;并键入信息。

   * 若要回复&#x200B;**[!UICONTROL 更新]**&#x200B;选项卡上的更新，请单击&#x200B;**[!UICONTROL 回复]**，然后键入您的回复。

     对于上述两个选项，您可以单击&#x200B;**[!UICONTROL 通知]**&#x200B;以指定回复的收件人，如步骤5所示。 准备就绪后，单击&#x200B;**[!UICONTROL 帖子]**&#x200B;以添加更新或回复。

   * 单击&#x200B;**[!UICONTROL 详细信息]**&#x200B;选项卡以查看新项目、任务或问题的详细信息。
