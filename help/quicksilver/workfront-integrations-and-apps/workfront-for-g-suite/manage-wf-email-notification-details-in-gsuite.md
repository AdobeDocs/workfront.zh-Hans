---
product-area: workfront-integrations
keywords: google，doc，document，sheet，幻灯片
navigation-topic: workfront-for-g-suite
title: 管理 [!DNL Adobe Workfront] 来自G Suite的通知详细信息
description: 在G Suite中，打开通知电子邮件Adobe [!DNL Workfront] 发送后，您可以查看关联的工作项详细信息并做出响应，而无需离开收件箱。 如果可以执行一些操作（例如批准请求），则可以直接从Workfront for G Suite中执行这些操作。
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 0934ae23a8e80dd18872efef7d274bd57d227647
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# 管理 [!DNL Adobe Workfront] 通知详细信息来自 [!DNL G Suite]

>[!NOTE]
>
>有 [已知问题](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) 的当前版本 [!DNL Workfront for G Suite] 无法按预期工作。 我们正在开发新版本，并期待该版本发布到 [!DNL Google Marketplace] 在不久的将来。

在 [!DNL G Suite]，当您打开通知电子邮件时 [!DNL Adobe Workfront] 已发送，您可以查看关联的工作项详细信息并做出响应，而无需离开 [!UICONTROL 收件箱]. 如果可以执行一些操作（例如批准请求），则您可以直接从 [!DNL Workfront for G Suite].

>[!NOTE]
>
> [!DNL Workfront for G Suite] 支持从接收的几乎每种类型的电子邮件通知 [!DNL Workfront] （大约120种不同类型）。 [!UICONTROL 每日摘要] 发送的电子邮件 [!DNL Workfront] 不显示在 [!DNL Workfront for G Suite]. 有关 [!DNL Workfront] 电子邮件通知类型，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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

在从 [!DNL G Suite]，您必须

* 安装 [!DNL Workfront for G suite]\
   有关说明，请参阅 [安装 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 管理 [!DNL Adobe Workfront] 通知详细信息来自 [!DNL G Suite]

1. 如果 [!DNL Workfront for G Suite] 未显示面板，请单击 [!DNL Workfront] 图标 ![](assets/wf-lion-icon.png) 在 [!DNL G Suite] 页面最右侧的附加组件侧栏。
1. 在 [!DNL G Suite]，打开 [!DNL Workfront] 通知电子邮件。
1. 单击 **[!UICONTROL 查看所有更新]** 如果显示在面板顶部附近，则不会显示。
1. 单击 **[!UICONTROL 详细信息]**.
1. 单击任何可用选项。

   可能显示的选项与您打开的电子邮件通知类型相关。 例如，如果是要求您批准任务的电子邮件通知，您会看到 **[!UICONTROL 批准]** 和 **[!UICONTROL 拒绝]** 而不是 **[!UICONTROL 处理它]** 或 **[!UICONTROL 完成]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>电子邮件通知的类型</th> 
      <th>操作</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>任务或问题</td> 
      <td><strong>[!UICONTROL Approve]</strong> 它， <strong>[!UICONTROL Reject]</strong> 它， <strong>[!UICONTROL授予]</strong> 访问权限， <strong>[!UICONTROL忽略]</strong> 请求访问该文件， <strong>[!UICONTROL Work it]</strong>，或者单击相应选项以指示您是 <strong>[!UICONTROL Done]</strong> 和</td> 
     </tr> 
     <tr> 
      <td>项目</td> 
      <td><strong>[!UICONTROL Approve]</strong> 它， <strong>[!UICONTROL Reject]</strong> 它， <strong>[!UICONTROL授予]</strong> 对其的访问权限，或 <strong>[!UICONTROL忽略]</strong> 访问请求</td> 
     </tr> 
     <tr> 
      <td>文档</td> 
      <td><strong>[!UICONTROL Approve]</strong> 它， <strong>[!UICONTROL Reject]</strong> 它， <strong>[!UICONTROL授予]</strong> 对其的访问权限，或 <strong>[!UICONTROL忽略]</strong> 访问请求</td> 
     </tr> 
     <tr> 
      <td>更新 </td> 
      <td> <p>查看项目整个更新列表的任何部分，以便您拥有所需的上下文 <strong>[!UICONTROL Post]</strong> 新更新或 <strong>[!UICONTROL Reply]</strong>. 您可以单击 <strong>[!UICONTROL Notify]</strong> 提醒特定用户您的回复。 </p> <p>有关更多信息，请参阅 <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">回复 [!DNL Adobe Workfront] 更新通知 [!DNL G Suite]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>批准请求</td> 
      <td><strong>[!UICONTROL Approve]</strong> 或 <strong>[!UICONTROL Reject]</strong> 它（您可以通过单击其他选项来改变主意）、下载它、查看它的所有者或查看它的参考编号</td> 
     </tr> 
     <tr> 
      <td>项目状态的更改</td> 
      <td> 查看有关项目的所有当前信息，包括任何自定义表单。 </td> 
     </tr> 
    </tbody> 
   </table>
