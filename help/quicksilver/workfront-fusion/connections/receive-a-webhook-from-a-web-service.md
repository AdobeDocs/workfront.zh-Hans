---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 从Web服务接收Web挂接
description: 如果Web服务当前未作为 [!DNL Adobe Workfront Fusion]，但是它支持发送webhooks，您可以将该服务添加到使用自定义webhook模块作为即时触发器的情景中。
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# 从Web服务接收Web挂接

如果Web服务当前未作为 [!DNL Adobe Workfront Fusion]，但是它支持发送webhooks，您可以将该服务添加到使用自定义webhook模块作为即时触发器的情景中。

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 接收网页挂接

1. 添加 **[!UICONTROL Webhooks] >[!UICONTROL 自定义Webhook]** 模块。
1. 单击 **[!UICONTROL 添加]**，键入 **[!UICONTROL Webhook名称]** 在显示的框中，单击 **[!UICONTROL 保存]**.

1. 单击 **[!UICONTROL 将地址复制到剪贴板]**，然后单击 **[!UICONTROL 确定]**.

1. 登录到Web服务，并在此执行以下操作：

   1. 在 [!UICONTROL 设置] 的区域，请创建webhook。
   1. 在步骤3中，将复制的地址粘贴到剪贴板。
   1. 选择将触发Webhook的事件。

1. 在 [!DNL Workfront Fusion] 方案中，指定要触发的事件 [!UICONTROL 自定义Webhook] 模块。
1. 运行方案。

   当一个或多个事件发生时， [!UICONTROL 自定义Webhook] 模块触发器，并运行方案。
