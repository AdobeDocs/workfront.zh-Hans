---
title: 通过调用MS Graph REST API [!DNL Adobe Workfront Fusion] HTTP &gt；创建OAuth 2.0请求模块
description: 通过调用MS Graph REST API [!DNL Adobe Workfront Fusion] HTTP &gt；创建OAuth 2.0请求模块
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# 调用[!UICONTROL  MS Graph REST API] 通过 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 发出OAuth 2.0请求] 模块

<!-- Audited: 3/2024-->

许多 [!DNL Microsoft] Web服务可通过 [!DNL Microsoft Graph API]. 您可以创建与 [!DNL Microsoft Graph API]，通过使用 [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL 发出OAuth 2.0请求] 模块。

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

## 注册 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]

要创建与 [!DNL Microsoft Graph REST API]，您必须先注册 [!DNL Adobe Workfront Fusion].

1. 开始注册新应用程序，如中所述 [注册您的应用程序](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) 在 [!DNL Microsoft] 文档。

   作为登记的一部分， [!DNL Microsoft] 需要以下信息：

   <table style="table-layout:auto">
      <tr>
        <td>[！UICONTROL应用程序名称]</td>
        <td>输入应用程序的名称，如“My” [!DNL Workfront Fusion] 应用程序。”</td>
      </tr>
      <tr>
        <td>[！UICONTROL重定向URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. 完成应用程序注册后，请注意 [!UICONTROL 应用程序Id].

   >[!IMPORTANT]
   >
   >您需要具有应用程序ID才能在中设置连接 [!DNL Workfront Fusion].

1. 生成 [!UICONTROL 应用程序密码]. 记下这个秘密。

   有关说明，请参阅 [注册您的应用程序](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) 在 [!DNL Microsoft] 文档。

   >[!IMPORTANT]
   >
   >您将需要 [!UICONTROL 应用程序密码] 在中设置连接 [!DNL Workfront Fusion].

1. 配置应用程序的权限。

   有关查找和配置这些字段的详细信息，请参阅中的“配置Microsoft Graph的权限”部分 [无需用户即可获得访问权限](https://docs.microsoft.com/en-us/graph/auth-v2-service) 在 [!UICONTROL Microsoft] 文档。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL您的应用程序需要哪种类型的权限？]</td> 
      <td>选择 <code>[!UICONTROL Delegated permissions]</code>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL Select permissions]</td> 
      <td> <p>选择以下权限：</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>您的集成所需的任何其他权限(例如： <code>User.Read</code>)</p> </li> 
       </ul> <p><b>重要</b>：您需要具有所选权限才能在中设置连接 [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 继续到 [配置您的 [!DNL MS Graph API] 中的连接 [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## 配置您的 [!DNL MS Graph API] 中的连接 [!DNL Workfront Fusion]

注册之后 [!DNL Workfront Fusion] 如中所述 [注册 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal)，您可在以下位置配置连接： [!UICONTROL HTTP] > [!UICONTROL 生成Oauth 2.0] 请求模块。

1. 添加 [!UICONTROL HTTP] > [!UICONTROL 进行OAuth 2.0调用] 模块到您的场景。
1. 单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 字段。
1. 按如下方式配置连接字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL连接名称]</td> 
      <td>输入连接的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[！UICONTROL流类型]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL授权URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL令牌URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL作用域]</td> 
      <td> <p>输入您在的步骤4中选择的权限 <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">注册 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]</a>.</p> <p>对于每个范围，单击 <b>[！UICONTROL添加]</b> 并键入权限。</p> <p>示例： <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL范围分隔符]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL客户端ID]</td> 
      <td>在中步骤2中输入[！UICONTROL应用程序ID] <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">注册 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL客户端密钥]</td> 
      <td>输入您在的步骤3中生成的[！UICONTROL应用程序密钥] <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">注册 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL Authorize parameters]</td> 
      <td> <p>添加以下授权参数：</p> 
       <ul> 
        <li> <p>[！UICONTROL Key]：<code> response_mode</code> [！UICONTROL值]： <code>query</code></p> </li> 
        <li> <p>[！UICONTROL Key]： <code>prompt </code>[！UICONTROL值]： <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL访问令牌参数]</td> 
      <td>您无需在此字段中输入任何内容。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL刷新令牌参数]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>单击 <b>[！UICONTROL添加]</b>.</p> </li> 
        <li value="2"> <p>在 <b>[！UICONTROL Key]</b> 字段，输入 <code>scope</code>.</p> </li> 
        <li value="3"> <p>在 <b>[！UICONTROL值]</b> 字段中，输入您在范围字段中输入的所有[！UICONTROL范围，并以空格分隔。</p> <p>示例： <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL Custom Headers]</td> 
      <td>您无需在此字段中输入任何内容。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL令牌放置]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 继续]**.
1. 在出现的窗口中，单击 **[!UICONTROL Accept]** 以完成连接并返回模块。
