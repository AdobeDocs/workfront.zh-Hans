---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Bynder模块
description: 在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Bynder]，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1664'
ht-degree: 0%

---

# [!DNL Bynder] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Bynder]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL Bynder] 模块，您必须具有 [!DNL Bynder] 帐户。

## Connect [!DNL Bynder] 到Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [创建连接 [!DNL Bynder] 起始日期 [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [生成 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密码] 在 [!DNL Bynder] （可选）](#generate-a-client-id-and-client-secret-in-bynder-optional)

### 创建连接 [!DNL Bynder] 起始日期 [!DNL Workfront Fusion]

您可以从中创建连接 [!DNL Workfront Fusion] 敬您的 [!DNL Bynder] 直接从 [!DNL Bynder] 模块。

1. 在任意 [!DNL Bynder] 模块，单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 字段。
1. 选择 [!DNL Bynder] 要连接的域。
1. （可选）单击 **[!UICONTROL 高级设置]**，然后输入您的 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密码].

   有关生成客户端ID和客户端密钥的说明，请参阅 [在中生成客户端ID和客户端密钥 [!DNL Bynder] （可选）](#generate-a-client-id-and-client-secret-in-bynder-optional) 本文章中。

1. 在 [!UICONTROL 登录] 窗口中，输入您的用户名（电子邮件地址）和密码。
1. 单击 **[!UICONTROL 继续]** 以创建连接并返回模块。

### 生成 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密码] 在 [!DNL Bynder] （可选）

如果要使用客户端ID和客户端密钥创建连接，则可以从生成连接 [!DNL Bynder] 帐户。 客户端ID和客户端密钥是在中创建应用程序时生成的 [!DNL Bynder].

有关在中创建应用程序的说明 [!DNL Bynder]，请参见 [Oauth 2.0应用程序](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) 在 [!DNL Bynder] 文档。

>[!NOTE]
>
>在中创建应用程序时 [!DNL Bynder]，请输入以下内容作为 `redirect uri`：
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] 模块及其字段

配置时 [!DNL Bynder] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Bynder] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [操作](#actions)
* [搜索](#searches)
* [触发器](#triggers)

### 操作

* [[!UICONTROL 自定义API调用]](#custom-api-call)
* [[!UICONTROL 读取资源元数据]](#read-asset-metadata)
* [[!UICONTROL 更新资源元数据]](#update-asset-metadata)
* [[!UICONTROL 将资产添加到收藏集]](#add-assets-to-a-collection)
* [[!UICONTROL 从收藏集中删除资产]](#remove-assets-from-collection)
* [[!UICONTROL 向资产添加标记]](#add-a-tag-to-assets)
* [[!UICONTROL 删除标记] 来自资产](#remove-a-tag-from-assets)
* [[!UICONTROL 下载资源]](#download-asset)
* [[!UICONTROL 上传资产]](#upload-asset)

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL Bynder] API。 这样，您就可以创建一个其他人无法实现的数据流自动化 [!DNL Bynder] 模块。

配置此模块时，会显示以下字段。

模块会返回一个状态代码，以及API调用的标头和正文。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>输入相对路径 <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如： <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion会为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL 读取资源元数据]

此操作模块读取资源的元数据。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID]</td> 
   <td>输入或映射要为其检索元数据的资源的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新资源元数据]

此操作模块更新现有资源的元数据。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID]</td> 
   <td>输入或映射要为其更新元数据的资源的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL字段]</td> 
   <td> <p>选择要为其输入信息的字段，然后输入要更新元数据的信息或将其映射到这些字段中。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL元属性]</p> </td> 
   <td>选择要更新的选项，然后输入信息或将信息映射到这些属性。 元属性是有关资源的信息，并不表示资源中的特定字段。</td> 
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
    <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL收藏集ID]</td> 
   <td> <p>输入或映射要添加资产的收藏集的ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID]</td> 
   <td> <p>对于要添加到收藏集的每个资产，请单击 <strong>[！UICONTROL添加项]</strong>，然后输入或映射资源ID。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL收藏集ID]</td> 
   <td> <p>输入或映射要删除资产的收藏集的ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID]</td> 
   <td> <p>对于要从收藏集中删除的每个资源，请单击 <strong>[！UICONTROL添加项]</strong>，然后输入或映射资源ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 向资产添加标记]

向一个或多个资源添加标记

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标记ID]</td> 
   <td> <p>输入或映射要添加到资产的标记的ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID]</td> 
   <td> <p>对于要标记的每个资产，单击 <strong>[！UICONTROL添加项]</strong>，然后输入或映射资源ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从资源中删除标记]

从一个或多个资源中删除标记

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标记ID]</td> 
   <td> <p>输入或映射要从资产中删除的标记的ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID]</td> 
   <td> <p>对于要从其中删除标记的每个资源，单击 <strong>[！UICONTROL添加项]</strong>，然后输入或映射资源ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载资源]

该操作模块可下载单个资产。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID]</td> 
   <td>输入或映射要下载的资源的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产版本]</td> 
   <td> <p>输入或映射要下载的资源版本。 要下载最新版本的资源，请将字段留空。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL另存为]</td> 
   <td> <p>选择要如何保存要上传的文件。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL新资产]</strong> </p> <p>选择要为其输入信息的字段和元属性，然后在这些字段中输入信息。</p> <p>输入或映射要用于上传的资产的品牌ID。</p> </li> 
     <li> <p><strong>[！UICONTROL新资产版本]</strong> </p> <p>输入要为其上传新版本的资产的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td>从上一个模块中选择一个源文件，或映射源文件的名称和数据。</td> 
  </tr> 
 </tbody> 
</table>

### 搜索

* [[!UICONTROL 列表记录]](#list-record)
* [[!UICONTROL 搜索资源]](#search-for-assets)

#### [!UICONTROL 列表记录]

此搜索模块可检索特定类型的所有项目。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要列出的记录类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL读取所有收藏集]</strong> </p> </li> 
     <li> <p><strong>[！UICONTROL阅读有关所有标记的信息]</strong> </p> </li> 
     <li> <p><strong>[！UICONTROL读取收藏集的所有资产]</strong> </p> <p>输入或映射要为其列出资产的收藏集的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td> <p>选择要包含在模块输出中的字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大资源数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索资源]

此搜索模块根据您提供的条件搜索资产。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标准]</td> 
   <td> <p>输入搜索条件。 </p> 
    <ul> 
     <li> <p><strong>[！UICONTROL字段]</strong> </p> <p>选择要在搜索中使用的字段</p> </li> 
     <li> <p><strong>[！UICONTROL逻辑运算符]</strong> </p> <p>选择要在搜索中使用的运算符。</p> </li> 
     <li> <p><strong>[！UICONTROL值]</strong> </p> <p>在选定字段中输入或映射要查找的值。 值类型应与所选字段的数据类型相同。 </p> <p>有关数据类型的更多信息，请参阅 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">中的项目数据类型 [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL结果集]</td> 
   <td>选择是要返回第一个匹配的资源还是所有匹配的资源。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序方式]</td> 
   <td> <p>选择要作为排序依据的字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序方向]</td> 
   <td> <p>选择是要升序排序还是降序排序。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td> <p>选择要包含在模块输出中的字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大资源数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 触发器

#### [!UICONTROL 观看资产]

此触发器模块会在创建或更新资产时启动方案。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Bynder] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[！UICONTROL收藏集]</td>
   <td> <p>选择要监视新资产的收藏集。 要观看所有收藏集，请将此字段留空。</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[！UICONTROL限制]</td>

<td> <p>输入您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>
