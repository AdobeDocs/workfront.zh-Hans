---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] 更新了安全措施
description: Google最近对用户使用其API的方式引入了限制。 本文介绍了如何连接 [!DNL Adobe Workfront Fusion] Google，请注意这些更新安全措施。
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] 更新了安全措施

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

## [!DNL Google Services] 限制

[!DNL Google] 自2020年6月1日起，对用户使用其API的方式引入了限制。 这些安全措施保护 [!DNL Google] 用户个人数据被泄露或滥用 [!DNL Google]. 这些限制与 [!DNL Gmail] 和 [!DNL Google Drive] 应用程序。 有关这些限制的更多信息，请参阅 [[!DNL Google] API服务用户数据策略](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

要访问受限作用域，连接的服务([!DNL Adobe Workfront Fusion] 或任何希望通过API访问用户数据的其他服务)必须经过验证，并且必须拥有一份评估函，以证明该服务对于用户如何使用数据是安全和透明的。 [!DNL Workfront Fusion] 符合所有 [!DNL Google]的限制范围访问要求。 但是，大多数第三方连接服务在 [!DNL Workfront Fusion] 没有评估函，因此不符合 [!DNL Google] 条款。 正因如此， [!DNL Workfront Fusion] 不允许将数据发送到这些服务。

## 例外情况 [!DNL Google Services] 限制

有一些例外情况允许将数据发送到没有评估书的未经批准的第三方服务，而不违反任何新限制。 它们之所以不同，是因为 [!DNL G Suite] 使用 [!DNL Workfront Fusion] OAuth客户端， [!DNL G Suite] 与其他OAuth客户端，或者 [!DNL @gmail.com] 和 [!DNL @google.mail.com].

* [[！DNL G suite]，带 [!DNL Workfront Fusion] OAuth客户端](#g-suite-with-workfront-fusion-oauth-client)
* [使用另一个OAuth客户端的[！DNL G suite]](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] 和 [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] 替换为 [!DNL Workfront Fusion] OAuth客户端

[!DNL Workfront Fusion] 使用 [!UICONTROL 全域安装] 例外。 全域安装适用于 [!DNL G Suite] ，允许用户集成未批准的服务，没有任何限制。 如果您是G Suite用户，则无需执行任何其他步骤，可以直接连接到未批准的服务。

### [!DNL G suite] 与其他OAuth客户端

[!DNL G Suite] 更喜欢使用自己的OAuth客户端而不是使用 [!DNL Workfront Fusion] OAuth客户端可以连接到 [!DNL Google Services] 通过 [!UICONTROL 内部] 使用方法。 此选项适用于高级用户。 有关说明，请参阅 [Connect [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] 使用自定义OAuth客户端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] 和 [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

具有访问权限的用户 [!DNL Google Services] 到 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 可以连接到 [!DNL Google Services] 通过“个人使用”方法。 此选项适用于高级用户。 有关说明，请参阅 [Connect [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] 使用自定义OAuth客户端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## 常见问题解答

* [中的应用程序 [!DNL Adobe Workfront Fusion] 是否受到影响？](#what-apps-in-adobe-workfront-fusion-are-affected)
* [我是否拥有[！DNL G Suite]帐户？](#do-i-have-a-g-suite-account)
* [如果我是，怎么办 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 用户？](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [如果我是[！DNL G Suite]用户，我应该怎么做？](#what-should-i-do-if-im-a-g-suite-user)

### 中的应用程序 [!DNL Adobe Workfront Fusion] 是否受到影响？ {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive]， [!DNL Gmail]和电子邮件(已连接到 [!DNL Gmail] 帐户)。

### 我是否有 [!DNL G Suite] 帐户？ {#do-i-have-a-g-suite-account}

如果您的电子邮件地址结尾为 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 您的帐户不是 [!DNL G Suite] 帐户。 如果您的 [!DNL Google] 帐户以自定义域结尾，例如@my-company.com ，然后它是 [!DNL G Suite] 帐户。

### 如果我是，怎么办 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 用户？ {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

这些新限制仅适用于集成 [!DNL Google Drive] 或 [!DNL Gmail]. 如果要连接到 [!DNL Google Drive] 或 [!DNL Gmail]，您可以

* 切换到 [!DNL G Suite]

  或

* 创建自定义OAuth客户端。 此选项适用于高级用户。

  有关说明，请参阅 [Connect [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] 使用自定义OAuth客户端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

如果您要集成 [!DNL Google Drive] 或 [!DNL Gmail]，这些限制不适用。

有关连接其他设备的说明 [!DNL Google Services] 到 [!DNL Workfront Fusion]，请参见 [将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) 在文章中 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### 如果我是 [!DNL G Suite] 用户？ {#what-should-i-do-if-im-a-g-suite-user}

无需执行任何操作。
