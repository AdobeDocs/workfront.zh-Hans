---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Salesforce模块
description: 在Adobe Workfront Fusion场景中，您可以自动执行使用Salesforce的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2720'
ht-degree: 0%

---

# [!DNL Salesforce] 模块

在Adobe Workfront Fusion场景中，您可以自动执行使用 [!DNL Salesforce]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* 并非所有版本 [!DNL Salesforce] 具有API访问权限。 有关详细信息，请参阅 [!DNL Salesforce] 在 [!DNL Salesforce] 社区站点。
>* 有关从 [!DNL Salesforce] API，请参阅 [!DNL Salesforce] API文档。 您还可以检查 [!DNL Salesforce] 任何可能的服务中断的API。
>


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

使用 [!DNL Salesforce] 模块，您必须 [!DNL Salesforce] 帐户。

## 关于搜索 [!DNL Salesforce] 对象

在搜索对象时，您可以输入单个搜索词，或使用通配符和运算符创建更复杂的查询：

* 使用星号通配符(\*)替换零个或多个字符。 例如，搜索Ca\*会查找以Ca开头的项目
* 使用问号通配符(?) 替换单个字符。 例如，搜索Jo?n会查找具有John或Joan但不包含Jon的项目
* 使用引号运算符(&quot; &quot;)查找精确的短语匹配。 例如：&quot;星期一会议&quot;

有关搜索可能性的更多信息，请参阅 [!DNL Salesforce] 关于SOQL和SOSL的开发人员文档。

## [!DNL Salesforce] 模块及其字段

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

* [[!UICONTROL 监视记录]](#watch-for-records)
* [[!UICONTROL Watch出站消息]](#watch-outbound-messages)
* [[!UICONTROL 观看字段]](#watch-a-field)

#### [!UICONTROL 监视记录]

当创建或更新对象中的记录时，此触发器模块会执行一个方案。 模块会返回与记录或记录关联的所有标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>选择 [!DNL Salesforce] 记录您希望模块监视的内容。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录字段]</td> 
   <td>选择您希望模块监视的字段。 可用字段取决于记录类型。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录的最大计数]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p>确定您是否希望方案仅监视所选类型的新记录，还是仅监视所选类型的新记录以及对该类型记录的所有其他更改。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch出站消息]

此触发器模块会在某人发送消息时执行方案。 模块会返回与记录或记录关联的所有标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

此模块需要一些额外的设置：

1. 转到 [!DNL Salesforce] 设置页面。

   要访问设置页面，请找到并单击标有“[!UICONTROL 设置]” [!DNL Salesforce] 帐户。 从 [!DNL Salesforce] 设置页面，找到“[!UICONTROL 快速查找/搜索]”栏。 搜索“[!UICONTROL 工作流规则].&quot;

1. 单击 **[!UICONTROL 工作流规则]**.
1. 在 [!UICONTROL 工作流规则] 页面，单击 **[!UICONTROL 新规则]** 并选择规则要应用的对象类型(例如“[!UICONTROL 机会]“如果您正在监控Opportunity记录的更新)。
1. 单击 **[!UICONTROL 下一个]**.
1. 设置规则名称、评估标准和规则标准，然后单击 **[!UICONTROL 保存]** 和 **[!UICONTROL 下一个]**.

1. 单击 **[!UICONTROL 完成]**.
1. 在新创建的工作流规则中，单击 **[!UICONTROL 编辑]**..
1. 从 **[!UICONTROL 添加工作流操作]** 下拉列表中，选择 **[!UICONTROL 新建出站消息]**.

1. 指定要包含在新出站消息中的名称、描述、端点URL和字段，然后单击 **[!UICONTROL 保存]**.

   的 **[!UICONTROL 端点URL]** 字段包含 [!DNL Salesforce] [!UICONTROL 出站消息] in [!DNL Workfront Fusion].

1. 配置以 [!UICONTROL 出站消息] 事件。

1. 单击 **&lt;/>** 图标，并复制提供的URL。
1. 返回到 **[!UICONTROL 工作流规则]** 页面，找到新创建的规则，然后单击 **[!UICONTROL 激活]**.

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>选择要用于监视传出消息的WebHook。 要添加网页挂接，请单击 <strong>[!UICONTROL Add]</strong> 并输入webhook的名称和连接。</p> <p>有关连接 [!DNL Salesforce] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!UICONTROL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录类型] </td> 
   <td> <p>选择 [!DNL Salesforce] 记录您希望模块监视传出消息。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL字段]</td> 
   <td> <p>选择您希望模块监视的传出消息字段。 可用字段取决于记录类型。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL 观看字段]*

当字段在 [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录类型] </td> 
   <td> <p>选择包含您希望模块监视的字段的记录类型。 必须选择已启用[!UICONTROL字段历史记录]的记录类型 [!DNL Salesforce] 设置。 有关更多信息，请参阅 <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">字段历史记录跟踪</a> 在 [!DNL Salesforce] 文档。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL字段]</td> 
   <td> <p>选择您希望模块监视的字段以进行更改。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大字段数。</p> </td> 
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

利用模块，可选择模块中可用对象的哪些字段。 这会减少在设置模块时必须滚动的字段数。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL记录类型] </p> </td> 
   <td> <p>选择 [!DNL Salesforce] 记录您希望模块创建的内容。 字段根据在[!UICONTROL记录类型]字段中选择的记录类型变为可用。 这些字段基于 [!DNL Salesforce] API。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL选择要映射的字段]</td> 
   <td> <p>选择您希望模块在创建新记录时配置的字段。 必填字段位于列表顶部。 </p> <p>您选择打开的字段位于此字段下方。 您现在可以在这些字段中输入值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

此操作模块从 [!DNL Salesforce].

您指定记录的ID。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL连接]</td>
   <td> <p>有关连接 [!DNL Salesforce] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL记录类型]</td>
    <td>选择 [!DNL Salesforce] 记录您希望模块[action].read。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL记录字段]</td>
    <td>选择您希望模块读取的字段。 必须至少选择一个字段。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>输入或映射唯一 [!DNL Salesforce] 您希望模块读取的记录的ID。</p> <p>要获取ID，请打开 [!DNL Salesforce] 对象，并复制URL末尾的上一个正斜杠(/)之后的文本。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除记录]

此操作模块会删除对象中的现有记录。

您指定记录的ID。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录类型] </td> 
   <td> <p>选择 [!DNL Salesforce] 记录您希望删除模块。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>输入或映射唯一 [!DNL Salesforce] 您希望模块删除的记录的ID。</p> <p>要获取ID，请打开 [!DNL Salesforce] 对象，并复制URL末尾的上一个正斜杠(/)之后的文本。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL Salesforce] API。 这样，您就可以创建数据流自动化，而另一个数据流无法实现 [!DNL Salesforce] 模块。

该模块会返回以下内容：

* **[!UICONTROL 状态代码]** （数字）：这表示HTTP请求的成功或失败。 这些是可在互联网上查找的标准代码。
* **[!UICONTROL 标题]** （对象）：与输出正文无关的响应/状态代码的更详细上下文。 响应标头中显示的并非所有标头都是响应标头，因此某些标头可能对您没有用处。

   响应标头取决于您在配置模块时选择的HTTP请求。

* **[!UICONTROL 正文]** （对象）：根据您在配置模块时选择的HTTP请求，您可能会收到一些数据。 该数据，例如 [!UICONTROL GET] 请求包含在此对象中。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>输入相对于<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>有关可用端点的列表，请参阅 <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Salesforce REST API开发人员指南</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。例如， <code>{"Content-type":"application/json"}</code>. Workfront Fusion会为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。例如： <code>{"name":"something-urgent"}</code></p> </td> 
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

>[!INFO]
>
>**示例：** 以下API调用会返回 [!DNL Salesforce] 帐户：
>
>* **URL**: `query`
>
>* **方法**: [!UICONTROL GET]
>
>* **查询字符串**:
>
>* **键**: `q`
>
>* **值**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>搜索的匹配项可在模块的输出下找到 **[!UICONTROL 捆绑] > [!UICONTROL 正文] > [!UICONTROL 记录]**.
>
>在本例中，返回了6个用户：
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL 上载附件/文档]

此操作模块上传文件并将其附加到您指定的记录，或上传文档。

模块会返回附件或文档及任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上传类型]</td> 
   <td>选择是希望模块上传附件还是文档。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>输入或映射要将附件上传到的对象的ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹]</td> 
   <td>选择包含要上传模块的文件的文件夹。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源文件]</td> 
   <td>从前一个模块中选择源文件，或映射源文件的名称和数据。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载附件/文档]

此操作模块从记录下载文档或附件。

您可以指定记录的ID以及所需下载的类型。

模块会返回附件或文档及任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL连接]</td>
   <td> <p>有关连接 [!DNL Salesforce] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL下载类型]</td>
    <td> <p>指定要从Salesforce下载的文件类型。</p> 
     <ul> 
      <li>[!UICONTROL附件]</li> 
      <li>[!UICONTROL Document]</li> 
      <li>[!UICONTROL ContentDocument](这是已上传到 [!DNL Saleforce CRM Content] 或 [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL附件ID] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>输入或映射唯一 [!DNL Salesforce] 您希望模块下载的记录ID。</p> <p>要获取ID，请打开 [!DNL Salesforce] 对象，并复制URL末尾的上一个正斜杠(/)之后的文本。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 更新记录]

此操作模块编辑对象中的记录。

利用模块，可选择模块中可用对象的哪些字段。 这会减少在设置模块时必须滚动的字段数。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>输入或映射要更新的记录的ID。</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL记录类型] </p> </td> 
   <td> <p>选择 [!DNL Salesforce] 记录您希望模块更新。 根据在“记录类型”字段中选择的记录类型，字段变为可用。 这些字段基于 [!DNL Salesforce] API。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL选择要映射的字段]</td> 
   <td> <p>选择您希望模块在创建新记录时配置的字段。 必填字段位于列表顶部。 </p> <p>您选择打开的字段位于此字段下方。 您现在可以在这些字段中输入值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

#### [!UICONTROL 使用查询搜索]

此搜索模块在 [!DNL Salesforce] 与您指定的搜索查询匹配。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Salesforce] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索类型]</td> 
   <td> <p>选择您希望模块执行的搜索类型：</p> 
    <ul> 
     <li> <p>[!UICONTROL Simple]</p> </li> 
     <li> <p>[!UICONTROL使用SOSL（Salesforce对象搜索语言）]</p> </li> 
     <li> <p>[!UICONTROL使用SOQL（Salesforce对象查询语言）]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>如果您选择了简单搜索类型，请选择 [!DNL Salesforce] 记录您希望模块搜索的内容。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL查询] / [!UICONTROL SOSL查询] / [!UICONTROL SOQL查询]</td> 
   <td> <p>输入要搜索的查询。</p> <p>有关SOSL的详细信息，请参阅 <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce对象搜索语言(SOSL)</a> 在 [!DNL Salesforce] 文档。</p> <p>有关SOQL的更多信息，请参阅 <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce对象查询语言(SOQL)</a> 在 [!DNL Salesforce] 文档。</p> <p>注意：请注意，参数的值 <code>RETURNING </code>会影响模块的输出。 如果您使用 <code>LIMIT</code>, [!DNL Fusion] 将忽略[!UICONTROL记录的最大计数]字段中的设置。 如果未设置任何限制，Fusion将插入值[!UICONTROL LIMIT = Maximal count of records]。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录的最大计数]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
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
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关连接 [!DNL Salesforce] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接[!DNL  Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td> <p>选择要搜索的对象类型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索标准]</td> 
   <td>选择要搜索的字段、要在查询中使用的运算符，以及要在字段中搜索的值。 可以使用AND或OR连接查询。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出]</td> 
   <td>选择要包含在模块输出中的字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL结果集]</td> 
   <td>选择是希望模块返回“所有匹配记录”，还是仅返回“第一个匹配记录”。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal]</td> 
   <td>输入或映射您希望模块在每个方案执行周期期间检索的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>
