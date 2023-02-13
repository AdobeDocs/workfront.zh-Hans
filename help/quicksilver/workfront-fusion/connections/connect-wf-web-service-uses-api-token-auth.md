---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 连接 [!DNL Adobe Workfront Fusion] 到使用API令牌授权的Web服务
description: 某些服务不允许集成解决方案，例如 [!DNL Adobe Workfront Fusion] 创建可在您的场景中轻松使用的应用程序。
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# 连接 [!DNL Adobe Workfront Fusion] 到使用API令牌授权的Web服务

某些服务不允许集成解决方案，例如 [!DNL Adobe Workfront Fusion] 创建可在您的场景中轻松使用的应用程序。

此情况有一种解决方法。 您可以将所需的服务（应用程序）连接到 [!DNL Workfront Fusion] 使用 [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] 模块。

本文介绍如何将几乎任何Web服务连接到 [!DNL Workfront Fusion] 使用API密钥/API令牌。

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

## 连接到使用API令牌的Web服务

对于大多数Web服务，通过API令牌连接服务的过程与此类似。

1. 按照 [创建新应用程序并获取API令牌](#create-a-new-application-and-obtain-the-api-token) 在本文中。
1. 获取API密钥或API令牌。
1. 添加 [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] > [!UICONTROL 请求] 模块。
1. 根据Web服务的API文档设置模块并运行方案，如部分中所述 [设置 [!UICONTROL HTTP] 模块](#set-up-the-http-module) 在本文中。

>[!NOTE]
>
>我们将使用 [!DNL Pushover] 通知服务（例如，本文中的示例）。

## 创建新应用程序并获取API令牌

>[!NOTE]
>
>Web服务可通过多种不同的方式创建和分发API密钥或API令牌。 有关为所需的Web服务获取API密钥和令牌的说明，请转到该服务的网站并搜索“API密钥”或“API令牌”。
>
>我们提供了仅作为您可能找到的内容示例，获取Pushover API密钥的说明。

1. 登录到 [!DNL Pushover] 帐户。
1. 单击 **[!UICONTROL 创建应用程序/API令牌]** 页面底部。
1. 填写应用程序信息并单击 **[!UICONTROL 创建应用程序]**.
1. 将提供的API令牌存储在安全位置。 您需要它 [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL 请求] 连接到所需web服务的模块([!DNL Pushover]，在本例中为)。

## 设置 [!UICONTROL HTTP] 模块

将Web服务连接到 [!DNL Workfront Fusion] 方案中，您需要使用 [!UICONTROL HTTP] >[!UICONTROL 请求] 模块，并根据web服务的API文档设置模块。

1. 添加 [!UICONTROL HTTP] >[!UICONTROL 请求] 模块。
1. 使用 [!DNL Workfront Fusion]，请按如下方式设置HTTP模块。

   >[!NOTE]
   >
   >这些模块设置与 [!DNL Pushover] web服务API文档。 其他Web服务的设置可能不同。 例如，可以将API令牌插入到 [!UICONTROL 标题] 而不是 [!UICONTROL 正文] 字段。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>URL字段包含可在Web服务API文档中找到的端点。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL方法]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>使用的方法取决于相应的端点。 用于推送消息的Pushover端点使用POST方法。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL标头]</p> </td> 
      <td> <p>某些Web服务可能使用标头来指定API令牌身份验证或其他参数。 在我们的示例中并非如此，因为Pushover推送消息的端点在所有请求类型中都使用Body（请参阅下文）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL查询字符串]</p> </td> 
      <td> <p>某些Web服务可能使用查询字符串来指定其他参数。 在我们的示例中并非如此，例如 [!DNL Pushover] Web服务对所有请求类型都使用[!UICONTROL主体]（请参阅下文）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Body Type]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>此设置允许您在下面的[!UICONTROL内容类型]字段中选择JSON内容类型。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL内容类型]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>[!UICONTROL Pushover]应用程序需要使用JSON作为内容类型。 这可能与其他Web服务不同。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL请求内容]</p> </td> 
      <td> <p>以JSON格式输入[!UICONTROL Body]请求内容。 您可以使用[!UICONTROL JSON] &gt; [!UICONTROL创建JSON]模块，如 <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">使用[!UICONTROL JSON] &gt; [!UICONTROL创建JSON]模块映射的JSON正文</a> 在本文中。 或者，您也可以手动输入JSON内容，如 <a href="#json-body-entered-manually" class="MCXref xref">手动输入的JSON正文</a> 在本文中。</p> <p>有关该Web服务所需的参数，请参阅Web服务的API文档。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 手动输入的JSON正文

以JSON格式指定参数和值。

>[!INFO]
>
>**示例:**
>
>
```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>
>
"token":"123459evz8aepwtxydndydgyumbfx",
>
>
"message":"Hello World!",
>
>
"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL用户]</p> </td> 
   <td> <p>您的USER_KEY。 这可在 [!DNL Pushover] 功能板。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL令牌] </td> 
   <td> <p>您创建的API令牌/API密钥 [!DNL Pushover] 应用程序。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息] </td> 
   <td> <p>发送到设备的推送通知的文本内容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>（可选）消息的标题。 如果未输入任何值，则会使用您的应用程序名称。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用映射的JSON正文 [!UICONTROL JSON] >[!UICONTROL 创建JSON] 模块

的 [!UICONTROL 创建JSON] 模块可简化指定JSON的过程。 它还允许您动态定义值。

有关JSON模块的更多信息，请参阅 [JSON模块](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. 输入或映射要从中创建JSON的值。

   ![](assets/json-values-350x288.png)

1. 连接 [!UICONTROL JSON] > [!UICONTROL 创建JSON] 模块添加到HTTP >发出请求模块。
1. 映射 [!UICONTROL 创建JSON] 模块 [!UICONTROL 请求内容] 字段 [!UICONTROL HTTP] >[!UICONTROL 请求] 模块。

   现在，当您运行该方案时，会将推送通知发送到在中注册的设备 [!DNL Pushover] 帐户。
