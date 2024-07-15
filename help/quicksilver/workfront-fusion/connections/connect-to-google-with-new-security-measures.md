---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: connections-annd-webhooks
title: 使用更新的安全措施连接 [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services]
description: Google最近对用户使用其API的方式引入了限制。 本文介绍了如何将 [!DNL Adobe Workfront Fusion] 连接到Google，并说明了这些更新安全措施。
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# 使用更新的安全措施将[!DNL Adobe Workfront Fusion]连接到[!DNL Google Services]

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

## [!DNL Google Services]限制

[!DNL Google]自2020年6月1日起对用户使用其API的方式进行了限制。 这些安全措施可保护[!DNL Google]用户不会在[!DNL Google]上泄漏或滥用其个人数据。 这些限制与[!DNL Gmail]和[!DNL Google Drive]应用相关。 有关这些限制的详细信息，请参阅[[!DNL Google] API服务用户数据策略](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)中的“特定API范围的其他要求”

要访问受限范围，必须验证连接的服务（[!DNL Adobe Workfront Fusion]或要通过API访问用户数据的任何其他服务），并且必须拥有评估书以证明该服务在使用数据方面是安全和透明的。 [!DNL Workfront Fusion]符合[!DNL Google]访问受限范围的所有要求。 但是，[!DNL Workfront Fusion]中的大多数第三方连接服务没有评估书，因此不符合[!DNL Google]条款。 因此，不允许[!DNL Workfront Fusion]将数据发送到这些服务。

## [!DNL Google Services]限制的异常

有一些例外情况可能会将数据发送到没有评估书的未经批准的第三方服务，而不违反任何新限制。 它们因具有[!DNL Workfront Fusion] OAuth客户端的[!DNL Google Workspace]、具有其他OAuth客户端的[!DNL Google Workspace]或[!DNL @gmail.com]和[!DNL @google.mail.com]而异。

* [具有 [!DNL Workfront Fusion] OAuth客户端的[!DNL Google Workspace]](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL Google Workspace]与其他OAuth客户端](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com]和 [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### 具有[!DNL Workfront Fusion] OAuth客户端的[!DNL Google Workspace]

[!DNL Workfront Fusion]使用[!UICONTROL 全域安装]异常。 全域安装适用于[!DNL Google Workspace]用户，允许用户不受任何限制地集成未批准的服务。 如果您是Google Workspace用户，则无需执行任何其他步骤，可以直接连接到未批准的服务。

### [!DNL Google Workspace]与其他OAuth客户端

希望使用自己的OAuth客户端而不使用[!DNL Workfront Fusion] OAuth客户端的[!DNL Google Workspace]用户可以通过[!UICONTROL 内部]使用方法连接到[!DNL Google Services]。 此选项适用于高级用户。 有关说明，请参阅[使用自定义OAuth客户端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)连接 [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] 。

### [!DNL @gmail.com]和[!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

通过[!DNL @gmail.com]或[!DNL @googlemail.com]访问[!DNL Google Services]的用户可以通过“个人使用”方法连接到[!DNL Google Services]。 此选项适用于高级用户。 有关说明，请参阅[使用自定义OAuth客户端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)连接 [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] 。

## 常见问题解答

* [ [!DNL Adobe Workfront Fusion] 中的哪些应用受到影响？](#what-apps-in-adobe-workfront-fusion-are-affected)
* [我是否有 [!DNL Google Workspace] 帐户？](#do-i-have-a-g-suite-account)
* [如果我是 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 用户，我应该怎么做？](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [如果我是 [!DNL Google Workspace] 用户，我应该怎么做？](#what-should-i-do-if-im-a-g-suite-user)

### [!DNL Adobe Workfront Fusion]中的哪些应用受到影响？ {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive]、[!DNL Gmail]和电子邮件（已连接到[!DNL Gmail]帐户）。

### 我是否有[!DNL Google Workspace]帐户？ {#do-i-have-a-g-suite-account}

如果您的电子邮件地址以[!DNL @gmail.com]或[!DNL @googlemail.com]结尾，则您的帐户不是[!DNL Google Workspace]帐户。 如果您的[!DNL Google]帐户以自定义域(如@my-company.com)结尾，则它是[!DNL Google Workspace]帐户。

### 如果我是[!DNL @gmail.com]或[!DNL @googlemail.com]用户，我应该怎么做？ {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

这些新限制仅适用于集成[!DNL Google Drive]或[!DNL Gmail]的情况。 如果要连接到[!DNL Google Drive]或[!DNL Gmail]，您可以

* 切换到[!DNL Google Workspace]

  或

* 创建自定义OAuth客户端。 此选项适用于高级用户。

  有关说明，请参阅[使用自定义OAuth客户端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)连接 [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] 。

如果要集成[!DNL Google Drive]或[!DNL Gmail]以外的任何其他服务，则这些限制不适用。

有关将其他[!DNL Google Services]连接到[!DNL Workfront Fusion]的说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案一文中的[将模块的应用或Web服务连接到 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect)。

### 如果我是[!DNL Google Workspace]用户，我应该怎么做？ {#what-should-i-do-if-im-a-g-suite-user}

无需执行任何操作。
