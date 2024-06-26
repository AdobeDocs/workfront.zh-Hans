---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: connections-annd-webhooks
title: 在中创建连接 [!DNL Adobe Workfront Fusion]
description: 连接必须遵循它所连接的应用程序或Web服务的API所设置的要求。 因此，设置连接的说明因应用程序或Web服务而异。 本文可帮助您识别和查找有关连接的说明 [!DNL Adobe Workfront Fusion] 到您选择的应用程序或Web服务。
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 1%

---

# 在中创建连接 [!DNL Adobe Workfront Fusion]

<!-- Audited: 3/2024-->

连接必须遵循它所连接的应用程序或Web服务的API所设置的要求。 因此，设置连接的说明因应用程序或Web服务而异。 本文可帮助您识别和查找有关连接的说明 [!DNL Adobe Workfront Fusion] 到您选择的应用程序或Web服务。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td>  
   <td> <p>任何</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td>  
   <td> <p>新文档： [！UICONTROL Standard]</p><p>或</p><p>当前： [！UICONTROL Work]或更高版本</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td>  
   <td> 
   <p>当前：否 [!DNL Workfront Fusion] 许可证要求。</p> 
   <p>或</p> 
   <p>旧版：任意 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">产品</td>  
   <td> 
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront] 计划：您的组织必须购买 [!DNL Adobe Workfront Fusion].</li><li>[！UICONTROL Ultimate] [!DNL Workfront] 计划： [!DNL Workfront Fusion] 中包含。</li></ul> 
   <p>或</p> 
   <p>当前：您的组织必须购买 [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 连接到不需要配置的应用程序或Web服务

在大多数情况下，您可以使用模块创建几乎没有或没有额外信息的连接。 [!DNL Workfront Fusion] 自动处理身份验证。

有关创建无特殊注意事项的连接的说明，请参见 [创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md).

## 连接到 [!DNL Microsoft] 应用程序或Web服务

大部分 [!DNL Microsoft] 中的应用程序 [!DNL Workfront Fusion] 允许您创建无额外信息的连接。

以下情况在创建连接时确实需要额外的步骤：

* 使用 [!DNL Microsoft Dynamics 365] 模块。

  有关说明，请参阅 [[!DNL Microsoft Dynamics 365] 模块](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* 连接到 [!DNL Microsoft Graph API] 使用 [!UICONTROL HTTP] 模块

  有关说明，请参阅 [调用 [!DNL MS Graph REST API] 通过 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 发出OAuth 2.0请求] 模块](../../workfront-fusion/connections/call-the-ms-graph-rest-api.md).

## 连接到 [!DNL Google] 应用程序或Web服务

连接到的过程 [!DNL Google] 应用程序可能因类别而异 [!DNL Google] 您正在使用的帐户。 另外， [!DNL Google] 当您连接到时，安全措施可能需要额外的配置 [!DNL Workfront Fusion].

有关更多信息，请参阅：

* [连接 [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] 使用自定义OAuth客户端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [连接 [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] 更新了安全措施](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## 需要其他配置的其他应用程序

以下应用程序不遵循的基本配置 [!DNL Workfront Fusion] 连接。 您可以在文章中找到有关连接这些应用程序的说明。

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>应用程序/Web服务</th> 
   <th>有关连接的其他信息</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">连接 [!DNL Adobe Workfront] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">连接 [!DNL Allocadia] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">连接 [!DNL Anaplan] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] 模块</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">连接 [!DNL AWS] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">连接 [!DNL Azure DevOps] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">连接 [!DNL Bynder] 到 [!DNL Workfront Fusion] </a> 在 <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">连接 [!DNL CloudConvert] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] 模块</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">连接 [!DNL Cvent] 到 [!DNL Adobe Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">连接 [!DNL Datadog] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">连接 [!DNL DocuSign] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>电子邮件</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">将您的电子邮件连接到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">[！UICONTROL Email]模块</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">连接 [!DNL Gmail] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">连接 [!DNL Jira Cloud] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">连接 [!DNL Jira Server] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">连接 [!DNL MariaDB] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">连接 [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">连接 [!DNL Microsoft Dynamics 365] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">正在连接 [!DNL Qualtrics] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">连接 [!DNL ServiceNow] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">[！UICONTROL SFTP]模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">连接 [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 在 <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">连接 [!DNL Split.io] 到 [!DNL Workfront Fusion] </a> 在 <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] 模块</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>加宽</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">连接 [!DNL Widen] 到 [!DNL Workfront Fusion] </a> 在 <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] 模块</a></td> 
  </tr> 
 </tbody> 
</table>
