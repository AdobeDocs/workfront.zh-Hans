---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文本模式语法概述
description: 您可以使用文本模式界面在列表和报告中创建更复杂的视图、筛选器、分组和自定义提示。 通过使用文本模式，您可以访问在标准模式界面中不可用的字段及其属性。
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '1857'
ht-degree: 0%

---

# 文本模式语法概述

您可以使用文本模式界面在列表和报告中创建更复杂的视图、筛选器、分组和自定义提示。 通过使用文本模式，您可以访问在标准模式界面中不可用的字段及其属性。

有关开始前文本模式的信息和注意事项，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

有关所有可报告字段及其属性的完整列表，请参阅 [API资源管理器](../../../wf-api/general/api-explorer.md).

有关使用文本模式创建报告（包括类、视频和教程）的更多信息，请参阅Adobe Experience League网站上的“学习”部分。

## 有关文本模式语法的注意事项

* 在开始以文本模式构建报表元素之前，您必须了解Adobe Workfront语法。 文本模式的Workfront语法是此应用程序所独有的，并具有您必须熟悉的独特特征。
* 在报表中开始使用文本模式之前，我们强烈建议您先参加有关高级报表的课程，以便更深入地了解我们的文本模式语言。 <!--outdated link: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* 您可以使用标准模式界面自定义视图、筛选器和分组。 但是，您只能使用文本模式构建自定义提示。

## 以文本模式构建报告元素的常见准则

以下是在文本模式下构建任何报表或列表元素时的常见准则：

* 在引用Workfront数据库中的对象或属性时，请始终使用驼峰式大小写。
* 请记住Workfront中的对象层次结构。 视图、筛选器和分组之间存在以下差异：

   * 可以在视图中显示与报表或列表对象相距三个对象的对象。
   * 在分组、过滤器或自定义提示中，不能引用远离主对象2个以上的对象。

  **示例：** 您可以在任务视图中显示“Portfolio所有者”的名称或GUID：


  `valuefield=project:portfolio:ownerID`

  您不能在任务视图中对“Portfolio所有者”进行分组、筛选或提示：

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`


  在这些示例中，Portfolio所有者ID是远离列表对象的三个对象。

  有关Workfront中对象层次的信息，请参阅：

   * [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API资源管理器](../../../wf-api/general/api-explorer.md)

* 尽量使用通配符，使报告和列表更加动态，避免为不同的用户和类似的时间线重复使用它们。

## 驼峰式拼写概述

在文本模式下引用Workfront字段或其属性时，Workfront要求您以驼峰式大小写键入其名称。 在这种情况下，单名字段以小写拼写。 复合字段的拼写遵循以下模式：

`camelCaseSyntax`

>[!IMPORTANT]
>
>所有报表元素都遵循此大小写模式。

骆驼案例的特点是：

* 第一个单词始终以小写字母开头。
* 以下单词始终以大写字母开头。
* 这两个字之间没有空格。

**示例：** 要引用项目的实际完成日期，可在构建文本模式报告元素时使用的字段名称是

`actualCompletionDate`

## 各种报表元素的文本模式语法

使用文本模式创建报告元素集时，以下报告元素集的语法存在以下相似之处：

* 视图和分组的代码行和语法类似。

  有关在文本模式下构建视图和分组代码的关键行的信息，请参阅：

   * [使用文本模式编辑视图](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [编辑分组中的文本模式](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* 过滤器和自定义提示的代码行和语法类似。

  有关更多信息，请参阅：

   * [使用文本模式编辑筛选器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### 视图和分组的语法

您可能会注意到构建视图和分组时的代码行类似。

有关创建视图和分组的信息，请参阅以下文章：

* [Adobe Workfront中的视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

视图或分组最重要的代码行是标识视图列或分组中引用的对象的代码行。 根据此字段是直接引用Workfront数据库字段还是多个字段之间的计算，代码行可能以 `valuefield` 或 `valueexpression`

下表列出了视图或分组中最常见的代码行：

| 代码行 | 描述 |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield` | 标识视图列或分组中引用的对象。 这是对引用对象的直接引用。 |
| `valueexpression` | 标识视图列或分组中引用的对象。 这是多个字段之间的计算。 |
| `valueformat` | 标识Workfront返回在valuefield或valueexpression行中指定的值的格式。 |
| `width` | 标识列的宽度（以像素为单位）。 |
| `stretch` | 标识哪些列占用了视图不需要的额外空间。 |

>[!TIP]
>
>* 尽管以下示例中的代码行在视图和分组之间相似，但请始终记住，分组的每行代码都以分组编号开头。
>
>  要在项目列表或报表中按项目名称分组，请使用以下行进行第一层分组：
>
>  `group.0.valuefield=name`
>  
>* 如果在同一列的视图中编辑多个列（与共享列的情况一样），请记住，每个列的每行代码都以列号开头。
>
>  使用以下格式标识视图的第一列：
>
>  `column.0.valuefield=name`
>  
>  有关共享列的信息，请参见 [视图：合并来自一个共享列中多个列的信息](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).
>

#### `Valuefield` 视图和分组的语法概述

`Valuefield=` 是视图和分组中的关键代码行，用于标识您直接引用的对象。

对于分组和视图，直接引用字段的语法相同。

以下规则适用于使用引用Workfront对象的情况 `valuefield` 行：

* 使用驼峰式大小写直接引用字段。

  **示例：** 要在任务视图中引用任务实际完成日期，请使用以下行：

  `valuefield=actualCompletionDate`

* 使用驼峰式大小写和冒号为同一对象分隔相互关联的字段。

  **示例：** 要在任务视图中引用项目计划完成日期，请使用以下行：

  `valuefield=project:plannedCompletionDate`

  有关对象如何在Workfront数据库中相互引用的信息，请参阅 [API资源管理器](../../../wf-api/general/api-explorer.md).

* 引用自定义字段时，请完全按照界面中显示的字段名称使用该字段。

  **示例：** 要在任务视图中引用标记为其他详细信息的项目自定义字段，请使用以下行：

  `valuefield=project:Additional Details`

#### `Valueexpression` 视图和分组的语法概述

您可以替换 `valuefield=` 代码行 `valueexpression=` 在文本模式下构建视图和分组时，如果要在两个或更多字段之间引用计算。

>[!TIP]
>
>尽管您可以构建可在报表中显示的计算字段，但计算视图和分组更加动态。 每次运行报表或显示列表时，计算出的视图和分组都会刷新并显示新信息。
>
>有关在视图中创建计算列的信息，请参见 [计算的自定义字段与计算的列](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

构建计算分组与在视图中构建计算列类似。

以下规则适用于使用引用Workfront对象的情况 `valueexpression` 行：

* 使用驼峰式大小写直接引用字段并用大括号括住每个字段。

  **示例：** 使用在任务列中显示任务名称字段 `valueexpression`，请使用以下行：

  `valueexpression={name}`


* 使用驼峰式大小写和句点分隔相互关联的字段。

  **示例：** 要在任务报告中显示与任务名称连接的项目名称，请使用以下行：

   * 在视图中：

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * 在分组中：

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  有关对象如何在Workfront数据库中相互引用的信息，请参阅 [API资源管理器](../../../wf-api/general/api-explorer.md).

* 引用自定义字段时，使用以下规则：

   * 使用与界面中显示的字段完全相同的名称。
   * 在字段名称前面加上“DE：”。
   * 用大括号括住该字段。
   * 按句点分隔与对象相关的字段。

  **示例：** 要在值表达式行的任务视图中显示“其他详细信息”项目自定义字段，请使用以下行：

  `valueexpression={project}.{DE:Additional Details}`

* 您可以在中使用通配符 `valueexpression` 但不是在 `valuefield` 行。

  有关通配符的信息，请参见 [通配符筛选器变量](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### `Valueformat` 视图和分组概述

视图或分组中第二最重要的代码行是 `valueformat=` 行。 这会告知Workfront采用哪种格式返回您在
`valuefield` 或valueexpression行。 尽管您可以对使用多种格式 `valueformat` 行中，我们建议您在使用时
`valueexpression`：

`valueformat=HTML`

其他 `valueformats` 值，另请参阅以下文章：

* [设置文本模式报表中的日期格式](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [设置文本模式报表中的数字、货币和百分比值的格式](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### `width` 视图概述

`width=` 是一行代码，您可以在其中指定每列的宽度（像素）。 Workfront会为每个字段提供建议的宽度，不过根据字段类型和格式，您可能需要进行调整。

您必须使用 `usewidths=true` 用于强制实施为列指定的宽度的代码行。

**示例：** 要显示宽度为80像素的列，请使用以下行：

`width=80`

`usewidths=true`

#### `stretch` 视图概述

此 `stretch` 用于标识哪些列占用了视图不需要的额外空间。 典型用户的工作区的用户界面宽度约为850像素。 这意味着，如果您有一个包含四列（每列150像素）的视图，则您的视图占用600个（850像素）。 UI中有250个额外的像素将被添加到提供了拉伸百分比的列中。

当您使用附加代码行时，将强制实施列的延伸： `usewidths=true` 视图中至少有一列的属性。

**示例：** 要指示某列可以使用视图中70%的空格，请使用以下行：

`stretch=70`

`usewidths=true`

### 过滤器和自定义提示的语法

创建过滤器的语法与创建自定义提示的语法类似。

>[!TIP]
>
>您可以首先为要包含在提示中的语句构建过滤器，从而创建自定义提示。 使用“&amp;”连接筛选器中的所有代码行，各行之间不留空格，这将会成为您的自定义提示。

有关构建过滤器和自定义提示的信息，请参阅：

* [Adobe Workfront中的过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

有关在文本模式下创建过滤器的信息，请参阅 [使用文本模式编辑筛选器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

您可以使用以下元素在文本模式下构建过滤器和自定义提示：

* 引用filter语句的对象的一行代码。 过滤器对象使用驼峰式大小写。
* 引用滤镜对象和滤镜对象值的修饰符的代码行。 此行中的滤镜对象使用驼峰式大小写。

  >[!TIP]
  >
  >在引用范围时，需要2个修饰符行。

* 连接多个过滤语句的语句连接器：

   * 和

     这是过滤器语句之间的默认连接器。

   * 或

     >[!TIP]
     >
     >语句连接器区分大小写，并且始终大写。 在文本模式下可以省略“AND”。

* 通配符，可使筛选器更动态，并针对当前时间或登录的用户自定义筛选器。 有关通配符的信息，请参见 [通配符筛选器变量](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
