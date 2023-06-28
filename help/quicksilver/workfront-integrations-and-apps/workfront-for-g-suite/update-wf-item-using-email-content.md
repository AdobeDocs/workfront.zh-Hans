---
product-area: workfront-integrations;projects
keywords: google，doc，文档，工作表，幻灯片
navigation-topic: workfront-for-g-suite
title: 更新 [!DNL Adobe Workfront] 使用电子邮件内容的G Suite中的项目
description: 您可以使用非Adobe Workfront电子邮件中的信息更新现有项目、任务或问题。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# 更新 [!DNL Adobe Workfront] 项目来源 [!DNL G Suite] 使用电子邮件内容

>[!NOTE]
>
>适用于Google的Adobe Workfront插件的最新版本于2023年6月26日发布。

您可以使用来自以下项的信息更新现有项目、任务或问题：[!DNL Adobe Workfront] 电子邮件。

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

在您可以更新 [!DNL Workfront] 使用来自的电子邮件内容的项目 [!DNL G Suite]，您必须

* 安装 [!DNL Workfront for G suite]\
   有关说明，请参阅 [安装 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 更新 [!DNL Workfront] 使用来自的电子邮件内容的项目 [!DNL G Suite]

1. 如果 [!UICONTROL 适用于G Suite的Workfront] 面板未显示，请单击Workfront图标 ![](assets/wf-lion-icon.png) 在 [!DNL G Suite] 页面最右侧的附加组件侧栏。
1. 在中打开电子邮件 [!DNL G Suite]，单击 **[!UICONTROL 发布为新更新]** 在 [!DNL G Suite] 面板。
1. 下 **[!UICONTROL 类型]**，单击下拉箭头，然后单击要添加更新的对象类型。
1. 单击 **[!UICONTROL 搜索]** 选项，开始键入要添加更新的对象的名称，然后在该项目出现在下面的列表中时选择该项目。

   此选项会根据您在步骤3中选择的内容而有所不同。 有可能 **[!UICONTROL 搜索项目]**， **[!UICONTROL 搜索任务]**，或 **[!UICONTROL 搜索问题]**.

   >[!NOTE]
   >
   >键入任务名称时，个人临时任务将从下面显示的名称列表中排除。

1. 进行以下任何可选更改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL更新]</td> 
      <td>编辑此文本的任何部分，这些部分取自电子邮件的主题行和正文文本。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL包含电子邮件附件]</td> 
      <td><p>（仅当电子邮件至少包含一个附件时才可用。） 单击此选项可将附件保存在任务或问题的[！UICONTROL文档]选项卡中。 </p><p>如果不想保存附件，请单击附件名称右侧的X。 </p><p>如果电子邮件包含指向中文档的链接 [!DNL Google Drive]，则链接将保存到您创建的任务或问题的[！UICONTROL概述]选项卡。 </p><p>重要提示： <span style="color: #ff1493;"><span style="color: #000000;">为了让此功能正常工作，您的</span></span>[!DNL Workfront] 管理员<span style="color: #ff1493;"><span style="color: #000000;"> 必须授权 [!DNL Google Drive] 使用 [!DNL Workfront]</span></span></p>
      <p>如果启用此选项，则对于您转换为任务、问题和更新的其他电子邮件，它仍保持启用状态。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">通知</td> 
      <td>单击 <strong>[！UICONTROL Notify]</strong>，单击 <strong>[！UICONTROL搜索用户或团队]</strong> 选项，然后开始键入人员或团队的名称，并在该名称出现在以下列表中时单击它。 对要添加的每个人员和团队重复此操作，然后单击 <strong>[！UICONTROL保存]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 更新]**.

   当您刷新浏览器时，会出现一条消息，其中底部有一个链接 [!DNL Workfront for G Suite] 面板确认您已将电子邮件转换为更新：

   您可以单击链接以转到 [!UICONTROL 更新] 按Tab键进入 [!DNL Workfront] （对于您在步骤4中指定的对象）。

   您可以重复这些步骤，将相同的电子邮件转换为更新、任务和问题(请参阅 [使用电子邮件内容在[！DNL G Suite]中创建Adobe Workfront问题](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md))。 当您刷新浏览器或在其他时间返回电子邮件时，您为该电子邮件创建的所有链接都列在 [!UICONTROL 适用于G Suite的Workfront] 面板。

1. （可选）继续使用中的更新 [!DNL Workfront] 通过执行以下任一操作，可访问附加面板：

   * 要在中添加其他更新，请执行以下操作 **[!UICONTROL 更新]** 选项卡，单击 **[!UICONTROL 开始新的更新]** 并键入相应信息。

   * 回复 **[!UICONTROL 更新]** 选项卡，单击 **[!UICONTROL 回复]** 并键入您的回复。

     对于以上两个选项，您可以单击 **[!UICONTROL 通知]** 以指定回复的收件人，如步骤5中所示。 准备就绪后，单击 **[!UICONTROL Post]** 以添加更新或回复。

   * 单击 **[!UICONTROL 详细信息]** 选项卡以查看新项目、任务或问题的详细信息。
