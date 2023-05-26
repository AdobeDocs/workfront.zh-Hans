---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: http-modules
title: 在Adobe Workfront Fusion的HTTP模块中使用双向TLS
description: 您可以在Adobe Workfront Fusion HTTP模块中使用双方TLS，允许信息交易双方验证对方的身份。
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: 790f5da3af32ffdfcbb596f467f882a7408e3f28
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# 在中使用HTTP模块中的双向TLS [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion需要 [!DNL Adobe Workfront Fusion] 许可证以及Adobe Workfront许可证。

## 双向TLS概述

当您通过Internet发送数据时，确保数据到达或来自正确的位置，并且只有目标收件人才能阅读这些数据非常重要。 启用TLS后，客户端（请求信息的计算机）使用证书来验证服务器的身份（提供信息的计算机）。 这会创建安全的HTTP连接。

双向TLS允许此身份确认双向进行。 当服务器向客户端发送其证书以验证其身份时，它还会请求客户端的证书。 这可确保服务器不会将信息发送给可能误用的网站或用户。

>[!INFO]
>
>**示例:**
>
>* **TLS**：当用户在浏览器中键入“MyGreatBank.com”时，他们希望确保自己将访问“我的伟大银行”，而不是可能滥用或出售其银行信息的网站。 他们还想确保自己的银行账户信息被加密。
   >
   >   当浏览器（客户端）连接到MyGreatBank.com （服务器）时，TLS需要来自MyGreatBank.com的证书来验证其身份。 证书由证书颁发机构提供，例如 [!DNL DigiCert] 或 [!DNL Thawte]. 由于浏览器信任证书颁发机构，因此允许连接。
>
>* **双向TLS**： MySoftware.com是一个软件客户端，需要来自MyGreatBank.com API的信息。 MyGreatBank仅允许受信任的客户端连接到其服务器。 因此，除了验证MyGreatBank.com身份的一般TLS之外，TLS/证书颁发机构进程还验证MySoftware.com发出的请求。


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
   <td> <p>[！UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

&#42;&#42;有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 提供您的 [!DNL Workfront Fusion] 公共证书


使用HTTP请求连接到Web服务时，Web服务通常需要 [!DNL Workfront Fusion] 公开证书以供验证。 这允许Web服务将HTTP请求中提供的证书与文件上的证书进行比较，以确保该证书位于Web服务的允许列表上。

有关上传 [!DNL Adobe Workfront Fusion] 将公共证书发布到Web服务，请参阅Web服务的文档。

>[!NOTE]
>
>除了证书之外，您可能需要提供其他信息。 有关Web服务需要什么的信息，请参阅Web服务的API文档。

您可以使用以下链接下载Workfront Fusion公共证书：

### 2023年5月25日至2024年6月9日的证书

>[!IMPORTANT]
>
>* 这些 [!DNL Workfront Fusion] 公共证书将于2024年6月9日到期。 您的证书过期后，您需要向Web服务上传新证书。 我们建议您：
   >
   >   * 记下过期日期，并设置提醒，以便您自己将证书上传到您的Web服务。
   >   * 将此页面加入书签以轻松查找新证书。
>
>* 这些是非通配符mTLS证书。


* [下载 [!DNL Workfront Fusion] 证书2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)
* [下载 [!DNL Workfront Fusion] 2023年欧盟证书](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)

   在欧盟使用

<!--

### Certificates for November 14, 2022 - July 15, 2023

>[!IMPORTANT]
>
>* These [!DNL Workfront Fusion] public certificates expire on July 15, 2023.
>* These are wildcard mTLS certificates.

* [Download [!DNL Workfront Fusion] Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [Download [!DNL Workfront Fusion] EU Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   For use in the EU 

   -->

## 在中启用双向TLS [!DNL Workfront Fusion] HTTP模块

全部 [!DNL Workfront Fusion] [!UICONTROL HTTP] 请求模块可以选择启用双向TLS。

在中启用双向TLS [!UICONTROL HTTP] 请求模块：

1. 添加 [!UICONTROL HTTP] 请求模块到您的场景。
1. 开始配置模块。

   有关配置 [!UICONTROL HTTP] 请求模块，请参阅下的相应文章 [[!UICONTROL HTTP] 模块](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. 启用 **[!UICONTROL 显示高级设置]** 靠近模块底部。
1. 启用 **[!UICONTROL 使用双向TLS]**.
