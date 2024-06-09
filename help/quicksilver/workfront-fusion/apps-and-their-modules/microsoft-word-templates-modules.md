---
filename: microsoft-word-templates-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Microsoft Word Template模块
description: 在Adobe Workfront Fusion场景中，您可以自动使用Microsoft Word模板的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 889b417c-04a9-4dbf-9a34-0dab65f11f03
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 0%

---

# [!DNL Microsoft Word Template] 模块

在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用 [!DNL Microsoft Word Templates]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
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

要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

要使用 [!DNL Miscrosoft Word Templates] 替换为 [!DNL Adobe Workfront Fusion]，则必须拥有 [!DNL Office 365] 帐户。 您可以在www.office.com创建一个。



## 连接 [!DNL Office] 服务对象 [!DNL Workfront Fusion]

有关连接 [!DNL Office] 帐户至 [!UICONTROL Workfront Fusion]，请参见 [创建与的连接 [!UICONTROL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>某些Microsoft应用程序使用相同的连接，该连接与单个用户权限相关联。 因此，在创建连接时，权限同意屏幕除了显示当前应用程序所需的任何新权限外，还会显示以前授予此用户连接的任何权限。
>
>例如，如果用户拥有通过Excel Connector授予的“读取表”权限，然后在Outlook Connector中创建连接以读取电子邮件，则权限同意屏幕将显示已授予的“读取表”权限和新要求的“写入电子邮件”权限。

## 使用 [!DNL Microsoft Word Templates] 模块

您可以使用 [!DNL Microsoft Word Template] 用于将多个Web服务中的数据合并到中的模块 [!DNL Microsoft Word] 文档。

例如，您可以使用此 [!DNL Microsoft Word] 模板：

![](assets/word-template-before-filled-350x62.png)

要创建此文档，请执行以下操作：

![](assets/word-template-exampled-filled-350x85.png)

## 关于值标记

A [!DNL Microsoft Word] 模板是常规模板 [!DNL Microsoft Word] 文档（.docx文件），其文本中包含特殊标记，这些标记可确定合并或填充数据的位置和方法。 有三种类型的标记：

* [简单值标记](#simple-value-tag)
* [条件标记](#condition-tag)
* [循环标记](#loop-tag)

### 简单值标记 {#simple-value-tag}

简单值标记被简单地替换为相应的值。 标记的名称对应于 [!UICONTROL 键] 字段的值，放置在双大括号内；例如，


<pre>&lbrace;&lbrace;name&rbrace;&rbrace;</pre>


。

**示例：** 要创建显示“嗨，彼得！”的文档，您可以使用 [!DNL Microsoft Word Template] 模块创建以下模板：

<pre>&gt;您好 &lbrace;&lbrace;name&rbrace;&rbrace;！</pre>

为此，您需要按如下方式设置模块：

![](assets/word-template-simple-value-350x286.png)

### 条件标记 {#condition-tag}

您可以使用条件标记对文本进行换行，这些文本仅在满足某些条件时才应呈现。 要换行文本，请将文本置于开始和结束条件标记之间，例如“hasPhone”（如果条件为数据是否包含电话号码）。 开始标记的名称前面加有井号#，结束标记的名称前面加有斜杠/，如下面的示例所示。

**示例：** 要生成包含客户电话号码的文档（如果输入数据包含电话号码但没有电子邮件地址），您可以使用 [!DNL Microsoft Word Template] 模块并创建以下模板：
<pre>&gt; &lbrace;&lbrace;#hasPhone&rbrace;&rbrace;电话： &lbrace;&lbrace;phone&rbrace;&rbrace; &lbrace;&lbrace;/hasPhone&rbrace;&rbrace;</pre><pre>&gt; &lbrace;&lbrace;#hasEmail&rbrace;&rbrace;电子邮件： &lbrace;&lbrace;email&rbrace;&rbrace; &lbrace;&lbrace;/hasEmail&rbrace;&rbrace;</pre>为此，您需要按如下方式设置模块：

![](assets/word-template-conditional-350x501.png)

在文档中，电话号码显示如下：
<pre>&gt;电话： 4445551234</pre>

### 循环标记 {#loop-tag}

您可以使用循环标签（也称为节标签）来重复文本节。 通过将文本置于开始和结束循环标记之间来绕排文本。 开始标记的名称前面加有井号#；结束标记的名称前面加有斜杠/。

* [使用填写文档模块循环标记](#loop-tag-with-fill-out-a-document-module)
  <!-- [Loop tag with Fill a document with a batch of data module](#loop-tag-with-fill-a-document-with-a-batch-of-data-module)-->

#### 使用填写文档模块循环标记 {#loop-tag-with-fill-out-a-document-module}

**示例：** 要生成列出客户列表中每个联系人的姓名和电话号码的文档，您可以使用 [!DNL Microsoft Word Template] 模块并创建以下模板：

<pre>&gt; &lbrace;&lbrace;#contact&rbrace;&rbrace;</pre><pre>&gt;     &lbrace;&lbrace;name&rbrace;&rbrace;， &lbrace;&lbrace;phone&rbrace;&rbrace;</pre><pre>&gt; &lbrace;&lbrace;/contact&rbrace;&rbrace;</pre>

为此，您需要按如下方式设置模块：


![](assets/word-template-fill-out-a-document-350x732.png)

模块将创建以下文档：

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
* [使用批量数据填充文档](#fill-a-document-with-a-batch-of-data)

### [!UICONTROL 填写文档] {#fill-out-a-document}

此转换器模块允许您使用指定的数据填充文档。 它可以与简单值标记、条件标记或循环标记一起使用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL要替换的文本的起始分隔符]</td> 
   <td> <p>输入要标记替换文本开头的字符。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>输入 <code>[[</code> 如果要替换类似于以下内容的文本： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL要替换的文本的结束分隔符]</p> </td> 
   <td> <p>输入要标记替换文本结尾的字符。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>输入 <code>]]</code> 如果要替换类似于以下内容的文本： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p> 映射您要从上一个模块上传的文件(例如，HTTP &gt;获取文件或Dropbox&gt;获取文件模块)。 或者手动输入数据文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL已填写文件的名称]</td> 
   <td>为目标输出文件输入文件名（包括扩展名）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL数据源]</td> 
   <td> <p>选择一个选项以指示您正在使用的数据是来自表单还是原始数据收集（未处理的计算机数据）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Values]</td> 
   <td> <p>这必须是集合数组，其中：</p> 
    <ul> 
     <li>每个收藏集对应于一个数据条目并包含一个项目 <code>entry</code></li> 
     <li>项目 <code>entry </code>包含 <code>key </code>和 <code>value</code></li> 
     <li>项目 <code>key </code>包含标记的名称</li> 
     <li>项目 <code>value </code>包含标记的值</li> 
    </ul> 
    <p>要添加条目，请执行以下操作：</p>
    <ol> 
     <li> 单击 <b>[！UICONTROL添加项]</b>. </li> 
     <li>选择条目的值类型。</li> 
     <li>添加名称和值。 有关更多信息，请参阅本文所选值类型的示例。 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">简单值标记</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">条件标记</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">循环标记</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 使用批量数据填充文档] {#fill-a-document-with-a-batch-of-data}

如果您的数据条目作为单独的捆绑包，此聚合器模块非常有用。 利用此模块，您可以轻松设置值字段所需的结构，并将其项映射到每个值项。 与填写文档模块相反，使用批量数据模块填写文档中的值字段仅允许包含变量的单个条目。

如果数据条目以数组形式提供，则也可以使用此模块，方法是使用 *迭代器* 模块，用于将数组的内容转换为一系列捆绑包。

为每个传入包创建和填充实际值。 处理完所有输入捆绑包后会生成模板。

此聚合器模块对于创建列表或报告特别有用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL源模块]</td> 
   <td>选择作为文本源的模块。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL要替换的文本的起始分隔符]</td> 
   <td> <p>输入要标记替换文本开头的字符。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>输入 <code>[[</code> 如果要替换类似于以下内容的文本： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL要替换的文本的结束分隔符]</p> </td> 
   <td> <p>输入要标记替换文本结尾的字符。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>输入 <code>]]</code> 如果要替换类似于以下内容的文本： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL分组依据]</td> 
   <td> 定义包含一个或多个映射项的表达式。 聚合的数据用同一表达式的值在“组”下分隔。 每个组输出为一个单独的包，其中包含带有已计算表达式的键和聚合文本。 这样，您就可以在后续模块中将键用作过滤器。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL在出现空聚合后停止处理]</td> 
   <td>启用此选项可在聚合不包含任何捆绑包时停止处理。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p> 映射您要从上一个模块上传的文件(例如，HTTP &gt;获取文件或Dropbox&gt;获取文件模块)。 或者手动输入数据文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL已填写文件的名称]</td> 
   <td>为目标输出文件输入文件名（包括扩展名）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL数据源]</td> 
   <td> <p>选择一个选项以指示您正在使用的数据是来自表单还是原始数据收集（未处理的计算机数据）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Values]</td> 
   <td> <p>这必须是集合数组，其中：</p> 
    <ul> 
     <li>每个收藏集对应于一个数据条目并包含一个项目 <code>entry</code></li> 
     <li>项目 <code>entry </code>包含 <code>key </code>和 <code>value</code></li> 
     <li>项目 <code>key </code>包含标记的名称</li> 
     <li>项目 <code>value </code>包含标记的值</li> 
    </ul> 
    <p>要添加条目，请执行以下操作：</p>
    <ol> 
     <li> 单击 <b>[！UICONTROL添加项]</b>. </li> 
     <li>选择条目的值类型。</li> 
     <li>添加名称和值。 有关更多信息，请参阅本文所选值类型的示例。 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">简单值标记</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">条件标记</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">循环标记</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>
