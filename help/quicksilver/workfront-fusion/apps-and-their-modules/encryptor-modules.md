---
title: 加密器
description: Adobe Workfront Fusion Encryptor模块允许您加密任何文本数据。 目前，它们支持通过AES256和PGP(OpenPGP)进行消息加密。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# 加密器

[!DNL Adobe Workfront Fusion] [!UICONTROL 加密器] 利用模块，可加密任何文本数据。 它们当前支持通过AES256和PGP([!UICONTROL OpenPGP])。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>   <p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 使用PGP的报文加解密

通过PGP加密和解密时，必须使用密钥链并创建私钥或公钥（或同时使用两者）。

有关公钥和私钥的更多信息，请参阅 [中的基本术语 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). 有关键链的更多信息，请参阅 [中的键 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL 加密器] 模块及其字段

配置 [!UICONTROL 加密器] 模块中，将显示以下字段。 模块中的粗体标题表示必填字段。

### 加密PGP消息

利用此模块，可使用公钥和私钥加密消息。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL私钥]</td>
        <td>输入发件人的私钥。 这可以验证发件人的身份。</td>
    </tr>
    <tr>
        <td>[!UICONTROL公钥]</td>
        <td>输入收件人的公共密钥。</td>
    </tr>
    <tr>
        <td>[!UICONTROL消息]</td>
        <td>输入要加密的消息。</td>
    </tr>

### 解密PGP消息

利用此模块，可使用公钥和私钥解密消息。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL私钥]</td>
        <td>输入收件人的私钥。</td>
    </tr>
    <tr>
        <td>[!UICONTROL公钥]</td>
        <td>输入收件人的公共密钥。 这可以验证发件人的身份。</td>
    </tr>
    <tr>
        <td>[!UICONTROL消息]</td>
        <td>映射要解密的消息。</td>
    </tr>
</table>
