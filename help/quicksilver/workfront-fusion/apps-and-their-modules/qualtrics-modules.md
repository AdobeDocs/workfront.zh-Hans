---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Qualtrics模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用Qualtrics的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Qualtrics模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Qualtrics]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## 先决条件

使用 [!DNL Qualtrics] 模块，您必须 [!UICONTROL Qualtrics] 帐户。

## 连接 [!DNL Qualtrics] to [!DNL Workfront Fusion]

您可以创建与 [!DNL Qualtrics] 直接从内部帐户 [!UICONTROL Qualtrics] 模块。

1. 在任意 [!UICONTROL Qualtrics] 模块，单击 **[!UICONTROL 添加]** 旁边 [!UICONTROL 连接] 字段。
1. 输入以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL连接名称]</p> </td> 
      <td> <p>输入新连接的名称。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL数据中心ID] </td> 
      <td>使用格式 <code>&lt;Data Center ID>.qualtrics.com</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API密钥]</td> 
      <td>要查找API密钥，请参阅 <a href="https://api.qualtrics.com/instructions/docs/Instructions/api-key-authentication.md">API令牌身份验证</a> 在 [!DNL Qualtrics] 文档。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 继续]** 创建连接，然后返回到模块。

## [!DNL Qualtrics] 模块及其字段

以下模块适用于 [!DNL Qualtrics] 连接器：

* [!UICONTROL 观看新的调查响应]
* [!UICONTROL 创建目录联系人]
* [!UICONTROL 删除目录联系人]
* [!UICONTROL 获取目录联系人]
* [!UICONTROL 更新目录联系人]
* [!UICONTROL 通过短信创建新的调查分发。]
* [!UICONTROL 通过电子邮件分发调查]
* [!UICONTROL 进行API调用]
* [!UICONTROL 列表目录联系人]
