---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文本模式语法概述
description: 您可以使用文本模式界面在列表和报表中创建更复杂的视图、过滤器、分组和自定义提示。 通过使用文本模式，您可以访问标准模式界面中不可用的字段及其属性。
author: Nolan
feature: Reports and Dashboards
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1498'
ht-degree: 0%

---

# 文本模式语法概述

您可以使用文本模式界面在列表和报表中创建更复杂的视图、过滤器、分组和自定义提示。 通过使用文本模式，您可以访问标准模式界面中不可用的字段及其属性。

有关开始之前文本模式的信息和注意事项，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

有关所有可报告字段及其属性的完整列表，请参阅 [API Explorer](../../../wf-api/general/api-explorer.md).

## 有关文本模式语法的注意事项

* 在开始以文本模式构建报表元素之前，您必须先了解Adobe Workfront语法。 文本模式的Workfront语法是此应用程序特有的，它具有您必须熟悉的独特特性。
* 在您开始在报表中使用文本模式之前，我们强烈建议您先学习我们的高级报表课程，以便更深入地了解我们的文本模式语言。 有关报告的培训材料，请参阅 [Workfront报表和功能板学习路径](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).
* 您可以使用标准模式界面自定义视图、过滤器和分组。 但是，您只能使用文本模式生成自定义提示。

## 在文本模式下构建报表元素的常见准则

以下是在文本模式下构建任何报表或列表元素时的常见准则：

* 在Workfront数据库中引用对象或属性时，始终使用驼峰式大小写。
* 请记住Workfront中对象的层次结构。 视图、过滤器和分组之间存在以下差异：

   * 您可以显示一个对象，该对象是与视图中的报表或列表对象相距三个对象。
   * 在分组、过滤器或自定义提示中，不能引用距主对象2个以上对象的对象。

   **示例：** 您可以在任务视图中显示Portfolio所有者的名称或GUID:

   ```
   valuefield=project:portfolio:ownerID
   ```

   在任务视图中，不能对Portfolio所有者进行分组、过滤或提示：

   ```
   project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa
   ```

   在这些示例中，Portfolio所有者ID是与列表对象相距的三个对象。

   有关Workfront中对象层次结构的信息，请参阅：

   * [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API Explorer](../../../wf-api/general/api-explorer.md)


* 尽可能使用通配符以使报表和列表更加动态，并避免为不同用户和类似时间轴复制通配符。

## 驼峰式案例概述

在文本模式下引用Workfront字段或其属性时，Workfront要求您以驼峰式键入其名称。 在这种情况下，单名称字段将以小写形式拼写。 复合字段按以下模式拼写：

```
camelCaseSyntax
```

>[!IMPORTANT]
>
>所有报表元素都遵循此大小写模式。

驼峰箱的特点是：

* 第一个单词始终以小写字母开头。
* 以下单词始终以大写字母开头。
* 字之间没有空格。

**示例：** 要引用项目的实际完成日期，在构建文本模式报表元素时将使用的字段名称为

```
actualCompletionDate
```

。

## 各种报表元素的文本模式语法

使用文本模式创建报表元素集时，下面这些报表元素集的语法之间存在以下相似之处：

* 对于视图和分组，代码行和语法类似。

   有关在文本模式下构建视图和分组代码关键行的信息，请参阅：

   * [使用文本模式编辑视图](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [在分组中编辑文本模式](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* 对于过滤器和自定义提示，代码行和语法类似。

   有关更多信息，请参阅：

   * [使用文本模式编辑过滤器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### 视图和分组的语法

您可能会注意到在构建视图和分组时代码行相似。

有关创建视图和分组的信息，请参阅以下文章：

* [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

视图或分组最重要的代码行是标识在视图列或分组中引用的对象的行。 根据此字段是对Workfront数据库字段的直接引用还是多个字段之间的计算，代码行可能以

```
valuefield
```

或

```
valueexpression
```

。

* [视图和分组的值字段语法概述](#valuefield-syntax-overview-for-views-and-groupings)
* [视图和分组的值表达式语法概述](#valueexpression-syntax-overview-for-views-and-groupings)

>[!TIP]
>
>* 尽管以下示例中的代码行在视图和分组之间相似，但请始终记住，分组的每一行代码都以分组编号开头。
>
>  要在项目列表或报表中按项目名称分组，请将以下行用于第一层分组：
>
>  
```>
>  group.0.valuefield=name
>  ```>
>* If you edit multiple columns in a view in the same column (as it is the case of shared columns), remember that every line of code for each column starts with the column number. 
>
>  
Use the following format to identify the first column of a view: 
>
>  
```>
>  column.0.valuefield=name
>  ```>
>  For information about sharing columns, see [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md). 
>



```
Valuefield
```

视图和分组的语法概述 {#valuefield-syntax-overview-for-views-and-groupings}

```
Valuefield=
```

是视图和分组中的一行关键代码，用于标识您直接引用的对象。

直接引用字段的语法对于分组和视图是相同的。

以下规则适用于使用

```
valuefield
```

行：

* 使用驼峰式大小写直接引用字段。

   **示例：** 要在任务视图中引用任务实际完成日期，请使用以下行：

   ```
   valuefield=actualCompletionDate
   ```

* 使用驼峰式大写和冒号来分隔同一对象中彼此相关的字段。

   **示例：** 要在任务视图中引用项目计划完成日期，请使用以下行：

   ```
   valuefield=project:plannedCompletionDate
   ```

   有关对象如何在Workfront数据库中相互引用的信息，请参阅 [API Explorer](../../../wf-api/general/api-explorer.md).

* 引用自定义字段时，请完全使用该字段在界面中显示的名称。

   **示例：** 要在任务视图中引用标记为“其他详细信息”的项目自定义字段，请使用以下行：

   ```
   valuefield=project:Additional Details
   ```

 

```
Valueexpression
```

视图和分组的语法概述 {#valueexpression-syntax-overview-for-views-and-groupings}

您可以将

```
valuefield=
```

代码行

```
valueexpression=
```

在文本模式下构建视图和分组时，需要引用2个或更多字段之间的计算。

>[!TIP]
>
>尽管您可以生成可在报表中显示的计算字段，但计算量度视图和分组更加动态。 每次运行报表或显示列表时，计算量度视图和分组都会使用新信息进行刷新。
>
>有关在视图中创建计算列的信息，请参阅 [计算自定义字段与计算列](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

构建计算分组与在视图中构建计算列类似。

以下规则适用于使用

```
valueexpression
```

行：

* 使用驼峰式大小写直接引用字段，并用大括号括住每个字段。

   **示例：** 在任务列中使用

   ```
   valueexpression
   ```

   ，请使用以下行：

   ```
   valueexpression={name}
   ```

* 使用驼峰式大小写和句点来分隔彼此相关的字段。

   **示例：** 要显示与任务报表中的任务名称连接的项目名称，请使用以下行：

   * 在视图中：

      ```
      valueexpression=CONCAT({project}.{name},' - ',{name})
      ```

   * 在分组中：

      ```
      group.0.valueexpression=CONCAT({project}.{name},' - ',{name})
      ```
   有关对象如何在Workfront数据库中相互引用的信息，请参阅 [API Explorer](../../../wf-api/general/api-explorer.md).

* 引用自定义字段时，请使用以下规则：

   * 完全使用字段在界面中显示的名称。
   * 在字段名称前面添加“DE：”。
   * 用大括号括住字段。
   * 按句点分隔与对象相关的字段。

   **示例：** 要在值表达式行的任务视图中显示“附加详细信息”项目自定义字段，请使用以下行：

   ```
   valueexpression={project}.{DE:Additional Details}
   ```

* 您可以在

   ```
   valueexpression
   ```

   但在

   ```
   valuefield
   ```

   行。

   有关通配符的信息，请参阅 [通配符过滤器变量](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

```
Valueformat
```

概述

在视图或分组中，第二行最重要的代码是

```
valueformat=
```

行。 这会告知Workfront以什么格式返回您在

```
valuefield
```

或值表达式行。 尽管您可以在

```
valueformat
```

行，我们建议您在使用

```
valueexpression
```

:

```
valueformat=HTML
```

### 过滤器和自定义提示的语法

创建过滤器的语法与创建自定义提示的语法类似。

>[!TIP]
>
>您可以先为要包含在提示中的语句构建过滤器，以创建自定义提示。 按“&amp;”连接过滤器中的所有代码行，且这些代码行之间不留任何空格，这将成为您的自定义提示。

有关生成过滤器和自定义提示的信息，请参阅：

* [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

有关在文本模式下创建过滤器的信息，请参阅 [使用文本模式编辑过滤器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

您可以使用以下元素在文本模式下构建过滤器和自定义提示：

* 引用filter语句对象的代码行。 对过滤器对象使用驼峰式大小写。
* 引用过滤器对象和用于过滤器对象值的修饰符的代码行。 对此行中的过滤器对象使用驼峰式大小写。

   >[!TIP]
   >
   >引用范围时，需要使用2个修饰符行。

* 连接多个filter语句的语句连接器：

   * 和

      这是筛选器语句之间的默认连接器。

   * 或

      >[!TIP]
      >
      >语句连接器区分大小写，并且始终为大写。 在文本模式中，可以忽略“和”。

* 通配符可使过滤器更加动态，并针对当前时间或登录用户自定义过滤器。 有关通配符的信息，请参阅 [通配符过滤器变量](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
