---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: connections-annd-webhooks
title: 连接 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 更新了安全措施
description: Google最近对用户如何使用其API进行了限制。 本文介绍了如何连接 [!DNL Adobe Workfront Fusion] 到Google，考虑这些更新的安全措施。
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# 连接 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 更新了安全措施

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

## [!DNL Google Services] 限制

[!DNL Google] 自2020年6月1日起，对用户如何使用其API引入了限制。 这些安全措施保护 [!DNL Google] 用户在 [!DNL Google]. 这些限制与 [!DNL Gmail] 和 [!DNL Google Drive] 应用程序。 有关这些限制的更多信息，请参阅 [[!DNL Google] API服务用户数据策略](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

要访问受限制的作用域，请连接的服务([!DNL Adobe Workfront Fusion] 或任何其他想要通过API访问用户数据的服务)必须进行验证，并且必须具有评估函以证明该服务对于用户如何使用数据是安全和透明的。 [!DNL Workfront Fusion] 遵守所有 [!DNL Google]访问受限范围的要求。 但是，大部分第三方关联服务 [!DNL Workfront Fusion] 没有评估函，因此不遵守 [!DNL Google] 术语。 因此， [!DNL Workfront Fusion] 不允许向这些服务发送数据。

## 例外 [!DNL Google Services] 限制

有少数例外情况允许在不违反任何新限制的情况下，将数据发送到未获得批准的第三方服务，该服务没有评估函。 不同之处在于 [!DNL G Suite] 和 [!DNL Workfront Fusion] OAuth客户端、 [!DNL G Suite] 使用其他OAuth客户端，或 [!DNL @gmail.com] 和 [!DNL @google.mail.com].

* [[!DNL G suite]，带有 [!DNL Workfront Fusion] OAuth客户端](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G Suite]（包含另一个OAuth客户端）](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] 和 [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] with [!DNL Workfront Fusion] OAuth客户端

[!DNL Workfront Fusion] 使用 [!UICONTROL 全域安装] 例外。 全域安装适合 [!DNL G Suite] 用户，并允许用户集成未经批准的服务，且不受任何限制。 如果您是G Suite用户，则无需执行任何其他步骤，而可以直接连接到未批准的服务。

### [!DNL G suite] 与另一个OAuth客户端

[!DNL G Suite] 偏好使用自己的OAuth客户端而不是使用 [!DNL Workfront Fusion] OAuth客户端可以连接到 [!DNL Google Services] 到 [!UICONTROL 内部] 使用方法。 此选项面向高级用户。 有关说明，请参阅 [连接 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自定义OAuth客户端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] 和 [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

访问 [!DNL Google Services] 至 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 可以连接到 [!DNL Google Services] 通过个人使用方法。 此选项面向高级用户。 有关说明，请参阅 [连接 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自定义OAuth客户端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## 常见问题解答

* [中的应用程序 [!DNL Adobe Workfront Fusion] 是否受到影响？](#what-apps-in-adobe-workfront-fusion-are-affected)
* [我是否拥有[!DNL G Suite]帐户？](#do-i-have-a-g-suite-account)
* [如果我 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 用户？](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [如果我是[!DNL G Suite]用户，该怎么办？](#what-should-i-do-if-im-a-g-suite-user)

### 中的应用程序 [!DNL Adobe Workfront Fusion] 是否受到影响？ {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail]、和电子邮件(已连接到 [!DNL Gmail] 帐户)。

### 我有 [!DNL G Suite] 帐户？ {#do-i-have-a-g-suite-account}

如果您的电子邮件地址以 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 您的帐户不是 [!DNL G Suite] 帐户。 如果 [!DNL Google] 帐户以自定义域(如@my-company.com)结尾，则它是 [!DNL G Suite] 帐户。

### 如果我 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 用户？ {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

这些新限制仅在您集成时才适用 [!DNL Google Drive] 或 [!DNL Gmail]. 如果要连接到 [!DNL Google Drive] 或 [!DNL Gmail]，您可以

* 切换到 [!DNL G Suite]

   或

* 创建自定义OAuth客户端。 此选项面向高级用户。

   有关说明，请参阅 [连接 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自定义OAuth客户端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

如果要集成 [!DNL Google Drive] 或 [!DNL Gmail]，则这些限制不适用。

有关连接其他 [!DNL Google Services] to [!DNL Workfront Fusion]，请参阅 [将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) 在文章中 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### 如果我是 [!DNL G Suite] 用户？ {#what-should-i-do-if-im-a-g-suite-user}

无需执行任何操作。
