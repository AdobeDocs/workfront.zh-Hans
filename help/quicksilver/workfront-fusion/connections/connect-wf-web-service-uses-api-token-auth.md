---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 将 [!DNL Adobe Workfront Fusion] 连接到使用API令牌授权的Web服务
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 0%

---

# 将[!DNL Adobe Workfront Fusion]连接到使用API令牌授权的Web服务

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [将Adobe Workfront Fusion连接到使用API令牌授权的Web服务](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-wf-web-service-uses-api-token-auth.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

某些服务不允许集成解决方案（如[!DNL Adobe Workfront Fusion]）创建可在场景中轻松使用的应用程序。

对于这种情况，有一个解决方法。 您可以使用[!DNL Workfront Fusion]的[!UICONTROL HTTP]模块将所需的服务（应用程序）连接到[!DNL Workfront Fusion]。

本文介绍如何使用API密钥/API令牌将几乎任何Web服务连接到[!DNL Workfront Fusion]。

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

## 连接到使用API令牌的Web服务

对于大多数Web服务，通过API令牌连接服务的过程都相似。

1. 在Web服务的网站上创建一个应用程序，如本文中的[创建新应用程序并获取API令牌](#create-a-new-application-and-obtain-the-api-token)部分所述。
1. 获取API密钥或API令牌。
1. 添加[!DNL Workfront Fusion]的[!UICONTROL HTTP] > [!UICONTROL 向方案发出请求]模块。
1. 根据Web服务的API文档设置模块并运行方案，如本文中的[设置[!UICONTROL HTTP]模块](#set-up-the-http-module)部分中所述。

>[!NOTE]
>
>本文中将使用[!DNL Pushover]通知服务作为示例。

## 创建新应用程序并获取API令牌

>[!NOTE]
>
>Web服务可通过多种不同的方式创建和分发API密钥或API令牌。 有关获取所需Web服务的API密钥和令牌的说明，请转至该服务的网站并搜索“API密钥”或“API令牌”。
>
>我们仅包括有关获取Pushover API密钥的说明，以作为您可能找到的内容的示例。

1. 登录到您的[!DNL Pushover]帐户。
1. 单击页面底部的&#x200B;**[!UICONTROL 创建应用程序/API令牌]**。
1. 填写应用程序信息，然后单击&#x200B;**[!UICONTROL 创建应用程序]**。
1. 将提供的API令牌存储在安全位置。 [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL 发出请求]模块需要它以连接到所需的Web服务（在本例中为[!DNL Pushover]）。

## 设置[!UICONTROL HTTP]模块

要将Web服务连接到[!DNL Workfront Fusion]方案，您需要使用[!UICONTROL HTTP] >[!UICONTROL 在方案中发出请求]模块，并根据Web服务的API文档设置该模块。

1. 添加[!UICONTROL HTTP] >[!UICONTROL 向方案发出请求]模块。
1. 要使用[!DNL Workfront Fusion]推送消息，请按如下方式设置HTTP模块。

   >[!NOTE]
   >
   >这些模块设置对应于[!DNL Pushover] Web服务API文档。 其他Web服务的设置可能不同。 例如，API令牌可以插入到[!UICONTROL 标头]，而不是[!UICONTROL 正文]字段。

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
      <td role="rowheader"> <p>[！UICONTROL Headers]</p> </td> 
      <td> <p>某些Web服务可能使用标头来指定API令牌身份验证或其他参数。 在我们的示例中并非如此，因为推送消息的Pushover端点对所有请求类型都使用Body（见下文）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL查询字符串]</p> </td> 
      <td> <p>某些Web服务可以使用查询字符串指定其他参数。 在我们的示例中并非如此，因为[!DNL Pushover] Web服务对所有请求类型使用[！UICONTROL Body]（见下文）。</p> </td> 
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
      <td> <p>以JSON格式输入[！UICONTROL Body]请求内容。 您可以使用[！UICONTROL JSON] &gt; [！UICONTROL创建JSON]模块，如本文中的<a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">使用[！UICONTROL JSON] &gt; [！UICONTROL创建JSON]模块映射的JSON主体</a>中所述。 或者，也可以手动输入JSON内容，如本文中<a href="#json-body-entered-manually" class="MCXref xref">手动输入的JSON正文</a>中所述。</p> <p>有关该Web服务所需的参数，请参阅Web服务的API文档。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 手动输入的JSON正文

以JSON格式指定参数和值。

>[!INFO]
>
>**示例：**
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
   <td> <p>您的用户密钥。 这可以在您的[!DNL Pushover]仪表板中找到。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL令牌] </td> 
   <td> <p>您生成的API令牌/API密钥创建了[!DNL Pushover]应用程序。</p> </td> 
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

## 使用[!UICONTROL JSON] >[!UICONTROL 创建JSON]模块映射的JSON主体

通过[!UICONTROL 创建JSON]模块，可以更轻松地指定JSON。 它还允许您动态定义值。

有关JSON模块的详细信息，请参阅[JSON模块](../../workfront-fusion/apps-and-their-modules/json-modules.md)。

1. 输入或映射要从中创建JSON的值。

   ![](assets/json-values-350x288.png)

1. 将[!UICONTROL JSON] > [!UICONTROL 创建JSON]模块连接到HTTP >发出请求模块。
1. 将[!UICONTROL 创建JSON]模块中的JSON字符串映射到[!UICONTROL HTTP] >[!UICONTROL 发出请求]模块中的[!UICONTROL 请求内容]字段。

   现在，当您运行场景时，推送通知将发送到已在您的[!DNL Pushover]帐户中注册的设备。
