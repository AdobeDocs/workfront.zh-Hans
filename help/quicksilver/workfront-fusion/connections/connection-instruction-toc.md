---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: connections-annd-webhooks
title: 在 [!DNL Adobe Workfront Fusion]中创建连接
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 1%

---

# 在[!DNL Adobe Workfront Fusion]中创建连接

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [连接到应用程序：文章索引](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-to-apps-toc.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

<!-- Audited: 3/2024-->

连接必须遵循它所连接的应用程序或Web服务的API所设置的要求。 因此，设置连接的说明因应用程序或Web服务而异。 本文可帮助您识别并查找有关将[!DNL Adobe Workfront Fusion]连接到您选择的应用程序或Web服务的说明。

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
   <p>当前：无[!DNL Workfront Fusion]许可证要求。</p> 
   <p>或</p> 
   <p>旧版：任意 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">产品</td>  
   <td> 
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront]计划：您的组织必须购买[!DNL Adobe Workfront Fusion]。</li><li>已包括[！UICONTROL Ultimate] [!DNL Workfront]计划： [!DNL Workfront Fusion]。</li></ul> 
   <p>或</p> 
   <p>当前：您的组织必须购买[!DNL Adobe Workfront Fusion]。</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 连接到不需要配置的应用程序或Web服务

在大多数情况下，您可以使用模块创建几乎没有或没有额外信息的连接。 [!DNL Workfront Fusion]自动处理身份验证。

有关创建无特殊注意事项的连接的说明，请参阅[创建与 [!DNL Adobe Workfront Fusion] 的连接 — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)。

## 连接到[!DNL Microsoft]应用或Web服务

[!DNL Workfront Fusion]中的大多数[!DNL Microsoft]应用允许您创建无额外信息的连接。

以下情况在创建连接时确实需要额外的步骤：

* 正在使用[!DNL Microsoft Dynamics 365]模块。

  有关说明，请参阅[[!DNL Microsoft Dynamics 365] 模块](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md)。

* 使用[!UICONTROL HTTP]模块连接到[!DNL Microsoft Graph API]

  有关说明，请参阅[通过 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP]调用 [!DNL MS Graph REST API]  > [!UICONTROL 发出OAuth 2.0请求]模块](../../workfront-fusion/connections/call-the-ms-graph-rest-api.md)。

## 连接到[!DNL Google]应用或Web服务

根据您使用的[!DNL Google]帐户类型，连接到[!DNL Google]应用的进程可能会有所不同。 此外，当您连接到[!DNL Workfront Fusion]时，[!DNL Google]安全措施可能需要额外的配置。

有关更多信息，请参阅：

* [使用自定义OAuth客户端连接 [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] ](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [使用更新的安全措施连接 [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] ](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## 需要其他配置的其他应用程序

以下应用不遵循[!DNL Workfront Fusion]连接的基本配置。 您可以在文章中找到有关连接这些应用程序的说明。

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
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">将[!DNL Adobe Workfront]连接到<a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">将[!DNL Allocadia]连接到<a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">将[!DNL Anaplan]连接到<a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">将[!DNL AWS]连接到<a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">将[!DNL Azure DevOps]连接到<a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">将[!DNL Bynder]连接到<a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder]模块中的[!DNL Workfront Fusion] </a></a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">将[!DNL CloudConvert]连接到<a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">将[!DNL Cvent]连接到<a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent]模块中的</a>[!DNL Adobe Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">将[!DNL Datadog]连接到<a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">将[!DNL DocuSign]连接到<a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>电子邮件</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">将您的电子邮件连接到<a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">[！UICONTROL Email]模块中的</a>[!DNL Workfront Fusion]</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">将[!DNL Gmail]连接到<a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">将[!DNL Jira Cloud]连接到<a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">将[!DNL Jira Server]连接到<a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">将[!DNL MariaDB]连接到<a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">将[!DNL Marketo]连接到<a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">将[!DNL Microsoft Dynamics 365]连接到<a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">正在将[!DNL Qualtrics]连接到<a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">将[!DNL ServiceNow]连接到<a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">将<a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">[！UICONTROL SFTP]模块中的SFTP连接到</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">将[!DNL SharePoint]连接到<a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint]模块中的</a>[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">将[!DNL Split.io]连接到<a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io]模块中的[!DNL Workfront Fusion] </a></a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>加宽</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">将[!DNL Widen]连接到<a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen]模块中的[!DNL Workfront Fusion] </a></a></td> 
  </tr> 
 </tbody> 
</table>
