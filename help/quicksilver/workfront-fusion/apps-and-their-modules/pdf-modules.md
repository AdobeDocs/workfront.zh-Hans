---
title: Adobe PDF服务
description: Adobe PDF服务
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: e0a5736b-dbdb-43c6-83ff-e88a5625a5bf
source-git-commit: b43ea012d7c649c94011f72f010ae24895e6ef4b
workflow-type: tm+mt
source-wordcount: '3590'
ht-degree: 0%

---

# [!DNL Adobe PDF Services]

使用 [!DNL Adobe Workfront Fusion] [!DNL Adobe PDF Services]中，您可以从PDF文件中提取数据，或从提供的数据中生成新的PDF文件。 此外，您可以将各种文件类型转换为PDF，或将PDF转换为其他文件类型。 PDF服务还允许您组合、压缩或读取PDF文件的元数据，以及控制对文件的密码保护。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

有关用于PDF服务的API的信息，请参阅 [Adobe文档生成API](https://www.adobe.io/apis/documentcloud/dcsdk/doc-generation.html).

## 使用时的安全注意事项 [!DNL Adobe PDF Services]

<!--

* [You do not need an [!DNL Adobe] account](#you-do-not-need-an-adobe-account) 
* [[!DNL Workfront Fusion] does not store your files](#workfront-fusion-does-not-store-your-files)

### You do not need an [!DNL Adobe] account 

Because [!DNL Workfront Fusion] is part of the [!DNL Adobe] product suite, you don't need a separate [!DNL Adobe] account to use these tools. Each tool accesses [!DNL Adobe] PDF functionality without using a connection.

Although [!DNL Workfront Fusion] does not require an [!DNL Adobe] account to use the PDF Services, the modules do require a connection. There are no credentials involved in this connection, and you provide only a name for the connection itself.

### [!DNL Workfront Fusion] does not store your files 

-->

此 [!DNL Adobe PDF Services] 可以读取、转换或修改您的文件，但两者都不能 [!DNL Adobe] 也不 [!DNL Workfront Fusion] 存储您的文件或数据。 这意味着：

* 您可以保持对文件的控制，包括其安全性
* 您无需拥有 [!UICONTROL Adobe] storage或cloud storage帐户来使用PDF服务。

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

要创建OAuth服务器到服务器，必须在Adobe开发人员控制台中添加Adobe PDF服务API。 添加API时，选择OAuth服务器到服务器选项。

有关说明，请参阅 [使用OAuth将API添加到项目](https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/) 在Adobe开发人员文档中。

## 创建与的连接 [!DNL Adobe PDF Services]

要为创建连接，请执行以下操作 [!DNL Adobe PDF Services] 模块：

1. 在任何 [!DNL Adobe PDF Services] 模块，单击 **[!UICONTROL 添加]** ，位于“Connection（连接）”框旁。

1. 填写以下字段：

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[！UICONTROL连接类型]</td>
          <td>
            <p>选择是要创建服务器到服务器连接还是JWT连接。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL连接名称]</td>
          <td>
            <p>输入此连接的名称。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL客户端ID]</td>
          <td>输入您的 [!DNL Adobe] [！UICONTROL客户端ID]。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].<p>有关查找凭据的说明，请参阅 <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >凭据</a> 在Adobe开发人员文档中。</p></td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL客户端密钥]</td>
          <td>输入您的 [!DNL Adobe] [！UICONTROL客户端密钥]。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].<p>有关查找凭据的说明，请参阅 <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >凭据</a> 在Adobe开发人员文档中。</p>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL技术帐户ID]（仅限JWT）</td>
          <td>输入您的 [!DNL Adobe] [！UICONTROL技术帐户ID]。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].<p>有关查找凭据的说明，请参阅 <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >凭据</a> 在Adobe开发人员文档中。</p>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL组织ID]（仅限JWT）</td>
          <td>输入您的 [!DNL Adobe] [！UICONTROL组织ID]。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].<p>有关查找凭据的说明，请参阅 <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >凭据</a> 在Adobe开发人员文档中。</p>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL元范围]（仅限JWT）</td>
          <td>
            输入连接所需的任何元范围。
          </td>
        </tr>
       </tbody>
    </table>
1. 单击 **[!UICONTROL 继续]** 以保存连接并返回到模块。


## [!DNL Adobe PDF Services] 模块及其字段

配置时 [!DNL PDF Services]， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还可能会显示其他字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
* [[!UICONTROL 用于PDF文件的OCR]](#ocr-for-pdf-file)
* [[!UICONTROL 页面操作]](#page-manipulation)
* [[!UICONTROL PDF辅助功能自动标记]](#pdf-accessibility-auto-tag)
* [[!UICONTROL 文件属性PDF]](#pdf-file-properties)
* [[!UICONTROL ProtectPDF文件]](#protect-pdf-file)
* [[!UICONTROL 删除PDF文件的保护]](#remove-protection-of-a-pdf-file)
* [拆分PDF文件](#split-a-pdf-file)

### [!UICONTROL 生成文档]

此 [!UICONTROL 生成文档] 模块是一种创建包含所选数据的PDF的强大方法。 您可以使用格式化 [!DNL Microsoft Word] 模板，或以JSON格式提供数据。

欲知关于 [!UICONTROL [!DNL Adobe PDF Services] 生成文档] 功能，请参见 [文档生成概述](https://www.adobe.io/apis/documentcloud/dcsdk/docs.html) 在 [!DNL Adobe Document Services] 文档。

* [使用 [!UICONTROL 生成文档] 模块带有 [!DNL Microsoft Word] 模板](#use-the-generate-document-module-with-a-microsoft-word-template)
* [使用 [!UICONTROL 生成文档] 带有JSON的模块](#use-the-generate-document-module-with-json)

#### 使用 [!UICONTROL 生成文档] 模块带有 [!DNL Microsoft Word] 模板

<!--
>[!NOTE]
>
>For a discussion of Microsoft Word templates, see [Microsoft Word Template modules](../../workfront-fusion/apps-and-their-modules/microsoft-word-templates-modules.md). 
>
>You do not need to use Microsoft Word template modules to use a Microsoft Word template with the PDF Services Generate document module.
-->

要使用 [!UICONTROL 生成文档] 模块带有 [!UICONTROL Microsoft Word] 模板，必须先创建模板。 有关说明，请在 [!DNL Microsoft Office] 文档。

填写 [!UICONTROL 生成文档] 模块字段，如下所示：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>此源文件是 [!DNL Microsoft Word ]模块用于生成新PDF的模板。</p> <p>我们建议在中创建一个项目 [!DNL Workfront] 对于 [!DNL Microsoft Word] 您在中使用的模板 [!DNL Workfront Fusion]. 然后，您可以使用 [!DNL Workfront] &gt; [！UICONTROL Download document]模块以将相应的模板提取到场景中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出格式]</td> 
   <td> <p>选择所生成文档的格式。</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">用于合并的[！UICONTROL数据]</td> 
   <td> <p>对于模板中要替换为文本的每个值标记，请填写以下内容：</p> 
    <ul> 
     <li> <p>[！UICONTROL Key]</p> <p>输入密钥。 在模板中，键是值标记中显示的文本。 例如，如果要在值标记中放置文本 <code>&#123;&#123;name&#125;&#125;</code>，输入 <code>name </code>键字段中。</p> </li> 
     <li> <p>值类型</p> <p>选择值字段中的数据是值、对象还是对象数组。</p> </li> 
     <li> <p>[！UICONTROL值]</p> <p>输入或映射要在生成的文档中显示的文本以代替值标记。</p> </li> 
    </ul> <p> <img src="assets/generate-with-template-350x241.png" style="width: 350;height: 241;"> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### 使用 [!UICONTROL 生成文档] 带有JSON的模块

要使用 [!UICONTROL 生成文档] 使用JSON的模块，请填写以下字段：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出格式]</td> 
   <td> <p>选择所生成文档的格式。</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">用于合并的[！UICONTROL数据]</td> 
   <td> <p>要在此模块中使用JSON，必须在此字段上启用映射。</p> <p>输入或映射要从中生成文档的JSON。 </p> <p>您可以直接在此字段中键入JSON，或从JSON模块映射JSON输出。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 提取文本/表]

此操作模块允许您从PDF文件中提取数据。 模块输出单独的文本元素，如段落或表格单个单元格中的文本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td>从上一个模块中选择源文件，或映射源文件的名称和数据。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">应该提取为JSON的[！UICONTROL元素]</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL Text]</p> </li> 
     <li> <p>[！UICONTROL Tables]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL是否提取定界框？]</td> 
   <td>启用此选项可提取有关文本定界框的数据。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL是否包含输出的样式信息？]</td> 
   <td>启用此选项以将样式信息添加到输出JSON。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 合并PDF文件]

此操作模块获取多个PDF文件，并将它们组合为一个PDF文件。 例如，此模块可以将所有文档合并到 [!UICONTROL Workfront] 将项目合并为单个PDF。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文档]</td> 
   <td> <p>您可以使用聚合器模块来收集要合并到PDF中的文档，也可以手动添加文档。 </p> <p>我们建议使用[！UICONTROL Array Aggregator]模块来聚合上一个模块的输出。 通过使用聚合器，您无需知道要合并的文件名称、位置或数量。 因此，使用汇总比手动输入要合并的文档要灵活和可伸缩得多。</p> <p>要将[！UICONTROL组合PDF]文件模块与聚合器一起使用，必须在[！UICONTROL文档]字段中启用映射。 </p> <p>在此示例中，[！UICONTROL读取相关记录]模块标识与项目关联的文档，而[！UICONTROL下载文档]模块下载每个文档。 所有PDF都聚合到一个数组中，该数组将传递到[！UICONTROL CombinePDF]文件模块中。</p> <p> <img src="assets/combine-example-350x104.png" style="width: 350;height: 104;"> </p> <p>您也可以手动输入文档。</p> <p>对于要包含在组合PDF中的每个文档：</p> 
    <ol> 
     <li value="1"> <p>单击[！UICONTROL添加文档]</p> </li> 
     <li value="2"> <p>在[！UICONTROL源文件]字段中，选择用于输出要包括的文档的模块，或映射源文件的名称和数据。 </p> </li> 
     <li value="3"> <p>（可选）如果只想包含源文件中的某些页面，则对于要添加的每个页面范围，单击 <strong>[！UICONTROL添加项]</strong> 在[！UICONTROL页面]字段中，输入要包含的页面范围的第一页和最后一页，然后单击 <strong>[！UICONTROL添加]</strong>. 您可以从单个文档中包含多个页面范围。</p> </li> 
     <li value="4"> <p>单击 <strong>[！UICONTROL添加]</strong>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 压缩PDF文件]

此操作模块获取PDF文件并对其进行压缩。 这对于节省带宽或内存非常有用。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>源文件必须采用PDF格式。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL压缩级别]</td> 
   <td>选择要使用的压缩级别。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 将文档转换为PDF文件]

此工具将文档转换为PDF文件。 源文件必须是以下文档格式之一：

* DOC
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>源文件必须为以下格式之一：</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>XLS</p> </li> 
     <li> <p>PPT</p> </li> 
     <li> <p>TXT</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL语言]</td> 
   <td> <p>选择源文档的默认语言。 这允许模块选择适当的字体（如果源文件中不包括字体）。</p> <p>从以下语言中选择：</p> 
    <ul> 
     <li> <p>en-US（默认）：英语（美利坚合众国）</p> </li> 
     <li> <p>ca-ES：加泰罗尼亚语（西班牙）</p> </li> 
     <li> <p>cs-CZ：捷克语（捷克共和国）</p> </li> 
     <li> <p>da-DK：丹麦语（丹麦）</p> </li> 
     <li> <p>de-DE：德语（德国）</p> </li> 
     <li> <p>en-AE：英语（阿拉伯联合酋长国）</p> </li> 
     <li> <p>en-GB：英语（英国）</p> </li> 
     <li> <p>en-IL：英语（以色列）</p> </li> 
     <li> <p>en-US：英语（美利坚合众国）</p> </li> 
     <li> <p>es-ES：西班牙语（西班牙）</p> </li> 
     <li> <p>es-MX：西班牙语（墨西哥）</p> </li> 
     <li> <p>eu-ES：巴斯克语（西班牙）</p> </li> 
     <li> <p>fi-FI：芬兰语（芬兰）</p> </li> 
     <li> <p>fr-CA：法语（加拿大）</p> </li> 
     <li> <p>fr-FR：法语（法国）</p> </li> 
     <li> <p>fr-MA：法语（摩洛哥）</p> </li> 
     <li> <p>hr-HR：克罗地亚语（克罗地亚）</p> </li> 
     <li> <p>hu-HU：匈牙利语（匈牙利）</p> </li> 
     <li> <p>it-IT：意大利语（意大利）</p> </li> 
     <li> <p>ja-JP：日语（日本）</p> </li> 
     <li> <p>kr-KR：韩语（韩国）</p> </li> 
     <li> <p>nb-NO：挪威语Bokmal（挪威）</p> </li> 
     <li> <p>nl-NL：荷兰语（荷兰）</p> </li> 
     <li> <p>pl-PL：波兰语（波兰）</p> </li> 
     <li> <p>pt-BR：葡萄牙语（巴西）</p> </li> 
     <li> <p>pt-PT：葡萄牙语（葡萄牙）</p> </li> 
     <li> <p>ro-RO：罗马尼亚语（罗马尼亚）</p> </li> 
     <li> <p>ru-RU：俄语（俄罗斯）</p> </li> 
     <li> <p>sk-SK：斯洛伐克语（斯洛伐克）</p> </li> 
     <li> <p>sl-SI：斯洛文尼亚语（斯洛文尼亚）</p> </li> 
     <li> <p>sv-SE：瑞典语（瑞典）</p> </li> 
     <li> <p>tr-TR：土耳其语（土耳其）</p> </li> 
     <li> <p>uk-UA：乌克兰语（乌克兰）</p> </li> 
     <li> <p>zh-CN：中文（中国大陆）</p> </li> 
     <li> <p>zh-TW：中文（台湾）</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 将HTML转换为PDF文件]

此工具将HTML文件转换为PDF文件。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>重要信息：源文件必须为HTML或ZIP格式。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL JSON]</td> 
   <td> <p>如果您的HTML引用JavaScript变量，则可以在此处包含这些变量。 </p> <p>对于每个变量，单击 <strong>[！UICONTROL添加项]</strong> 并包含变量的键和值。</p> <p>注释:   
     <ul> 
      <li> <p>从ZIP文件创建PDF时，源宣传材料必须包括脚本元素，例如： <code> &lt;script src='./json.js' type='text/javascript'&gt;&lt;/script&gt;</code> </p> </li> 
      <li> <p>从URL创建PDF时，此JSON对象的内容将在呈现页面之前插入到浏览器VM中。 </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Include页眉和页脚]</td> 
   <td> <p>启用此选项以创建PDF文档的页眉和页脚。</p> 
    <ul> 
     <li> <p>标题包括日期和文档标题。</p> </li> 
     <li> <p>页脚包括文件名和页码。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL页面宽度]</td> 
   <td>输入纸张的宽度（以英寸为单位）。 模块将使用此信息来格式化所创建PDF文件中的页面。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL页面高度]</td> 
   <td>输入纸张的高度，以英寸为单位。 模块将使用此信息来格式化所创建PDF文件中的页面。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 将图像转换为PDF文件]

此工具将图像转换为PDF文件。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和图像文件。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 将PDF转换为文档]

此工具将PDF文件转换为文档。 您可以为输出文件选择以下格式之一。

* DOC
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>源文件必须采用PDF格式。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出文件格式]</td> 
   <td> <p>选择您希望文件输出为的格式：</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>DOCX</p> </li> 
     <li> <p>PPTX</p> </li> 
     <li> <p>XLSX</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 将PDF转换为图像]

此工具将PDF转换为PNG或JPEG格式的图像，然后输出为ZIP。 PDF将转换为每页一个图像，每个图像以页码结尾。 然后将图像文件合并到ZIP文件中。

例如，一个名为“TestFile”且包含8页的文件将生成8个图像，分别命名为“TestFile_1”和“TestFile_8”。 该模块的输出是一个包含8个图像的ZIP文件。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>源文件必须采用PDF格式。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出文件格式]</td> 
   <td> <p>选择您希望文件输出为的格式：</p> 
    <ul> 
     <li>PNG</li> 
     <li>JPEG</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 线性化PDF文件]

此工具将PDF文档线性化，以创建Web优化的PDF文档。 线性化PDF文档可以逐页查看，而无需下载整个文档。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 用于PDF文件的OCR]

此工具对文件执行光学字符识别(OCR)并生成PDF。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL OCR类型]</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL Modified original image]类型可确保文本可搜索且可供选择，但在清除过程中会修改原始图像（例如，扭曲原始图像），然后再在其上放置不可见的文本图层。 此类型会删除不需要的工件，并且在某些情况下可能会导致文档更易读。 </p> </li> 
     <li> <p>[！UICONTROL Unchanged original image]类型还会将可搜索的文本图层叠加在原始图像上，但在本例中，原始图像保持不变。 此类型生成原始图像的最大保真度。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL语言]</td> 
   <td>选择此文档的语言。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 页面操作]

此模块允许您选择性地旋转或删除PDF文档中的页面。 例如，您可以将纵向视图更改为横向视图，或从PDF文档中删除某些页面。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL操作]</td> 
   <td> <p>选择要对文件执行的操作。</p> 
    <ul> 
     <li> <p><b>[！UICONTROL Delete]</b> </p> <p>选择此选项可从文档中删除页面。</p> </li> 
     <li> <p><b>[！UICONTROL旋转]</b> </p> <p>选择此选项可旋转页面，然后输入要相对于文档页面的起始方向旋转文档页面的顺时针角度（以度为单位）。</p> <p>要从纵向旋转到横向，或者反之，请将页面旋转90度或270度。</p> <p>如果某页是颠倒的，请将其旋转180度。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Pages]</td> 
   <td> <p>对于每个要删除的页面范围，单击 <strong>[！UICONTROL添加]</strong> 然后输入页面范围的首页和最后一页。 </p> <p>注释:   
     <ul> 
      <li> <p>您可以使用负数从文档结尾往回计数。 文档的最后一页为–1，最后一页的第二页为–2，依此类推。</p> </li> 
      <li> <p>要删除单个页面，请将起始页码和结束页码设置为相同的页码。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射每个方案执行周期中您希望模块使用的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF辅助功能自动标记]

此操作模块会创建一个标记为辅助功能用例的PDF。 它还创建了一个可选的Microsoft Excel报表，其中列出了问题并提供了修复建议。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL班次标题]</td> 
   <td> <p>启用此选项以移动文档上的标题。</p> 
    <ul> 
     <li> <p><b>[！UICONTROL生成报告]</b> </p> <p>启用此选项可生成报告，其中列出PDF中的辅助功能问题及其位置，并提供有关如何修复这些问题的建议。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 文件属性PDF]

此工具提取有关文档的基本信息，例如：

* 页数
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL ProtectPDF文件]

此工具使用用户或所有者密码保护PDF文档。 它还对PDF文档中的打印、编辑和复制等特定功能设置了限制。 选择要加密的内容类型和加密算法。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>源文件必须采用PDF格式。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL密码保护类型]</td> 
   <td> <p>启用此选项可使用密码加密输入PDF文档。 如果启用此选项，则必须为以下一项或两项指定并输入值： </p> 
    <ul> 
     <li> <p>[！UICONTROL userPassword]</p> </li> 
     <li> <p>[！UICONTROL ownerPassword] </p> </li> 
    </ul> <p>每个密码的长度最多为128个字符。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL加密算法]</td> 
   <td> <p>选择加密算法。 </p> 
    <ul> 
     <li> <p>[！UICONTROL AES-128加密]</p> <p>密码仅支持LATIN-I字符。 </p> </li> 
     <li> <p>[！UICONTROL AES-256加密]</p> <p>密码支持Unicode字符集</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL要加密的内容]</td> 
   <td> <p>选择要加密的内容类型。</p> 
    <ul> 
     <li> <p>[！UICONTROL所有内容]</p> </li> 
     <li> <p>[！UICONTROL除元数据以外的所有内容]</p> </li> 
     <li> <p>[！UICONTROL仅嵌入数据] </p> </li> 
    </ul> <p>选择“[！UICONTROL Only embedded data]”将使任何提供的访问权限无效。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Permissions]</td> 
   <td> <p>选择要包括的任何权限以允许打印、编辑或内容复制。</p> <p>只有在[！UICONTROL Password Protection Type]字段中设置了[！UICONTROL ownerPassword]时，才使用权限设置。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 删除PDF文件的保护]

此工具从PDF文档中删除安全性（密码保护）。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>源文件必须采用PDF格式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL密码]</td> 
   <td>输入当前保护文件的密码。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 拆分PDF文件]

此操作模块将PDF文档拆分为多个较小的文档。 您可以指定是否按文件数、每个文件的页数或页面范围拆分它。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>选择要用于此模块的连接。</p> 有关创建与的连接 [!DNL Adobe PDF Services]，请参见 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >创建与的连接 [!DNL Adobe PDF Services]</a> 本文章中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> <p>源文件必须采用PDF格式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL拆分选项]</td> 
   <td>选择要如何拆分文件。 
   <ul>
   <li><p><b>页面范围</b></p><p>对于要拆分为单独文档的每个页面范围，单击 <b>添加</b> 并输入要在其上开始的页面和要在其上结束的页面。</p></li>
   <li><p><b>页数</b></p><p>输入要包括在新文档中的页数。</p></li>
   <li><p><b>文件数</b></p><p>输入要分割文档的均匀大小的文件数。</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

