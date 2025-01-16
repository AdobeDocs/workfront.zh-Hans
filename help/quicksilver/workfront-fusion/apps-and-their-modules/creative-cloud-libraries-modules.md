---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Creative Cloud库模块
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 0%

---

# Adobe Creative Cloud库模块

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [Adobe Creative Cloud Libraries模块](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/creative-cloud-libraries-modules.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

使用[!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries]模块，您可以在创建或更新元素或库时启动方案。 您还可以上传、检索、存档或列出元素，或调用[!DNL Adobe Creative Cloud Libraries] API。

如果需要有关创建方案的说明，请参阅[创建方案](../../workfront-fusion/scenarios/create-a-scenario.md)。

有关模块的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模块。

>[!IMPORTANT]
>
>当前无法在Creative Cloud Libraries连接器中创建连接。 现有连接按预期工作。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
      <td>
        <p>[！UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
      <td>
        <p>[！UICONTROL计划]，[！UICONTROL工作]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td>
      <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">产品</td>
      <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td>
    </tr>
  </tbody>
</table>


要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先决条件

要使用[!DNL Adobe Creative Cloud Libraries]模块，您必须具有[!UICONTROL Adobe Creative Cloud]帐户。

## Adobe Creative Cloud Libraries API信息

Adobe Creative Cloud Libraries连接器使用以下对象：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基本URL</td> 
   <td>https://cc-libraries.adobe.io/api/v1</td> 
  </tr>
  <tr> 
   <td role="rowheader">API标记</td> 
   <td>v1.1.7</td> 
  </tr>
 </tbody> 
 </table>

## [!UICONTROL Adobe Creative Cloud Libraries]模块及其字段

配置[!UICONTROL Adobe Creative Cloud Libraries]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Adobe Creative Cloud Libraries]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)


* [元素](#elements)

* [库](#libraries)

* [其他](#other)


### 元素

* [[!UICONTROL 存档元素]](#archive-an-element)

* [[!UICONTROL 获取元素]](#get-an-element)

* [[!UICONTROL 列出元素]](#list-elements)

* [[!UICONTROL 上传元素]](#upload-an-element)

* [！UICONTROL [查看库中的新元素]](#watch-new-element-in-library)

* [[!UICONTROL 观看更新的元素]](#watch-updated-elements)


#### [!UICONTROL 存档元素]

此操作模块可存档库中的元素。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>选择现有Creative Cloud Libraries连接。 当前无法在Creative Cloud Libraries连接器中创建连接。 现有连接按预期工作。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL库ID]</td>
      <td >选择包含要存档的元素的库。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[！UICONTROL元素ID]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">选择要存档的元素。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 获取元素]

此操作模块从库中返回单个元素。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>选择现有Creative Cloud Libraries连接。 当前无法在Creative Cloud Libraries连接器中创建连接。 现有连接按预期工作。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL库ID]</td>
      <td >选择包含要检索的元素的库。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL元素ID]</td>
      <td>输入或映射要检索的元素的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL选择器]</td>
      <td>
        <p>选择模块返回的信息类型。 </p>
        <ul>
          <li>
            <p><b>[！UICONTROL默认值]</b>
            </p>
            <p>基础数据</p>
          </li>
          <li>
            <p><b>[！UICONTROL详细信息]</b>
            </p>
            <p>所有可用数据</p>
          </li>
          <li>
            <p><b>[！UICONTROL呈现]</b>
            </p>
            <p>与库元素关联的资源平面化列表</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出元素]

此操作模块可检索库中的元素列表。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>选择现有Creative Cloud Libraries连接。 当前无法在Creative Cloud Libraries连接器中创建连接。 现有连接按预期工作。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL库ID]</td>
      <td >选择要从中列出元素的库。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Order by]</td>
      <td>选择是要按名称对结果排序，还是要按上次修改元素的日期对结果排序。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL类型]</td>
      <td >输入MIME类型以将结果限制为使用指定MIME类型标识的元素。 示例： <code>string</code>。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL选择器]</td>
      <td>
        <p>选择模块返回的信息类型。 </p>
        <ul>
          <li>
            <p><b>[！UICONTROL默认值]</b>
            </p>
            <p>基础数据</p>
          </li>
          <li>
            <p><b>[！UICONTROL详细信息]</b>
            </p>
            <p>所有可用数据</p>
          </li>
          <li>
            <p><b>[！UICONTROL呈现]</b>
            </p>
            <p>与库元素关联的资源平面化列表</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td>
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
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>选择现有Creative Cloud Libraries连接。 当前无法在Creative Cloud Libraries连接器中创建连接。 现有连接按预期工作。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL库ID]</td>
      <td >选择要从中列出元素的库。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL调用模式]</td>
      <td>
        <p>选择要用于调用此请求进程的处理模式。</p>
        <ul>
          <li>
            <p><b>[！UICONTROL同步]</b>
            </p>
            <p>API调用会同步处理。 处理完成后会发送响应（除非调用超时）。</p>
          </li>
          <li>
            <p><b>[！UICONTROL异步]</b>
            </p>
            <p>将立即返回异步监视器响应，并异步进行请求处理。 调用负责轮询端点，直到完成。</p>
          </li>
          <li>
            <p><b>[！UICONTROL sync，async]</b>（默认）</p>
            <p>尝试同步处理请求。 当处理时间超过5000 ms时，将返回异步监视器响应。 应轮询监视器URL，直到请求完成。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL类型文件]</td>
      <td >输入或映射上载文件的MIME类型。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Source File]</td>
      <td>
        <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 观看库中的新元素]

将元素添加到库后，此触发器模块会启动一个方案。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>选择现有Creative Cloud Libraries连接。 当前无法在Creative Cloud Libraries连接器中创建连接。 现有连接按预期工作。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL库ID]</td>
      <td >选择要监视更新元素的库。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL 观看更新的元素]

此触发器模块会在更新库中的元素时启动方案。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>选择现有Creative Cloud Libraries连接。 当前无法在Creative Cloud Libraries连接器中创建连接。 现有连接按预期工作。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL库ID]</td>
      <td >选择要监视新元素的库。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td>
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
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>选择现有Creative Cloud Libraries连接。 当前无法在Creative Cloud Libraries连接器中创建连接。 现有连接按预期工作。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td>
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
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>选择现有Creative Cloud Libraries连接。 当前无法在Creative Cloud Libraries连接器中创建连接。 现有连接按预期工作。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td>
    </tr>
  </tbody>
</table>

### 其他

#### [!UICONTROL 进行API调用]

此模块对[!DNL Adobe Creative Cloud Libraries] API进行自定义API调用。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td> <p>有关将Adobe Creative Cloud帐户连接到Workfront Fusion的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe Workfront Fusion的连接 — 基本说明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL URL]</td>
      <td>
        <p>输入相对于<code>https://cc-libraries.adobe.io/api</code>的路径。</p>
    <p>例如<code>/v1/libraries</code>。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL API版本]</td>
      <td>
        <p>选择要连接的[!DNL Adobe Analytics] API的版本。</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[！UICONTROL方法]</td>
      <td> <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP请求方法。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以标准JSON对象的形式添加请求的标头。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion会为您添加授权标头。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL查询字符串]</td>
      <td>
        <p>以标准JSON对象的形式添加API调用的查询。</p>
        <p>例如： <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Body]</td>
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>在JSON中使用条件语句（如<code>if</code>）时，请将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[！UICONTROL上传临时文档]</td>
      <td>
      <p>如果要上载临时文档，请输入要上载文档的源文件。</p>
      <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p>
    </td>
    </tr>

</tbody>
</table>
