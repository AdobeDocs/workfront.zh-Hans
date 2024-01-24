---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Salesforce模块
description: 在Adobe Workfront Fusion场景中，您可以自动使用Salesforce的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2740'
ht-degree: 0%

---

# [!DNL Salesforce] 模块

在Adobe Workfront Fusion场景中，您可以自动使用 [!DNL Salesforce]，并将其连接到多个第三方应用程序和服务。

有关Salesforce连接器的视频介绍，请参阅：

* [Salesforce](https://video.tv.adobe.com/v/3427027/){target=_blank}

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* 并非所有版本 [!DNL Salesforce] 拥有API访问权限。 有关详细信息，请参阅有关 [!DNL Salesforce] 具有API访问权限的版本 [!DNL Salesforce] 社区站点。
>* 有关从返回的特定错误的信息 [!DNL Salesforce] API，请参见 [!DNL Salesforce] API文档。 您还可以检查 [!DNL Salesforce] API可用于任何可能的服务中断。
>

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
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!DNL Salesforce] 模块，您必须拥有 [!DNL Salesforce] 帐户。

## 关于搜索 [!DNL Salesforce] 对象

在搜索对象时，您可以输入单个搜索词，也可以使用通配符和运算符创建更复杂的查询：

* 使用星号通配符(\*)代替零个或多个字符。 例如，搜索Ca\*会查找以Ca开头的项目
* 使用问号通配符(？) 作为单个字符的替代。 例如，搜索Jo？n将查找词为John或Joan但不包含Jon的项目
* 使用引号运算符(“ ”)查找精确匹配的短语。 例如：“星期一会议”

有关搜索可能性的详细信息，请参阅 [!DNL Salesforce] 有关SOQL和SOSL的开发人员文档。

## [!DNL Salesforce] 模块及其字段

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

* [[!UICONTROL 留意记录]](#watch-for-records)
* [[!UICONTROL 观看出站消息]](#watch-outbound-messages)
* [[!UICONTROL 观看字段]](#watch-a-field)

#### [!UICONTROL 留意记录]

此触发器模块在创建或更新对象中的记录时执行场景。 该模块返回与一个或多个记录关联的所有标准字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL类型] </td> 
   <td> <p>选择类型 [!DNL Salesforce] 录制您希望模块观看的内容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL记录字段]</td> 
   <td>选择您希望模块监视的字段。 可用字段取决于记录类型。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大记录数]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL监视]</td> 
   <td> <p>确定您希望方案仅监视所选类型的新记录，还是只监视所选类型的新记录以及该类型记录的所有其他更改。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看出站消息]

此触发器模块会在有人发送消息时执行场景。 该模块返回与一个或多个记录关联的所有标准字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

此模块需要一些额外的设置：

1. 转到 [!DNL Salesforce] 设置页面。

   要访问设置页面，请找到并单击标有“[!UICONTROL 设置]”位于的右上角 [!DNL Salesforce] 帐户。 从 [!DNL Salesforce] 设置页面，找到&quot;[!UICONTROL 快速查找/搜索]”栏在左侧。 搜索&quot;[!UICONTROL 工作流规则]“

1. 单击 **[!UICONTROL 工作流规则]**.
1. 在 [!UICONTROL 工作流规则] 页面上，单击 **[!UICONTROL 新建规则]** 并选择要应用规则的对象类型(如&quot;[!UICONTROL 机会]”如果您在监视Opportunity记录的更新)。
1. 单击 **[!UICONTROL 下一个]**.
1. 设置规则名称、评估标准和规则标准，然后单击 **[!UICONTROL 保存]** 和 **[!UICONTROL 下一个]**.

1. 单击 **[!UICONTROL 完成]**.
1. 在新创建的工作流规则中，单击 **[!UICONTROL 编辑]**..
1. 从 **[!UICONTROL 添加工作流操作]** 下拉列表，选择 **[!UICONTROL 新建出站消息]**.

1. 指定名称、说明、端点URL以及要包括在新出站消息中的字段，然后单击 **[!UICONTROL 保存]**.

   此 **[!UICONTROL 端点URL]** 字段包含在上提供的URL。 [!DNL Salesforce] [!UICONTROL 出站消息] 在 [!DNL Workfront Fusion].

1. 配置以开头的方案 [!UICONTROL 出站消息] 事件。

1. 单击 **&lt;/>** 图标，并复制提供的URL。
1. 返回到 **[!UICONTROL 工作流规则]** 页面上，找到新创建的规则，然后单击 **[!UICONTROL 激活]**.

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Webhook]</td> 
   <td> <p>选择要用于监视传出消息的webhook。 要添加webhook，请单击 <strong>[！UICONTROL添加]</strong> 并输入webhook的名称和连接。</p> <p>有关连接 [!DNL Salesforce] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[！UICONTROL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL记录类型] </td> 
   <td> <p>选择类型 [!DNL Salesforce] 录制您希望模块监视传出消息的消息。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL字段]</td> 
   <td> <p>选择您希望模块监视传出消息的字段。 可用字段取决于记录类型。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL 观看字段]*

此触发器模块在中更新字段时启动方案 [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL记录类型] </td> 
   <td> <p>选择记录类型，其中包含您希望模块监视的字段。 您必须选择已打开[！UICONTROL字段历史记录]的记录类型 [!DNL Salesforce] 设置。 有关更多信息，请参阅 <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">字段历史记录跟踪</a> 在 [!DNL Salesforce] 文档。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL字段]</td> 
   <td> <p>选择您希望模块关注更改的字段。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期中返回的最大字段数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 创建记录]](#create-a-record)
* [[!UICONTROL 读取记录]](#read-a-record)
* [[!UICONTROL 删除记录]](#delete-a-record)
* [[!UICONTROL 自定义API调用]](#custom-api-call)
* [[!UICONTROL 上载附件/文档]](#upload-attachmentdocument)
* [[!UICONTROL 下载附件/文档]](#download-attachmentdocument)

#### [!UICONTROL 创建记录]

此操作模块在对象中创建新记录。

利用模块，可选择模块中可用的对象字段。 这减少了设置模块时必须滚动的字段数。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL记录类型] </p> </td> 
   <td> <p>选择类型 [!DNL Salesforce] 您希望模块创建的记录。 根据[！UICONTROL记录类型]字段中选择的记录类型，字段将变为可用。 这些字段基于 [!DNL Salesforce] API。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL选择要映射的字段]</td> 
   <td> <p>选择您希望模块在创建新记录时配置的字段。 必填字段位于列表顶部。 </p> <p>您选择的字段在此字段下打开。 您现在可以在这些字段中输入值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

此操作模块从中的单个对象读取数据 [!DNL Salesforce].

您指定记录的ID。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[！UICONTROL Connection]</td>
   <td> <p>有关连接 [!DNL Salesforce] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL记录类型]</td>
    <td>选择类型 [!DNL Salesforce] 记录您希望模块执行[action].read。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL记录字段]</td>
    <td>选择您希望模块读取的字段。 您必须至少选择一个字段。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL ID]</td>
    <td> <p>输入或映射唯一的 [!DNL Salesforce] 您希望模块读取的记录的ID。</p> <p>要获取ID，请打开 [!DNL Salesforce] 对象，并复制URL末尾的最后一个正斜杠(/)之后的文本。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除记录]

此操作模块删除对象中的现有记录。

您指定记录的ID。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL记录类型] </td> 
   <td> <p>选择类型 [!DNL Salesforce] 您希望模块删除的记录。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL ID]</td> 
   <td> <p>输入或映射唯一的 [!DNL Salesforce] 您希望模块删除的记录的ID。</p> <p>要获取ID，请打开 [!DNL Salesforce] 对象，并复制URL末尾的最后一个正斜杠(/)之后的文本。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL Salesforce] API。 这样，您就可以创建另一个无法实现的数据流自动化 [!DNL Salesforce] 模块。

模块返回以下内容：

* **[!UICONTROL 状态代码]** （数字）：这表示HTTP请求是成功还是失败。 这些是标准代码，您可以在互联网上查找。
* **[!UICONTROL 标题]** （对象）：与输出正文无关的响应/状态代码的更详细的上下文。 并非响应标头中显示的所有标头都是响应标头，因此某些标头可能对您没什么用。

  响应标头取决于您在配置模块时选择的HTTP请求。

* **[!UICONTROL 正文]** （对象）：根据在配置模块时选择的HTTP请求，您可能会接收回一些数据。 该数据，例如来自 [!UICONTROL GET] 请求，包含在此对象中。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>输入相对路径<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>有关可用端点的列表，请参阅 <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Salesforce REST API开发人员指南</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。例如， <code>{"Content-type":"application/json"}</code>. Workfront Fusion会为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：** 以下API调用返回中所有用户的列表。 [!DNL Salesforce] 帐户：
>
>* **URL**： `query`
>
>* **方法**： [!UICONTROL GET]
>
>* **查询字符串**：
>
>* **键**： `q`
>
>* **值**： `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>搜索匹配项可在模块的“输出”中找到，位于 **[!UICONTROL 捆绑] > [!UICONTROL 正文] > [!UICONTROL 记录]**.
>
>在我们的示例中，返回了6个用户：
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL 上载附件/文档]

此操作模块上传文件并将其附加到您指定的记录，或上传文档。

模块会返回附件或文档的ID以及任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上载类型]</td> 
   <td>选择您希望模块上载附件还是文档。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL ID]</td> 
   <td>输入或映射要向其上载附件的对象的ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹]</td> 
   <td>选择包含您希望模块上传的文件的文件夹。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL源文件]</td> 
   <td>从上一个模块中选择源文件，或映射源文件的名称和数据。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载附件/文档]

此操作模块从记录中下载文档或附件。

您可以指定记录的ID以及所需的下载类型。

模块会返回附件或文档的ID以及任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[！UICONTROL Connection]</td>
   <td> <p>有关连接 [!DNL Salesforce] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL下载类型]</td>
    <td> <p>指定要从Salesforce下载的文件类型。</p> 
     <ul> 
      <li>[！UICONTROL附件]</li> 
      <li>[！UICONTROL文档]</li> 
      <li>[！UICONTROL ContentDocument]（此文档已上载到中的库） [!DNL Saleforce CRM Content] 或 [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[！UICONTROL ID] / </p> <p>[！UICONTROL附件ID] / </p> <p>[！UICONTROL内容文档ID]</p> </td>
    <td> <p>输入或映射唯一的 [!DNL Salesforce] 您希望模块下载的记录的ID。</p> <p>要获取ID，请打开 [!DNL Salesforce] 对象，并复制URL末尾的最后一个正斜杠(/)之后的文本。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 更新记录]

此操作模块编辑对象中的记录。

利用模块，可选择模块中可用的对象字段。 这减少了设置模块时必须滚动的字段数。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL ID]</td> 
   <td>输入或映射要更新的记录ID。</td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL记录类型] </p> </td> 
   <td> <p>选择类型 [!DNL Salesforce] 记录您希望模块更新的内容。 根据在“记录类型”字段中选择的记录类型，字段变为可用。 这些字段基于 [!DNL Salesforce] API。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL选择要映射的字段]</td> 
   <td> <p>选择您希望模块在创建新记录时配置的字段。 必填字段位于列表顶部。 </p> <p>您选择的字段在此字段下打开。 您现在可以在这些字段中输入值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

#### [!UICONTROL 通过查询搜索]

此搜索模块查找对象中的记录 [!DNL Salesforce] 匹配您指定的搜索查询的规则。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜索类型]</td> 
   <td> <p>选择您希望模块执行的搜索类型：</p> 
    <ul> 
     <li> <p>[！UICONTROL Simple]</p> </li> 
     <li> <p>[！UICONTROL使用SOSL（Salesforce对象搜索语言）]</p> </li> 
     <li> <p>[！UICONTROL使用SOQL （Salesforce对象查询语言）]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL类型] </p> </td> 
   <td> <p>如果选择了“简单”搜索类型，则选择 [!DNL Salesforce] 您希望模块搜索的记录。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL查询] / [！UICONTROL SOSL查询] / [！UICONTROL SOQL查询]</td> 
   <td> <p>输入要作为搜索依据的查询。</p> <p>有关SOSL的详细信息，请参见 <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce对象搜索语言(SOSL)</a> 在 [!DNL Salesforce] 文档。</p> <p>有关SOQL的详细信息，请参阅 <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce对象查询语言(SOQL)</a> 在 [!DNL Salesforce] 文档。</p> <p>注意：请注意，参数的值 <code>RETURNING </code>会影响模块的输出。 如果您使用 <code>LIMIT</code>， [!DNL Fusion] 将忽略[！UICONTROL最大记录计数]字段中的设置。 如果不设置任何限制，Fusion将插入值[！UICONTROL LIMIT = Maximum count of records]。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大记录数]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索]

此操作模块可检索符合给定条件的所有记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>有关连接 [!DNL Salesforce] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接[!DNL  Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL类型]</td> 
   <td> <p>选择要搜索的对象类型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜索条件]</td> 
   <td>选择要搜索的字段、要在查询中使用的运算符以及要在字段中搜索的值。 您可以使用AND或OR连接查询。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td>选择要包含在模块输出中的字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL结果集]</td> 
   <td>选择您希望模块返回所有匹配记录，还是仅返回第一个匹配记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最大]</td> 
   <td>输入或映射您希望模块在每个方案执行周期中检索的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>
