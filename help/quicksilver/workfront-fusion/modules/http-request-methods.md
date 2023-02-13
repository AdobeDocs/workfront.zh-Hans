---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 中的HTTP请求方法 [!DNL Adobe Workfront Fusion]
description: 在模块中配置API调用时，需要填写HTTP请求方法的字段。
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 中的HTTP请求方法 [!DNL Adobe Workfront Fusion]

在模块中配置API调用时，需要填写HTTP请求方法的字段。

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## HTTP方法

使用以下HTTP方法之一。

* **[!UICONTROL GET]**:根据您的参数从Web服务器中检索数据。 [!UICONTROL GET] 请求指定资源的表示，并接收 [!UICONTROL 200 OK] 如果成功，则包含请求内容的响应消息。
* **[!UICONTROL POST]**:根据您的参数向Web服务器发送数据。 [!UICONTROL POST] 请求包括诸如上传文件之类的操作。 多个 [!UICONTROL POST]可能会导致与单个 [!UICONTROL POST]，因此请谨慎地意外发送多个 [!UICONTROL POST]s.如果 [!UICONTROL POST] 成功时，您会收到 [!UICONTROL 200 OK] 响应消息。
* **[!UICONTROL PUT]**:根据您的参数将数据发送到Web服务器中的某个位置。 [!UICONTROL PUT] 请求包括诸如上传文件之类的操作。 区分 [!UICONTROL PUT] 和 [!UICONTROL POST] 是PUT是幂等的，这意味着单次成功的结果 [!UICONTROL PUT] 与许多相同 [!UICONTROL PUT]s.如果PUT成功，您会收到200条响应消息（通常为201或204条）。
* **[!UICONTROL PATCH]**:（不适用于某些API调用模块）根据您的参数对Web服务器上的资源进行部分修改。 [!UICONTROL PATCH] 不是幂等，这表示多个 [!UICONTROL PATCH]这可能会产生意想不到的后果。 如果 [!UICONTROL PATCH] 成功时，您将收到200条响应消息（通常为204条）。
* **[!UICONTROL DELETE]**:根据您的参数（如果存在）从Web服务器中删除指定的资源。 如果 [!UICONTROL DELETE] 成功时，您会收到一则“200 OK(200 OK)”响应消息。
