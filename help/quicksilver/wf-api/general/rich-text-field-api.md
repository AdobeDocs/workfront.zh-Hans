---
content-type: api
navigation-topic: general-api
title: Adobe Workfront API中的富文本字段
description: Adobe Workfront API中的富文本字段
author: John
feature: Workfront API
exl-id: 67fc34dc-0722-4419-8254-0371ad5abfc3
source-git-commit: 40698643b0fa530b38da465f3bc1e4d841fcc190
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---


# Adobe Workfront API中的富文本字段

Adobe Workfront中的某些对象允许存储富文本格式的文本。 在Workfront API中，使用开源框架Draft.js将富文本存储为JSON。

## 概述示例

调用具有富文本格式的自定义字段 **包含富文本的字段** 和可以关联以下值：

![](assets/rich-text-example-350x158.png)

**示例：** 用于检索自定义表单字段值的基本GET请求 **包含富文本的字段**:

<!-- [Copy](javascript:void(0);) -->
<pre><OBJ Code><OBJ ID><OBJ Code><OBJ ID></pre>

**示例：** 此请求将返回 **包含富文本的字段** 存储在 **parameterValue** **DE：富文本字段**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

**示例：** 这是上图所显示的格式化响应版本

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

## 块

存储富文本内容的JSON对象由两个主要部分组成： **块** 和 **entityMaps**.

块是表示单行带格式文本的JSON对象。 由于单个自定义字段可以有多行文本，因此每行文本都有其自己的块，并且每个块都表示为一个名为的父数组中的元素 **块**.

**示例：** 在此，自定义字段中的每行文本都映射到数组块中的块元素

![](assets/copy-of-rich-text-mapping-350x159.png)

由于每个块元素也是JSON对象，因此每个块都由以下元素组成： **key**, **文本**, **type**, **深度**, **inlineStyleRanges**, **entityRanges**&#x200B;和 **数据**. 其中每个元素的作用如下所示：

* **键** 是该块的唯一标识符。 键用于通过entityMaps映射文本行。 有关entityMaps的详细信息，请参阅此文档的entityMaps部分。
* **文本** 是从自定义字段中存储的文本内容行。
* **类型** 描述所表示的文本类型。 例如，存储在块中的文本行可能是列表的一部分。 如果该行文本是未排序列表的一部分，则其类型将定义为：未排序列表项。
* 目前不支持列表，但应该很快会提供。
* **深度** 当行是有序或无序列表的嵌套部分时，此参数定义行的深度。
* **inlineStyleRanges** 是一个数组，用于描述应用于由当前块表示的文本行的格式类型。

**示例：** 以下是一个inlineStyleRanges数组，用于描述字符级别的每种样式。 在这种情况下：9个字符(长度：9)从索引0开始(偏移：0)有风格 **粗体** 已应用：

![](assets/copy-of-rich-text-mapping-2-350x136.png)

如果将多种类型的格式应用于单行，则样式将映射到** inlineStyleRanges**数组中的其他元素。

**示例：** 以下是存储包含混合格式的一行文本时块的样子： **粗体文本和斜体**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

>[!NOTE]
>
>20.3版本之后的所有版本都将支持粗体、斜体和下划线格式选项。

## entityMaps和entityRanges

数据块可能包含超链接或其他类型的格式化格式等实体，这些实体连接到位于自定义文本字段外的数据源。

## 示例

### 从JSON检索纯文本

提交具有富文本格式的自定义字段时，所有文本都存储在数组中 **块**. 但是，全文的每一行都存储在 **文本参数** 组成父数组的每个单独块元素内 **块**. 因此，为了检索全文，需要提取每一行单独的文本，并将其分段回去。 可以通过循环遍历块中的所有元素并使用行分隔符(\n)将每个文本参数连接在一起来实现这一点。

**示例：** 以下是您的JS的样子：

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

### 使用Workfront API保存富文本字段值

要使用Workfront API保存富文本字段的以下值，请执行以下操作：
<pre>
		Hello <strong>世界</strong>!!!
		这是我的第一个 <strong>富文本</strong></pre>

1. 构建JSON，该JSON表示您尝试通过将每行文本组织到数组中的块元素来捕获的富文本字段的值 **块**

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 使用 **inlineStyleRanges** 参数

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 要捕获第二行，文本“富文本”必须同时使用粗体和斜体格式。

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

   >[!NOTE]
   >
   >虽然初始版本期间不支持entityMap功能，但在请求中传递此JSON仍是必填字段

1. 使用 **字符串** 方法来生成 **PUT** 请求和发送更新

   <!-- [Copy](javascript:void(0);) -->
   <pre><OBJ Code><OBJ ID></pre>
