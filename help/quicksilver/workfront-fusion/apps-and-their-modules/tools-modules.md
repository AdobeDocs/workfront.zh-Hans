---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 工具
description: 此 [!DNL Adobe Workfront Fusion Tools] 部分包含几个可增强场景的有用模块。
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2290'
ht-degree: 0%

---

# [!UICONTROL 工具]

此 [!DNL Adobe Workfront Fusion Tools] 部分包含几个可增强场景的有用模块。

[!UICONTROL 工具] 模块可从应用程序列表中获得，也可从 [!UICONTROL 工具] 图标 ![](assets/tools-icon-small.png) 在屏幕底部。

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
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr>
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 工具] 和他们的领域

* [触发器](#triggers)
* [操作](#actions)
* [汇总](#aggregators)
* [转换器](#transformers)

### 触发器

#### [!UICONTROL 基本触发器]

利用此模块，可创建自定义触发器并定义其输入包。

例如，您可以将此模块用于安排发送到指定电子邮件地址的联系人或任何其他列表(例如 [!UICONTROL 电子邮件] >[!UICONTROL 发送电子邮件]，或 [!DNL Gmail] >[!UICONTROL 发送电子邮件] 模块)，或作为简单提醒，以便在您需要时触发。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL包]</td> 
   <td> <p>通过添加数组项创建自定义包。 数组由名称 — 值对组成。</p> </td> 
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

此模块检索之前由创建的值 [!UICONTROL 设置变量] 或 [!UICONTROL 设置多个变量] 模块。

此模块可以读取在场景中的任意位置设置的变量，即使该变量是在不同的路由中设置的，而 [!UICONTROL 获取多个变量] 找到模块。 唯一的要求是 [!UICONTROL 工具] > [!UICONTROL 设置变量] 或 [!UICONTROL 工具] > [!UICONTROL 设置多个变量] 模块在以下位置之前执行： [!UICONTROL 工具] > [!UICONTROL 获取多个变量] 模块。 有关模块执行顺序的更多信息，请参阅 [中的路由器模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL变量]</td>
        <td>添加您希望模块获取的变量。</td>
    </tr>
    <tr>
        <td>[！UICONTROL变量名称]</td>
        <td>对于您添加的每个变量，映射您要获取的变量的名称。</td>
    </tr>
</table>

>[!INFO]
>
>**示例：**  以下是可使用的 [!UICONTROL 设置]/[!UICONTROL 获取多个变量] 模块：
>
>* 用于存储计算值以供以后使用，即使是在不同的路由中。 当值在多个模块中使用并且用于计算值的公式过于复杂时，此变量将非常有用。
>* 调试公式。 如果模块中使用的公式似乎未提供正确结果，请复制该公式并将其粘贴到 [!UICONTROL 设置变量] 您在相关模块之前插入的模块。 断开模块连接。 [!UICONTROL 设置变量] 模块并执行场景。 验证 [!UICONTROL 设置变量] 模块的输出，调整或简化公式，再次执行场景，并继续执行该操作直到问题得到解决。


#### [!UICONTROL 获取变量]

此模块可检索之前由创建的值 [!UICONTROL 设置变量] 或 [!UICONTROL 设置多个变量] 模块。

此模块可以读取在场景中的任意位置设置的变量，即使该变量是在不同的路由中设置的，而 [!UICONTROL 获取变量] 找到模块。 唯一的要求是 [!UICONTROL 工具] > [!UICONTROL 设置变量] 或 [!UICONTROL 工具] > [!UICONTROL 设置多个变量] 模块在以下位置之前执行： [!UICONTROL 工具] > [!UICONTROL 获取变量] 模块。 有关模块执行顺序的更多信息，请参阅 [中的路由器模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL变量名称]</td> 
   <td> <p>映射您希望模块获取的变量的名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 增量函数]

每个模块运行后，此模块会返回一个以1为单位的值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL重置值]</td> 
   <td> <p>选择您希望模块递增值的时间。 </p> 
    <ul> 
     <li>[！UICONTROL After One cycle]</li> 
     <li>[！UICONTROL After one scenario run]</li> 
     <li>[！UICONTROL从不]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例:**
>
>该模块的用途之一是实现任务、商机、电子邮件等的“轮询”分配，以提供给群组中的用户。 算法按照一定的合理顺序从一组中选择被分配人，通常是从列表的顶部到底部。 当算法到达列表结尾时，它将给位于列表顶部的用户下一个分配，并继续沿列表进行分配。
>
>以下方案会向运行奇数方案的第一个收件人发送电子邮件，并向运行偶数方案的第二个收件人发送电子邮件。
>
>![](assets/example-email-350x246.gif)
>
>1. 要创建此方案，请执行以下操作：
>1. 设置模块的 **[!UICONTROL 重置值]** 字段为从不。
>1. 为奇数值设置路由。 使用等于的模数数学函数设置此路由的过滤器 `1`：
>
>   ![](assets/odd-350x459.png)
>
>  **注释**：别忘了更改 [!UICONTROL 等于] 默认设置中的运算符 [!UICONTROL 文本] 运算符到 [!UICONTROL 数值] 运算符。
>
>1. 使用等于的模数数学函数为偶数值设置路由 `0`：
>
>增量函数在每次场景运行时都添加一个。 过滤器会检查增量并根据其值执行操作，以确保电子邮件均匀分布。

#### [!UICONTROL 设置多个变量]

此模块创建可由路由中的其他模块映射的变量。 变量也可以映射到 [!UICONTROL 获取变量] 或 [!UICONTROL 获取多个变量] 场景中任意路由的模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL变量]</td> 
   <td>添加您希望模块设置的变量。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL变量名称] </td> 
   <td>对于每个变量，输入变量名称。 在其他模块中映射变量时，将显示此名称。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL变量值] </td> 
   <td>对于每个变量，输入变量的值。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL变量生命周期] </td> 
   <td> <p>选择您希望变量保持有效的时长（保持相同的值）。</p> 
    <ul> 
     <li><strong>[！UICONTROL One cycle]</strong>：变量在一个周期内有效。 在收到一个场景运行中的多个Webhook时（更多Webhook =更多周期）非常有用。 </li> 
     <li><strong>[！UICONTROL One execution]</strong>：变量对一个场景执行有效。 一个执行可以包含一个或多个周期。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 设置变量]

此模块创建一个可由路由中的其他模块映射的变量。 变量也可以映射到 [!UICONTROL 获取变量] 或 [!UICONTROL 获取多个变量] 场景中任意路由的模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL变量名称] </td> 
   <td>输入变量名称。 在其他模块中映射变量时，将显示此名称。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL变量生命周期] </td> 
   <td> <p>选择您希望变量保持有效的时长（保持相同的值）。</p> 
    <ul> 
     <li><strong>[！UICONTROL One cycle]</strong>：变量在一个周期内有效。 在收到一个场景运行中的多个Webhook时（更多Webhook =更多周期）非常有用。 </li> 
     <li><strong>[！UICONTROL One execution]</strong>：变量对一个场景执行有效。 一个执行可以包含一个或多个周期。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL变量值] </td> 
   <td>输入或映射变量的值。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 睡眠]

利用此模块，可将方案流延迟最多300秒（5分钟）。

例如，如果要降低 [!DNL target] 加载服务服务器或模拟发送批量短信或电子邮件时的人类行为。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL延迟]</p> </td> 
   <td> <p>输入方案将暂停的秒数。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>如果您希望将流量暂停更长时间，我们建议将您的方案拆分为两个方案：
>
>* 第一个方案将包含暂停前的部分。
>* 第二个方案将包含其后的部分。
>
>第一种情形的结果是，将所有必需的信息连同当前时间戳一起存储在一个数据存储中。 第二种方案将定期检查数据存储中是否存在时间戳早于预期延迟的记录，检索记录，完成数据的处理，并从数据存储中删除记录。
>
>有关数据存储的详细信息，请参阅 [数据存储位置 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>有关特定数据存储模块的更多信息，请参阅 [[!UICONTROL 数据存储] 模块](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### 汇总

* [[!UICONTROL 数值汇总]](#numeric-aggregator)
* [[!UICONTROL 表格汇总]](#table-aggregator)
* [[!UICONTROL 文本汇总]](#text-aggregator)

#### [!UICONTROL 数值汇总]

利用此模块，可检索数值，然后应用选定的函数之一(SUM、AVG、COUNT、MAX、MIN)，并将结果返回一个捆绑包中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL源模块]</p> </td> 
   <td> <p>选择要从中聚合字段的模块。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL聚合函数]</p> </td> 
   <td> <p>选择要用于聚合值的函数。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL分组依据]</p> </td> 
   <td> <p>定义要将聚合输出分组依据的表达式。 此表达式可以包含一个或多个映射项。 然后，使用此表达式的值将聚合的数据分成多个组。 每个组输出为一个单独的捆绑，其中包含键（求得的表达式）和值（聚合值）。 您可以在后续模块中将该键用作过滤器。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL停止处理空聚合]</td> 
   <td>启用此选项可在没有结果时停止场景。</td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL值]</p> </td> 
   <td> <p>输入或映射要聚合的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 表格汇总]

此模块使用指定的列和行分隔符（允许您创建表）将接收捆绑的选定字段中的值合并到单个捆绑中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL源模块]</p> </td> 
   <td> <p>选择要从中聚合字段的模块。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL聚合字段]</td> 
   <td> <p> 从上面选择的模块中选择包含要聚合到一个捆绑包中的值的字段。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL列分隔符]</p> </td> 
   <td> <p>选择或输入分隔符类型，该分隔符将分隔结果包中的字段值列。 如果选择[！UICONTROL其他]，则在分隔符字段中输入要将值分隔的字符。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL行分隔符]</p> </td> 
   <td> <p>选择或输入分隔符类型，该分隔符将分隔结果捆绑中的字段值行。 如果选择[！UICONTROL其他]，则在分隔符字段中输入要将值分隔的字符。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL分组依据]</p> </td> 
   <td> <p>定义要将聚合输出分组依据的表达式。 此表达式可以包含一个或多个映射项。 然后，将使用此表达式的值将聚合的数据分成不同的组。 每个组输出为一个单独的捆绑，其中包含键（求得的表达式）和值（聚合值）。 您可以在后续模块中将该键用作过滤器。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL停止处理空聚合]</td> 
   <td>选择此选项可在没有结果时停止方案。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 文本汇总]

此模块将接收捆绑的选定字段中的值合并到单个捆绑中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL源模块]</p> </td> 
   <td> <p>选择要从中聚合字段的模块。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL行分隔符]</p> </td> 
   <td> <p>选择或输入分隔符类型，该分隔符将分隔结果捆绑中的字段值行。 如果选择[！UICONTROL其他]，则在分隔符字段中输入要将值分隔的字符。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL分组依据]</p> </td> 
   <td> <p>定义包含一个或多个映射项的表达式。 聚合的数据用同一表达式的值分显示在组下。 每个组输出为一个单独的捆绑，其中包含带有计算表达式的键和聚合文本。 这样，您便可以将键用作后续模块中的筛选条件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文本]</td> 
   <td> <p> 输入或映射您希望模块聚合的文本。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL停止处理空聚合]</td> 
   <td>选择此选项可在没有结果时停止方案。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：** 您可以使用文本聚合将更多值（例如，客户名称或注释）插入到单个包中，并发送一封包含电子邮件正文或电子邮件主题中所有值的电子邮件。

### 转换器

* [[!UICONTROL 撰写字符串]](#compose-a-string)
* [[!UICONTROL 转换文本的编码]](#convert-the-encoding-of-the-text)
* [[!UICONTROL 切换]](#switch)

#### [!UICONTROL 撰写字符串]

将任意值转换为字符串数据类型（文本）。 映射时（例如，映射二进制数据），它使映射更容易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL文本]</td> 
   <td> <p>输入或映射要转换为文本的数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 转换文本的编码]

将输入的输入文本（或二进制数据）转换为所选的编码。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL输入数据]</p> </td> 
   <td> <p>输入或映射要转换的内容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL输入数据代码页]</td> 
   <td> <p>选择输入数据的编码类型。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL输出数据代码页]</p> </td> 
   <td> <p>选择目标（输出）数据的编码类型。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 切换]

检查输入值是否与提供的值列表匹配。 根据结果返回输出。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL输入]</p> </td> 
   <td> <p>输入要计算的表达式。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL使用正则表达式进行匹配]</td> 
   <td> <p>启用此选项可使用正则表达式。 模块根据正则表达式确定大小写，而不是完全匹配。</p> 
    <div> 
     <p>正则表达式是一系列字符，其中每个字符要么是具有特殊意义的元字符，要么是具有文字意义的正则字符。 这些字符和元字符标识了可用于搜索文本的模式。 例如，如果要搜索名称，可以设置正则表达式来搜索由两个以大写字母开头的连续单词组成的模式。 正则表达式是用于搜索和处理文本的强大工具。</p> 
     <p>对正则表达式的讨论超出了本文的范围。 我们建议使用以下资源：</p> 
     <ul> 
      <li>有关元字符的完整列表，请参见 <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">正则表达式</a> MDN Web文档中的。</li> 
      <li>有关如何创建正则表达式的教程，我们建议 <a href="https://regexone.com/">正则表达式</a>.</li> 
      <li>为了试验正则表达式，我们建议 <a href="https://regex101.com/">正则表达式101</a> 网站。 在左侧面板中选择ECMAScript (JavaScript) FLAVOR。</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL用例] </td> 
   <td> <p>如果输入包含输入到[！UICONTROL模式]字段中的值，则会返回输入到[！UICONTROL输出]字段中的值。</p> <p>如果输入与您在[！UICONTROL模式]字段中设置的任何值都不匹配，则会出现以下情况之一：</p> 
    <ul> 
     <li>返回[！UICONTROL Else]字段中的值</li> 
     <li>如果[！UICONTROL Else]字段中没有值，则不会返回任何输出。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Else]</p> </td> 
   <td> <p>输入当不符合案例字段中设置的标准时返回的值。 </p> </td> 
  </tr> 
 </tbody> 
</table>
