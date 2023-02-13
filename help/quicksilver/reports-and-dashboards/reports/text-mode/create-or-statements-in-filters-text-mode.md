---
product-area: reporting
navigation-topic: text-mode-reporting
title: 在文本模式筛选器中创建“OR”语句
description: 在列表和报表中创建过滤器时，可以包含多个语句。
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 在文本模式筛选器中创建“OR”语句

在列表和报表中创建过滤器时，可以包含多个语句。

有关创建过滤器的信息，请参阅以下文章：

* [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [使用文本模式编辑过滤器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## 文本模式筛选器运算符

有关标准过滤器界面中Adobe Workfront过滤器运算符的信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront有2个过滤器运算符，用于连接每个过滤器语句：

* **和**:当使用AND运算符连接2 filter语句时，您表示希望同时满足两个filter语句。

   默认情况下，过滤器中的语句使用AND运算符联接。

   在文本模式界面中构建AND过滤器时，无需使用AND运算符。 这是假设的。

   **示例：** 要筛选计划完成日期为今天且完成百分比低于100%的任务，请使用以下文本模式代码：

   <pre>planedCompletionDate=$TODAY</pre><pre>planedCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **或**:当使用OR运算符连接2个filter语句时，您表示希望满足任一语句。

   >[!TIP]
   >
   >将AND语句更改为OR语句时，报表中的项目数应会增加。

   使用文本模式界面构建OR过滤器时，必须使用OR运算符。

   **示例：** 要筛选计划完成日期为今天或完成百分比低于100%的任务，请使用以下文本模式代码：

   <pre>planedCompletionDate=$TODAY</pre><pre>planedCompletionDate_Mod=eq</pre><pre>或:1:percentComplete=100</pre><pre>或:1:percentComplete_Mod=lt</pre>

## OR过滤器的文本模式语法

OR筛选器的文本模式语法必须包含以下内容：

* OR运算符后跟一个冒号、一个数字和另一个冒号，位于每个过滤行的开头，引用OR语句中的对象。 这包括引用过滤器字段或属性的行，以及引用过滤器修饰符的行。

   构建OR过滤器时，请遵循以下模式：

   <pre><field name in camel case>=<value></pre><pre><field name in camel case>_修改=<modifier value></pre><pre>或:1:<field name in camel case>=<value></pre><pre>或:1:<field name in camel case>_修改=<modifier value></pre>

   >[!TIP]
   >
   >OR运算符区分大小写，并且始终为大写。

   过滤器中可能有多个OR语句。 在这种情况下，每个OR语句都会按您希望应用语句的顺序接收一个数字。

   **示例：**  要筛选计划完成日期为今天或完成百分比低于100%或状态为新的任务，请使用以下文本模式代码：

   <pre>planedCompletionDate=$TODAY</pre><pre>planedCompletionDate_Mod=eq</pre><pre>或:1:status=NEW</pre><pre>或:1:status_Mod=in</pre><pre>或:2:percentComplete=100</pre><pre>或:2:percentComplete_Mod=lt</pre>

* 您在过滤器中引用的字段或属性的名称必须用驼峰式写入。 有关驼峰式病例的信息，请参阅 [文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* 在OR过滤器中引用自定义字段时，必须插入DE:在OR修饰符语法和自定义字段名称之间。 您必须拼写自定义字段在Workfront界面中显示的名称。

   **示例：** 要过滤状态为“新”或“完成百分比”小于100%的任务，或过滤值为“等于”的名为“帐户类型”的自定义字段，请使用以下文本模式代码：

   <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>或:1:percentComplete=100</pre><pre>或:1:percentComplete_Mod=lt</pre><pre>或:2:DE:Account Type=Capital</pre><pre>或:2:DE:Account Type_Mod=in</pre>
