---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: connections-annd-webhooks
title: 在中创建连接 [!DNL Adobe Workfront Fusion]
description: 连接必须符合由它所连接的应用程序或Web服务的API设置的要求。 因此，设置连接的说明因应用程序或Web服务而异。 本文可帮助您识别并找到连接说明 [!DNL Adobe Workfront Fusion] 到您选择的应用程序或web服务。
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# 在中创建连接 [!DNL Adobe Workfront Fusion]

连接必须符合由它所连接的应用程序或Web服务的API设置的要求。 因此，设置连接的说明因应用程序或Web服务而异。 本文可帮助您识别并找到连接说明 [!DNL Adobe Workfront Fusion] 到您选择的应用程序或web服务。

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

</tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 连接 [!DNL Adobe Workfront] to [!DNL Workfront Fusion]

Workfront和 [!DNL Workfront Fusion] 设计为能够协同工作。 您创建的连接决定了 [!DNL Workfront Fusion] 用于在Workfront中执行操作。

有关说明，请参阅 [连接 [!DNL Workfront] to [!DNL Workfront Fusion]](../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect) in [[!DNL Adobe Workfront] 模块](../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

## 连接到不需要配置的应用程序或Web服务

在大多数情况下，您可以使用模块创建包含少量或无额外信息的连接。 [!DNL Workfront Fusion] 自动处理身份验证。

有关创建无特殊注意事项的连接的说明，请参阅 [创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md).

## 连接到 [!DNL Microsoft] 应用程序或web服务

大多数 [!DNL Microsoft] 应用程序 [!DNL Workfront Fusion] 允许您创建无额外信息的连接。

在以下情况下，创建连接时确实需要额外的步骤：

* 使用 [!DNL Microsoft Dynamics 365] 模块。

   有关说明，请参阅 [[!DNL Microsoft Dynamics 365] 模块](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* 连接到 [!DNL Microsoft Graph API] 使用 [!UICONTROL HTTP] 模块

   有关说明，请参阅 [调用 [!DNL MS Graph REST API] 通过 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 发出OAuth 2.0请求] 模块](../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## 连接到 [!DNL Google] 应用程序或web服务

连接到的过程 [!DNL Google] 应用程序可能会因应用程序类型而异 [!DNL Google] 帐户。 此外， [!DNL Google] 连接时，安全措施可能需要额外配置 [!DNL Workfront Fusion].

有关更多信息，请参阅：

* [连接 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自定义OAuth客户端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [连接 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 更新了安全措施](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## 需要其他配置的其他应用程序

以下应用程序不遵循 [!DNL Workfront Fusion] 连接。 您可以在该应用程序的文章中找到有关连接这些应用程序的说明。

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>应用程序/ Web服务</th> 
   <th>有关连接的其他信息</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">连接 [!DNL Adobe Workfront] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">连接 [!DNL Allocadia] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">连接 [!DNL Anaplan] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] 模块</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">连接 [!DNL AWS] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">连接 [!DNL Azure DevOps] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">连接 [!DNL Bynder] to [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] 模块</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">连接 [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">连接 [!DNL Datadog] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">连接 [!DNL DocuSign] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>电子邮件</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">将您的电子邮件连接到 [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">[!UICONTROL Email]模块</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">连接 [!DNL Gmail] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Intacct]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/intacct-modules.md#connecti" class="MCXref xref">连接 [!DNL Intacct] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/intacct-modules.md" class="MCXref xref">[!DNL Intacct] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">连接 [!DNL Jira Cloud] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">连接 [!DNL Jira Server] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">连接 [!DNL MariaDB] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">连接 [!DNL Marketo] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">连接 [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">连接 [!DNL Qualtrics] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">连接 [!DNL ServiceNow] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">[!UICONTROL SFTP]模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">连接 [!DNL Split.io] to [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>加宽</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">连接 [!DNL Widen] to [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] 模块</a></td> 
  </tr> 
 </tbody> 
</table>
