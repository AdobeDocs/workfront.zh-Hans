---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的字符串函数
description: Adobe Workfront Fusion映射面板中提供了以下字符串函数。
author: Becky
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: 0b286e43ed77669329fbee25618394ee5641e428
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

# 中的字符串函数 [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL 长度（文本或缓冲区）]

返回文本字符串的长度（字符数）或二进制缓冲区的长度（缓冲区大小，以字节为单位）。

>[!INFO]
>
>**示例：**
>
>`length( hello )`
>
>返回：5

## [!UICONTROL lower（文本）]

将文本字符串中的所有字母字符转换为小写。

>[!INFO]
>
>**示例：**
>
>`lower( Hello )`
>
>返回： hello

## [!UICONTROL 大写（文本）]

将文本字符串中的第一个字符转换为大写。

>[!INFO]
>
>**示例：**
>
>`capitalize( workfront )`
>
>返回： [!DNL Workfront]

## [!UICONTROL startcase（文本）]

每个单词的首字母使用大写，其他字母使用小写。

>[!INFO]
>
>**示例：**
>`startcase( hello WORLD )`
>
>返回： [!UICONTROL 《你好世界》]

## [!UICONTROL ascii(文本； [删除变音符号])]

从文本字符串中删除所有非ascii字符。

>[!INFO]
>
>**示例：**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
>
>   返回： [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
>
>   返回： [!UICONTROL escrz]



## [!UICONTROL 替换（文本；搜索字符串；替换字符串）]

将搜索字符串替换为新的字符串。

>[!INFO]
>
>**示例：**
>
>`replace( Hello World ; Hello ; Hi )`
>
>返回： [!UICONTROL Hi World]

正则表达式(包含在 `/.../`)可用作具有标记组合(例如 `g`， `i`， `m`)已附加：

>[!INFO]
>
>**示例：**
>
>![](assets/replace---1-350x31.png)
>
>所有这些数字X X X X X都替换为X

替换字符串可以包含以下特殊替换模式：

* `$&` 插入匹配的子字符串。
* `$n` 其中n是小于100的正整数，插入带括号的n个子匹配字符串。 这是1索引。

>[!INFO]
>
>**示例：**
>
>![](assets/variable-value-350x63.png)
>
>返回：电话号码 `+420777111222`
>>
>![](assets/variable-value---2-350x55.png)
>
>返回：电话号码： `+420777111222`

>[!CAUTION]
>
>不要使用指定的捕获组，例如 `/ is (?<number>\d+)/` 替换字符串参数中的。 这样做会导致错误。

有关正则表达式的详细信息，请参阅 [文本分析器](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL trim（文本）]

删除文本开头或结尾的空格字符。

## [!UICONTROL upper（文本）]

将文本字符串中的所有字母字符转换为大写。

>[!INFO]
>
>**示例：**
>
>`upper( Hello )`
>
>返回： [!UICONTROL 您好]

## [!UICONTROL 子字符串（文本；开始；结束）]

返回文本字符串在“开始”位置和“结束”位置之间的部分。

>[!INFO]
>
>**示例：**
>
>* `substring( Hello ; 0 ; 3)`
>
>   返回：帮助
>
>* `substring( Hello ; 1 ; 3 )`
>
>   返回： el

## [!DNL indexOf (string; value; [start])]

返回指定值在字符串中第一次出现的位置。 如果搜索的值不存在，则此方法将返回“–1”。 起始值表示搜索在字符串中的开始位置。

>[!INFO]
>
>**示例：**
>
>* `indexOf( Workfront ; o )`
>
>   返回： 1
>
>* `indexOf( Workfront ; x )`
>
>   返回： -1
>
>* `indexOf( Workfront ; o ; 3 )`
>
>   返回：6

## [!UICONTROL toBinary（值）]

将任意值转换为二进制数据。

您还可以指定编码作为第二个参数，以将十六进制或base64的二进制转换应用于二进制数据。

>[!INFO]
>
>**示例：**
>
>* `toBinary( Workfront )`
>
>   返回：57 6f 72 6b 66 72 6f 6e 74
>
>* `toBinary( V29ya2Zyb250 ; base64 )`
>
>   返回：57 6f 72 6b 66 72 6f 6e 74

## [!UICONTROL toString（值）]

将任意值转换为字符串。

## [!UICONTROL encodeURL（文本）]

将某些文本中的特殊字符编码为有效的URL地址。

## [!UICONTROL decodeURL（文本）]

将URL中的特殊字符解码为文本。

>[!INFO]
>
>**示例：**
>`decodeURL( Automate%20your%20workflow )`
>
>返回： [!UICONTROL 自动化您的工作流]

## [!UICONTROL escapeHTML（文本）]

转义文本中的所有HTML标签。

>[!INFO]
>
>**示例：**
>
>`escapeHTML( <b>Hello</b> )`
>
> 返回： `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(text)]

转义文本中的所有Markdown标记。

>[!INFO]
>
>**示例：**
>
>`escapeMarkdown( # Header )`
>
>返回： `&#35; Header`

## [!UICONTROL stripHTML（文本）]

从文本中删除所有HTML标签。

>[!INFO]
>
>**示例：**
>
>`stripHTML( <b>Hello</b> )`
>
>返回： Hello

## 包含（文本；搜索字符串）

验证文本是否包含搜索字符串。

>[!INFO]
>
>**示例：**
>
>* `contains( Hello World ; Hello )`
>
>   返回： [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
>
>   返回： [!UICONTROL false]

## [!UICONTROL 拆分（文本；分隔符）]

通过将字符串拆分为子字符串，将字符串拆分为字符串数组。

>[!INFO]
>
>**示例：**
>
>`split( John, George, Paul ; , )`

## [!UICONTROL md5（文本）]

计算字符串的md5哈希值。

>[!INFO]
>
>**示例：**
>
>`md5( Workfront )`
>
>返回： `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL sha1(文本； [编码]； [键])]

计算字符串的sha1哈希。 如果指定了键参数，则返回sha1 HMAC哈希。 支持的编码：“hex”（默认）、“base64”或“latin1”。

>[!INFO]
>
>**示例：**
>
>`sha1( workfront )`
>
>返回：b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256(文本； [编码]； [键])]

计算字符串的sha256哈希。 如果指定了键参数，则返回sha256 HMAC哈希。 支持的编码：“hex”（默认）、“base64”或“latin1”。>

>[!INFO]
>
>**示例：**
>
>`sha256( workfront )`
>
>返回：ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512(文本； [输出编码]； [键]； [密钥编码])]

计算字符串的sha512哈希。 如果指定了键参数，则返回sha512 HMAC哈希。

支持的编码：

* &quot;[!UICONTROL 十六进制]“（默认）
* &quot;[!UICONTROL 基数64]&quot;
* &quot;[!UICONTROL latin1]&quot;

支持的密钥编码：

* &quot;[!UICONTROL 文本]“（默认）
* &quot;[!UICONTROL 十六进制]&quot;
* &quot;[!UICONTROL 基数64]”或“[!UICONTROL 二进制]&quot;

使用&quot;[!UICONTROL 二进制]“密钥编码，密钥必须是缓冲区，而不是字符串。

>[!INFO]
>
>**示例：**
>
>`sha512(workfront)`
>
>返回：789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b85e1e19db58bb44b234493af35fd431639c0345aadf2cf7ec26e9f4a7fb19

## [!UICONTROL base64（文本）]

将文本转换为base64。

>[!INFO]
>
>**示例：**
>
>`base64( workfront )`
>
>返回：d29ya2Zyb250==
