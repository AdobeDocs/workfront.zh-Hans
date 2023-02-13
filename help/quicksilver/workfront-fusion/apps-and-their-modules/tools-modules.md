---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 工具
description: 的 [!DNL Adobe Workfront Fusion Tools] 部分包含一些可以增强方案的有用模块。
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2246'
ht-degree: 0%

---

# [!UICONTROL 工具]

的 [!DNL Adobe Workfront Fusion Tools] 部分包含一些可以增强方案的有用模块。

[!UICONTROL 工具] 模块可从应用程序列表或 [!UICONTROL 工具] 图标 ![](assets/tools-icon-small.png) 屏幕底部。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr>
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 工具] 他们的田地

* [触发器](#triggers)
* [操作](#actions)
* [聚合器](#aggregators)
* [变形金刚](#transformers)

### 触发器

#### [!UICONTROL 基本触发器]

此模块允许您创建自定义触发器并定义其输入包。

例如，您可以将此模块用于联系人或计划发送到指定电子邮件地址的任何其他列表(例如 [!UICONTROL 电子邮件] >[!UICONTROL 发送电子邮件]或 [!DNL Gmail] >[!UICONTROL 发送电子邮件] 模块)，或作为需要时触发的简单提醒。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL包]</td> 
   <td> <p>通过添加数组项目创建自定义包。 数组由名称 — 值对组成。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 获取多个变量]](#get-multiple-variables)
* [[!UICONTROL 获取变量]](#get-variable)
* [[!UICONTROL 增量函数]](#increment-function)
* [[!UICONTROL 设置多个变量]](#set-multiple-variables)
* [[!UICONTROL 设置变量]](#set-variable)
* [[!UICONTROL 睡眠]](#sleep)

#### [!UICONTROL 获取多个变量]

此模块检索之前由 [!UICONTROL 设置变量] 或 [!UICONTROL 设置多个变量] 模块。

此模块可以读取在场景中任意位置设置的变量，即使变量是在与 [!UICONTROL 获取多个变量] 模块。 唯一的要求是 [!UICONTROL 工具] > [!UICONTROL 设置变量] 或 [!UICONTROL 工具] > [!UICONTROL 设置多个变量] 模块在 [!UICONTROL 工具] > [!UICONTROL 获取多个变量] 模块。 有关执行模块的顺序的更多信息，请参阅 [中的路由器模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL变量]</td>
        <td>添加您希望模块获取的变量。</td>
    </tr>
    <tr>
        <td>[!UICONTROL变量名称]</td>
        <td>对于您添加的每个变量，映射要获取的变量的名称。</td>
    </tr>
</table>

>[!INFO]
>
>**示例：**  以下是 [!UICONTROL 已设置]/[!UICONTROL 获取（多个）变量] 模块：
>
>* 用于存储计算值，以供日后使用，即使在不同的路由中也是如此。 当值用于多个模块且计算值的公式过于复杂时，此选项非常有用。
>* 调试公式。 如果模块中使用的公式似乎没有提供正确的结果，请复制该公式并将其粘贴到 [!UICONTROL 设置变量] 模块。 在 [!UICONTROL 设置变量] 并执行方案。 验证 [!UICONTROL 设置变量] 模块的输出、调整或简化公式、再次执行方案，并继续执行，直到问题得到解决。



#### [!UICONTROL 获取变量]

此模块检索之前由 [!UICONTROL 设置变量] 或 [!UICONTROL 设置多个变量] 模块。

此模块可以读取在场景中任意位置设置的变量，即使变量是在与 [!UICONTROL 获取变量] 模块。 唯一的要求是 [!UICONTROL 工具] > [!UICONTROL 设置变量] 或 [!UICONTROL 工具] > [!UICONTROL 设置多个变量] 模块在 [!UICONTROL 工具] > [!UICONTROL 获取变量] 模块。 有关执行模块的顺序的更多信息，请参阅 [中的路由器模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL变量名称]</td> 
   <td> <p>映射您希望模块获取的变量的名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 增量函数]

此模块会返回一个在每个模块操作后递增1的值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL重置值]</td> 
   <td> <p>选择希望模块递增值的时间。 </p> 
    <ul> 
     <li>[!UICONTROL After one cycle]</li> 
     <li>[!UICONTROL在运行一个方案后]</li> 
     <li>[!UICONTROL Never]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例:**
>
>该模块的一个用途是对组中的用户执行任务、潜在客户、电子邮件等的“循环”分配。 算法从一组中按某种合理顺序选择受分配者，通常从列表的顶部到底部。 当算法到达列表末尾时，它将在列表顶部向用户提供下一个分配，并继续在列表中进行分配。
>
>以下方案在运行每个奇数方案后向第一个收件人发送电子邮件，在运行每个偶数方案后向第二个收件人发送电子邮件。
>
>![](assets/example-email-350x246.gif)
>
>1. 要创建此方案，请执行以下操作：
>1. 设置模块的 **[!UICONTROL 重置值]** 字段。
>1. 设置奇数值的路由。 使用等于的模数数学函数设置此路由的筛选器 `1`:

>
>   ![](assets/odd-350x459.png)
>
>  **注意**:不要忘记更改 [!UICONTROL 等于] 运算符 [!UICONTROL 文本] 运算符 [!UICONTROL 数值] 运算符。
>
>1. 使用等于的模数数学函数设置偶数值的路由 `0`:
>
>每次运行方案时，增量函数都会添加一个。 过滤器会检查增量并对其值执行相应操作，以确保电子邮件的平均分发。

#### [!UICONTROL 设置多个变量]

此模块会创建可由路由中其他模块映射的变量。 变量还可以映射到 [!UICONTROL 获取变量] 或 [!UICONTROL 获取多个变量] 模块，用于方案中的任何路由。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL变量]</td> 
   <td>添加您希望模块设置的变量。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL变量名称] </td> 
   <td>对于每个变量，输入变量名称。 在其他模块中映射变量时，将显示此名称。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL变量值] </td> 
   <td>对于每个变量，输入变量的值。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL变量生命周期] </td> 
   <td> <p>选择希望变量保持有效的时长（保留相同的值）。</p> 
    <ul> 
     <li><strong>[!UICONTROL One Cycle]</strong>:变量对一个周期有效。 当在一个方案运行中收到多个Web挂接时（多个Web挂接=多个周期），此选项非常有用。 </li> 
     <li><strong>[!UICONTROL One Execution]</strong>:变量对于一个方案执行有效。 一个执行可以包含一个或多个循环。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 设置变量]

此模块会创建一个变量，该变量可由路由中的其他模块映射。 变量还可以映射到 [!UICONTROL 获取变量] 或 [!UICONTROL 获取多个变量] 模块，用于方案中的任何路由。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL变量名称] </td> 
   <td>输入变量名称。 在其他模块中映射变量时，将显示此名称。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL变量生命周期] </td> 
   <td> <p>选择希望变量保持有效的时长（保留相同的值）。</p> 
    <ul> 
     <li><strong>[!UICONTROL One Cycle]</strong>:变量对一个周期有效。 当在一个方案运行中收到多个Web挂接时（多个Web挂接=多个周期），此选项非常有用。 </li> 
     <li><strong>[!UICONTROL One Execution]</strong>:变量对于一个方案执行有效。 一个执行可以包含一个或多个循环。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL变量值] </td> 
   <td>输入或映射变量的值。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 睡眠]

此模块允许您将方案流延迟多达300秒（5分钟）。

例如，如果您想要降低 [!DNL target] 服务服务器加载或在发送批量短信或电子邮件时模拟人的行为。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Delay]</p> </td> 
   <td> <p>输入方案将暂停的秒数。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>如果要将流程暂停较长时间，我们建议将方案分为两种方案：
>
>* 第一种方案将在暂停之前包含该部分。
>* 第二种情景将包含其后的部分。
>
>第一种情况是，将所有必需的信息连同当前时间戳一起存储到数据存储中。 第二种方案将定期检查数据存储中是否存在时间戳早于预期延迟的记录，检索记录，完成数据处理并从数据存储中删除记录。
>
>有关数据存储的更多信息，请参阅 [数据存储在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>有关特定数据存储模块的更多信息，请参阅 [[!UICONTROL 数据存储] 模块](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### 聚合器

* [[!UICONTROL 数值聚合器]](#numeric-aggregator)
* [[!UICONTROL 表聚合器]](#table-aggregator)
* [[!UICONTROL 文本聚合器]](#text-aggregator)

#### [!UICONTROL 数值聚合器]

此模块允许您检索数值，然后应用选定函数之一(SUM、AVG、COUNT、MAX、MIN)，并在一个包中返回结果。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL源模块]</p> </td> 
   <td> <p>选择要从中聚合字段的模块。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL聚合函数]</p> </td> 
   <td> <p>选择要用于聚合值的函数。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>定义要将聚合输出分组为的表达式。 此表达式可以包含一个或多个映射的项目。 然后，使用此表达式的值将聚合数据分成组。 每个组以一个键（求值表达式）和一个值（求值）的单独包输出。 您可以在后续模块中将键用作过滤器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL空聚合后停止处理]</td> 
   <td>启用此选项可在没有结果时停止方案。</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL值]</p> </td> 
   <td> <p>输入或映射要聚合的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 表聚合器]

此模块使用指定的列和行分隔符（用于创建表）将来自接收包的选定字段的值合并到单个包中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL源模块]</p> </td> 
   <td> <p>选择要从中聚合字段的模块。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL聚合字段]</td> 
   <td> <p> 从上面选择的模块中选择字段，其中包含要聚合到一个包中的值。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL列分隔符]</p> </td> 
   <td> <p>选择或输入分隔结果包中字段值列的分隔符类型。 如果选择[!UICONTROL Other]，请在分隔符字段中输入要用于分隔值的字符。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL行分隔符]</p> </td> 
   <td> <p>选择或输入分隔结果包中字段值行的分隔符类型。 如果选择[!UICONTROL Other]，请在分隔符字段中输入要用于分隔值的字符。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>定义要将聚合输出分组为的表达式。 此表达式可以包含一个或多个映射的项目。 然后，将使用此表达式的值将聚合数据分为多个组。 每个组以一个键（求值表达式）和一个值（求值）的单独包输出。 您可以在后续模块中将键用作过滤器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL空聚合后停止处理]</td> 
   <td>选择此选项可在没有结果时停止方案。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 文本聚合器]

此模块将接收包的选定字段中的值合并到单个包中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL源模块]</p> </td> 
   <td> <p>选择要从中聚合字段的模块。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL行分隔符]</p> </td> 
   <td> <p>选择或输入分隔结果包中字段值行的分隔符类型。 如果选择[!UICONTROL Other]，请在分隔符字段中输入要用于分隔值的字符。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>定义包含一个或多个映射项目的表达式。 聚合数据在具有相同表达式值的组下进行分隔。 每个组输出为一个单独的包，包含一个键值，该键值具有计算表达式和聚合文本。 通过执行此操作，您可以在后续模块中将密钥用作过滤器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text]</td> 
   <td> <p> 输入或映射希望模块聚合的文本。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL空聚合后停止处理]</td> 
   <td>选择此选项可在没有结果时停止方案。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：** 您可以使用文本聚合器将更多值（例如，客户名称或注释）插入到单个包中，并发送一封包含电子邮件正文或电子邮件主题中所有值的电子邮件。

### 变形金刚

* [[!UICONTROL 撰写字符串]](#compose-a-string)
* [[!UICONTROL 转换文本的编码]](#convert-the-encoding-of-the-text)
* [[!UICONTROL 交换机]](#switch)

#### [!UICONTROL 撰写字符串]

将任何值转换为字符串数据类型（文本）。 在映射（例如，二进制数据）时，这样可以更轻松地进行映射。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p>输入或映射要转换为文本的数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 转换文本的编码]

将输入的输入文本（或二进制数据）转换为所选编码。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL输入数据]</p> </td> 
   <td> <p>输入或映射要转换的内容。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL输入数据代码页]</td> 
   <td> <p>选择输入数据的编码类型。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL输出数据代码页]</p> </td> 
   <td> <p>选择目标（输出）数据的编码类型。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 交换机]

检查输入值是否与提供的值列表匹配。 根据结果返回输出。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input]</p> </td> 
   <td> <p>输入要求计算的表达式。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL使用正则表达式匹配]</td> 
   <td> <p>启用此选项可使用正则表达式。 模块根据正则表达式而不是精确匹配来确定大小写。</p> 
    <div> 
     <p>正则表达式是一系列字符，其中每个字符可以是具有特殊含义的元字符，也可以是具有文字含义的正则字符。 这些字符和元字符标识可用于搜索文本的模式。 例如，如果要搜索名称，可以设置一个正则表达式来搜索由两个以大写字母开头的连续单词组成的模式。 正则表达式是用于搜索和处理文本的强大工具。</p> 
     <p>对正则表达式的讨论不在本条的涵盖范围内。 我们建议使用以下资源：</p> 
     <ul> 
      <li>有关元字符的完整列表，请参阅 <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">正则表达式</a> 在MDN Web文档中。</li> 
      <li>有关如何创建正则表达式的教程，我们建议 <a href="https://regexone.com/">RegexOne</a>.</li> 
      <li>要试用正则表达式，我们建议 <a href="https://regex101.com/">正则表达式101</a> 网站。 在左侧面板中选择ECMAScript(JavaScript)风格。</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL案例] </td> 
   <td> <p>如果输入包含输入到[!UICONTROL Pattern]字段的值，则返回输入到[!UICONTROL Output]字段的值。</p> <p>如果输入与在[!UICONTROL Pattern]字段中设置的任何值都不匹配，则会出现以下情况之一：</p> 
    <ul> 
     <li>将返回[!UICONTROL Else]字段的值</li> 
     <li>如果[!UICONTROL Else]字段中没有值，则不会返回任何输出。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>输入在“案例”字段中设置的条件未满足时返回的值。 </p> </td> 
  </tr> 
 </tbody> 
</table>
