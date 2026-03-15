---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文本模式语法概述
description: 您可以使用文本模式界面在列表和报告中创建更复杂的视图、过滤器、分组和自定义提示。 通过使用文本模式，您可以访问在标准模式界面中不可用的字段及其属性。
author: Courtney
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '1862'
ht-degree: 0%

---

# 文本模式语法概述

<!--Audited: 1/2025-->

您可以使用文本模式界面在列表和报告中创建更复杂的视图、过滤器、分组和自定义提示。 通过使用文本模式，您可以访问在标准模式界面中不可用的字段及其属性。

有关开始前的文本模式的信息和注意事项，请参阅[文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

有关所有可报告字段及其属性的完整列表，请参阅[API资源管理器](../../../wf-api/general/api-explorer.md)。

有关使用文本模式创建报告（包括课程、视频和教程）的更多信息，请访问Adobe Experience League网站上的“学习”部分。

## 有关文本模式语法的注意事项

* 您必须先了解Adobe Workfront语法，然后才能开始以文本模式构建报表元素。 用于文本模式的Workfront语法是此应用程序所独有的，并具有您必须熟悉的独特特征。
* 在开始使用报告中的文本模式之前，我们强烈建议您参加高级报告课程，以更深入地了解我们的文本模式语言。
* 您可以使用标准模式界面自定义视图、筛选器和分组。 但是，您只能使用文本模式构建自定义提示。

## 以文本模式构建报告元素的常见准则

以下是在文本模式下构建任何报表或列表元素时的常见准则：

* 在引用Workfront数据库中的对象或属性时，请始终使用驼峰式大小写。
* 请记住Workfront中对象的层次结构。 视图、筛选器和分组之间存在以下差异：

   * 可以在视图中显示一个与报表或列表对象相距三个对象的对象。
   * 在编组、滤镜或自定义提示中，不能引用距离主对象超过2个对象的对象。

  **示例：**&#x200B;您可以在任务视图中显示Portfolio所有者的名称或GUID：

  `valuefield=project:portfolio:ownerID`

  不能在任务视图中对Portfolio所有者进行分组、筛选或提示：

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`

  在这些示例中，Portfolio所有者ID是远离列表对象的三个对象。

  有关Workfront中对象层次结构的信息，请参阅：

   * [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API 资源管理器](../../../wf-api/general/api-explorer.md)

* 请尽可能使用通配符，以使报表和列表更加动态，并避免在不同的用户和类似的时间轴中重复使用通配符。

## 驼峰式案例概述

在文本模式下引用Workfront字段或其属性时，Workfront要求您按驼峰式大小写键入其名称。 在这种情况下，单名字段使用小写字母进行拼写。 复合字段的拼写遵循以下模式：

`camelCaseSyntax`

>[!IMPORTANT]
>
>所有报告元素均遵循此大小写模式。

骆驼案例的特点是：

* 第一个单词始终以小写字母开头。
* 以下单词始终以大写字母开头。
* 两个字之间没有空格。

**示例：**&#x200B;要引用项目的实际完成日期，在生成文本模式报告元素时将使用的字段名称是

`actualCompletionDate`

## 各种报表元素的文本模式语法

使用文本模式创建报告元素集时，以下报告元素集的语法存在以下相似之处：

* 视图和组的代码行和语法类似。

  有关在文本模式下构建视图和分组时，视图和分组的关键代码行的信息，请参阅：

   * [使用文本模式编辑视图](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [使用文本模式编辑分组](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* 筛选器和自定义提示的代码行和语法类似。

  有关更多信息，请参阅：

   * [使用文本模式编辑筛选器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [向报告添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### 视图和分组的语法

构建视图和分组时的代码行类似。

有关创建视图和组的信息，请参阅以下文章：

* [查看Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

视图或分组中最重要的代码行是标识视图列或分组中引用的对象的行。 此代码行可以以`valuefield`或`valueexpression`开头，具体取决于该字段是对Workfront数据库字段的直接引用还是多个字段之间的计算。

下表列出了视图或分组中最常见的代码行：

| 代码行 | 描述 |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield` | 标识视图的列或分组中引用的对象。 这是对引用对象的直接引用。 |
| `valueexpression` | 标识视图的列或分组中引用的对象。 这是在若干字段之间进行的计算。 |
| `valueformat` | 标识Workfront返回在valuefield或valueexpression行中指定的值的格式。 |
| `width` | 标识列的宽度（以像素为单位）。 |
| `stretch` | 标识哪些列占用了视图不需要的额外空间。 |

>[!TIP]
>
>* 尽管以下示例中的代码行在视图和分组之间类似，但请始终记住，分组的每行代码都以分组编号开头。
>
>  要在项目列表或报表中按项目名称分组，请将以下行用于第一层分组：
>
>  `group.0.valuefield=name`
>  
>* 如果在同一列中编辑视图中的多个列（共享列的情况也是如此），请记住，每个列的每行代码都以列号开头。
>
>  使用以下格式标识视图的第一列：
>
>  `column.0.valuefield=name`
>  
>  有关共享列的信息，请参阅[查看：合并一个共享列中多个列的信息](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)。
>

#### 视图和分组的`Valuefield`语法概述

`Valuefield=`是视图和分组中的关键代码行，用于标识直接引用的对象。

对于分组和视图，直接引用字段的语法相同。

使用`valuefield`行引用Workfront对象时，适用以下规则：

* 使用驼峰式大小写直接引用字段。

  **示例：**&#x200B;要在任务视图中引用任务实际完成日期，请使用以下行：

  `valuefield=actualCompletionDate`

* 使用驼峰式大小写和冒号为同一对象分隔相互关联的字段。

  **示例：**&#x200B;要在任务视图中引用项目计划完成日期，请使用以下行：

  `valuefield=project:plannedCompletionDate`

  有关对象如何在Workfront数据库中相互引用的信息，请参阅[API资源管理器](../../../wf-api/general/api-explorer.md)。

* 引用自定义字段时，请完全按照界面中显示的字段名称使用该字段。

  **示例：**&#x200B;若要在任务视图中引用标记为“其他详细信息”的项目自定义域，请使用以下行：

  `valuefield=project:Additional Details`

#### 视图和分组的`Valueexpression`语法概述

在文本模式下生成视图和分组时，如果您要引用2个或更多字段之间的计算，则可以将`valuefield=`行代码替换为`valueexpression=`。

>[!TIP]
>
>尽管您可以构建可在报表中显示的计算字段，但计算视图和分组更为动态。 每次运行报表或显示列表时，计算视图和分组都会刷新为新信息。
>
>有关在视图中创建计算列的信息，请参阅[计算自定义字段与计算列](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md)。

构建计算分组类似于在视图中构建计算列。

使用`valueexpression`行引用Workfront对象时，适用以下规则：

* 使用驼峰式大小写直接引用字段，并用大括号括起每个字段。

  **示例：**&#x200B;要使用`valueexpression`在任务列中显示“任务名称”字段，请使用以下行：

  `valueexpression={name}`


* 使用驼峰形事例和句点分隔彼此相关的字段。

  **示例：**&#x200B;要在任务报告中显示与任务名称串联的项目名称，请使用以下行：

   * 在视图中：

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * 在分组中：

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  有关对象如何在Workfront数据库中相互引用的信息，请参阅[API资源管理器](../../../wf-api/general/api-explorer.md)。

* 在引用自定义字段时，请使用以下规则：

   * 使用与界面中显示的字段名称完全相同的名称。
   * 在字段名称前加上“DE：”。
   * 用大括号将字段括起来。
   * 按句点分隔与对象相关的字段。

  **示例：**&#x200B;要在值表达式行的任务视图中显示其他详细信息项目自定义域，请使用以下行：

  `valueexpression={project}.{DE:Additional Details}`

* 您可以在`valueexpression`中使用通配符，但不能在`valuefield`行中使用。

  有关通配符的信息，请参阅[通配符筛选器变量概述](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。


#### 视图和分组的`Valueformat`概述

视图或分组中第二重要的代码行是`valueformat=`行。 这将告知Workfront使用哪种格式返回您在`valuefield`行或`valueexpression`行中指定的值。 虽然您可以对`valueformat`行使用各种格式，但我们建议您在使用`valueexpression`时始终使用以下值：

`valueformat=HTML`

有关其他`valueformat`值，另请参阅以下文章：

* [设置文本模式报表中的日期格式](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [设置文本模式报表中的数字、货币和百分比值的格式](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### 查看的`width`概述

`width=`是代码行，您可以在其中指定每列的宽度（以像素为单位）。 Workfront会为每个字段提供建议的宽度，但根据字段的类型和格式，您可能需要进行调整。

您必须使用额外的`usewidths=true`行代码来强制为列指定的宽度。

**示例：**&#x200B;若要显示宽度为80像素的列，请使用以下行：

`width=80`

`usewidths=true`

#### 查看的`stretch`概述

`stretch`用于标识哪些列占用了视图不需要的额外空间。 典型用户的工作区的用户界面宽度约为850像素。 这意味着，如果您有一个包含四列（每列150像素）的视图，则视图会占用600个，即850个像素。 UI中会额外添加250个像素，这些像素将添加到提供拉伸百分比的列中。

当您对视图中的至少一个列使用附加代码行`usewidths=true`时，将强制延伸列。

**示例：**&#x200B;要指示列可使用视图中70%的空白空间，请使用以下行：

`stretch=70`

`usewidths=true`

### 筛选器和自定义提示的语法

创建过滤器的语法与创建自定义提示的语法类似。

>[!TIP]
>
>您可以先为要包含在提示中的语句构建筛选器，以创建自定义提示。 按“&amp;”连接筛选条件中的所有代码行，各行之间不留空格，这将会成为您的自定义提示。

有关生成筛选器和自定义提示的信息，请参阅：

* [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [向报告添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

有关在文本模式下创建滤镜的信息，请参阅[使用文本模式编辑滤镜](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)。

您可以使用以下元素在文本模式下构建筛选器和自定义提示：

* 引用filter语句的对象的代码行。 对滤镜对象使用驼峰式大小写。
* 引用filter对象和filter对象值的修饰符的代码行。 对此行中的滤镜对象使用驼峰式大小写。

  >[!TIP]
  >
  >在引用范围时，这需要2个修改量行。

* 连接多个过滤器语句的语句连接器：

   * 和

     这是过滤器语句之间的默认连接器。

   * 或者

     >[!TIP]
     >
     >语句连接器区分大小写，并且始终大写。 在文本模式下可以省略“AND”。

* 通配符，可使筛选器更动态，并针对当前时间或登录的用户自定义筛选器。 有关通配符的信息，请参阅[通配符筛选器变量概述](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。
