---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: 按模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Bynder]，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1616'
ht-degree: 0%

---

# [!DNL Bynder] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Bynder]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL Bynder] 模块，您必须 [!DNL Bynder] 帐户。

## 连接 [!DNL Bynder] 到Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [创建连接 [!DNL Bynder] 从 [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [生成 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密钥] in [!DNL Bynder] （可选）](#generate-a-client-id-and-client-secret-in-bynder-optional)

### 创建连接 [!DNL Bynder] 从 [!DNL Workfront Fusion]

您可以通过 [!DNL Workfront Fusion] 至 [!DNL Bynder] 直接从内部帐户 [!DNL Bynder] 模块。

1. 在任意 [!DNL Bynder] 模块，单击 **[!UICONTROL 添加]** 旁边 [!UICONTROL 连接] 字段。
1. 选择 [!DNL Bynder] 域。
1. （可选）单击 **[!UICONTROL 高级设置]**，然后输入 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密钥].

   有关生成客户端ID和客户端密钥的说明，请参阅 [在中生成客户端ID和客户端密钥 [!DNL Bynder] （可选）](#generate-a-client-id-and-client-secret-in-bynder-optional) 在本文中。

1. 在 [!UICONTROL 登录] 窗口，输入用户名（电子邮件地址）和密码。
1. 单击 **[!UICONTROL 继续]** 创建连接，然后返回到模块。

### 生成 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密钥] in [!DNL Bynder] （可选）

如果要使用客户端ID和客户端密钥创建连接，则可以从 [!DNL Bynder] 帐户。 在中创建应用程序时，会生成客户端ID和客户端密钥 [!DNL Bynder].

有关在中创建应用程序的说明 [!DNL Bynder]，请参阅 [Oauth 2.0应用程序](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) 在 [!DNL Bynder] 文档。

>[!NOTE]
>
>在中创建应用程序时 [!DNL Bynder]，输入以下作为 `redirect uri`:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] 模块及其字段

配置 [!DNL Bynder] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Bynder] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [操作](#actions)
* [搜索](#searches)
* [触发器](#triggers)

### 操作

* [[!UICONTROL 自定义API调用]](#custom-api-call)
* [[!UICONTROL 读取资产元数据]](#read-asset-metadata)
* [[!UICONTROL 更新资产元数据]](#update-asset-metadata)
* [[!UICONTROL 将资产添加到收藏集]](#add-assets-to-a-collection)
* [[!UICONTROL 从收藏集中删除资产]](#remove-assets-from-collection)
* [[!UICONTROL 向资产添加标记]](#add-a-tag-to-assets)
* [[!UICONTROL 删除标记] 从资产](#remove-a-tag-from-assets)
* [[!UICONTROL 下载资产]](#download-asset)
* [[!UICONTROL 上传资产]](#upload-asset)

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL Bynder] API。 这样，您就可以创建数据流自动化，而另一个数据流无法实现 [!DNL Bynder] 模块。

配置此模块时，将显示以下字段。

模块会返回状态代码，以及API调用的标头和正文。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">连接 [!DNL Bynder] to [!DNL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>输入相对于 <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如： <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion会为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:  <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取资产元数据]

此操作模块读取资产的元数据。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">连接 [!DNL Bynder] to [!DNL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资产ID]</td> 
   <td>输入或映射要为其检索元数据的资产的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新资产元数据]

此操作模块会更新现有资产的元数据。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">连接 [!DNL Bynder] to [!DNL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资产ID]</td> 
   <td>输入或映射要更新其元数据的资产ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL字段]</td> 
   <td> <p>选择要输入信息的字段，然后输入或映射要更新元数据的信息到这些字段中。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL元属性]</p> </td> 
   <td>选择要更新的选项，然后输入信息或将其映射到这些属性中。 元属性是指有关资产不表示资产中特定字段的信息。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将资产添加到收藏集]

此操作模块可向收藏集添加一个或多个资产。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">连接 [!DNL Bynder] to [!DNL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL集合ID]</td> 
   <td> <p>输入或映射要在其中添加资产的集合ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资产ID]</td> 
   <td> <p>对于要添加到收藏集的每个资产，单击 <strong>[!UICONTROL添加项目]</strong>，然后输入或映射资产ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从收藏集中删除资产]

此操作模块会从收藏集中删除一个或多个资产。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">连接 [!DNL Bynder] to [!DNL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL集合ID]</td> 
   <td> <p>输入或映射您要删除资产的集合ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资产ID]</td> 
   <td> <p>对于要从收藏集中删除的每个资产，单击 <strong>[!UICONTROL添加项目]</strong>，然后输入或映射资产ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 向资产添加标记]

向一个或多个资产添加标记

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">连接 [!DNL Bynder] to [!DNL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标记ID]</td> 
   <td> <p>输入或映射要添加到资产的标记的ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资产ID]</td> 
   <td> <p>对于要标记的每个资产，单击 <strong>[!UICONTROL添加项目]</strong>，然后输入或映射资产ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从资产中删除标记]

从一个或多个资产中删除标记

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">连接 [!DNL Bynder] to [!DNL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标记ID]</td> 
   <td> <p>输入或映射要从资产中删除的标记的ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资产ID]</td> 
   <td> <p>对于要从中删除标记的每个资产，单击 <strong>[!UICONTROL添加项目]</strong>，然后输入或映射资产ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载资产]

此操作模块下载单个资产。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">连接 [!DNL Bynder] to [!DNL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资产ID]</td> 
   <td>输入或映射要下载的资产的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资产版本]</td> 
   <td> <p>输入或映射要下载的资产版本。 要下载资产的最新版本，请将字段留空。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上传资产]

此操作模块上传单个资产。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">连接 [!DNL Bynder] to [!DNL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL另存为]</td> 
   <td> <p>选择要保存上传文件的方式。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL新资产]</strong> </p> <p>选择要为其输入信息的字段和元属性，然后在这些字段中输入信息。</p> <p>输入或映射要用于已上传资产的品牌ID。</p> </li> 
     <li> <p><strong>[!UICONTROL新资产版本]</strong> </p> <p>输入您要为其上传新版本的资产的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td>从前一个模块中选择源文件，或映射源文件的名称和数据。</td> 
  </tr> 
 </tbody> 
</table>

### 搜索

* [[!UICONTROL 列表记录]](#list-record)
* [[!UICONTROL 搜索资产]](#search-for-assets)

#### [!UICONTROL 列表记录]

此搜索模块可检索特定类型的所有项目。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">连接 [!DNL Bynder] to [!DNL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td> <p>选择要列出的记录类型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL读取所有集合]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL读取有关所有标记的信息]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL读取集合的所有资产]</strong> </p> <p>输入或映射要列出其资产的集合的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出]</td> 
   <td> <p>选择要包含在模块输出中的字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大资产数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索资产]

此搜索模块会根据您提供的条件搜索资产。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">连接 [!DNL Bynder] to [!DNL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标准]</td> 
   <td> <p>输入搜索标准。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL字段]</strong> </p> <p>选择要在搜索中使用的字段</p> </li> 
     <li> <p><strong>[!UICONTROL逻辑运算符]</strong> </p> <p>选择要在搜索中使用的运算符。</p> </li> 
     <li> <p><strong>[!UICONTROL值]</strong> </p> <p>输入或映射要在选定字段中查找的值。 值类型应与选定字段的数据类型相同。 </p> <p>有关数据类型的更多信息，请参阅 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">中的项目数据类型 [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL结果集]</td> 
   <td>选择要返回第一个匹配的资产还是所有匹配的资产。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序依据]</td> 
   <td> <p>选择要排序的字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序方向]</td> 
   <td> <p>选择是升序排序还是降序排序。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出]</td> 
   <td> <p>选择要包含在模块输出中的字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大资产数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 触发器

#### [!UICONTROL 监视资产]

此触发器模块会在创建或更新资产时启动方案。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">连接 [!DNL Bynder] to [!DNL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL收藏集]</td>
   <td> <p>选择您要监视的新资产集合。 要观看所有收藏集，请将此字段留空。</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL限制]</td>

<td> <p>输入您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>
