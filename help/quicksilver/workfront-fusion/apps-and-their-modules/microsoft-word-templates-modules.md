---
filename: microsoft-word-templates-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Microsoft Word模板模块
description: 在Adobe Workfront Fusion场景中，您可以自动执行使用Microsoft Word模板的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
source-git-commit: 43b64d1371438909063d2ac81cccb90b97179dfc
workflow-type: tm+mt
source-wordcount: '1286'
ht-degree: 0%

---


# [!DNL Microsoft Word Template] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Microsoft Word Templates]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> 
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

为了使用 [!DNL Miscrosoft Word Templates] with [!DNL Adobe Workfront Fusion]，则需要具有 [!DNL Office 365] 帐户。 您可以在www.office.com上创建一个。

## 使用 [!DNL Microsoft Word Templates] 模块

您可以使用 [!DNL Microsoft Word Template] 将来自多个web服务的数据合并到中的模块 [!DNL Microsoft Word] 文档。

例如，您可以使用 [!DNL Microsoft Word] 模板：

![](assets/word-template-before-filled-350x62.png)

要创建此文档，请执行以下操作：

![](assets/word-template-exampled-filled-350x85.png)

## 关于值标记

A [!DNL Microsoft Word] 模板是常规模板 [!DNL Microsoft Word] 文档（.docx文件）的文本中带有特殊标记，可确定合并或填充数据的位置和方式。 标记有三种类型：

* [简单值标记](#simple-value-tag)
* [条件标记](#condition-tag)
* [循环标记](#loop-tag)

### 简单值标记 {#simple-value-tag}

简单值标记只会被替换为相应的值。 标记的名称与 [!UICONTROL 键] 字段的值，它位于双大括号内；例如，


<pre>{{name}}</pre>


。

**示例：** 要创建一个“嗨，Petr！”的文档，您可以使用 [!DNL Microsoft Word Template] 模块以创建以下模板：

<pre>&gt;嗨{name}}!</pre>

为此，您应按如下方式设置模块：

![](assets/word-template-simple-value-350x286.png)

### 条件标记 {#condition-tag}

您可以使用条件标记来换行仅在满足特定条件时才应呈现的文本。 要隐藏文本，请将其置于开始和结束条件标记之间，如“hasPhone”（条件为数据是否包含电话号码）。 开始标记的名称前面附加有井号#，结束标记的名称前面附加有斜杠/，如以下示例所示。

**示例：** 要生成包含客户电话号码的文档（如果输入数据包含电话号码，但没有电子邮件地址），您可以使用 [!DNL Microsoft Word Template] 模块并创建以下模板：
<pre>&gt; {{#hasPhone}}电话：{{phone}} {{/hasPhone}}</pre><pre>&gt; {{#hasEmail}}电子邮件：{{email}} {{/hasEmail}}</pre>为此，您应按如下方式设置模块：

![](assets/word-template-conditional-350x501.png)

在文档中，电话号码将如下所示：
<pre>&gt;电话：4445551234</pre>

### 循环标记 {#loop-tag}

您可以使用循环标记（也称为区域标记）来重复文本的区域。 将文本置于开始和结束循环标记之间，以环绕文本。 开始标记的名称前面加有井号#;结束标记的名称前面加有斜杠/。

* [使用“填写文档”模块循环标记](#loop-tag-with-fill-out-a-document-module)

<!-- [Loop tag with Fill a document with a batch of data module](#loop-tag-with-fill-a-document-with-a-batch-of-data-module)-->

#### 使用“填写文档”模块循环标记 {#loop-tag-with-fill-out-a-document-module}

**示例：** 要生成列出客户列表中每个联系人的姓名和电话号码的文档，您可以使用 [!DNL Microsoft Word Template] 模块并创建以下模板：

<pre>&gt; {{#contact}}</pre><pre>&gt; {{name}}, {{phone}}</pre><pre>&gt; {{/contact}}</pre>

为此，您应按如下方式设置模块：


![](assets/word-template-fill-out-a-document-350x732.png)

该模块将创建以下文档：

```
> Jan Toman, 4445551234
> Eduard Salo, 4445552345
```

<!--

#### Loop tag with Fill a document with a batch of data module {#loop-tag-with-fill-a-document-with-a-batch-of-data-module}

**Example:** You can export Google contacts into a table that you create using loop tags.

The first module loads the template. The next module retrieves all contacts from the group you specify in [!DNL Google Contacts]. The aggregator module aggregates all values retrieved from Google Contacts and merges them into the template. And the last module saves the filled template to the desired location.

![](assets/word-template-batch-scenario-350x124.png)

You could use this scenario with the following template:

![](assets/word-template-batch-template-350x26.png)

To do this, you would set up the module as follows:

![](assets/word-template-batch-module-setup-350x323.png)

The module would create the following document:

![](assets/word-template-batch-document-350x46.png)
-->

## [!DNL Microsoft Word Template] 模块

这些模块不需要连接。

* [填写文档](#fill-out-a-document)
* [用一批数据填写文档](#fill-a-document-with-a-batch-of-data)

### [!UICONTROL 填写文档] {#fill-out-a-document}

利用此变压器模块，可使用您指定的数据填充文档。 它可与简单值标记、条件标记或循环标记一起使用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL要替换的文本的开始分隔符]</td> 
   <td> <p>输入要标记替换文本开头的字符。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>输入 <code>[[</code> 如果要替换类似于以下文本的文本： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL替换文本的结束分隔符]</p> </td> 
   <td> <p>输入要标记替换文本结尾的字符。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>输入 <code>]]</code> 如果要替换类似于以下文本的文本： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p> 映射要从上一个模块上传的文件(例如，“HTTP”&gt;“获取文件”或“Dropbox”&gt;“获取文件”模块)。 或者手动输入数据文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL已填写文件的名称]</td> 
   <td>输入目标输出文件的文件名（包括扩展名）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL数据源]</td> 
   <td> <p>选择一个选项，以指示您使用的数据是来自表单还是来自原始数据收集（未处理的计算机数据）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL值]</td> 
   <td> <p>这必须是集合数组，其中：</p> 
    <ul> 
     <li>每个集合对应一个数据条目，并包含一个项目 <code>entry</code></li> 
     <li>项目 <code>entry </code>包含 <code>key </code>和 <code>value</code></li> 
     <li>项目 <code>key </code>包含标记的名称</li> 
     <li>项目 <code>value </code>包含标记的值</li> 
    </ul> 
    <p>添加条目：</p>
    <ol> 
     <li> 单击 <b>[!UICONTROL Add Item]</b>. </li> 
     <li>选择条目的值类型。</li> 
     <li>添加名称和值。 有关更多信息，请参阅本文中所选值类型的示例。 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">简单值标记</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">条件标记</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">循环标记</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 用一批数据填写文档] {#fill-a-document-with-a-batch-of-data}

如果您的数据条目作为单独的包，则此聚合模块非常有用。 通过此模块，您可以轻松设置“值”字段所需的结构，并将项目映射到每个值项目。 与“填写文档”模块不同，“使用批量数据模块填充文档”中的“值”字段仅允许包含变量的单个条目。

如果您的数据条目是数组，则也可以使用 *迭代器* 模块，将数组的内容转换为一系列包。

将为每个传入包创建并填充实际值。 在处理所有输入包后会生成模板。

此聚合模块对于创建列表或报告特别有用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模块]</td> 
   <td>选择文本源的模块。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL要替换的文本的开始分隔符]</td> 
   <td> <p>输入要标记替换文本开头的字符。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>输入 <code>[[</code> 如果要替换类似于以下文本的文本： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL替换文本的结束分隔符]</p> </td> 
   <td> <p>输入要标记替换文本结尾的字符。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>输入 <code>]]</code> 如果要替换类似于以下文本的文本： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by]</td> 
   <td> 定义包含一个或多个映射项目的表达式。 聚合数据在具有相同表达式值的组下进行分隔。 每个组输出为一个单独的包，包含一个键值，该键值具有计算表达式和聚合文本。 通过执行此操作，您可以在后续模块中将密钥用作过滤器。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL空聚合后停止处理]</td> 
   <td>启用此选项可在聚合不包含包时停止处理。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p> 映射要从上一个模块上传的文件(例如，“HTTP”&gt;“获取文件”或“Dropbox”&gt;“获取文件”模块)。 或者手动输入数据文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL已填写文件的名称]</td> 
   <td>输入目标输出文件的文件名（包括扩展名）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL数据源]</td> 
   <td> <p>选择一个选项，以指示您使用的数据是来自表单还是来自原始数据收集（未处理的计算机数据）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL值]</td> 
   <td> <p>这必须是集合数组，其中：</p> 
    <ul> 
     <li>每个集合对应一个数据条目，并包含一个项目 <code>entry</code></li> 
     <li>项目 <code>entry </code>包含 <code>key </code>和 <code>value</code></li> 
     <li>项目 <code>key </code>包含标记的名称</li> 
     <li>项目 <code>value </code>包含标记的值</li> 
    </ul> 
    <p>添加条目：</p>
    <ol> 
     <li> 单击 <b>[!UICONTROL Add Item]</b>. </li> 
     <li>选择条目的值类型。</li> 
     <li>添加名称和值。 有关更多信息，请参阅本文中所选值类型的示例。 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">简单值标记</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">条件标记</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">循环标记</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

