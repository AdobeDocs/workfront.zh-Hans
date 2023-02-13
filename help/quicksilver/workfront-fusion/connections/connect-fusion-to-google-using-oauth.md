---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 连接 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自定义OAuth客户端
description: 您可以使用 [!DNL Adobe Workfront Fusion] 连接到 [!DNL Google Services] 使用自定义OAuth客户端。 此过程需要现有 [!DNL Google] 帐户。
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# 连接 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自定义OAuth客户端

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

## 先决条件

您需要现有 [!DNL Google] 帐户建立此连接。

## 在上创建项目 [!DNL Google Cloud Platform]

以下过程适用于：

* 个人用途([!DNL @gmail.com] 和 [!DNL @googlemail.com] 用户)
* 内部使用([!DNL G Suite] 偏好使用自定义OAuth客户端的用户)

在上创建项目 [!DNL Google Cloud] 平台：

1. 登录到 [[!DNL Google Cloud] 平台](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 使用 [!DNL Google] 凭据。
1. 在左侧面板中，单击 **[!UICONTROL 功能板]**.
1. 单击 **[!UICONTROL 创建项目]** 中。
1. 输入 **[!UICONTROL 项目名称]**，然后单击 **[!UICONTROL 创建]**.

1. 单击 **[!UICONTROL 启用API和服务]** 选项卡。
1. 在 **[!UICONTROL 搜索API和服务]** 字段中，键入要使用的服务名称(例如 [!DNL Gmail] API或 [!DNL Google Drive] API)。
1. 显示时，单击要连接的API或服务 [!DNL Workfront Fusion].
1. 单击 **[!UICONTROL 启用]** 以启用所选API。
1. 对要启用的每个API重复步骤6-8。

   >[!NOTE]
   >
   >必须启用 [!DNL Google Drive] API以及所有 [!DNL Google] 要使用的应用程序(例如 [!DNL Google Sheets] API)。

1. 在显示的屏幕上，单击 **[!UICONTROL 创建凭据]** 中。
1. 继续部分 [配置OAuth同意设置](#configure-oauth-consent-settings) 在本文中。

## 配置 [!UICONTROL OAuth同意] 设置

1. 在左侧面板中，单击 **[!UICONTROL OAuth同意屏幕]**.
1. 选择 **[!UICONTROL 外部]**，然后单击 **[!UICONTROL 创建]**.

   >[!NOTE]
   >
   >选择此选项时，您无需支付任何费用。 有关更多信息，请参阅 [!DNL Google]有关验证要求的例外的信息。

1. 按如下方式填写必填字段：

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL应用程序名称]</p> </td> 
      <td> <p>输入请求同意的应用程序名称。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL用户支持电子邮件]</td> 
      <td>输入一个电子邮件地址，供用户在连接到此应用程序时，如果遇到有关其同意的问题，请联系您。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL电子邮件地址]</td> 
      <td>输入一个或多个电子邮件地址，Google可使用这些地址通知您项目的任何更改。</td> 
     </tr> 
    </tbody> 
   </table>

1. 在 [!UICONTROL 授权域]，单击 **[!UICONTROL 添加域]**，然后输入 `workfrontfusion.com`.

1. 单击 **[!UICONTROL 保存并继续]**.
1. 单击 **[!UICONTROL 添加或删除作用域]**.
1. 在右侧面板中，启用以下范围：

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>服务/API</th> 
      <th>必需的范围</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

您可能需要展开该列表或转到列表的下一页，才能看到所有列表。

1. 单击 **[!UICONTROL 更新]**.
1. 单击 **[!UICONTROL 保存并继续]**.
1. （可选）将任何测试用户添加到项目。
1. 单击 **[!UICONTROL 保存并继续]**.
1. 检查信息的准确性，然后单击 **[!UICONTROL 返回到功能板]**.

   >[!NOTE]
   >
   >您无需提交同意屏幕和申请以供验证 [!DNL Google].

1. 继续 [创建OAuth凭据](#create-oauth-credentials).

## 创建OAuth凭据

1. 在左侧面板中，单击 **[!UICONTROL 凭据]**.

   >[!NOTE]
   >
   >如果这不是第一个API或服务([!DNL Gmail] 或 [!DNL Google Drive])，则无需创建新凭据。

1. 单击 **[!UICONTROL 创建凭据]** 在屏幕顶部附近，选择 **[!UICONTROL OAuth客户端ID]** 下拉菜单中。

1. 按如下方式填写必填字段：

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL应用程序类型]</td> 
      <td> <p> [!UICONTROL Web应用程序]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL名称]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 [!UICONTROL 授权的重定向URI]，单击 **[!UICONTROL 添加URI]** 输入 **one** （二）以下各项：

   * 对于 [!DNL Gmail] 或 [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * 对于其他 [!DNL Google] 应用程序： `https://app.workfrontfusion.com/oauth/cb/google`

1. 单击&#x200B;**[!UICONTROL 创建]**。

   的 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密钥] 显示。

1. 复制 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密钥] 到安全位置。 您将使用它们在 [!DNL Workfront Fusion].
1. 继续 [连接到 [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

## 连接到 [!DNL Google] in [!DNL Workfront Fusion]

创建与的连接的过程 [!DNL Google] 根据您是否使用的模块， [!DNL Google] 服务(例如 [!DNL Google Sheets] 或 [!DNL Google Docs])，或者如果您连接到 [!DNL Google] 通过 [!UICONTROL HTTP] >[!UICONTROL 制作OAuth2.0] 请求模块。

* [连接到 [!DNL Google] 在 [!DNL Google] 服务](#connect-to-google-in-a-google-service)
* [连接到 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 发出OAuth2.0请求] 模块](#connect-to-google-in-the-http--make-an-oauth20-request-module)

### 连接到 [!DNL Google] 在 [!DNL Google] 服务

1. 在 [!DNL Workfront Fusion]，找到 [!DNL Google] 模块。
1. 单击 **[!UICONTROL 创建连接]**，然后单击 **[!UICONTROL 显示高级设置]**.

1. 输入 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密钥] 检索到 [[!UICONTROL 创建OAuth凭据]](#create-oauth-credentials) 在相应的字段中，单击 **[!UICONTROL 继续]**.

1. 使用 [!DNL Google] 帐户。

   的 **[!UICONTROL 未验证此应用程序]** 窗口。 请注意，窗口标题中提及的“应用程序”是您在上面创建的OAuth客户端。

1. 单击 **[!UICONTROL 高级]**，然后单击 **[!UICONTROL 转到 [!DNL Workfront Fusion] （不安全）]** 允许使用您的自定义OAuth客户端进行访问。

1. 单击 **[!UICONTROL 允许]** 授予 [!DNL Workfront Fusion] 权限。
1. 在出现的窗口中，单击 **[!UICONTROL 允许]** 再次确认您的选择。

   与所需的 [!DNL Google] 使用自定义OAuth客户端的服务已建立。

### 连接到 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 发出OAuth2.0请求] 模块 {#connect-to-google-in-the-http--make-an-oauth20-request-module}

有关连接到的说明 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 发出OAuth2.0请求] 模块，请参阅 [创建连接的说明 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 发出OAuth 2.0请求] 模块](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) in [[!UICONTROL HTTP] > [!UICONTROL 发出OAuth 2.0请求] 模块](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## 可能的错误消息：[!UICONTROL [403] 未配置访问]

如果 [!UICONTROL [403] 未配置访问] 错误消息，您需要在Google云平台中启用相应的API。 要启用API，请按照部分中的步骤操作 [在上创建项目 [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) 在本文中。
