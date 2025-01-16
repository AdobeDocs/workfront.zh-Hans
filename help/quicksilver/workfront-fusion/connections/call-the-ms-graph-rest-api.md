---
title: 通过 [!DNL Adobe Workfront Fusion] HTTP &amp；gt；调用MS Graph REST API。生成OAuth 2.0请求模块
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 1%

---

# 通过[!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 发出OAuth 2.0请求]模块调用[!UICONTROL  MS Graph REST API]

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [调用MS Graph REST API](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/call-the-ms-graph-rest-api.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

<!-- Audited: 3/2024-->

通过[!DNL Microsoft Graph API]访问许多[!DNL Microsoft] Web服务。 您可以使用[!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL 发出OAuth 2.0请求]模块来创建与[!DNL Microsoft Graph API]的连接。

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

## 在[!DNL Microsoft Application Registration Portal]中注册[!DNL Workfront Fusion]

要创建与[!DNL Microsoft Graph REST API]的连接，必须首先注册[!DNL Adobe Workfront Fusion]。

1. 开始注册新应用程序，如[!DNL Microsoft]文档中的[注册您的应用程序](https://docs.microsoft.com/en-us/graph/auth-register-app-v2)中所述。

   作为注册的一部分，[!DNL Microsoft]需要以下信息：

   <table style="table-layout:auto">
      <tr>
        <td>[！UICONTROL应用程序名称]</td>
        <td>输入应用程序的名称，如“我的[!DNL Workfront Fusion]应用程序”。</td>
      </tr>
      <tr>
        <td>[！UICONTROL重定向URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. 完成应用程序注册后，记下[!UICONTROL 应用程序ID]。

   >[!IMPORTANT]
   >
   >您需要应用程序ID才能在[!DNL Workfront Fusion]中设置连接。

1. 生成[!UICONTROL 应用程序密钥]。 记下这个秘密。

   有关说明，请参阅[!DNL Microsoft]文档中的[注册您的应用程序](https://docs.microsoft.com/en-us/graph/auth-register-app-v2)。

   >[!IMPORTANT]
   >
   >你需要[!UICONTROL 应用程序密钥]才能在[!DNL Workfront Fusion]中设置连接。

1. 配置应用程序的权限。

   有关查找和配置这些字段的详细信息，请参阅[!UICONTROL Microsoft]文档中[在没有用户的情况下获取访问权限](https://docs.microsoft.com/en-us/graph/auth-v2-service)中的“配置Microsoft Graph的权限”部分。

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
        <li> <p>您的集成所需的任何其他权限（示例： <code>User.Read</code>）</p> </li> 
       </ul> <p><b>重要信息</b>：您需要所选权限才能在[!DNL Workfront Fusion]中设置连接。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 继续在 [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion)中[配置您的 [!DNL MS Graph API] 连接。

## 在[!DNL Workfront Fusion]中配置您的[!DNL MS Graph API]连接

在 [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal)中注册[注册 [!DNL Workfront Fusion] 中讨论的[!DNL Workfront Fusion]后，您可以在[!UICONTROL HTTP] > [!UICONTROL 创建Oauth 2.0]请求模块中配置连接。

1. 添加[!UICONTROL HTTP] > [!UICONTROL 对方案进行OAuth 2.0调用]模块。
1. 单击[!UICONTROL 连接]字段旁边的&#x200B;**[!UICONTROL 添加]**。
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
      <td> <p>输入您在[!DNL Microsoft Application Registration Portal]</a>中<a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">注册[!DNL Workfront Fusion]的步骤4中选择的权限。</p> <p>对于每个作用域，单击<b>[！UICONTROL添加]</b>并键入权限。</p> <p>示例： <code>offline_access</code>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL范围分隔符]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL客户端ID]</td> 
      <td>在[!DNL Microsoft Application Registration Portal]</a>的<a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">注册[!DNL Workfront Fusion]中，输入步骤2中的[！UICONTROL应用程序ID]。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL客户端密钥]</td> 
      <td>在[!DNL Microsoft Application Registration Portal]</a>的<a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">注册[!DNL Workfront Fusion]中输入您在步骤3中生成的[！UICONTROL应用程序密钥]。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL Authorize parameters]</td> 
      <td> <p>添加以下授权参数：</p> 
       <ul> 
        <li> <p>[！UICONTROL Key]：<code> response_mode</code> [！UICONTROL Value]： <code>query</code></p> </li> 
        <li> <p>[！UICONTROL键]： <code>prompt </code>[！UICONTROL值]： <code>consent</code></p> </li> 
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
        <li value="1"> <p>单击<b>[！UICONTROL添加]</b>。</p> </li> 
        <li value="2"> <p>在<b>[！UICONTROL Key]</b>字段中，输入<code>scope</code>。</p> </li> 
        <li value="3"> <p>在<b>[！UICONTROL值]</b>字段中，输入您在范围字段中输入的所有[！UICONTROL范围]，并以空格分隔。</p> <p>示例： <code>offline_access openid User.Read</code></p> </li> 
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

1. 单击&#x200B;**[!UICONTROL 继续]**。
1. 在出现的窗口中，单击&#x200B;**[!UICONTROL 接受]**&#x200B;以完成连接并返回模块。
