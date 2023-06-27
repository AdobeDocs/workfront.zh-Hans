---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Frame.io模块
description: 此 [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io] 帐户。
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2311'
ht-degree: 0%

---

# [!DNL Frame.io] 模块

此 [!DNL Adobe Workfront Fusion] [!DNL Frame.io] 通过模块，您可以监测、创建、更新、检索或删除中的资源和注释 [!DNL Frame.io] 帐户。

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

## 先决条件

使用 [!DNL Frame.io] 模块，您必须具有 [!DNL Frame.io] 帐户

## Connect [!DNL Frame.io] 到 [!UICONTROL Adobe Workfront Fusion]

您可以连接到 [!DNL Frame.io] 使用API令牌或使用OAuth 2.0。

[连接到 [!DNL Frame.io] 使用API令牌](#connect-to-frameio-using-an-api-token)

[连接到 [!DNL Frame.io] 使用OAuth 2.0 PKCE](#connect-to-frameio-using-oauth-20-pkce)

### 连接到 [!DNL Frame.io] 使用API令牌

连接您的 [!DNL Frame.io] 目标帐户 [!DNL Workfront Fusion] 使用API令牌，您必须在中创建该API令牌 [!DNL Frame.io] 帐户，并将其插入 [!DNL Workfront Fusion] [!DNL Frame.io] [!UICONTROL 创建连接] 对话框。

1. 登录 [!DNL Frame.io] 帐户。
1. 转到 **[!UICONTROL 令牌]** 中的页面 [!DNL Frame.io] 开发人员。
1. 单击 **[!UICONTROL 新]**.
1. 输入令牌的名称，选择要使用的范围，然后单击 **[!UICONTROL 创建]**.
1. 复制提供的令牌。
1. 转到 [!DNL Workfront Fusion] 然后打开 [!DNL Frame.io] 模块的 **[!UICONTROL 创建连接]** 对话框。
1. 在 **[!UICONTROL 连接类型]** 字段，选择 **[!DNL Frame.io]**.
1. 输入您在步骤5中复制的令牌到 **[!UICONTROL 您的 [!DNL Frame.io] API密钥]** 字段并单击 **[!UICONTROL 继续]** 以建立连接。

已建立连接。 您可以继续设置模块。

### 连接到 [!DNL Frame.io] 使用OAuth 2.0 PKCE

您可以创建到以下对象的连接： [!DNL Frame.io] 将OAuth 2.0 PKCE与可选的客户端ID结合使用。 如果要在连接中包含客户端ID，则必须在中创建一个OAuth 2.0应用程序 [!DNL Frame.io] 帐户。

* [连接到 [!DNL Frame.io] 使用OAuth 2.0 PKCE（不带客户端ID）](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [连接到 [!DNL Frame.io] 使用OAuth 2.0 PKCE（带客户端ID）](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### 连接到 [!DNL Frame.io] 使用OAuth 2.0 PKCE（不带客户端ID）

1. 转到 [!DNL Workfront Fusion] 然后打开 [!DNL Frame.io] 模块的 **[!UICONTROL 创建连接]** 对话框。
1. 在 **[!UICONTROL 连接类型]** 字段，选择 **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. 在中输入新连接的名称 **[!UICONTROL 连接名称]** 字段。
1. 单击 **[!UICONTROL 继续]** 以建立连接。

已建立连接。 您可以继续设置模块。

#### 连接到 [!DNL Frame.io] 使用OAuth 2.0 PKCE（带客户端ID）

1. 在中创建OAuth 2.0应用程序 [!DNL Frame.io]. 有关说明，请参阅 [!DNL Frame.io] 相关文档 [!UICONTROL OAuth 2.0代码授权流程].

   >[!IMPORTANT]
   >
   >在中创建OAuth 2.0应用程序时 [!DNL Frame.io]：
   >
   >* 输入以下内容作为重定向URI：
   >   
   >  美洲/APAC `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  EMEA `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* 启用PCKE选项。


1. 复制提供的 `client_id`.
1. 转到 [!DNL Workfront Fusion] 然后打开 [!DNL Frame.io] 模块的 **[!UICONTROL 创建连接]** 对话框。
1. 在 **[!UICONTROL 连接类型]** 字段，选择 **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. 在中输入新连接的名称 **[!UICONTROL 连接名称]** 字段。
1. 单击 **[!UICONTROL 显示高级设置]**.
1. 输入 `client_id` 您在步骤2中复制到 **[!UICONTROL 客户端ID]** 字段。
1. 单击 **[!UICONTROL 继续]** 以建立连接。

已建立连接。 您可以继续设置模块。

## [!DNL Frame.io] 模块及其字段

配置时 [!DNL Frame.io] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Frame.io] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [资产](#assets)
* [注释](#comments)
* [项目](#projects)
* [其他](#other)

### 资产

* [[!UICONTROL 创建资产]](#create-an-asset)
* [[!UICONTROL 删除资源]](#delete-an-asset)
* [[!UICONTROL 获取资源]](#get-an-asset)
* [[!UICONTROL 列出资产]](#list-assets)
* [[!UICONTROL 更新资产]](#update-an-asset)
* [[!UICONTROL 观看资源已删除]](#watch-asset-deleted)
* [[!UICONTROL 观看资源标签已更新]](#watch-asset-label-updated)
* [[!UICONTROL 观看新资产]](#watch-new-asset)

#### [!UICONTROL 创建资产]

此操作模块将创建新资产。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择或映射拥有要为其创建资源的项目的团队。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目ID] </td> 
   <td> <p>选择项目或映射要为其创建资源的项目的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID] </td> 
   <td> <p>选择文件夹或映射要在其中创建资产的文件夹的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL类型] </td> 
   <td> <p>选择是创建文件夹还是文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名称] </td> 
   <td> <p>输入新文件或文件夹的名称。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Type </td> 
    <td> <p>Select the type of file you want to upload.</p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Size </td> 
    <td> <p>The file size in bytes.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">[！UICONTROL源URL] </td> 
   <td> <p>输入要上载文件的URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL描述] </td> 
   <td> <p>输入资产的简要说明。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除资源]

此操作模块删除指定的资产。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择或映射拥有包含要删除的资源的项目的团队。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目ID]</td> 
   <td> <p> 选择包含要删除的资源的项目或。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID] </td> 
   <td> <p>选择包含要删除的资源的文件夹</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID] </td> 
   <td> <p>选择或映射要删除的资源。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取资源]

此操作模块可检索资产详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择或映射拥有项目的团队，该项目包含要检索其详细信息的资产。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目ID]</td> 
   <td> <p> 选择包含要检索其详细信息的资源的项目。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID] </td> 
   <td> <p>选择包含要检索其详细信息的资源的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID] </td> 
   <td> <p>选择资源或映射要检索其详细信息的资源的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出资产]

此搜索模块可检索指定项目文件夹中的所有资产。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择或映射拥有项目的团队，该项目包含您要从中检索资产的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目ID]</td> 
   <td> <p> 选择包含要从中检索资产的文件夹的项目。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID] </td> 
   <td> <p>选择要从中列出资产的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>设置最大资源数 [!DNL Workfront Fusion] 将在一个执行周期内返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### `[!UICONTROL Update an Asset]`

此操作模块允许您更新现有资源的名称、描述或自定义字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择或映射拥有要为其更新资源的项目的团队。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目ID] </td> 
   <td> <p>选择项目或映射要为其更新资源的项目的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID] </td> 
   <td> <p>选择文件夹或映射要更新资产的文件夹的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名称] </td> 
   <td> <p>输入更新文件的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL描述] </td> 
   <td> <p>输入已更新资产的简要说明。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看资源已删除]

此触发器模块会在删除资产后启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook名称]</td> 
   <td> <p> 输入webhook的名称，例如已删除的资产。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择为其创建此webhook的团队。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看资源标签已更新]

此触发器模块在设置、更改或删除资产状态时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook名称]</td> 
   <td> <p> 输入webhook的名称，例如，资产状态已更新。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择为其创建此webhook的团队。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看新资产]

此触发器模块会在创建新资产后启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook名称]</td> 
   <td> <p> 输入webhook的名称，例如创建的资产。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择为其创建此webhook的团队。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 注释

* [[!UICONTROL 创建评论]](#create-a-comment)
* [[!UICONTROL 删除评论]](#delete-a-comment)
* [[!UICONTROL 获取评论]](#get-a-comment)
* [[!UICONTROL 列出注释]](#list-comments)
* [[!UICONTROL 更新评论]](#update-a-comment)
* [[!UICONTROL 观看评论已更新]](#watch-comment-updated)
* [[!UICONTROL 观看新评论]](#watch-new-comment)

#### [!UICONTROL 创建评论]

此操作模块向资源添加新评论或回复。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL类型] </td> 
   <td> <p>选择是要创建评论还是回复评论。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择或映射拥有项目的团队，该项目包含要添加注释的资产。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目ID] </td> 
   <td> <p>选择项目或映射项目ID，该项目包含要添加注释的资产。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID] </td> 
   <td> <p>选择文件夹或映射包含要添加评论的资源的文件夹的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID] </td> 
   <td> <p>选择或映射要添加评论的资产。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL注释ID] </td> 
   <td> <p>选择或映射您要添加回复的评论。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文本]</td> 
   <td> <p> 输入评论或回复的文本内容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL时间戳] </td> 
   <td> <p>在视频中输入评论应链接到的帧号。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除评论]

此操作模块删除现有评论。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID]</td> 
   <td> <p> 选择或映射拥有项目的团队，该项目包含您要从中删除评论的资产。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目ID]</td> 
   <td> <p> 选择项目或映射项目ID，该项目包含您要从中删除评论的资产。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID]</td> 
   <td> <p> 选择包含要删除评论的资源的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID] </td> 
   <td> <p>选择包含要删除的评论的资源。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL注释ID] </td> 
   <td> <p>选择要删除的注释。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取评论]

此操作模块检索指定注释的详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择或映射拥有项目的团队，该项目包含您要从中检索资产的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目ID] </td> 
   <td> <p>选择包含要从中检索资产的文件夹的项目。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID] </td> 
   <td> <p>选择要从中列出资产的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID] </td> 
   <td> <p>选择包含要检索的注释的资源。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL注释ID] </td> 
   <td> <p>选择要检索其详细信息的注释。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出注释]

此搜索模块检索指定资源的所有注释。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择或映射拥有项目的团队，该项目包含要从中检索注释的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目ID] </td> 
   <td> <p>选择包含要从中检索注释的文件夹的项目。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID] </td> 
   <td> <p>选择包含要从中列出注释的资源的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID] </td> 
   <td> <p>选择要为其列出注释的资源。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>设置评论的最大数量 [!DNL Workfront Fusion] 将在一个执行周期内返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新评论]

此操作模块编辑现有评论。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择或映射拥有项目的团队，该项目包含要更新评论的资产。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目ID] </td> 
   <td> <p>选择包含要更新评论的资源的项目\。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID] </td> 
   <td> <p>选择包含要更新评论的资源的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID] </td> 
   <td> <p>选择要更新评论的资产。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL注释ID] </td> 
   <td> <p>选择要更新的注释。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文本]</td> 
   <td> <p> 输入注释的文本内容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL时间戳] </td> 
   <td> <p>在评论链接到的视频中输入帧号。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看评论已更新]

此触发器模块在编辑评论时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook名称] </td> 
   <td> <p>输入webhook的名称，例如“已编辑注释”。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择为其创建此webhook的团队。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看新评论]

此触发器模块会在创建新评论或回复时启动场景。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook名称] </td> 
   <td> <p>输入webhook的名称，例如新建注释。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择为其创建此webhook的团队。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 项目

#### [!UICONTROL 列出项目]

此搜索模块检索指定团队的所有项目。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL团队ID] </td> 
   <td> <p>选择或映射要为其检索项目的团队。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>设置最大项目数 [!DNL Workfront Fusion] 将在一个执行周期内返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

#### [!UICONTROL 进行API调用]

此模块允许您执行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td>有关创建与的连接 [!DNL Frame.io]，请参见 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>输入相对路径 <code>https://api.frame.io</code>. 示例: <code> /v2/teams</code></p> <p>注意：有关可用端点的列表，请参阅 [!DNL Frame.io] API引用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自动添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串] </td> 
   <td> <p>输入请求查询字符串。 对于要包含在查询字符串中的每个参数，单击 <b>[！UICONTROL添加项]</b> 并输入字段名称和所需值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注释:  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**示例：** 以下API调用返回中的所有团队及其详细信息 [!DNL Frame.io] 帐户：

URL: `/v2/teams`

方法: `GET`

![](assets/api-call-example.png)

结果可在模块的“输出”中找到，位于“包”>“主体”下。

在我们的示例中，返回了1个团队的详细信息：

![](assets/api-call-output.png)
