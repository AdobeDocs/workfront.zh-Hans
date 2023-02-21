---
product-area: workfront-integrations;projects
keywords: google，doc，document，sheet，幻灯片
navigation-topic: workfront-for-g-suite
title: 更新 [!DNL Adobe Workfront] 使用电子邮件内容的G Suite中的项目
description: 您可以使用非Adobe Workfront电子邮件中的信息更新现有项目、任务或问题。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 925e8f9d57d65fcb44068274800450d9db5c9d34
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# 更新 [!DNL Adobe Workfront] 项目自 [!DNL G Suite] 使用电子邮件内容

>[!NOTE]
>
>有 [已知问题](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) 的当前版本 [!DNL Workfront for G Suite] 无法按预期工作。 我们正在开发新版本，并期待该版本发布到 [!DNL Google Marketplace] 在不久的将来。

您可以使用非[!DNL Adobe Workfront] 电子邮件。

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

在更新 [!DNL Workfront] 使用电子邮件内容的项目 [!DNL G Suite]，您必须

* 安装 [!DNL Workfront for G suite]\
   有关说明，请参阅 [安装 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 更新 [!DNL Workfront] 使用电子邮件内容的项目 [!DNL G Suite]

1. 如果 [!UICONTROL Workfront for G Suite] 面板时，单击Workfront图标 ![](assets/wf-lion-icon.png) 在 [!DNL G Suite] 页面最右侧的附加组件侧栏。
1. 在中打开电子邮件 [!DNL G Suite]，单击 **[!UICONTROL 发布为新更新]** 在 [!DNL G Suite] 的上界。
1. 在 **[!UICONTROL 类型]**，单击下拉箭头，然后单击要在其中添加更新的对象类型。
1. 单击 **[!UICONTROL 搜索]** 选项，开始键入要添加更新的对象的名称，然后在项目显示在下面的列表中时选择该项目。

   此选项会因您在步骤3中选择的内容而异。 可能是 **[!UICONTROL 搜索项目]**, **[!UICONTROL 搜索任务]**&#x200B;或 **[!UICONTROL 搜索问题]**.

   >[!NOTE]
   >
   >在键入任务名称时，临时个人任务将从下面显示的名称列表中排除。

1. 进行以下任意可选更改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL更新]</td> 
      <td>编辑此文本的任何部分，该部分取自电子邮件的主题行和正文文本。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL包含电子邮件附件]</td> 
      <td><p>（仅当电子邮件至少包含一个附件时才可用。） 单击此选项可在[!UICONTROL Documents]选项卡中保存任务或问题的附件。 </p><p>如果不想保存附件，请单击其名称右侧的X。 </p><p>如果电子邮件包含指向 [!DNL Google Drive]，则这些链接会保存到您所创建任务或问题的[!UICONTROL概述]选项卡。 </p><p>重要信息： <span style="color: #ff1493;"><span style="color: #000000;">为了使其正常工作，</span></span>[!DNL Workfront] 管理员<span style="color: #ff1493;"><span style="color: #000000;"> 必须授权 [!DNL Google Drive] 使用 [!DNL Workfront]</span></span></p>
      <p>如果启用此选项，则对于您转换为任务、问题和更新的其他电子邮件，此选项将保持启用状态。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">通知</td> 
      <td>单击 <strong>[!UICONTROL Notify]</strong>，请单击 <strong>[!UICONTROL搜索用户或团队]</strong> 选项，然后开始键入人员或团队的名称，并在出现在下面的列表中时单击该名称。 对要添加的每个人员和团队重复此操作，然后单击 <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 更新]**.

   刷新浏览器时，会在 [!DNL Workfront for G Suite] 面板会确认您已将电子邮件转换为更新：

   您可以单击链接以转到 [!UICONTROL 更新] 选项卡 [!DNL Workfront] 对于您在步骤4中指定的对象。

   您可以重复这些步骤以将同一电子邮件转换为更新、任务和问题(请参阅 [在[!DNL G Suite]中使用电子邮件内容创建Adobe Workfront问题](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md))。 当您再次刷新浏览器或返回到电子邮件时，您为该电子邮件创建的所有链接都将列在 [!UICONTROL Workfront for G Suite] 的上界。

1. （可选）继续处理 [!DNL Workfront] 附加组件面板，方法是执行以下任一操作：

   * 在 **[!UICONTROL 更新]** ，单击 **[!UICONTROL 开始新更新]** 并键入信息。

   * 对 **[!UICONTROL 更新]** ，单击 **[!UICONTROL 回复]** 然后键入您的回复。

      对于上述两个选项，您可以单击 **[!UICONTROL 通知]** 按步骤5指定回复的收件人。 准备就绪后，单击 **[!UICONTROL 帖子]** 添加更新或回复。

   * 单击 **[!UICONTROL 详细信息]** 选项卡，以查看有关新项目、任务或问题的详细信息。
