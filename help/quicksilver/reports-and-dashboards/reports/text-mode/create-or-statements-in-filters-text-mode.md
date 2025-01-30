---
product-area: reporting
navigation-topic: text-mode-reporting
title: 在文本模式过滤器中创建“OR”语句
description: 在列表和报告中创建过滤器时，可以包含多个语句。
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: af4a82ad11b57c7a7457d5d7ee74ee18494a1dc0
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# 在文本模式过滤器中创建“OR”语句

在列表和报告中创建过滤器时，可以包含多个语句。

有关创建过滤器的信息，请参阅以下文章：

* [筛选器概述](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [使用文本模式编辑筛选器](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## 文本模式筛选器运算符

有关标准筛选器界面中Adobe Workfront筛选器运算符的信息，请参阅[筛选器概述](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

Workfront有2个过滤器运算符连接每个过滤器语句：

* **AND**：当您通过AND运算符连接2个filter语句时，您指示希望同时满足两个filter语句。

  默认情况下，过滤器中的语句使用AND运算符连接。

  在文本模式界面中构建AND过滤器时，无需使用AND运算符。 假设是这样。

  **示例：**&#x200B;要筛选计划完成日期为今天且完成百分比低于100%的任务，请使用以下文本模式代码：

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq 
  percentComplete=100 percent
  Complete_Mod=lt
  ```

* **OR**：当您通过OR运算符连接2个筛选语句时，表示希望满足任一语句。

  >[!TIP]
  >
  >将AND语句更改为OR语句时，报表中的项目数应会增加。

  在使用文本模式界面构建OR过滤器时，必须使用OR运算符。

  **示例：**&#x200B;要筛选计划完成日期为今天或完成百分比低于100%的任务，请使用以下文本模式代码：

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  ```

## OR过滤器的文本模式语法

OR过滤器的文本模式语法必须包含以下内容：

* OR运算符，后跟一个冒号、一个数字和另一个冒号，位于每个引用OR语句中对象的筛选行的开头。 这包括引用过滤器字段或属性的行和引用过滤器修饰符的行。

  构建OR过滤器时，请遵循以下模式：

  ```
  <field name in camel case>=<value>
  <field name in camel case>_Mod=<modifier value>
  OR:1:<field name in camel case>=<value>
  OR:1:<field name in camel case>_Mod=<modifier value>
  ```

  >[!TIP]
  >
  >OR运算符区分大小写，并且始终为大写。

  过滤器中可以有多个OR语句。 在这种情况下，每个OR语句都会按您希望应用语句的顺序接收一个数字。

  **示例：**&#x200B;要筛选计划完成日期为今天、完成百分比低于100%或状态为新的任务，请使用以下文本模式代码：

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:status=NEW
  OR:1:status_Mod=in
  OR:2:percentComplete=100
  OR:2:percentComplete_Mod=lt
  ```

* 您在筛选器中引用的字段或属性的名称必须以驼峰式大小写形式编写。 有关驼峰式大小写的信息，请参阅[文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)。
* 在OR筛选器中引用自定义字段时，必须在OR修饰符语法和自定义字段名称之间插入DE： 。 您必须拼写自定义字段的名称，使其在Workfront界面中显示。

  **示例：**&#x200B;要筛选状态为“新”或“完成百分比”低于100%的任务，或者筛选名为“帐户类型”且值为“等于”的自定义字段，请使用以下文本模式代码：

  ```
  status=NEW
  status_Mod=in
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  OR:2:DE:Account Type=Capital
  OR:2:DE:Account Type_Mod=in
  ```
