---
product-area: workfront-integrations;projects
keywords: google，doc，文档，工作表，幻灯片
navigation-topic: workfront-for-g-suite
title: 创建 [!DNL Adobe Workfront] G Suite中使用电子邮件内容的任务
description: 您可以转换外部电子邮件(不由Adobe生成) [!DNL Workfront])到Workfront任务。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 0%

---

# 创建 [!DNL Adobe Workfront] 任务位置 [!DNL G Suite] 使用电子邮件内容

>[!NOTE]
>
>适用于Google的Adobe Workfront插件的最新版本于2023年6月26日发布。

您可以转换外部电子邮件（不是由生成的） [!DNL Adobe Workfront])到 [!DNL Workfront] 任务。

您还可以将外部电子邮件转换为现有任务上的更新。 有关更多信息，请参阅 [更新 [!DNL Adobe Workfront] 使用电子邮件内容的[！DNL G Suite]中的项目](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

有关使用的信息 [!DNL G Suite] 处理发送通知电子邮件的方式 [!DNL Workfront]，请参见 [管理 [!DNL Adobe Workfront] 来自[！DNL G Suite]的通知详细信息](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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
   <td> <p>[！UICONTROL工作]，[！UICONTROL计划]</p> </td> 
  </tr> 
   </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 先决条件

在创建 [!DNL Workfront] 任务位置 [!DNL G Suite]，您必须

* 安装 [!DNL Workfront for G suite]\
   有关说明，请参阅 [安装 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 创建 [!DNL Adobe Workfront] 任务位置 [!DNL G Suite] 使用电子邮件内容

1. 如果 [!UICONTROL 适用于G Suite的Workfront] 面板未显示，请单击 [!DNL Workfront] 图标 ![](assets/wf-lion-icon.png) 在 [!DNL G Suite] 页面最右侧的附加组件侧栏。
1. 在中打开电子邮件 [!DNL G Suite]中，单击某个选项 [!DNL Workfront for G Suite] 将电子邮件转换为新电子邮件 [!DNL Workfront] 任务。

1. 选择 **[!UICONTROL 新建]** 用于指示任务是要成为项目的一部分还是独立于项目的个人任务的选项。
1. 如果要将任务附加到父项目，请单击 **[!UICONTROL 项目名称]**，开始键入要将任务放置在其中的项目名称，然后在项目名称显示在以下列表中时单击该名称。
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
      <td>编辑此文本的任何部分，这些部分取自电子邮件的正文。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL分配给]</td> 
      <td>单击 <strong>[！UICONTROL分配给]</strong>，单击 <strong>[！UICONTROL将此项分配给]</strong> 选项，然后开始键入人员姓名，并在姓名出现在以下列表中时单击该名称。 对要添加的每个人重复此操作，然后单击 <strong>[！UICONTROL保存]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL计划持续时间]</td> 
      <td> <p>单击 <strong>[！UICONTROL计划持续时间]</strong>，然后键入您希望任务花费的天数。 </p> <p>注意：可以通过不同方式为您的组织配置此选项。 例如，对于您的组织，您可能需要键入小时数而不是天数。 如果您需要更多信息，请参见 [!DNL Workfront] 管理员。 如果要指定非配置默认的时间段，请键入 <strong>m</strong>， <strong>h</strong>， <strong>d</strong>， <strong>w</strong>，或 <strong>月</strong> 在数字之后，表示分钟、小时、天、周或月。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL优先级]</td> 
      <td>单击下拉箭头，然后单击任务所需的优先级。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL包含电子邮件附件]</td> 
      <td> <p>（仅当电子邮件至少包含一个附件时才可用。） 单击此选项可将电子邮件中的附件保存到任务的[！UICONTROL文档]区域。 </p> <p>如果不想保存附件，请单击附件名称右侧的X。 </p> <p>如果电子邮件包含指向中文档的链接 [!DNL Google Drive]，则它们会保存到正在创建的任务的[！UICONTROL概述]选项卡中。 </p> <p>重要提示：为了让此功能发挥作用，请 [!DNL Workfront] 管理员必须授权 [!DNL Google Drive] 在中处理文档 [!DNL Workfront]，如一节中所述 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">配置集成以管理文档</a> 在文章中 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">配置文档集成</a>.</p> <p>如果启用此选项，则对于您转换为任务、问题和更新的其他电子邮件，它仍保持启用状态。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL包含电子邮件文件]</td> 
      <td> <p>单击此选项可将原始电子邮件另存为电子邮件(EML)文件 <span>到[！UICONTROL文档]区域</span> 任务的。 从该位置，您可以双击文件以在电子邮件应用程序中打开电子邮件。</p> <p>如果启用此选项，则对于您转换为任务、问题和更新的其他电子邮件，它仍保持启用状态。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 创建任务]**.

   此 **[!UICONTROL 详细信息]** 新任务的选项卡显示在 [!DNL Workfront for G Suite] 面板。 您可以单击 **[!UICONTROL 更新]** 并且立即开始与协作者通信，无需离开您的收件箱。

   在底部 **[!UICONTROL 详细信息]** 选项卡，您还可以单击 **[!UICONTROL 在中查看[!DNL Workfront]]** 转到Workfront中的新任务。

   当您刷新浏览器时，会出现一条消息，其中底部有一个链接 [!DNL Workfront for G Suite] 面板确认您已将电子邮件转换为任务：

   您可以单击链接以转到详细信息视图，该视图位于 [!DNL Workfront for G Suite] 面板，用于您已创建的任务。

   您可以重复这些步骤，将同一电子邮件转换为多个任务。 当您刷新浏览器或在其他时间返回电子邮件时，您为该电子邮件创建的所有链接都列在 [!UICONTROL 适用于G Suite的Workfront] 面板。

1. （可选）继续使用 [!DNL Workfront for G Suite] 执行以下任一操作来创建panel ：

   * 要在中添加更新，请执行以下操作 **[!UICONTROL 更新]** 选项卡，单击 **[!UICONTROL 开始新的更新]** 并键入更新。

   * 回复 **[!UICONTROL 更新]** 选项卡，单击 **[!UICONTROL 回复]** 并键入您的回复。

     对于上述两个操作，您可以通知特定用户您的评论。 单击 **[!UICONTROL 通知]**，开始键入用户的名称，然后在名称出现在下拉列表中时单击该名称。 对要通知的其他用户重复此过程，然后单击 **[!UICONTROL Post]**.

   * 单击 **[!UICONTROL 文档]** 选项卡，查看随任务一起保存的任何文档。

您可以重复这些步骤，将同一电子邮件转换为多个任务。 当您刷新浏览器或在其他时间返回电子邮件时，您为该电子邮件创建的所有链接都列在 [!DNL Workfront for G Suite] 面板。
