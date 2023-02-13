---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的字符串函数
description: 以下字符串函数在Adobe Workfront Fusion映射面板中可用。
author: Becky
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 3%

---

# 中的字符串函数 [!DNL Adobe Workfront Fusion]

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL ascii（文本）； [删除变音符])]

从文本字符串中删除所有非ascii字符。

>[!INFO]
>
>**示例:**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
   >
   >   返回： [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
   >
   >   返回： [!UICONTROL escrz]


## [!UICONTROL base64（文本）]

将文本转换为base64。

>[!INFO]
>
>**示例:**
>
>`base64( workfront )`
>
>返回：d29ya2Zyb250==

## [!UICONTROL 大写（文本）]

将文本字符串中的第一个字符转换为大写。

>[!INFO]
>
>**示例:**
>
>`capitalize( workfront )`
>
>返回： [!DNL Workfront]

## 包含（文本）；搜索字符串)

验证文本是否包含搜索字符串。

>[!INFO]
>
>**示例:**
>
>* `contains( Hello World ; Hello )`
   >
   >   返回： [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
   >
   >   返回： [!UICONTROL false]


## [!UICONTROL decodeURL(text)]

将URL中的特殊字符解码为文本。

>[!INFO]
>
>**示例:**
>`decodeURL( Automate%20your%20workflow )`
>
>返回： [!UICONTROL 自动执行工作流]

## [!UICONTROL encodeURL（文本）]

将某些文本中的特殊字符编码为有效的URL地址。

## [!UICONTROL escapeHTML（文本）]

对文本中的所有HTML标记进行转义。

>[!INFO]
>
>**示例:**
>
>`escapeHTML( <b>Hello</b> )`
>
> 返回： `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(text)]

对文本中的所有Markdown标记进行转义。

>[!INFO]
>
>**示例:**
>
>`escapeMarkdown( # Header )`
>
>返回： `&#35; Header`

## [!DNL indexOf (string; value; [start])]

返回字符串中首次出现指定值的位置。 如果搜索的值不在，此方法将返回“–1”。 开始值指示搜索在字符串中应开始的位置。

>[!INFO]
>
>**示例:**
>
>* `indexOf( Workfront ; o )`
   >
   >   返回：1
>
>* `indexOf( Workfront ; x )`
   >
   >   返回：-1
>
>* `indexOf( Workfront ; o ; 3 )`
   >
   >   返回：6


## [!UICONTROL 长度（文本或缓冲区）]

返回文本字符串的长度（字符数）或二进制缓冲区的长度(缓冲区大小（以字节为单位）。

>[!INFO]
>
>**示例:**
>
>`length( hello )`
>
>返回：5

## [!UICONTROL 下（文本）]

将文本字符串中的所有字母字符转换为小写。

>[!INFO]
>
>**示例:**
>
>`lower( Hello )`
>
>返回：hello

## [!UICONTROL md5（文本）]

计算字符串的md5哈希。

>[!INFO]
>
>**示例:**
>
>`md5( Workfront )`
>
>返回： `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL 替换(文本；搜索字符串；替换字符串)]

将搜索字符串替换为新字符串。

>[!INFO]
>
>**示例:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>返回： [!UICONTROL Hi World]

正则表达式(包含在 `/.../`)可用作带有标记组合的搜索字符串(例如 `g`, `i`, `m`)已附加：

>[!INFO]
>
>**示例:**
>
>![](assets/replace---1-350x31.png)
>
>所有这些数字X X X X都被X替换

替换字符串可以包括以下特殊的替换模式：

* `$&` 插入匹配的子字符串。
* `$n` 其中n是小于100的正整数，插入第n个以括号表示的子匹配字符串。 这是1索引。

>[!INFO]
>
>**示例:**
>
>![](assets/variable-value-350x63.png)
>
>返回：电话号码 `+420777111222`
>>![](assets/variable-value---2-350x55.png)
>返回：电话号码： `+420777111222`

>[!CAUTION]
请勿使用命名的捕获组，例如 `/ is (?<number>\d+)/` 替换字符串参数中。 这样做会导致错误。

有关正则表达式的更多信息，请参阅 [文本解析器](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL sha1（文本）； [编码]; [key])]

计算字符串的sha1哈希。 如果指定了键参数，则返回sha1 HMAC哈希。 支持的编码：&quot;hex&quot;（默认）、&quot;base64&quot;或&quot;latin1&quot;。

>[!INFO]
**示例:**
`sha1( workfront )`
返回：b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256(文本； [编码]; [key])]

计算字符串的sha256哈希。 如果指定了键参数，则会返回sha256 HMAC哈希。 支持的编码：“hex”（默认）、“base64”或“latin1”。>

>[!INFO]
**示例:**
`sha256( workfront )`
返回：ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512(文本； [输出编码]; [key]; [密钥编码])]

计算字符串的sha512哈希。 如果指定了键参数，则会返回sha512 HMAC哈希。

支持的编码：

* &quot;[!UICONTROL 十六进制]&quot;（默认）
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

支持的键编码：

* &quot;[!UICONTROL 文本]&quot;（默认）
* &quot;[!UICONTROL 十六进制]&quot;
* &quot;[!UICONTROL base64]&quot;或&quot;[!UICONTROL 二进制]&quot;

使用“[!UICONTROL 二进制]“键编码，键必须是缓冲区，而不是字符串。

>[!INFO]
**示例:**
`sha512(workfront)`
返回：789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b85e1e19db58bb44b234493af35fd431639c0345aadf2c7e26e9f4fb19

## [!UICONTROL 拆分（文本）；分隔符]

通过将字符串分隔为子字符串，将字符串拆分为字符串数组。

>[!INFO]
**示例:**
`split( John, George, Paul ; , )`

## [!UICONTROL startcase（文本）]

将每个单词的第一个字母大写，并将所有其他字母的小写。

>[!INFO]
**示例：**
`startcase( hello WORLD )`
返回： [!UICONTROL 《你好世界》]

## [!UICONTROL stripHTML（文本）]

从文本中删除所有HTML标记。

>[!INFO]
**示例:**
`stripHTML( <b>Hello</b> )`
返回：Hello

## [!UICONTROL 子字符串（文本）；开始；结束)]

返回在“开始”位置和“结束”位置之间的文本字符串的一部分。

>[!INFO]
**示例:**
* `substring( Hello ; 0 ; 3)`

   返回：赫尔
* `substring( Hello ; 1 ; 3 )`

   返回：el


## [!UICONTROL toBinary（值）]

将任何值转换为二进制数据。

您还可以将编码指定为第二个参数，以将十六进制或base64的二进制转换应用于二进制数据。

>[!INFO]
**示例:**
* `toBinary( Workfront )`

   返回：57 6f 72 6b 66 72 6f 6e 74
* `toBinary( V29ya2Zyb250 ; base64 )`

   返回：57 6f 72 6b 66 72 6f 6e 74


## [!UICONTROL toString(value)]

将任何值转换为字符串。

## [!UICONTROL 裁切（文本）]

删除文本开头或结尾的空格字符。

## [!UICONTROL 大写（文本）]

将文本字符串中的所有字母字符转换为大写字母。

>[!INFO]
**示例:**
`upper( Hello )`
返回： [!UICONTROL HELLO]
