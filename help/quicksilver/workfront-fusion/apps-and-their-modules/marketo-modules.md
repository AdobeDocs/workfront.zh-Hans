---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Marketo模块
description: 在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Marketo]，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2062'
ht-degree: 0%

---

# [!DNL Marketo] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Marketo]，并将其连接到多个第三方应用程序和服务。

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

使用 [!DNL Marketo] 模块，您必须具有 [!DNL Marketo] 帐户。

## Connect [!DNL Marketo] 到Workfront Fusion {#connect-marketo-to-workfront-fusion}

您可以创建与 [!DNL Marketo] 从内部直接获得帐户 [!DNL Marketo] 模块。

1. 在任意 [!DNL Marketo] 模块，单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 字段。
1. 输入您的 [!DNL Marketo] 帐户或 [!DNL Marketo] [!UICONTROL Munchkin] ID。 这是分配给您帐户的基本URL或端点的唯一部分，您使用它进行访问 [!DNL Marketo] 通过 [!UICONTROL REST] API。 有关查找此内容的说明，请参阅 [基本URL](https://developers.marketo.com/rest-api/base-url/) 在 [!DNL Marketo] 文档。
1. 输入您的 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密码]. 有关查找这些内容的说明，请参阅 [身份验证](https://developers.marketo.com/rest-api/authentication/) 在 [!DNL Marketo] 文档。
1. 单击 **[!UICONTROL 继续]** 以创建连接并返回模块。

## [!DNL Marketo] 模块及其字段

配置时 [!DNL Marketo] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Marketo] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

* [[!UICONTROL 观看记录]](#watch-records)
* [[!UICONTROL 观看活动（即时）]](#watch-events-instant)

#### [!UICONTROL 观看记录]

此触发器模块在创建或更新记录时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Marketo] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要创建的记录类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL活动]</strong> </p> <p>选择要监视的活动类型。 </p> <p>模块仅监视新活动。<br></p> </li> 
     <li> <p><strong>[！UICONTROL潜在客户]</strong> </p> <p>选择是否要监视新记录、更新的记录、新记录和更新的记录或特定字段更新。 如果选择监视特定字段更新，请选择您希望模块监视的字段。</p> </li> 
     <li> <p><strong>[！UICONTROL程序]</strong> </p> <p>选择是要监视新记录、更新的记录，还是同时监视新记录和更新的记录。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看活动（即时）]

此触发器模块在创建或更新记录时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Webhook]</p> </td> 
   <td> <p>输入您希望模块使用的webhook。</p> <p>有关Webhook的更多信息，请参阅 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">中的即时触发器(Webhook) [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 自定义API调用]](#custom-api-call)
* [[!UICONTROL 创建记录]](#create-a-record)
* [[!UICONTROL 更新记录]](#update-a-record)
* [[!UICONTROL 下载文件]](#download-a-file)
* [[!UICONTROL 上传文件]](#upload-a-file)
* [[!UICONTROL 读取记录]](#read-a-record)
* [[!UICONTROL 将潜在客户添加到列表]](#add-leads-to-a-list)
* [[!UICONTROL 从列表中删除潜在客户]](#remove-leads-from-a-list)
* [[!UICONTROL 计划活动]](#schedule-a-campaign)
* [[!UICONTROL 复制项目]](#copy-a-program)

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL Marketo] API。 这样，您就可以创建一个其他人无法实现的数据流自动化 [!DNL Marketo] 模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Marketo] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>输入相对路径 <code>https://{your-base-url}.mktorest.com/</code>.</td> 
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
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内使用的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建记录]

此操作模块在中创建新记录 [!DNL Marketo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Marketo] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要创建的记录类型。</p> 
    <ul> 
     <li> <p>[！UICONTROL公司]</p> </li> 
     <li> <p>[！UICONTROL文件夹]</p> </li> 
     <li> <p>[！UICONTROL潜在客户]</p> </li> 
     <li> <p>[！UICONTROL程序]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择要映射的字段]</td> 
   <td>如果要创建公司或销售线索，请选择要在创建新记录时为其设置值的字段，然后为这些字段输入值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL程序类型]</td> 
   <td>如果要创建程序，请选择要创建的程序类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL计划渠道] </td> 
   <td>如果您正在创建项目群，请选择要创建项目群的项目群渠道。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹] / [！UICONTROL项目名称]</td> 
   <td>如果要创建文件夹或程序，请输入或映射新记录的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL描述]</td> 
   <td> <p>如果要创建文件夹或程序，请输入或映射新记录的描述。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL父文件夹ID]</td> 
   <td>如果要创建文件夹或程序，请输入或映射要创建新记录的父文件夹的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL成本]</td> 
   <td>如果要创建项目，请添加任何成本。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标记]</td> 
   <td>如果要创建项目，请添加任意标记</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新记录]

此操作模块使用其ID更新现有记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Marketo] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要创建的记录类型。</p> 
    <ul> 
     <li> <p>[！UICONTROL公司]</p> </li> 
     <li> <p>[！UICONTROL潜在客户]</p> </li> 
     <li> <p>[！UICONTROL程序]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL公司] / [！UICONTROL潜在客户] / [！UICONTROL项目ID]</td> 
   <td>输入或映射要更新的记录ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择要映射的字段]</td> 
   <td>如果要更新“公司”或“销售线索”，请选择要更新值的字段，然后为这些字段输入值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目名称]</td> 
   <td>如果要更新程序，请输入或映射程序的新名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL描述]</td> 
   <td> <p>如果要更新程序，请输入或映射程序的新描述。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL开始日期]</td> 
   <td>如果要更新程序，请输入或映射程序的新起始日期。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL结束日期]</td> 
   <td>如果要更新项目群，请输入或映射项目群的新结束日期。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL成本]</td> 
   <td>如果要更新项目，请添加任何成本。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标记]</td> 
   <td>如果要更新项目，请添加任意标记</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载文件]

此操作模块使用文件ID下载文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Marketo] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件ID]</td> 
   <td>映射要下载的文件的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上传文件]

此操作模块会将新文件上传到 [!UICONTROL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Marketo] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td>从上一个模块中选择一个源文件，或映射源文件的名称和数据。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID]</td> 
   <td>输入或映射希望新文件所在的文件夹的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL描述]</td> 
   <td>输入已上传文件的描述。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

该操作模块使用记录的ID读取有关记录的信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Marketo] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要创建的记录类型。</p> 
    <ul> 
     <li> <p>[！UICONTROL营销活动]</p> </li> 
     <li> <p>[！UICONTROL公司]</p> </li> 
     <li> <p>[！UICONTROL潜在客户]</p> </li> 
     <li> <p>[！UICONTROL列表]</p> </li> 
     <li> <p>[！UICONTROL程序]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td>选择要包含在此模块的输出包中的信息。 根据您选择的[！UICONTROL记录类型]字段可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL &lt;object&gt; ID]</td> 
   <td>输入或映射要检索相关信息的对象的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将潜在客户添加到列表]

此操作模块使用潜在客户ID向列表添加一个或多个潜在客户。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Marketo] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL列表ID]</td> 
   <td>输入或映射要添加潜在客户的列表的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL潜在客户ID]</td> 
   <td> <p>对于要添加到列表中的每个潜在客户，单击 <b>[！UICONTROL添加]</b>，然后输入或映射要添加的潜在客户的ID。 您最多可以为模块添加300个潜在客户以添加到列表中。</p> <p>单击映射切换可映射要添加到列表中的现有潜在客户集合。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从列表中删除潜在客户]

此操作模块使用潜在客户ID从列表中删除一个或多个潜在客户。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Marketo] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL列表ID]</td> 
   <td>输入或映射要删除潜在客户的列表的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL潜在客户ID]</td> 
   <td> <p>对于要从列表中删除的每个潜在客户，单击 <b>[！UICONTROL添加]</b>，然后输入或映射要删除的潜在客户的ID。 您最多可以添加300个潜在客户，以便模块从列表中删除。 </p> <p>单击映射切换可映射要从列表中删除的现有潜在客户集合。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 计划活动]

此操作模块为特定日期计划一个现有营销活动。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Marketo] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL营销活动ID]</td> 
   <td>输入或映射要计划的营销活动的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL日期计划]</p> </td> 
   <td>选择要运行营销活动的日期。 如果此字段留空，则营销活动将在方案开始后5分钟运行。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 复制项目]

该操作模块使用现有程序的ID制作程序副本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Marketo] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL现有项目ID]</td> 
   <td>输入或映射要复制的程序的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL新项目名称]</p> </td> 
   <td> <p>输入或映射新项目的名称</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID]</td> 
   <td>输入或映射您希望新程序所在的文件夹的ID。</td> 
  </tr> 
 </tbody> 
</table>

### 搜索

* [[!UICONTROL 列出记录]](#list-records)
* [[!UICONTROL 搜索记录]](#update-a-record)

#### [!UICONTROL 列出记录]

此操作模块可检索特定类型的所有记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Marketo] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要列出的记录类型。</p> 
    <ul> 
     <li> <p>[！UICONTROL读取所有营销活动]</p> </li> 
     <li> <p>[！UICONTROL读取所有程序]</p> </li> 
     <li> <p>[！UICONTROL读取所有潜在客户] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL字段]</td> 
   <td>如果已选择检索潜在客户，请选择是要从列表还是项目群中检索潜在客户。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td>选择要包含在此模块的输出包中的信息。 根据您选择的[！UICONTROL记录类型]字段可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索记录]

此搜索模块检索符合特定搜索条件的记录列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Marketo] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要搜索的记录类型。</p> 
    <ul> 
     <li> <p>[！UICONTROL营销活动]</p> </li> 
     <li> <p>[！UICONTROL潜在客户]</p> </li> 
     <li> <p>[！UICONTROL程序]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL字段]</p> </td> 
   <td> <p>选择您要按名称、项目名称或工作区名称搜索。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值]</td> 
   <td>对于要搜索的每个值，单击 <b>[！UICONTROL添加项]</b> 并输入值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>
