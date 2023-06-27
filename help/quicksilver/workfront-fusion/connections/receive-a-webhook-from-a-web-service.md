---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 从Web服务接收Webhook
description: 如果某个Web服务当前未作为应用程序在中实施 [!DNL Adobe Workfront Fusion]，但它支持发送webhook，您可以将服务添加到使用自定义webhook模块作为即时触发器的场景中。
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# 从Web服务接收Webhook

如果某个Web服务当前未作为应用程序在中实施 [!DNL Adobe Workfront Fusion]，但它支持发送webhook，您可以将服务添加到使用自定义webhook模块作为即时触发器的场景中。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 接收webhook

1. 添加 **[!UICONTROL Webhook] >[!UICONTROL 自定义webhook]** 模块到您的场景。
1. 单击 **[!UICONTROL 添加]**，键入 **[!UICONTROL Webhook名称]** 在显示的框中，然后单击 **[!UICONTROL 保存]**.

1. 单击 **[!UICONTROL 将地址复制到剪贴板]**，然后单击 **[!UICONTROL 确定]**.

1. 登录到Web服务，并在该处执行以下操作：

   1. 在 [!UICONTROL 设置] 区域，创建webhook。
   1. 在步骤3中将您复制的地址粘贴到剪贴板。
   1. 选择将触发webhook的事件。

1. 在 [!DNL Workfront Fusion] 场景下，指定要触发的一个或多个事件 [!UICONTROL 自定义webhook] 模块。
1. 运行方案。

   当一个或多个事件发生时， [!UICONTROL 自定义webhook] 模块触发并运行场景。
