---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 连接 [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] 使用自定义OAuth客户端
description: 您可以使用 [!DNL Adobe Workfront Fusion] 以连接到 [!DNL Google Services] 使用自定义OAuth客户端。 此过程需要现有 [!DNL Google] 帐户。
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 7d2b4a9940cb21de1b8b5f2955f53b3d88040e44
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# 连接 [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] 使用自定义OAuth客户端

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

## 先决条件

您需要一个现有的 [!DNL Google] 帐户建立此连接。

## 使用自定义OAuth客户端将Fusion连接到Google服务

要创建此连接，必须在Google Cloud平台上创建和配置项目，然后根据该项目在Fusion中配置连接。

* [创建项目 [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [配置 [!UICONTROL OAuth同意] 设置](#configure-oauth-consent-settings)
* [创建OAuth凭据](#create-oauth-credentials)
* [连接到 [!DNL Google] 在 [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>此过程适用于：
>
>* 个人使用([!DNL `@gmail.com`] 和 [!DNL `@googlemail.com`] 用户)
>* 内部使用([!DNL G Suite] 更喜欢使用自定义OAuth客户端的用户)

### 创建项目 [!DNL Google Cloud Platform]

创建项目 [!DNL Google Cloud] 平台：

1. 登录 [[!DNL Google Cloud] 平台](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 使用 [!DNL Google] 凭据。
1. 在左侧面板中，单击 **[!UICONTROL 仪表板]**.
1. 单击 **[!UICONTROL 创建项目]** 屏幕右上角的。
1. 输入 **[!UICONTROL 项目名称]**，然后单击 **[!UICONTROL 创建]**.

1. 单击 **[!UICONTROL 启用API和服务]** 选项卡。
1. 在 **[!UICONTROL 搜索API和服务]** 字段，键入要使用的服务的名称(例如 [!DNL Gmail] API或 [!DNL Google Drive] API)。
1. 显示时，单击要连接的API或服务 [!DNL Workfront Fusion].
1. 单击 **[!UICONTROL 启用]** 以启用选定的API。
1. 对要启用的每个API重复步骤6-8。

   >[!NOTE]
   >
   >您必须启用 [!DNL Google Drive] API以及所有应用程序的API [!DNL Google] 要使用的应用程序(例如 [!DNL Google Sheets] API)。

1. 在显示的屏幕上，单击 **[!UICONTROL 创建凭据]** 在右上角。
1. 转到部分 [配置OAuth同意设置](#configure-oauth-consent-settings) 本文章中。

### 配置 [!UICONTROL OAuth同意] 设置

1. 在左侧面板中，单击 **[!UICONTROL OAuth同意屏幕]**.
1. 选择 **[!UICONTROL 外部]**，然后单击 **[!UICONTROL 创建]**.

   >[!NOTE]
   >
   >选择此选项时不会向您收取费用。 有关更多信息，请参阅 [!DNL Google]的信息，了解验证要求的例外情况。

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

1. 下 [!UICONTROL 授权域]，单击 **[!UICONTROL 添加域]**，并输入 `workfrontfusion.com`.

1. 单击 **[!UICONTROL 保存并继续]**.
1. 单击 **[!UICONTROL 添加或删除范围]**.
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

1. 单击 **[!UICONTROL 更新]**.
1. 单击 **[!UICONTROL 保存并继续]**.
1. （可选）将任何测试用户添加到项目。
1. 单击 **[!UICONTROL 保存并继续]**.
1. 检查信息是否准确，然后单击 **[!UICONTROL 返回仪表板]**.

   >[!NOTE]
   >
   >您无需提交同意屏幕和申请以进行验证 [!DNL Google].

1. 继续 [创建OAuth凭据](#create-oauth-credentials).

### 创建OAuth凭据

1. 在左侧面板中，单击 **[!UICONTROL 凭据]**.

   >[!NOTE]
   >
   >如果这不是第一个API或服务([!DNL Gmail] 或 [!DNL Google Drive])已启用，则无需创建新凭据。

1. 单击 **[!UICONTROL 创建凭据]** 在屏幕顶部附近，然后选择 **[!UICONTROL OAuth客户端ID]** 从下拉菜单中。

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

1. 下 [!UICONTROL 授权的重定向URI]，单击 **[!UICONTROL 添加URI]** 并输入 **一** 下列各项之一：

   * 对象 [!DNL Gmail] 或 [!DNL Google Drive]： `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * 对于其他 [!DNL Google] 应用程序： `https://app.workfrontfusion.com/oauth/cb/google`

1. 单击 **[!UICONTROL 创建]**.

   此 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密码] 显示。

1. 复制 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密码] 到一个安全的地方。 您将使用它们在中建立连接 [!DNL Workfront Fusion].
1. 继续 [连接到 [!DNL Google] 在 [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### 连接到 [!DNL Google] 在 [!DNL Workfront Fusion]

创建与的连接 [!DNL Google] 根据您使用的模块是否来自 [!DNL Google] 服务(例如 [!DNL Google Sheets] 或 [!DNL Google Docs])，或者如果您要连接到 [!DNL Google] 通过 [!UICONTROL HTTP] >[!UICONTROL 生成OAuth2.0] 请求模块。

* [连接到 [!DNL Google] 在 [!DNL Google] 服务](#connect-to-google-in-a-google-service)
* [连接到 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 发出OAuth2.0请求] 模块](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### 连接到 [!DNL Google] 在 [!DNL Google] 服务

1. 在 [!DNL Workfront Fusion]，找到 [!DNL Google] 需要为其创建连接的模块。
1. 单击 **[!UICONTROL 创建连接]**，然后单击 **[!UICONTROL 显示高级设置]**.

1. 输入 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密码] 您的检索位置 [[!UICONTROL 创建OAuth凭据]](#create-oauth-credentials) 在相应的字段中，然后单击 **[!UICONTROL 继续]**.

1. 使用您的登录 [!DNL Google] 帐户。

   此 **[!UICONTROL 此应用未验证]** 窗口随即显示。 请注意，窗口标题中提到的“应用程序”是您在上面创建的OAuth客户端。

1. 单击 **[!UICONTROL 高级]**，然后单击 **[!UICONTROL 转到 [!DNL Workfront Fusion] （不安全）]** 以允许使用您的自定义OAuth客户端进行访问。

1. 单击 **[!UICONTROL 允许]** 授予 [!DNL Workfront Fusion] 许可。
1. 在出现的窗口中，单击 **[!UICONTROL 允许]** 再次确认您的选择。

   与所需设备的连接 [!DNL Google] 使用自定义OAuth客户端的服务已建立。

#### 连接到 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 发出OAuth2.0请求] 模块 {#connect-to-google-in-the-http--make-an-oauth20-request-module}

有关连接的说明 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 发出OAuth2.0请求] 模块，请参见 [有关创建连接的说明 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 发出OAuth 2.0请求] 模块](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) 在 [[!UICONTROL HTTP] > [!UICONTROL 发出OAuth 2.0请求] 模块](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## 可能的错误消息：[!UICONTROL [403] 未配置访问]

如果 [!UICONTROL `403 Access Not Configured`] 错误消息显示，您需要在Google Cloud平台中启用相应的API。 要启用API，请按照部分中的步骤操作 [创建项目 [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) 本文章中。
