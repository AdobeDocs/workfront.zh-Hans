---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: http-modules
title: 在Adobe Workfront Fusion的HTTP模块中使用互TLS
description: 您可以在Adobe Workfront Fusion HTTP模块中使用相互TLS，从而允许信息事务的双方验证对方的身份。
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: d54a6072524274cf77ee0ca7b7cfa24987c97782
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# 在的HTTP模块中使用相互TLS [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion需要 [!DNL Adobe Workfront Fusion] 许可证和Adobe Workfront许可证。

## 相互TLS概述

当您通过Internet发送数据时，务必确保数据从正确的位置转到或从正确的位置发送，并且只有预期的收件人可以读取数据。 启用TLS后，客户端（请求信息的计算机）使用证书来验证服务器的身份（提供信息的计算机）。 这样可实现安全的HTTP连接。

双向TLS允许双向确认此身份。 当服务器发送其证书以验证其身份到客户端时，它还会请求客户端的证书。 这可确保服务器不会向滥用信息的网站或用户发送信息。

>[!INFO]
>
>**示例:**
>
>* **TLS**:当某人在浏览器中键入“MyGreatBank.com”时，他们希望确保自己会进入“我的Great Bank”，而不是可能滥用或出售其银行信息的网站。 他们还希望确保自己的银行账户信息被加密。
   >
   >   当浏览器（客户端）连接到MyGreatBank.com（服务器）时，TLS需要MyGreatBank.com的证书来验证其身份。 证书由证书颁发机构提供，例如 [!DNL DigiCert] 或 [!DNL Thawte]. 由于浏览器信任证书颁发机构，因此允许连接。
>
>* **相互TLS**:MySoftware.com是一个软件客户端，需要MyGreatBank.com API中的信息。 MyGreatBank仅允许受信任的客户连接到其服务器。 因此，除了验证MyGreatBank.com身份的常规TLS外，TLS/证书颁发机构流程还验证来自MySoftware.com的请求。


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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

&#42;&#42;有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 提供 [!DNL Workfront Fusion] 公共证书


当您通过HTTP请求连接到Web服务时，Web服务通常需要 [!DNL Workfront Fusion] 公共验证证书。 这允许Web服务将HTTP请求中提供的证书与文件中的证书进行比较，以确保证书位于Web服务的允许列表上。

有关上传 [!DNL Adobe Workfront Fusion] web服务的公共证书，请参阅web服务的文档。

>[!NOTE]
>
>除了证书之外，您可能还需要提供其他信息。 有关Web服务所需内容的信息，请参阅Web服务的API文档。

您可以使用以下链接下载Workfront Fusion公共证书：

### 2023年5月25日至2024年6月9日的证明

>[!IMPORTANT]
>
>* 这些 [!DNL Workfront Fusion] 公共证书将于2024年6月9日到期。 在您的证书过期后，您需要将新证书上载到Web服务。 我们建议您：
   >
   >   * 记下过期日期，并设置提醒，供您自己将证书上传到Web服务。
   >   * 将此页面加入书签以轻松查找新证书。
>
* 它们是非通配符mTLS证书。
>

* [下载 [!DNL Workfront Fusion] 证书2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-us-mtls-certificate.pem)
* [下载 [!DNL Workfront Fusion] 2023年欧盟证书](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)

   用于欧盟

### 2022年11月14日至2023年7月15日的证书

>[!IMPORTANT]
>
>* 这些 [!DNL Workfront Fusion] 公共证书将于2023年7月15日到期。
>* 它们是通配符mTLS证书。


* [下载 [!DNL Workfront Fusion] 证书2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [下载 [!DNL Workfront Fusion] 2023年欧盟证书](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   用于欧盟

## 在中启用相互TLS [!DNL Workfront Fusion] HTTP模块

全部 [!DNL Workfront Fusion] [!UICONTROL HTTP] 请求模块可以选择启用相互TLS。

在 [!UICONTROL HTTP] 请求模块：

1. 添加 [!UICONTROL HTTP] 请求模块添加到您的方案。
1. 开始配置模块。

   有关配置 [!UICONTROL HTTP] 请求模块，请参阅 [[!UICONTROL HTTP] 模块](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. 启用 **[!UICONTROL 显示高级设置]** 接近模块底部。
1. 启用 **[!UICONTROL 使用互相TLS]**.
