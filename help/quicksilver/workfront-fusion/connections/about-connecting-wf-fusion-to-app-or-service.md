---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 关于连接 [!DNL Adobe Workfront Fusion] 至应用程序或服务
description: 对于大多数应用程序，需要创建一个连接，通过该连接 [!DNL Adobe Workfront Fusion] 可以根据特定场景的设置与给定的第三方服务通信。
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 关于连接 [!DNL Adobe Workfront Fusion] 至应用程序或服务

对于大多数应用程序，需要创建一个连接，通过该连接 [!DNL Adobe Workfront Fusion] 可以根据特定场景的设置与给定的第三方服务通信。

例如，如果要创建一个方案，以从中检索信息 [!DNL Workfront]，您必须授予访问权限 [!DNL Workfront Fusion] 访问 [!DNL Workfront] 帐户。

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

## 访问权限

对于每一个连接， [!DNL Workfront Fusion] 仅需要那些成功完成给定方案所需的访问权限。 例如，如果您创建一个方案以列出文档 [!DNL Google Docs]， [!DNL Workfront Fusion] 不要求获取文档内容的权限。

很遗憾，并非所有服务都允许您限制对特定任务的访问。 因此， [!DNL Workfront Fusion] 必须要求完全访问权限。 有关如何限制的详细信息 [!DNL Workfront Fusion] 访问您在这些服务上注册的帐户，请参阅特定于应用程序的文档。

## 关于管理连接

您可以管理所有连接，从 [!UICONTROL 连接] 区域。 在此，您可以：

* 查看授予了哪些权限 [!DNL Workfront Fusion] 每个连接
* 重命名连接
* 重新授权现有连接
* 删除现有连接
* 验证是否成功建立了与服务的连接

打开 [!UICONTROL 连接] 区域，单击 <b>[!UICONTROL 连接]</b> 左侧导航栏中。

## 续订连接

[!DNL Workfront Fusion] 通常不受限制地获得对给定服务的访问权限。 然而，情况并非总是如此。 对于某些服务，必须在特定时间段后续订访问权限。 在这些情况下， [!DNL Workfront Fusion] 在访问权限过期前不久，通过电子邮件通知您。

要续订连接，请执行以下操作：

1. 单击 **[!UICONTROL 重新授权]** 中的按钮 **[!UICONTROL 连接]** 区域。
