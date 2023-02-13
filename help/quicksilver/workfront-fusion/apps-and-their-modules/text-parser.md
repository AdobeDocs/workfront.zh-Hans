---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: 文本解析器
description: 您可以使用文本解析器工具来解析文本，以供在其他 [!DNL Adobe Workfront Fusion] 方案模块。 文本解析器不需要连接。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# [!UICONTROL 文本解析器]

您可以使用 [!UICONTROL 文本解析器工具] 解析文本以供在其他 [!DNL Adobe Workfront Fusion] 方案模块。 的 [!UICONTROL 文本解析器] 不需要连接。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 文本解析器] 模块及其字段

配置 [!UICONTROL 文本解析器] 模块， [!DNL Adobe Workfront Fusion] 显示下面列出的字段。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 变形金刚

* [[!UICONTROL 从HTML获取元素]](#get-elements-from-html)
* [[!UICONTROL 从文本中获取元素]](#get-elements-from-text)
* [[!UICONTROL HTML到文本]](#html-to-text)
* [[!UICONTROL 匹配模式]](#match-pattern)
* [[!UICONTROL 替换]](#replace)

#### [!UICONTROL 从HTML获取元素]

从HTML代码中检索所需的元素。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL即使模块未找到匹配项，仍继续执行路由]</td> 
   <td> <p>启用此选项可确保模块在未返回任何结果时不会停止方案。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Element type]</td> 
   <td> <p> 从元素代码中选择要检索的元素类型HTML。 </p> 
    <ul> 
     <li>[!UICONTROL图像]</li> 
     <li>[!UICONTROL链接]</li> 
     <li>[!UICONTROL iFrame元素]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROLHTML] </td> 
   <td> <p>输入或映射要从中检索指定元素类型的HTML代码。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从文本中获取元素]

根据给定模式解析文本中的元素。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL输入文本]</td> 
   <td> <p>输入或映射要解析的文本。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL模式]</td> 
   <td> <p>从文本中选择反映要解析的元素的模式。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL忽略重复发生次数]</td> 
   <td> <p>选中此框可忽略文本元素的重复出现。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTML到文本]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROLHTML] </td> 
   <td> <p>输入要转换为纯文本的HTML代码。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL换行符] </td> 
   <td> <p>选择换行符类型（换行符）。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL大写标题]</p> </td> 
   <td> <p>启用此选项可转换标题标记中包含的文本(例如 &lt;h2&gt; &lt;/h2&gt;)替换为大写文本。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 匹配模式]

的 [!UICONTROL 匹配模式] 模块允许您从给定文本中查找和提取与搜索模式匹配的字符串元素。 此模块使用正则表达式（也称为正则表达式或regexp）。

正则表达式是一系列字符，其中每个字符可以是具有特殊含义的元字符，也可以是具有文字含义的正则字符。 这些字符和元字符标识可用于搜索文本的模式。 例如，如果要搜索名称，可以设置一个正则表达式来搜索由两个以大写字母开头的连续单词组成的模式。 正则表达式是用于搜索和处理文本的强大工具。

对正则表达式的讨论不在本条的涵盖范围内。 我们建议使用以下资源：

* 有关元字符的完整列表，请参阅 [正则表达式](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) 在MDN Web文档中。
* 有关如何创建正则表达式的教程，我们建议 [RegexOne](https://regexone.com/).
* 要试用正则表达式，我们建议 [正则表达式101](https://regex101.com/) 网站。 在左侧面板中选择ECMAScript(JavaScript)风格。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL模式] </td> 
   <td> <p>输入正则表达式模式。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> 在提供的文本中提取所有数字。</p> <p>注释:  <p>该模式应在括号中至少包含一个捕获组 <code>()</code>. 如果模式不包含任何捕获组，则输出包为空。</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL全局匹配]</td> 
   <td> <p>启用此选项可检索文本中的所有匹配项。 每个匹配项都将输出到单独的包中。 如果禁用此选项，则模块仅检索第一个条目。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL区分大小写]</td> 
   <td> <p> 为此模块启用此选项，可将文本视为区分大小写。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL多行] </td> 
   <td> <p>启用此选项可确保开始和结束元字符(<code>^</code> 和 <code>$</code>)匹配每行的开头或结尾，而不只是整个输入字符串的开头或结尾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>启用此选项可确保句点(.) 匹配换行符(<code>\n</code>)。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL即使模块未返回任何结果，仍继续执行路由]</td> 
   <td> <p>启用此选项可确保模块在未返回任何结果时不会停止方案。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>输入或映射要匹配模式的文本。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 替换]

搜索输入的文本以查找指定的值或正则表达式，并将结果替换为新值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL模式] </td> 
   <td> <p>输入搜索词。 您还可以使用正则表达式。 有关正则表达式的更多详细信息，请参阅 <a href="#match-pattern" class="MCXref xref">[!UICONTROL匹配模式]</a> 模块。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL新值]</td> 
   <td> <p> 输入一个值以替换搜索词。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL全局匹配]</td> 
   <td> <p>启用此选项可检索文本中的所有匹配项。 每个匹配项都将输出到单独的包中。 如果禁用此选项，则模块仅检索第一个条目。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL区分大小写]</td> 
   <td> <p> 为此模块启用此选项，可将文本视为区分大小写。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL多行] </td> 
   <td> <p>启用此选项可确保开始和结束元字符(<code>^</code> 和 <code>$</code>)匹配每行的开头或结尾，而不只是整个输入字符串的开头或结尾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>启用此选项可确保句点(.) 匹配换行符(<code>\n</code>)。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>输入要搜索的文本。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 数据刮取

数据抓取（有时称为Web抓取、数据提取或Web收集）是从网站中收集数据并将其存储到本地数据库或电子表格中的过程。 如果要从网站中抓取数据，并且您不熟悉正则表达式，则可以使用数据抓取工具：

* [Apify](https://apify.com/)
* [2019年最佳数据刮取工具](https://www.octoparse.com/blog/best-data-scraping-tools-for-2019-top-10-reviews)

如果数据刮取工具提供REST API，则可以通过我们的通用 [[!UICONTROL HTTP] 模块](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) 和 [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) 模块。
