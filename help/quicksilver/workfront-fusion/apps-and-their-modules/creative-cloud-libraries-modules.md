---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Creative Cloud库模块
description: 使用 [!DNL Adobe Workfront Fusion Adobe Creative Cloud] 库模块中，您可以在创建或更新元素或库时启动方案。 您还可以上传、检索、存档或列表元素，或者调用 [!DNL Adobe Creative Cloud Libraries] API。
author: Becky
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1193'
ht-degree: 0%

---

# Adobe Creative Cloud库模块

使用 [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries] 模块中，您可以在创建或更新元素或库时启动方案。 您还可以上传、检索、存档或列表元素，或者调用 [!DNL Adobe Creative Cloud Libraries] API。

如果您需要有关创建方案的说明，请参阅 [创建方案](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
      <td>
        <p>[!UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
      <td>
        <p>[!UICONTROL Plan]、[!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成）</p>
      </td>
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

使用 [!DNL Adobe Creative Cloud Libraries] 模块，您必须具有 [!UICONTROL Adobe Creative Cloud] 帐户。

## [!UICONTROL Adobe Creative Cloud库] 模块及其字段

配置 [!UICONTROL Adobe Creative Cloud库] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Adobe Creative Cloud Libraries] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [元素](#elements)

* [库](#libraries)

* [其他](#other)


### 元素

* [[!UICONTROL 存档元素]](#archive-an-element)

* [[!UICONTROL 获取元素]](#get-an-element)

* [[!UICONTROL 列表元素]](#list-elements)

* [[!UICONTROL 上传元素]](#upload-an-element)

* [!UICONTROL [在库中观看新元素]](#watch-new-element-in-library)

* [[!UICONTROL 观看更新的元素]](#watch-updated-elements)


#### [!UICONTROL 存档元素]

此操作模块会存档库中的元素。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td>有关连接 [!DNL Adobe Creative Cloud] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL库ID]</td>
      <td >选择包含要存档的元素的库。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL元素ID]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">选择要存档的元素。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 获取元素]

此操作模块会从库中返回单个元素。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td>有关连接 [!DNL Adobe Creative Cloud] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL库ID]</td>
      <td >选择包含要检索的元素的库。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL元素ID]</td>
      <td>输入或映射要检索的元素的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL选择器]</td>
      <td>
        <p>选择模块返回的信息类型。 </p>
        <ul>
          <li>
            <p><b>[!UICONTROL默认]</b>
            </p>
            <p>基本数据</p>
          </li>
          <li>
            <p><b>[!UICONTROL详细信息]</b>
            </p>
            <p>所有可用数据</p>
          </li>
          <li>
            <p><b>[!UICONTROL表示法]</b>
            </p>
            <p>与库元素关联的资产的扁平化列表</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列表元素]

此操作模块可检索库中的元素列表。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td>有关连接 [!DNL Adobe Creative Cloud] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL库ID]</td>
      <td >选择要从中列出元素的库。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by]</td>
      <td>选择是要按名称还是按元素的上次修改日期对结果进行排序。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type]</td>
      <td >输入MIME类型，以将结果限制为使用指定MIME类型标识的元素。 示例: <code>string</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL选择器]</td>
      <td>
        <p>选择模块返回的信息类型。 </p>
        <ul>
          <li>
            <p><b>[!UICONTROL默认]</b>
            </p>
            <p>基本数据</p>
          </li>
          <li>
            <p><b>[!UICONTROL详细信息]</b>
            </p>
            <p>所有可用数据</p>
          </li>
          <li>
            <p><b>[!UICONTROL表示法]</b>
            </p>
            <p>与库元素关联的资产的扁平化列表</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 上传元素]

此操作模块会将小文件资产上传到现有库。 最大文件大小为1 GB。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td>有关连接 [!DNL Adobe Creative Cloud] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL库ID]</td>
      <td >选择要从中列出元素的库。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL调用模式]</td>
      <td>
        <p>选择处理模式，以通过调用此请求进程。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL同步]</b>
            </p>
            <p>API调用将同步处理。 处理完成时（除非调用超时）会发送响应。</p>
          </li>
          <li>
            <p><b>[!UICONTROL异步]</b>
            </p>
            <p>将立即返回异步监视器响应，并异步进行请求处理。 调用负责轮询端点直到完成。</p>
          </li>
          <li>
            <p><b>[!UICONTROL同步，异步]</b> （默认）</p>
            <p>尝试同步处理请求。 当处理超过5000毫秒时，将返回异步监视器响应。 在请求完成之前，应对监视器URL进行轮询。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL类型文件]</td>
      <td >输入或映射已上传文件的MIME类型。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL源文件]</td>
      <td>
        <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 在库中观看新元素]

当将元素添加到库时，此触发器模块会启动一个方案。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td>有关连接 [!DNL Adobe Creative Cloud] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL库ID]</td>
      <td >选择要监视已更新元素的库。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL 观看更新的元素]

此触发器模块会在库中的元素更新时启动方案。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td>有关连接 [!DNL Adobe Creative Cloud] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL库ID]</td>
      <td >选择要监视新元素的库。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td>
    </tr>
  </tbody>
</table>

### 库

* [[!UICONTROL 观看新库]](#watch-new-libraries)

* [[!UICONTROL 观看更新的库]](#watch-updated-libraries)


#### [!UICONTROL 观看新库]

此触发器模块会在创建新库时启动方案。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td>有关连接 [!DNL Adobe Creative Cloud] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 观看更新的库]

此触发器模块会在更新现有库时启动方案。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td>有关连接 [!DNL Adobe Creative Cloud] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td>
    </tr>
  </tbody>
</table>

### 其他

#### [!UICONTROL 进行API调用]

此模块对 [!DNL Adobe Creative Cloud Libraries] API。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td> <p>有关将Adobe Creative Cloud帐户连接到Workfront Fusion的说明，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe Workfront Fusion的连接 — 基本说明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>输入相对于 <code>https://cc-libraries.adobe.io/api</code>.</p>
    <p>例如 <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL API版本]</td>
      <td>
        <p>选择 [!DNL Adobe Analytics] 要连接到的API。</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL方法]</td>
      <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL标头]</td>
      <td>
        <p>以标准JSON对象的形式添加请求的标头。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion会为您添加授权标头。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL查询字符串]</td>
      <td>
        <p>以标准JSON对象的形式添加API调用的查询。</p>
        <p>例如： <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL主体]</td>
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:  <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL上传临时文档]</td>
      <td>
      <p>如果要上载临时文档，请输入要上载的文档的源文件。</p>
      <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p>
    </td>
    </tr>

</tbody>
</table>
