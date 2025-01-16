---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: 文本分析器
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 0%

---

# [!UICONTROL 文本分析器]

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [文本分析器](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/text-parser.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

您可以使用[!UICONTROL 文本解析器工具]来解析要在其他[!DNL Adobe Workfront Fusion]方案模块中使用的文本。 [!UICONTROL 文本分析器]不需要连接。

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
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## 文本分析器API信息

文本解析器连接器使用以下内容：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API标记</td> 
   <td>v2</td> 
  </tr>
 </tbody> 
 </table>

## [!UICONTROL 文本分析器]模块及其字段

配置[!UICONTROL 文本分析器]模块时，[!DNL Adobe Workfront Fusion]显示下面列出的字段。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

### 变压器

* [[!UICONTROL 从HTML获取元素]](#get-elements-from-html)
* [[!UICONTROL 从文本中获取元素]](#get-elements-from-text)
* [[!UICONTROL 文本HTML]](#html-to-text)
* [[!UICONTROL 匹配模式]](#match-pattern)
* [[!UICONTROL 替换]](#replace)

#### [!UICONTROL 从HTML获取元素]

从HTML代码中检索所需的元素。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL即使模块找不到匹配项，仍继续执行路由]</td> 
   <td> <p>启用此选项以确保模块在未返回任何结果时不会停止场景。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL元素类型]</td> 
   <td> <p> 选择要从HTML代码中检索的元素类型。 </p> 
    <ul> 
     <li>[！UICONTROL图像]</li> 
     <li>[！UICONTROL链接]</li> 
     <li>[！UICONTROL iFrame元素]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROLHTML] </td> 
   <td> <p>输入或映射要从中检索指定元素类型的HTML代码。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从文本中获取元素]

根据给定的模式解析文本中的元素。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL输入文本]</td> 
   <td> <p>输入或映射要分析的文本。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL模式]</td> 
   <td> <p>选择反映要从文本中解析的元素的图案。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL忽略重复发生次数]</td> 
   <td> <p>选中此框可忽略文本元素的重复出现次数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 文本HTML]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROLHTML] </td> 
   <td> <p>输入要转换为纯文本的HTML代码。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL换行符] </td> 
   <td> <p>选择换行符（换行符）的类型。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL大写标题]</p> </td> 
   <td> <p>启用此选项可将标题标记中包含的文本（如&lt;h2&gt; &lt;/h2&gt;）转换为大写文本。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 匹配模式]

[!UICONTROL 匹配模式]模块允许您从给定文本中查找和提取与搜索模式匹配的字符串元素。 此模块使用正则表达式（也称为正则表达式或正则表达式）。

正则表达式是一系列字符，其中每个字符要么是具有特殊意义的元字符，要么是具有字面含义的常规字符。 这些字符和元字符标识了可用于搜索文本的模式。 例如，如果要搜索名称，可设置正则表达式以搜索由两个以大写字母开头的连续单词组成的模式。 正则表达式是用于搜索和处理文本的强大工具。

有关正则表达式的讨论超出了本文的讨论范围。 我们建议使用以下资源：

* 有关元字符的完整列表，请参阅MDN Web文档中的[正则表达式](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions)。
* 有关如何创建正则表达式的教程，我们建议[RegexOne](https://regexone.com/)。
* 若要试验正则表达式，我们建议使用[正则表达式101](https://regex101.com/)网站。 在左侧面板中选择ECMAScript (JavaScript) FLAVOR。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL模式] </td> 
   <td> <p>输入正则表达式模式。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code>提取所提供文本中的所有数字。</p> <p>注意：  <p>模式应至少包含一个位于括号<code>()</code>中的捕获组。 如果模式不包含任何捕获组，则输出包为空。</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL全局匹配]</td> 
   <td> <p>启用此选项以检索文本中的所有匹配项。 每个匹配项都在单独的捆绑包中输出。 如果禁用此选项，则模块将仅检索第一个条目。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL区分大小写]</td> 
   <td> <p> 启用此选项可让此模块将文本视为区分大小写。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Multiline] </td> 
   <td> <p>启用此选项可确保开始和结束元字符（<code>^</code>和<code>$</code>）匹配每行的开始或结束，而不只是整个输入字符串的开始或结束。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL单行]</td> 
   <td>启用此选项以确保句点(.)与换行符(<code>\n</code>)匹配。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL即使模块未返回任何结果，仍继续执行路由]</td> 
   <td> <p>启用此选项以确保模块在未返回任何结果时不会停止场景。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Text] </td> 
   <td> <p>输入或映射要与模式匹配的文本。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 替换]

在输入的文本中搜索指定的值或正则表达式，并将结果替换为新的值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL模式] </td> 
   <td> <p>输入搜索词。 您也可以使用正则表达式。 有关正则表达式的更多详细信息，请参阅<a href="#match-pattern" class="MCXref xref">[！UICONTROL匹配模式]</a>模块。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL新值]</td> 
   <td> <p> 输入替换搜索词的值。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL全局匹配]</td> 
   <td> <p>启用此选项以检索文本中的所有匹配项。 每个匹配项都在单独的捆绑包中输出。 如果禁用此选项，则模块将仅检索第一个条目。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL区分大小写]</td> 
   <td> <p> 启用此选项可让此模块将文本视为区分大小写。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Multiline] </td> 
   <td> <p>启用此选项可确保开始和结束元字符（<code>^</code>和<code>$</code>）匹配每行的开始或结束，而不只是整个输入字符串的开始或结束。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL单行]</td> 
   <td>启用此选项以确保句点(.)与换行符(<code>\n</code>)匹配。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Text] </td> 
   <td> <p>输入要搜索的文本。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 数据擦除

数据抓取（有时称为网页抓取、数据提取或网页收集）是从网站收集数据，并将其存储在本地数据库或电子表格中的过程。 如果要从网站中刮取数据，并且不熟悉正则表达式，则可以使用数据刮取工具。

如果数据抓取工具提供REST API，则可以通过我们的通用[[!UICONTROL HTTP]模块](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)和[Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)模块连接到该工具。
