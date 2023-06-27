---
title: 加宽模块
description: 在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!UICONTROL 加宽]，并将其连接到多个第三方应用程序和服务。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 1%

---

# [!DNL Widen] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!UICONTROL 加宽]，并将其连接到多个第三方应用程序和服务。

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

使用 [!UICONTROL 加宽] 模块，您必须具有 [!UICONTROL 加宽] 帐户。

## Connect [!DNL Widen] 到 [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

您可以创建与 [!DNL Widen] 直接从 [!DNL Widen] 模块。

1. 在任意 [!DNL Widen] 模块，单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 字段。
1. 选择 [!DNL Widen] 要连接的域。
1. 输入您的令牌 [!DNL Widen] 帐户。 有关查找此令牌的说明，请参阅 [[!DNL Widen] API常见问题解答](https://community.widen.com/collective/s/article/API-FAQs).
1. 单击 **[!UICONTROL 继续]** 以创建连接并返回模块。

## [!DNL Widen] 模块及其字段

配置时 [!DNL Widen] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Widen] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器模块](#trigger-modules)
* [操作模块](#action-modules)
* [搜索模块](#search-modules)

### 触发器模块

#### [!UICONTROL 观看资产]

此触发器模块会在创建或更新资产时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Widen] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件类型]</td> 
   <td> <p>选择您是要观看新资源还是更新的资源。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展开]</td> 
   <td> <p>除了资源字段之外，还选择要包含在模块输出中的属性。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td>选择要包含在模块输出中的字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内使用的最大资源数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作模块

* [[!UICONTROL 自定义API调用]](#custom-api-call)
* [[!UICONTROL 读取资源信息]](#read-asset-info)
* [[!UICONTROL 将资源添加到收藏集]](#add-assets-to-collections)
* [[!UICONTROL 从收藏集中删除资产]](#remove-assets-from-collection)
* [[!UICONTROL 更新资源元数据]](#update-asset-metadata)
* [[!UICONTROL 下载文件]](#download-file)
* [[!UICONTROL 上传] 文件](#upload-a-file)

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL Widen] API。 这样，您就可以创建一个其他人无法实现的数据流自动化 [!DNL Widen] 模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Widen] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL API版本]</td> 
   <td>选择是否要使用最新版本的 [!DNL Widen] API或版本1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>输入或映射API调用的URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[！UICONTROL Workfront Fusion]会为您添加授权标头。</p> </td> 
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

#### [!UICONTROL 读取资源信息]

此操作模块按其唯一ID检索单个资产。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Widen] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID]</td> 
   <td> <p>输入或映射要为其读取信息的资源的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展开]</td> 
   <td> <p>除了资源字段之外，还选择要包含在模块输出中的属性。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td>选择要包含在模块输出中的字段。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将资源添加到收藏集]

此操作模块向收藏集添加一个或多个资产。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Widen] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL收藏集ID]</td> 
   <td> <p>对于要将资产添加到的每个收藏集：</p> 
    <ol> 
     <li value="1"> <p> 单击 <strong>[！UICONTROL添加]</strong>.</p> </li> 
     <li value="2"> <p>输入或映射[！UICONTROL收藏集ID]。</p> </li> 
     <li value="3"> <p>单击 <strong>[！UICONTROL添加项]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID]</td> 
   <td> <p>对于要添加到收藏集的每个资产：</p> 
    <ol> 
     <li value="1"> <p> 单击 <strong>[！UICONTROL添加]</strong>.</p> </li> 
     <li value="2"> <p>输入或映射资源ID。</p> </li> 
     <li value="3"> <p>单击 <strong>[！UICONTROL添加项]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内使用的最大资源数。</p> </td> 
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
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Widen] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL收藏集ID]</td> 
   <td> <p>对于要从中删除资产的每个收藏集：</p> 
    <ol> 
     <li value="1"> <p> 单击 <strong>[！UICONTROL添加]</strong>.</p> </li> 
     <li value="2"> <p>输入或映射收藏集ID。</p> </li> 
     <li value="3"> <p>单击 <strong>[！UICONTROL添加项]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">资产ID</td> 
   <td> <p>对于要从收藏集中移除的每个资源：</p> 
    <ol> 
     <li value="1"> <p> 单击 <strong>[！UICONTROL添加]</strong>.</p> </li> 
     <li value="2"> <p>输入或映射资源ID。</p> </li> 
     <li value="3"> <p>单击 <strong>[！UICONTROL添加项]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内使用的最大资源数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新资源元数据]

此操作模块可更新资源的元数据字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Widen] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID]</td> 
   <td> <p>输入或映射要更新元数据的资源的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL元数据类型]</td> 
   <td> <p>选择要更新的元数据的元数据类型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL元数据]</td> 
   <td>选择要更新的元数据字段。 对于每个字段，输入该字段的新值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内使用的最大资源数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载文件]

此操作模块从下载资产 [!DNL Widen] 帐户。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Widen] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资产ID]</td> 
   <td> <p>输入或映射要下载的资源的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上传文件]

此操作模块将文件上传到 [!DNL Widen] 帐户。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Widen] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL上传配置文件]</td> 
   <td> <p>选择您希望模块使用的上传配置文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL上载方法]</td> 
   <td> <p>选择上载文件的方式。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL From File]</strong> </p> <p>从上一个模块中选择或映射源文件。</p> </li> 
     <li> <p><strong>[！UICONTROL By URL]</strong> </p> <p>输入或映射要上载的文件的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件名]</td> 
   <td>输入或映射已上传文件的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL元数据类型]</td> 
   <td>为要上载的文件选择元数据类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL元数据]</td> 
   <td>选择要包含在文件上载中的元数据字段。 对于每个字段，输入该字段的[！UICONTROL值]。</td> 
  </tr> 
 </tbody> 
</table>

### 搜索模块

* [[!UICONTROL 读取收藏集资产]](#read-collection-assets)
* [[!UICONTROL 搜索资源]](#search-assets)

#### [!UICONTROL 读取收藏集资产]

此操作模块可检索收藏集中的资产列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Widen] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL收藏集ID]</td> 
   <td> <p>输入或映射包含要读取的资产的收藏集的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL开始]</td> 
   <td>输入或映射要列出的第一个项目的编号。 这是对记录进行分页的一种方式。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Max]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序方式]</td> 
   <td> <p>选择要对资源进行排序的属性。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顺序]</td> 
   <td>选择您希望对资源进行升序排序还是降序排序。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td>选择要包含在模块输出中的字段。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索资源]

此搜索模块可检索与特定搜索条件匹配的资源列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Widen] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 到 [!DNL Workfront Fusion] </a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜索查询]</td> 
   <td> <p>输入搜索资产所依据的标准。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序方式]</td> 
   <td> <p>选择您希望如何对资源进行排序。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顺序]</td> 
   <td>选择您希望对资源进行升序排序还是降序排序。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Include已删除]</td> 
   <td>启用此选项可在搜索中包含已删除的资产。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Include已存档]</p> </td> 
   <td> <p>启用此选项可在搜索中包含已存档的资产。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜索文档文本]</td> 
   <td>启用此选项可在搜索中包含文档文本，启用此选项则仅包含标题与搜索条件匹配的资产。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL偏移]</td> 
   <td>输入或映射要检索其详细信息的第一个项目的编号。 这是对记录进行分页的一种方式。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL滚动]</td> 
   <td>启用此选项可允许滚动。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展开]</td> 
   <td> <p>除了资源字段之外，还选择要包含在模块输出中的属性。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td>选择要包含在模块输出中的字段。</td> 
  </tr> 
 </tbody> 
</table>
