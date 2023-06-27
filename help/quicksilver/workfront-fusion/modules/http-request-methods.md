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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 中的HTTP请求方法 [!DNL Adobe Workfront Fusion]

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

## HTTP方法

使用以下HTTP方法之一。

* **[!UICONTROL GET]**：根据您的参数从Web服务器检索数据。 [!UICONTROL GET] 请求指定资源的表示形式，并接收 [!UICONTROL 200 OK] 响应消息，其中包含请求的内容（如果成功）。
* **[!UICONTROL POST]**：根据您的参数向Web服务器发送数据。 [!UICONTROL POST] 请求包括上载文件等操作。 多个 [!UICONTROL POST]s可能导致与单个不同的结果 [!UICONTROL POST]因此，对于无意中发送多个IP地址时请务必谨慎 [!UICONTROL POST]s.如果 [!UICONTROL POST] 成功，您将收到 [!UICONTROL 200 OK] 响应消息。
* **[!UICONTROL PUT]**：根据您的参数将数据发送到Web服务器中的某个位置。 [!UICONTROL PUT] 请求包括上载文件等操作。 以下各项之间的差异： [!UICONTROL PUT] 和 [!UICONTROL POST] PUT是幂等的，也就是说一次成功的结果 [!UICONTROL PUT] 与许多相同项目相同 [!UICONTROL PUT]s.如果PUT成功，您将收到200响应消息（通常为201或204）。
* **[!UICONTROL PATCH]**：（对某些API调用模块不可用）根据您的参数对Web服务器上的资源应用部分修改。 [!UICONTROL PATCH] 不是幂等的，也就是说多次波的结果 [!UICONTROL PATCH]可能会造成意想不到的后果。 如果 [!UICONTROL PATCH] 成功，您将收到一条200响应消息（通常为204）。
* **[!UICONTROL DELETE]**：根据您的参数（如果资源存在）从Web服务器中删除指定的资源。 如果 [!UICONTROL DELETE] 成功，您将收到“200 OK”响应消息。
