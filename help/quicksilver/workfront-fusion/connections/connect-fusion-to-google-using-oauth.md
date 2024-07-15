---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 使用自定义OAuth客户端连接 [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services]
description: 您可以使用 [!DNL Adobe Workfront Fusion] 使用自定义OAuth客户端连接到 [!DNL Google Services] 。 此过程需要现有的 [!DNL Google] 帐户。
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# 使用自定义OAuth客户端将[!DNL Adobe Workfront Fusion]连接到[!DNL Google Services]

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

## 先决条件

您需要一个现有的[!DNL Google]帐户才能建立此连接。

## 使用自定义OAuth客户端将Fusion连接到Google服务

要创建此连接，必须在Google Cloud平台上创建和配置项目，然后根据该项目在Fusion中配置连接。

* [在 [!DNL Google Cloud Platform]上创建项目](#create-a-project-on-google-cloud-platform)
* [配置[!UICONTROL OAuth同意]设置](#configure-oauth-consent-settings)
* [创建OAuth凭据](#create-oauth-credentials)
* [连接到 [!DNL Workfront Fusion]中的 [!DNL Google] ](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>此过程适用于：
>
>* 个人使用（[!DNL `@gmail.com`]和[!DNL `@googlemail.com`]用户）
>* 内部使用（更喜欢使用自定义OAuth客户端的[!DNL Google Workspace]用户）

### 在[!DNL Google Cloud Platform]上创建项目

要在[!DNL Google Cloud]平台上创建项目，请执行以下操作：

1. 使用您的[!DNL Google]凭据登录到[[!DNL Google Cloud] 平台](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project)。
1. 在左侧面板中，单击&#x200B;**[!UICONTROL 仪表板]**。
1. 单击屏幕右上角的&#x200B;**[!UICONTROL 创建项目]**。
1. 输入&#x200B;**[!UICONTROL 项目名称]**，然后单击&#x200B;**[!UICONTROL 创建]**。

1. 单击屏幕顶部附近的&#x200B;**[!UICONTROL 启用API和服务]**&#x200B;选项卡。
1. 在屏幕顶部的&#x200B;**[!UICONTROL 搜索API和服务]**&#x200B;字段中，键入要使用的服务的名称（如[!DNL Gmail] API或[!DNL Google Drive] API）。
1. 显示时，单击要连接到[!DNL Workfront Fusion]的API或服务。
1. 单击&#x200B;**[!UICONTROL 启用]**&#x200B;以启用选定的API。
1. 对要启用的每个API重复步骤6-8。

   >[!NOTE]
   >
   >必须启用[!DNL Google Drive] API以及要使用的所有[!DNL Google]应用（如[!DNL Google Sheets] API）的API。

1. 在出现的屏幕上，单击右上角的&#x200B;**[!UICONTROL 创建凭据]**。
1. 继续阅读本文中的[配置OAuth同意设置](#configure-oauth-consent-settings)部分。

### 配置[!UICONTROL OAuth同意]设置

1. 在左侧面板中，单击&#x200B;**[!UICONTROL OAuth同意屏幕]**。
1. 选择&#x200B;**[!UICONTROL 外部]**，然后单击&#x200B;**[!UICONTROL 创建]**。

   >[!NOTE]
   >
   >选择此选项时不会向您收取费用。 有关详细信息，请参阅[!DNL Google]关于验证要求异常的信息。

1. 按如下方式填写必填字段：

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL应用程序名称]</p> </td> 
      <td> <p>输入请求同意的应用程序名称。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL用户支持电子邮件]</td> 
      <td>输入电子邮件地址，以便用户在连接到此应用程序时能够就同意问题与您联系。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL电子邮件地址]</td> 
      <td>输入一个或多个电子邮件地址，Google可使用这些地址通知您对项目所做的任何更改。</td> 
     </tr> 
    </tbody> 
   </table>

1. 在[!UICONTROL 授权域]下，单击&#x200B;**[!UICONTROL 添加域]**，然后输入`workfrontfusion.com`。

1. 单击&#x200B;**[!UICONTROL 保存并继续]**。
1. 单击&#x200B;**[!UICONTROL 添加或删除作用域]**。
1. 在右侧面板中，启用以下范围：

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>服务/API</th> 
      <th>所需的范围</th> 
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

您可能需要展开列表或转到列表的下一页以查看所有内容。

1. 单击&#x200B;**[!UICONTROL 更新]**。
1. 单击&#x200B;**[!UICONTROL 保存并继续]**。
1. （可选）将任何测试用户添加到项目。
1. 单击&#x200B;**[!UICONTROL 保存并继续]**。
1. 检查信息是否准确，然后单击&#x200B;**[!UICONTROL 返回仪表板]**。

   >[!NOTE]
   >
   >您无需提交同意屏幕和申请以供[!DNL Google]验证。

1. 继续[创建OAuth凭据](#create-oauth-credentials)。

### 创建OAuth凭据

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 凭据]**。

   >[!NOTE]
   >
   >如果这不是您启用的第一个API或服务（[!DNL Gmail]或[!DNL Google Drive]），则不必创建新凭据。

1. 单击屏幕顶部附近的&#x200B;**[!UICONTROL 创建凭据]**，然后从下拉菜单中选择&#x200B;**[!UICONTROL OAuth客户端ID]**。

1. 按如下方式填写必填字段：

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL应用程序类型]</td> 
      <td> <p> [！UICONTROL Web应用程序]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL名称]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. 在[!UICONTROL 授权重定向URI]下，单击&#x200B;**[!UICONTROL 添加URI]**&#x200B;并输入以下内容中的&#x200B;**one**：

   * 对于[!DNL Gmail]或[!DNL Google Drive]： `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * 对于其他[!DNL Google]应用： `https://app.workfrontfusion.com/oauth/cb/google`

1. 单击&#x200B;**[!UICONTROL 创建]**。

   显示[!UICONTROL 客户端ID]和[!UICONTROL 客户端密钥]。

1. 将[!UICONTROL 客户端ID]和[!UICONTROL 客户端密钥]复制到安全位置。 您将使用它们在[!DNL Workfront Fusion]中建立连接。
1. 继续[在 [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)中连接到 [!DNL Google] 。

### 连接到[!DNL Workfront Fusion]中的[!DNL Google]

创建与[!DNL Google]的连接过程有所不同，这取决于您使用的是来自[!DNL Google]服务（如[!DNL Google Sheets]或[!DNL Google Docs]）的模块，还是通过[!UICONTROL HTTP] >[!UICONTROL 创建OAuth2.0]请求模块连接到[!DNL Google]。

* [连接到 [!DNL Google] 服务中的 [!DNL Google] ](#connect-to-google-in-a-google-service)
* [连接到[!UICONTROL HTTP] > [!UICONTROL 发出OAuth2.0请求]模块中的 [!DNL Google] ](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### 连接到[!DNL Google]服务中的[!DNL Google]

1. 在[!DNL Workfront Fusion]中，找到需要为其创建连接的[!DNL Google]模块。
1. 单击&#x200B;**[!UICONTROL 创建连接]**，然后单击&#x200B;**[!UICONTROL 显示高级设置]**。

1. 在相应字段中输入您在[[!UICONTROL 创建OAuth凭据]](#create-oauth-credentials)中检索到的[!UICONTROL 客户端ID]和[!UICONTROL 客户端密钥]，然后单击&#x200B;**[!UICONTROL 继续]**。

1. 使用您的[!DNL Google]帐户登录。

   显示&#x200B;**[!UICONTROL 此应用未验证]**&#x200B;窗口。 请注意，窗口标题中提到的“应用程序”是您在上面创建的OAuth客户端。

1. 单击&#x200B;**[!UICONTROL 高级]**，然后单击&#x200B;**[!UICONTROL 转到[!DNL Workfront Fusion] （不安全）]**&#x200B;以允许使用您的自定义OAuth客户端进行访问。

1. 单击&#x200B;**[!UICONTROL 允许]**&#x200B;以授予[!DNL Workfront Fusion]权限。
1. 在出现的窗口中，再次单击&#x200B;**[!UICONTROL 允许]**&#x200B;以确认您的选择。

   已使用自定义OAuth客户端建立与所需[!DNL Google]服务的连接。

#### 连接到[!UICONTROL HTTP] > [!UICONTROL 发出OAuth2.0请求]模块中的[!DNL Google] {#connect-to-google-in-the-http--make-an-oauth20-request-module}

有关在[!UICONTROL HTTP] > [!UICONTROL 发出OAuth2.0请求]模块中连接到[!DNL Google]的说明，请参阅[在[!UICONTROL HTTP] > [!UICONTROL 在[[!UICONTROL HTTP] > [!UICONTROL 发出OAuth 2.0请求]模块](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)中创建 [!DNL Google] 的连接的说明。]](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)

## 可能的错误消息：[!UICONTROL [403]未配置访问]

如果显示[!UICONTROL `403 Access Not Configured`]错误消息，则需要在Google Cloud平台中启用相应的API。 要启用API，请按照本文中[在 [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)上创建项目一节中的步骤操作。
