---
title: Adobe PDF服务
description: Adobe PDF服务
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: e0a5736b-dbdb-43c6-83ff-e88a5625a5bf
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3213'
ht-degree: 0%

---

# [!DNL Adobe PDF Services]

使用 [!DNL Adobe Workfront Fusion] [!DNL Adobe PDF Services]，则可以从PDF文件提取数据，或从提供的数据生成新的PDF文件。 此外，您还可以将各种文件类型转换为PDF，或将PDF转换为其他文件类型。 PDF服务还允许您合并、压缩或读取PDF文件的元数据，以及控制文件上的密码保护。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

有关用于PDF服务的API的信息，请参阅 [Adobe文档生成API](https://www.adobe.io/apis/documentcloud/dcsdk/doc-generation.html).

## 使用时的注意事项 [!DNL Adobe PDF Services]

* [您不需要 [!DNL Adobe] 帐户](#you-do-not-need-an-adobe-account)
* [[!DNL Workfront Fusion] 不存储文件](#workfront-fusion-does-not-store-your-files)

### 您不需要 [!DNL Adobe] 帐户

因为 [!DNL Workfront Fusion] 是 [!DNL Adobe] 产品包中，您不需要 [!DNL Adobe] 帐户来使用这些工具。 每个工具访问 [!DNL Adobe] PDF功能，而无需使用连接。

尽管 [!DNL Workfront Fusion] 不需要 [!DNL Adobe] 要使用PDF服务，模块需要连接。 此连接中未涉及凭据，您只提供连接本身的名称。

### [!DNL Workfront Fusion] 不存储文件

的 [!DNL Adobe PDF Services] 可以读取、转换或修改文件，但 [!DNL Adobe] nor [!DNL Workfront Fusion] 存储文件或数据。 这意味着：

* 您可以保持对文件的控制，包括其安全性
* 您无需拥有 [!UICONTROL Adobe] 存储或云存储帐户来使用PDF服务。

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

## [!DNL Adobe PDF Services] 模块及其字段

配置 [!DNL PDF Services], [!DNL Workfront Fusion] 显示下面列出的字段。 此外，还可能显示其他字段，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 生成文档]](#generate-document)
* [[!UICONTROL 提取文本/表]](#extract-text--table)
* [[!UICONTROL 合并PDF文件]](#combine-pdf-files)
* [[!UICONTROL 压缩PDF文件]](#compress-pdf-files)
* [[!UICONTROL 将文档转换为PDF文件]](#convert-document-to-pdf-file)
* [[!UICONTROL 将HTML转换为PDF文件]](#convert-html-to-pdf-file)
* [[!UICONTROL 将图像转换为PDF文件]](#convert-image-to-pdf-file)
* [[!UICONTROL 将PDF转换为文档]](#convert-pdf-to-document)
* [[!UICONTROL 将PDF转换为图像]](#convert-pdf-to-image)
* [[!UICONTROL 线性化PDF文件]](#linearize-a-pdf-file)
* [[!UICONTROL OCR(PDF文件)]](#ocr-for-pdf-file)
* [[!UICONTROL PDF页面操作]](#pdf-page-manipulation)
* [[!UICONTROL PDF文件属性]](#pdf-file-properties)
* [[!UICONTROL ProtectPDF文件]](#protect-pdf-file)
* [[!UICONTROL 删除对PDF文件的保护]](#remove-protection-of-a-pdf-file)

### [!UICONTROL 生成文档]

的 [!UICONTROL 生成文档] 模块是创建包含您选择的数据的PDF的一种有效方法。 您可以使用 [!DNL Microsoft Word] 模板，或者通过以JSON格式提供数据来实现。

有关 [!UICONTROL [!DNL Adobe PDF Services] 生成文档] 功能，请参阅 [文档生成概述](https://www.adobe.io/apis/documentcloud/dcsdk/docs.html) 在 [!DNL Adobe Document Services] 文档。

* [使用 [!UICONTROL 生成文档] 带有 [!DNL Microsoft Word] 模板](#use-the-generate-document-module-with-a-microsoft-word-template)
* [使用 [!UICONTROL 生成文档] 具有JSON的模块](#use-the-generate-document-module-with-json)

#### 使用 [!UICONTROL 生成文档] 带有 [!DNL Microsoft Word] 模板

<!--
>[!NOTE]
>
>For a discussion of Microsoft Word templates, see [Microsoft Word Template modules](../../workfront-fusion/apps-and-their-modules/microsoft-word-templates-modules.md). 
>
>You do not need to use Microsoft Word template modules to use a Microsoft Word template with the PDF Services Generate document module.
-->

使用 [!UICONTROL 生成文档] 带有 [!UICONTROL Microsoft Word] 模板时，必须先创建模板。 有关说明，请在 [!DNL Microsoft Office] 文档。

填写 [!UICONTROL 生成文档] 模块字段如下所示：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>此源文件是 [!DNL Microsoft Word ]模板，模块使用该模板生成新PDF。</p> <p>我们建议在 [!DNL Workfront] 对于 [!DNL Microsoft Word] 在中使用的模板 [!DNL Workfront Fusion]. 然后，您可以使用 [!DNL Workfront] &gt; [!UICONTROL下载文档]模块，以将相应的模板拉入您的方案中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出格式]</td> 
   <td> <p>选择所生成文档的格式。</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！用于合并的UICONTROL数据]</td> 
   <td> <p>对于模板中要替换为文本的每个值标记，请填写以下内容：</p> 
    <ul> 
     <li> <p>[!UICONTROL密钥]</p> <p>输入键。 在模板中，键是值标记中显示的文本。 例如，如果要在值标记中放置文本 <code>&#123;&#123;name&#125;&#125;</code>，输入 <code>name </code>键字段。</p> </li> 
     <li> <p>值类型</p> <p>选择值字段中的数据是值、对象还是对象数组。</p> </li> 
     <li> <p>[!UICONTROL值]</p> <p>输入或映射要在生成的文档中显示的文本以代替值标记。</p> </li> 
    </ul> <p> <img src="assets/generate-with-template-350x241.png" style="width: 350;height: 241;"> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### 使用 [!UICONTROL 生成文档] 具有JSON的模块

使用 [!UICONTROL 生成文档] 模块，请按如下方式填写字段：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出格式]</td> 
   <td> <p>选择所生成文档的格式。</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！用于合并的UICONTROL数据]</td> 
   <td> <p>要在此模块中使用JSON，必须在此字段上启用映射。</p> <p>输入或映射JSON以从中生成文档。 </p> <p>您可以直接在此字段中键入JSON，或从JSON模块映射JSON输出。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 提取文本/表]

此操作模块允许您从PDF文件提取数据。 该模块输出单个文本元素，如段落或表格单个单元格中的文本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td>从前一个模块中选择源文件，或映射源文件的名称和数据。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL元素，应作为JSON提取]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Text]</p> </li> 
     <li> <p>[!UICONTROL表]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL提取边界框？]</td> 
   <td>启用此选项可提取有关文本定界框的数据。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL是否包含输出的样式信息？]</td> 
   <td>启用此选项可向输出JSON添加样式信息。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 合并PDF文件]

此操作模块会获取多个PDF文件，并将它们合并为单个PDF文件。 例如，此模块可以将 [!UICONTROL Workfront] 项目完成后整合到单个PDF中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文档]</td> 
   <td> <p>您可以使用聚合模块收集文档以组合到PDF中，也可以手动添加文档。 </p> <p>我们建议使用[!UICONTROL Array Aggregator]模块来聚合来自前一模块的输出。 通过使用聚合器，您无需知道要合并的文件的名称、位置或数量。 因此，使用聚合器比手动输入要组合的文档要灵活得多，并且可缩放得多。</p> <p>要将[!UICONTROL合并PDF]文件模块与聚合器一起使用，必须在[!UICONTROL Documents]字段上启用映射。 </p> <p>在此示例中， [!UICONTROL读取相关记录]模块标识与项目关联的文档，而[!UICONTROL下载文档]模块则下载每个文档。 所有PDF都会聚合到一个数组中，该数组会传递到[!UICONTROL合并PDF]文件模块中。</p> <p> <img src="assets/combine-example-350x104.png" style="width: 350;height: 104;"> </p> <p>您还可以手动输入文档。</p> <p>对于要包含在组合PDF中的每个文档：</p> 
    <ol> 
     <li value="1"> <p>单击[!UICONTROL添加文档]</p> </li> 
     <li value="2"> <p>在[!UICONTROL源文件]字段中，选择输出要包含的文档的模块，或映射源文件的名称和数据。 </p> </li> 
     <li value="3"> <p>（可选）如果您只想包含源文件中的某些页面，则对于要添加的每个页面范围，单击 <strong>[!UICONTROL添加项目]</strong> 在[!UICONTROL页面]字段中，输入要包含的页面范围的首页和最后一页，然后单击 <strong>[!UICONTROL Add]</strong>. 您可以从单个文档中包含多个页面范围。</p> </li> 
     <li value="4"> <p>单击 <strong>[!UICONTROL Add]</strong>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 压缩PDF文件]

此操作模块会获取一个PDF文件并对其进行压缩。 这对于节省带宽或内存非常有用。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>源文件必须为PDF格式。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL压缩级别]</td> 
   <td>选择要使用的压缩级别。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 将文档转换为PDF文件]

此工具可将文档转换为PDF文件。 源文件必须是以下文档格式之一：

* 文档
* XLS
* PPT
* TXT
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>源文件必须采用以下格式之一：</p> 
    <ul> 
     <li> <p>文档</p> </li> 
     <li> <p>XLS</p> </li> 
     <li> <p>PPT</p> </li> 
     <li> <p>TXT</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL语言]</td> 
   <td> <p>选择源文档的默认语言。 如果源文件中不包含字体，则允许模块选择适当的字体。</p> <p>从以下语言中进行选择：</p> 
    <ul> 
     <li> <p>en-US（默认）：英语（美利坚合众国）</p> </li> 
     <li> <p>ca-ES:加泰罗尼亚语（西班牙）</p> </li> 
     <li> <p>cs-CZ:捷克语（捷克共和国）</p> </li> 
     <li> <p>da-DK:丹麦语（丹麦）</p> </li> 
     <li> <p>去除：德语（德国）</p> </li> 
     <li> <p>AE:英语（阿拉伯联合酋长国）</p> </li> 
     <li> <p>en-GB:英语（英国）</p> </li> 
     <li> <p>终了：英语（以色列）</p> </li> 
     <li> <p>美国：英语（美利坚合众国）</p> </li> 
     <li> <p>es-ES:西班牙语（西班牙）</p> </li> 
     <li> <p>es-MX:西班牙语（墨西哥）</p> </li> 
     <li> <p>eu-ES:巴斯克语（西班牙）</p> </li> 
     <li> <p>Fi-FI:芬兰语（芬兰）</p> </li> 
     <li> <p>fr-CA:法语（加拿大）</p> </li> 
     <li> <p>fr-FR:法语（法国）</p> </li> 
     <li> <p>fr-MA:法语（摩洛哥）</p> </li> 
     <li> <p>hr-HR:克罗地亚语（克罗地亚）</p> </li> 
     <li> <p>胡虎：匈牙利语（匈牙利）</p> </li> 
     <li> <p>it-IT:意大利语（意大利）</p> </li> 
     <li> <p>ja-JP:日语（日本）</p> </li> 
     <li> <p>kr-KR:朝鲜语（韩国）</p> </li> 
     <li> <p>nb-NO:挪威博克马尔语（挪威）</p> </li> 
     <li> <p>nl-NL:荷兰语（荷兰）</p> </li> 
     <li> <p>PL:波兰语（波兰）</p> </li> 
     <li> <p>pt-BR:葡萄牙语（巴西）</p> </li> 
     <li> <p>pt-PT:葡萄牙语（葡萄牙）</p> </li> 
     <li> <p>ro-RO:罗马尼亚语（罗马尼亚）</p> </li> 
     <li> <p>ru-RU:俄语（俄罗斯）</p> </li> 
     <li> <p>sk-SK:斯洛伐克语（斯洛伐克）</p> </li> 
     <li> <p>sl-SI:斯洛文尼亚（斯洛文尼亚）</p> </li> 
     <li> <p>sv-SE:瑞典语（瑞典）</p> </li> 
     <li> <p>tr-TR:土耳其语（土耳其）</p> </li> 
     <li> <p>uk-UA:乌克兰语（乌克兰）</p> </li> 
     <li> <p>zh-CN:中文（中国大陆）</p> </li> 
     <li> <p>zh-TW:中文（台湾）</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 将HTML转换为PDF文件]

此工具可将HTML文件转换为PDF文件。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>重要信息：源文件必须为HTML或ZIP格式。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON]</td> 
   <td> <p>如果您的HTML引用JavaScript变量，则可以在此处包含这些变量。 </p> <p>对于每个变量，单击 <strong>[!UICONTROL添加项目]</strong> 和包含变量的键和值。</p> <p>注释:   
     <ul> 
      <li> <p>从ZIP文件创建PDF时，源宣传资料必须包含脚本元素，例如： <code> &lt;script src='./json.js' type='text/javascript'&gt;&lt;/script&gt;</code> </p> </li> 
      <li> <p>从URL创建PDF时，此JSON对象的内容会在页面呈现之前插入到浏览器VM中。 </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include header and footer]</td> 
   <td> <p>启用此选项可为PDF文档创建页眉和页脚。</p> 
    <ul> 
     <li> <p>标题包括日期和文档标题。</p> </li> 
     <li> <p>页脚包括文件名和页码。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL页面宽度]</td> 
   <td>输入纸的宽度（以英寸为单位）。 模块使用此信息在创建的PDF文件中设置页面格式。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL页面高度]</td> 
   <td>输入纸张的高度（以英寸为单位）。 模块使用此信息在创建的PDF文件中设置页面格式。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 将图像转换为PDF文件]

此工具可将图像转换为PDF文件。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和图像文件。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 将PDF转换为文档]

此工具可将PDF文件转换为文档。 您可以为输出文件选择以下格式之一。

* 文档
* DOCX
* PPTX
* XLSX
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>源文件必须为PDF格式。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出文件格式]</td> 
   <td> <p>选择要将文件输出为的格式：</p> 
    <ul> 
     <li> <p>文档</p> </li> 
     <li> <p>DOCX</p> </li> 
     <li> <p>PPTX</p> </li> 
     <li> <p>XLSX</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 将PDF转换为图像]

此工具可将PDF转换为PNG或JPEG格式的图像，然后以ZIP格式输出。 该PDF将转换为每页一个图像，每个图像以页码结束。 然后，图像文件将合并为ZIP文件。

例如，名为“TestFile”的文件（包含8页）将生成8个图像，名为“TestFile_1”（通过“TestFile_8”）。 模块的输出是一个包含8张图像的ZIP文件。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>源文件必须为PDF格式。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出文件格式]</td> 
   <td> <p>选择要将文件输出为的格式：</p> 
    <ul> 
     <li>PNG</li> 
     <li>JPEG</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 线性化PDF文件]

此工具可线性化PDF文档以创建Web优化PDF文档。 线性化的PDF文档可以逐页查看，而无需下载整个文档。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL OCR(PDF文件)]

此工具对文件执行光学字符识别(OCR)并生成PDF。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL OCR类型]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL修改的原始图像]类型可确保文本可搜索和选择，但在清除过程中（例如，描述原始图像）会修改原始图像，然后再将不可见的文本层置于其上方。 此类型会删除不需要的工件，并在某些情况下可能会生成更易读的文档。 </p> </li> 
     <li> <p>[!UICONTROL未更改的原始图像]类型还会在原始图像上叠加一个可搜索的文本层，但在这种情况下，原始图像将保持不变。 此类型对原始图像产生最大保真度。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL语言]</td> 
   <td>选择此文档的语言。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF页面操作]

利用此模块，可有选择地旋转或删除PDF文档中的页面。 例如，您可以将纵向视图更改为横向视图，或从PDF文档中删除某些页面。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> <p>选择要对文件执行的操作。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Delete]</b> </p> <p>选择此选项可从文档中删除页面。</p> </li> 
     <li> <p><b>[!UICONTROL旋转]</b> </p> <p>选择此选项可旋转页面，然后输入要相对于文档页面的起始方向旋转的角度（顺时针角度）。</p> <p>要从纵向旋转到横向或反之，请将页面旋转90度或270度。</p> <p>如果页面颠倒过来，则将其旋转180度。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL页面]</td> 
   <td> <p>对于要删除的每个页面范围，单击 <strong>[!UICONTROL Add]</strong> 然后输入页面范围的首页和最后一页。 </p> <p>注释:   
     <ul> 
      <li> <p>您可以使用负数从文档末尾开始计数。 文档的最后一页是–1，最后一页的第二页是–2，依此类推。</p> </li> 
      <li> <p>要删除单个页面，请将相同的页码设置为范围的开始和结束。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间处理的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF文件属性]

此工具提取有关文档的基本信息，例如：

* 页面计数
* PDF版本
* 文件是否已加密
* 文件是否已线性化
* 文件是否包含嵌入的文件

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL ProtectPDF文件]

此工具使用用户或所有者密码保护PDF文档。 它还对某些功能(如在PDF文档中打印、编辑和复制)设置了限制。 选择要加密的内容类型和加密算法。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>源文件必须为PDF格式。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL密码保护类型]</td> 
   <td> <p>启用此选项可使用密码加密输入PDF文档。 如果启用此选项，则必须指定并输入以下任一项或两个项的值： </p> 
    <ul> 
     <li> <p>[!UICONTROL userPassword]</p> </li> 
     <li> <p>[!UICONTROL ownerPassword] </p> </li> 
    </ul> <p>每个密码的长度最多为128个字符。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL加密算法]</td> 
   <td> <p>选择加密算法。 </p> 
    <ul> 
     <li> <p>[!UICONTROL AES-128加密]</p> <p>密码仅支持LATIN-I字符。 </p> </li> 
     <li> <p>[!UICONTROL AES-256加密]</p> <p>密码支持Unicode字符集</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL要加密的内容]</td> 
   <td> <p>选择要加密的内容类型。</p> 
    <ul> 
     <li> <p>[!UICONTROL All content]</p> </li> 
     <li> <p>[!UICONTROL除元数据外的所有内容]</p> </li> 
     <li> <p>[!UICONTROL仅嵌入数据] </p> </li> 
    </ul> <p>选择“[!UICONTROL仅嵌入数据]”会将任何提供的访问权限呈现为无效。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL权限]</td> 
   <td> <p>选择要包含的任何权限，以允许打印、编辑或内容复制。</p> <p>仅当在[!UICONTROL Password Protection Type]字段中设置了[!UICONTROL ownerPassword]时，才使用权限设置。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 删除对PDF文件的保护]

此工具可从PDF文档中删除安全（密码保护）。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>选择要用于此模块的连接。</p> <p>您不需要 [!DNL Adobe] 帐户创建PDF服务连接。 有关更多信息，请参阅 <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">您不需要 [!DNL Adobe] 帐户</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>源文件必须为PDF格式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL密码]</td> 
   <td>输入当前保护文件的密码。</td> 
  </tr> 
 </tbody> 
</table>
