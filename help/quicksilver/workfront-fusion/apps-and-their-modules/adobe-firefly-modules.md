---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Firefly模块
description: 在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用 [!DNL Adobe Firefly]，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: c932f869de9ff842a7bbb809bc60ec1d53350b51
workflow-type: tm+mt
source-wordcount: '1215'
ht-degree: 0%

---

# [!DNL Adobe Firefly] 模块

在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用 [!DNL Adobe Firefly]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [创建方案](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

在使用 [!DNL Adobe Firefly] 连接器时，必须确保满足以下先决条件：

* 您必须拥有有效的 [!DNL Adobe Firefly] 帐户。

## 创建与的连接 [!DNL Adobe Firefly]

要为创建连接，请执行以下操作 [!DNL Adobe Firefly] 模块：

1. 单击 **[!UICONTROL 添加]** ，位于“Connection（连接）”框旁。

1. 填写以下字段：

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[！UICONTROL连接名称]</td>
        <td>
          <p>输入此连接的名称。</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL环境]</td>
        <td>选择您要连接到生产环境还是非生产环境。</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL类型]</td>
        <td>选择您是要连接到服务帐户还是个人帐户。</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL客户端ID]</td>
        <td>输入您的[！UICONTROLAdobe] [！UICONTROL客户端ID]。 可在[！UICONTROL Credentials]的 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL客户端密钥]</td>
        <td>输入您的 [!DNL Adobe] [！UICONTROL客户端密钥]。 可在[！UICONTROL Credentials]的 [!DNL Adobe Developer Console]</td>
        </tr>
      </tbody>
    </table>

1. 单击 **[!UICONTROL 继续]** 以保存连接并返回到模块。

## [!DNL Adobe Firefly] 模块及其字段

配置时 [!DNL Adobe Firefly] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Adobe Firefly] 字段可能会显示，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 进行自定义API调用

此操作模块对FireflyAPI进行自定义调用。

有关特定的可用API，请参阅 [ADOBE FIREFLYAPI](https://developer.adobe.com/firefly-services/docs/firefly-api/) 请参阅Adobe Developer文档。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Firefly]，请参见 <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >创建与的连接 [!DNL Adobe Firefly]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL URL]</td>
      <td>
        <p>输入相对路径 <code>https://firefly-api-enterprise-stage.adobe.io/</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以标准JSON对象的形式添加请求的标头。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自动添加授权标头。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Body]</td>
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### 展开图像

此操作模块可展开图像，可以选择从提供的提示中使用内容。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>有关创建与的连接 [!DNL Adobe Campaign]，请参见 <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >创建与的连接 [!DNL Adobe Firefly]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Prompt]</td> 
   <td>输入或映射要用于展开图像的内容的提示。 如果未提供任何提示，则图像将展开，并且内容与原始图像匹配。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL扩展图像格式]</td> 
   <td>选择将保存扩展图像的文件格式。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td>  <p>从上一个模块中选择一个源文件，或映射源文件的图像文件名和图像文件（数据）。</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL大小]</td> 
   <td>选择希望扩展图像的大小。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Seed]</td> 
   <td>输入或映射整数。 您可以在另一个扩展图像模块中使用此相同的种子，以生成具有不同样式的相似图像。 </td> 
  </tr> 
 </tbody> 
</table>

## 填充图像

此操作模块会填充图像的蒙版区域，可以选择使用您提供的提示中的内容。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>有关创建与的连接 [!DNL Adobe Campaign]，请参见 <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >创建与的连接 [!DNL Adobe Firefly]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Prompt]</td> 
   <td>输入或映射要用于填充图像的内容的提示。 如果未提供任何提示，则图像将填充与原始图像匹配的内容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL填充图像格式]</td> 
   <td>选择将保存已填充图像的文件格式。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL图像]</td> 
   <td>  <p> 单击 <b>添加图像</b>. 从上一个模块中选择一个源文件，或映射源文件的图像文件名和图像数据。</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL蒙版]</td> 
   <td>  <p> 单击 <b>添加蒙版</b>. 从上一个模块中选择一个源文件，或映射源文件的“蒙版”文件名和“蒙版”数据。 蒙版文件表示将使用生成的内容填充的自定义蒙版。</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL大小]</td> 
   <td>选择希望填充图像的大小。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Seed]</td> 
   <td>输入或映射整数。 您可以在另一个扩展图像模块中使用此相同的种子，以生成具有不同样式的相似图像。 </td> 
  </tr> 
 </tbody> 
</table>

## 生成图像

该操作模块会根据您提供的提示生成和图像。 您还可以提供一个可选的参考图像，生成的图像将与参考图像的样式匹配。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>有关创建与的连接 [!DNL Adobe Campaign]，请参见 <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >创建与的连接 [!DNL Adobe Firefly]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Prompt]</td> 
   <td>为要创建的图像输入或映射提示。 在提示中显示更多详细信息，将允许您更好地控制映像中显示的内容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL生成的图像格式]</td> 
   <td>选择将保存扩展图像的文件格式。 如果选择default，则在未提供参考图像的情况下，文件格式将JPEG。 如果提供了参考图像，则生成的图像的文件格式将与参考图像相同。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td>  <p>从上一个模块中选择一个源文件，或映射源文件的“参考图像文件名”和“参考图像文件（数据）”。 将创建生成的图像以匹配参考图像的样式。</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL预设]</td> 
   <td>如果要使用预设样式，请单击“添加项目”，然后输入或映射要使用的样式。<p>有关预设样式的列表，请参阅 <a href="https://developer.adobe.com/firefly-services/docs/firefly-api/guides/concepts/styles/" >图像模型样式</a> 在Adobe开发人员文档中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL负提示]</td> 
   <td>在生成的内容中输入或映射要避免使用的单词。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL内容类]</td> 
   <td>选择您希望生成的图像更类似于照片，还是更类似于创建的图片。 <ul><li><b>照片</b><p>输入“光圈”、“快门速度”（以秒为单位）和“视场”（以毫米为单位）的值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Seed]</td> 
   <td>输入或映射整数。 您可以在另一个扩展图像模块中使用此相同的种子，以生成具有不同样式的相似图像。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL大小]</td> 
   <td>选择希望生成的图像的大小。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL强度]</td> 
   <td>输入或映射一个整数，该整数表示生成的图像与预设样式或参考图像的样式匹配的强度。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL视觉强度]</td> 
   <td>输入或映射一个整数，该整数表示照片现有视觉特征的整体强度。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL区域设置]</td> 
   <td>如果提供了区域设置，则模块会生成与指定区域设置更相关的内容。 <p>必须以ISO 639-1语言代码和ISO 3166-1区域提供区域设置。</p><p> 示例： <code>en-US</code></p></td> 
  </tr> 
 </tbody> 
</table>


