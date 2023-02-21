---
product-area: workfront-integrations;projects
keywords: google，doc，document，sheet，幻灯片
navigation-topic: workfront-for-g-suite
title: 创建 [!DNL Adobe Workfront] 使用电子邮件内容的G Suite中的任务
description: 您可以转换外部电子邮件(不是由Adobe生成) [!DNL Workfront])到Workfront任务。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 925e8f9d57d65fcb44068274800450d9db5c9d34
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# 创建 [!DNL Adobe Workfront] 任务 [!DNL G Suite] 使用电子邮件内容

>[!NOTE]
>
>有 [已知问题](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) 的当前版本 [!DNL Workfront for G Suite] 无法按预期工作。 我们正在开发新版本，并期待该版本发布到 [!DNL Google Marketplace] 在不久的将来。

您可以转换外部电子邮件(不是由 [!DNL Adobe Workfront]) [!DNL Workfront] 任务。

您还可以将外部电子邮件转换为现有任务的更新。 有关更多信息，请参阅 [更新 [!DNL Adobe Workfront] 使用电子邮件内容从[!DNL G Suite]中获取项目](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

有关使用 [!DNL G Suite] 处理由发送的通知电子邮件 [!DNL Workfront]，请参阅 [管理 [!DNL Adobe Workfront] 来自[!DNL G Suite]的通知详细信息](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

## 先决条件

在创建 [!DNL Workfront] 任务 [!DNL G Suite]，您必须

* 安装 [!DNL Workfront for G suite]\
   有关说明，请参阅 [安装 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 创建 [!DNL Adobe Workfront] 任务 [!DNL G Suite] 使用电子邮件内容

1. 如果 [!UICONTROL Workfront for G Suite] 未显示面板，请单击 [!DNL Workfront] 图标 ![](assets/wf-lion-icon.png) 在 [!DNL G Suite] 页面最右侧的附加组件侧栏。
1. 在中打开电子邮件 [!DNL G Suite]，单击 [!DNL Workfront for G Suite] 将电子邮件转换为 [!DNL Workfront] 任务。

1. 选择 **[!UICONTROL 新建]** 选项来指示任务是属于项目还是属于独立于项目的个人任务。
1. 如果要将任务附加到父项目，请单击 **[!UICONTROL 项目名称]**，开始键入所需任务的项目名称，然后在项目名称出现在下面的列表中时单击该名称。
1. 进行以下任何更改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL任务名称]</td> 
      <td>编辑此文本的任何部分，该部分取自电子邮件的主题行。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td>编辑此文本的任何部分，该部分取自电子邮件正文。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Assign To]</td> 
      <td>单击 <strong>[!UICONTROL Assign To]</strong>，请单击 <strong>[!UICONTROL将其分配给]</strong> 选项，然后开始键入人员的姓名，并在出现在下面的列表时单击该姓名。 对要添加的每个人员重复此操作，然后单击 <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL计划持续时间]</td> 
      <td> <p>单击 <strong>[!UICONTROL计划持续时间]</strong>，然后键入您希望该任务所用的天数。 </p> <p>注意：可以通过不同方式为贵组织配置此选项。 例如，对于您的组织，您可能需要键入小时数而不是天数。 如果您需要更多信息，请参阅 [!DNL Workfront] 管理员。 如果要指定除已配置的默认值之外的其他时间段，请键入 <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong>或 <strong>mo</strong> 在数字之后，表示分钟、小时、天、周或月。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL优先级]</td> 
      <td>单击下拉箭头，然后单击任务所需的优先级。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL包含电子邮件附件]</td> 
      <td> <p>（仅当电子邮件至少包含一个附件时才可用。） 单击此选项可将电子邮件中的附件保存到任务的[!UICONTROL Documents]区域。 </p> <p>如果不想保存附件，请单击其名称右侧的X。 </p> <p>如果电子邮件包含指向 [!DNL Google Drive]，则会将它们保存到您所创建任务的[!UICONTROL概述]选项卡。 </p> <p>重要信息：为了使其正常工作， [!DNL Workfront] 管理员必须授权 [!DNL Google Drive] 在 [!DNL Workfront]，如一节中所述 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">配置集成以管理文档</a> 在文章中 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">配置文档集成</a>.</p> <p>如果启用此选项，则对于您转换为任务、问题和更新的其他电子邮件，此选项将保持启用状态。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email file]</td> 
      <td> <p>单击此选项可将原始电子邮件另存为电子邮件(EML)文件 <span>到[!UICONTROL Documents]区域</span> 任务。 从此处，您可以双击文件以在电子邮件应用程序中打开电子邮件。</p> <p>如果启用此选项，则对于您转换为任务、问题和更新的其他电子邮件，此选项将保持启用状态。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 创建任务]**.

   的 **[!UICONTROL 详细信息]** 选项卡 [!DNL Workfront for G Suite] 的上界。 您可以单击 **[!UICONTROL 更新]** 并立即开始与协作者通信，而不会离开您的盒子。

   在 **[!UICONTROL 详细信息]** ，也可以单击 **[!UICONTROL 查看[!DNL Workfront]]** 去Workfront执行新任务。

   刷新浏览器时，会在 [!DNL Workfront for G Suite] 面板会确认您已将电子邮件转换为任务：

   您可以单击该链接以转到 [!DNL Workfront for G Suite] 面板。

   您可以重复这些步骤，将同一封电子邮件转换为多个任务。 当您再次刷新浏览器或返回到电子邮件时，您为该电子邮件创建的所有链接都将列在 [!UICONTROL Workfront for G Suite] 的上界。

1. （可选）继续处理 [!DNL Workfront for G Suite] 面板，方法是执行以下任一操作：

   * 在 **[!UICONTROL 更新]** ，单击 **[!UICONTROL 开始新更新]** 并键入更新。

   * 对 **[!UICONTROL 更新]** ，单击 **[!UICONTROL 回复]** 然后键入您的回复。

      对于上述两个操作，您可以通知特定用户您的评论。 单击 **[!UICONTROL 通知]**，开始键入用户的名称，然后在下拉列表中显示该名称时单击该名称。 对要通知的其他用户重复此过程，然后单击 **[!UICONTROL 帖子]**.

   * 单击 **[!UICONTROL 文档]** 选项卡，以查看随任务保存的任何文档。

您可以重复这些步骤，将同一封电子邮件转换为多个任务。 当您再次刷新浏览器或返回到电子邮件时，您为该电子邮件创建的所有链接都将列在 [!DNL Workfront for G Suite] 的上界。
