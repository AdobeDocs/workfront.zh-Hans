---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] 到使用API令牌授权的Web服务
description: 某些服务不允许集成解决方案，例如 [!DNL Adobe Workfront Fusion] 创建可在场景中轻松使用的应用程序。
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: e61dc6646e221cffb30aad055663dcf8fd3299e2
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] 到使用API令牌授权的Web服务

某些服务不允许集成解决方案，例如 [!DNL Adobe Workfront Fusion] 创建可在场景中轻松使用的应用程序。

对于这种情况，有一个解决方法。 您可以将所需的服务（应用程序）连接到 [!DNL Workfront Fusion] 使用 [!DNL Workfront Fusion]的 [!UICONTROL HTTP] 模块。

本文介绍了如何将几乎任何Web服务连接到 [!DNL Workfront Fusion] API密钥/API令牌。

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

## 连接到使用API令牌的Web服务

对于大多数Web服务，通过API令牌连接服务的过程都类似。

1. 在Web服务的网站上创建一个应用程序，如一节中所述 [创建新应用程序并获取API令牌](#create-a-new-application-and-obtain-the-api-token) 本文章中。
1. 获取API密钥或API令牌。
1. 添加 [!DNL Workfront Fusion]的 [!UICONTROL HTTP] > [!UICONTROL 提出请求] 模块到您的场景。
1. 根据Web服务的API文档设置模块并运行场景，如部分中所述 [设置 [!UICONTROL HTTP] 模块](#set-up-the-http-module) 本文章中。

>[!NOTE]
>
>我们将使用 [!DNL Pushover] 通知服务。

## 创建新应用程序并获取API令牌

>[!NOTE]
>
>Web服务可通过多种不同的方式创建和分发API密钥或API令牌。 有关获取所需Web服务的API密钥和令牌的说明，请转到该服务的网站并搜索“API密钥”或“API令牌”。
>
>我们提供的有关获取Pushover API密钥的说明仅作为您可能找到的内容的示例。

1. 登录 [!DNL Pushover] 帐户。
1. 单击 **[!UICONTROL 创建应用程序/API令牌]** 页面底部的。
1. 填写应用程序信息并单击 **[!UICONTROL 创建应用程序]**.
1. 将提供的API令牌存储在安全位置。 您需要它用于 [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL 提出请求] 连接到所需Web服务的模块([!DNL Pushover]，在本例中)。

## 设置 [!UICONTROL HTTP] 模块

要将Web服务连接到 [!DNL Workfront Fusion] 方案，您需要使用 [!UICONTROL HTTP] >[!UICONTROL 提出请求] 模块在场景中根据Web服务的API文档设置模块。

1. 添加 [!UICONTROL HTTP] >[!UICONTROL 提出请求] 模块到您的场景。
1. 要推送消息，请使用 [!DNL Workfront Fusion]，请按如下方式设置HTTP模块。

   >[!NOTE]
   >
   >这些模块设置对应于 [!DNL Pushover] Web服务API文档。 其他Web服务的设置可能不同。 例如，可以将API令牌插入 [!UICONTROL 页眉] 而不是到 [!UICONTROL 正文] 字段。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>URL字段包含您可以在Web服务的API文档中找到的端点。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL方法]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>使用的方法取决于对应的端点。 推送消息的Pushover端点使用POST方法。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL标头]</p> </td> 
      <td> <p>某些Web服务可能使用标头来指定API令牌身份验证或其他参数。 在我们的示例中并非如此，因为推送消息的Pushover端点会对所有请求类型使用Body（见下文）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL查询字符串]</p> </td> 
      <td> <p>某些Web服务可以使用查询字符串指定其他参数。 在我们的示例中并非如此，因为 [!DNL Pushover] Web服务对所有请求类型使用[！UICONTROL主体]（见下文）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL主体类型]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>此设置允许您在下面的[！UICONTROL内容类型]字段中选择JSON内容类型。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL内容类型]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON是[！UICONTROL Pushover]应用程序所需的内容类型。 这可能与其他Web服务不同。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL请求内容]</p> </td> 
      <td> <p>以JSON格式输入[！UICONTROL Body]请求内容。 您可以使用[！UICONTROL JSON] &gt; [！UICONTROL创建JSON]模块，如中所述 <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">使用[！UICONTROL JSON] &gt; [！UICONTROL创建JSON]模块映射的JSON主体</a> 本文章中。 或者，您也可以手动输入JSON内容，如中所述 <a href="#json-body-entered-manually" class="MCXref xref">手动输入的JSON正文</a> 本文章中。</p> <p>有关该Web服务所需的参数，请参阅Web服务的API文档。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 手动输入的JSON正文

以JSON格式指定参数和值。

>[!INFO]
>
>**示例:**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>"token":"123459evz8aepwtxydndydgyumbfx",
>"message":"Hello World!",
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL用户]</p> </td> 
   <td> <p>您的USER_KEY。 这可以在您的网站中找到 [!DNL Pushover] 仪表板。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL令牌] </td> 
   <td> <p>您生成的API令牌/API密钥是您创建的 [!DNL Pushover] 应用程序。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL消息] </td> 
   <td> <p>发送到设备的推送通知的文本内容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标题] </td> 
   <td> <p>（可选）消息的标题。 如果未输入值，则使用您应用程序的名称。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用的JSON正文映射 [!UICONTROL JSON] >[!UICONTROL 创建JSON] 模块

此 [!UICONTROL 创建JSON] 模块简化了指定JSON的过程。 它还允许您动态定义值。

有关JSON模块的更多信息，请参见 [JSON模块](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. 输入或映射要从中创建JSON的值。

   ![](assets/json-values-350x288.png)

1. 连接 [!UICONTROL JSON] > [!UICONTROL 创建JSON] HTTP >创建请求模块的模块。
1. 从映射JSON字符串 [!UICONTROL 创建JSON] 模块到 [!UICONTROL 请求内容] 中的字段 [!UICONTROL HTTP] >[!UICONTROL 提出请求] 模块。

   现在，当您运行场景时，推送通知将发送到已在中注册的设备 [!DNL Pushover] 帐户。
