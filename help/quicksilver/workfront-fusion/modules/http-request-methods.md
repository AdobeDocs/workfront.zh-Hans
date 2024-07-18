---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: ' [!DNL Adobe Workfront Fusion]中的HTTP请求方法'
description: 在模块中配置API调用时，需要填写HTTP请求方法的字段。
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的HTTP请求方法

在模块中配置API调用时，需要填写HTTP请求方法的字段。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

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
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## HTTP方法

使用以下HTTP方法之一。

* **[!UICONTROL GET]**：根据您的参数从Web服务器中检索数据。 [!UICONTROL GET]请求指定资源的表示形式，并在成功时接收包含所请求内容的[!UICONTROL 200 OK]响应消息。
* **[!UICONTROL POST]**：根据您的参数向Web服务器发送数据。 [!UICONTROL POST]请求包括上载文件等操作。 多个[!UICONTROL POST]可能会产生与单个[!UICONTROL POST]不同的结果，因此，对于无意中发送多个[!UICONTROL POST]，请务必谨慎。如果[!UICONTROL POST]成功，您将收到[!UICONTROL 200 OK]响应消息。
* **[!UICONTROL PUT]**：根据您的参数将数据发送到Web服务器中的某个位置。 [!UICONTROL PUT]请求包括上载文件等操作。 [!UICONTROL PUT]和[!UICONTROL POST]之间的区别在于PUT是幂等的，这意味着单个成功的[!UICONTROL PUT]的结果与许多相同的[!UICONTROL PUT]的结果相同。如果PUT成功，您将收到200响应消息（通常为201或204）。
* **[!UICONTROL PATCH]**： （对于某些API调用模块不可用）根据您的参数对Web服务器上的资源进行部分修改。 [!UICONTROL PATCH]不是幂等的，这意味着多个[!UICONTROL PATCH]的结果可能会产生意外结果。 如果[!UICONTROL PATCH]成功，您将收到200响应消息（通常为204）。
* **[!UICONTROL DELETE]**：根据您的参数从Web服务器删除指定的资源（如果该资源存在）。 如果[!UICONTROL DELETE]成功，您将收到“200确定”响应消息。
