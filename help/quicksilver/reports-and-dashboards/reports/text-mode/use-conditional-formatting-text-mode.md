---
product-area: reporting
navigation-topic: text-mode-reporting
title: 在文本模式中使用条件格式
description: 在文本模式中使用条件格式
author: Nolan
feature: Reports and Dashboards
exl-id: 48fc8450-35c6-4d59-89d3-0feffe662b25
source-git-commit: 16d59c6e3d790f2804795f5a6fef05c8dca71b30
workflow-type: tm+mt
source-wordcount: '1758'
ht-degree: 2%

---

# 在文本模式中使用条件格式

<!--
(NOTE: Alina: this article might need to be split in its sections. Tony asked that numbers and dates should be in separate articles (??))
-->

标准界面生成器在创建报表元素时提供了大量灵活性，可满足您组织的需求。

您可以使用标准界面在视图中应用条件格式。\
有关对视图应用条件格式的详细信息，请参阅 [在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对过滤器、视图、分组的访问权限</p> <p>编辑对报表、功能板、日历的访问权限，以编辑报表中的视图</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限以编辑报表中的视图</p> <p>管理要编辑的视图的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 文本模式中的条件格式

文本模式允许您通过使用标准界面中不可用的字段来创建更复杂的视图、过滤器、分组和提示。

有关所有可报告字段的完整列表，请参阅  [API Explorer](../../../wf-api/general/api-explorer.md).

有关使用文本模式语法的更多信息，请参阅 [文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

您还可以使用文本模式来设置报表和列表中视图的格式。 使用条件格式，您可以通过更改报表中结果的字体类型和背景以及图标和标记来更改报表的视图。 我们建议您始终先使用标准界面构建视图，并仅在绝对必要时切换到文本模式界面。

>[!NOTE]
>
> 不支持使用CSS样式自定义条件格式。 您而是必须使用Adobe Workfront中提供的预先设计的格式选项。

## 向视图添加条件格式

有关在标准生成器界面中对视图应用条件格式的详细信息，请参阅 [在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

要在文本模式界面中向视图添加条件格式，请执行以下操作：

1. 转到对象列表。
1. 展开要向其添加条件格式的视图的下拉菜单。
1. 单击 **自定义视图**.
1. 在要应用条件格式的视图中单击该列。
1. 单击 **切换到文本模式**.
1. 在 **在此列中显示：** 区域，单击 **单击以编辑文本**.
1. 添加中提供的代码示例 [使用文本模式设置视图格式](#format-views-using-text-mode) 列中文本的底部。
1. 单击 **保存**，然后单击 **保存视图**.

## 使用文本模式设置视图格式 {#format-views-using-text-mode}

您可以将以下组件添加到视图中的列，以在文本模式下有条件地设置其格式：

* [列设置](#column-settings)
* [列规则](#column-rules)
* [有条件地设置值表达式的格式](#conditionally-format-a-valueexpression)

### 列设置 {#column-settings}

在向视图添加条件格式之前，您必须熟悉文本模式界面。

在视图中使用条件格式时，可以自定义列的以下元素：

* [列标题](#column-headers)
* [设置日期格式](#format-dates)
* [设置数字格式](#format-numbers)

#### 列标题 {#column-headers}

要更改显示的列标题，请将以下代码添加到列中： `displayname= [Name of column]`. 例如，要将列命名为“项目所有者”，文本代码将如下所示：

```
displayname=Project Owner
```

#### 设置日期格式 {#format-dates}

日期可以配置为以多种格式显示。

有关更多信息，请参阅 [在文本模式报表中设置日期格式](../../../reports-and-dashboards/reports/text-mode/format-dates-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above)</p>
<p>To establish a date format, you must modify the <code>valueformat</code> line of the text mode code in the column.</p>
<pre>valueformat= [new date format]</pre>
<p>For example, if you wanted the Projected Completion Date to be displayed as MM/DD/YY the code would look like:</p>
<pre>valueformat=atDate<br>valuefield=projectedCompletionDate </pre>
<p>If you wanted to show the Planned Completion Date as <em>Mth, DD, Year</em>, the code would look like:</p>
<pre>valueformat=mediumAtdate<br>valuefield=plannedCompletionDate</pre>
<p>You can format dates using the following <code>valueformat</code> text mode values:</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Format</strong> </th>
<th scope="col">Example </th>
<th scope="col"><em><strong>valueformat=</strong></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>atDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY Time</td>
<td>10/11/18 12:00pm</td>
<td><pre>longAtDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>shortAtDate</pre> </td>
</tr>
<tr>
<td>Mth, DD, YR</td>
<td>Oct, 11, 2018</td>
<td><pre>mediumAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR</td>
<td>Mon, Oct, 11, 2018</td>
<td><pre>partialAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR Time</td>
<td>Mon, Oct, 11, 2018 12:00 pm</td>
<td><pre>fullAtDate</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

#### 设置数字格式 {#format-numbers}

您可以设置数值格式以显示最符合报表需求的信息。

有关更多信息，请参阅 [在文本模式报表中设置数字、货币和百分比值的格式](../../../reports-and-dashboards/reports/text-mode/format-numbers-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To modify the format of a numeric value, you must edit the <strong>valueformat</strong> line of your column.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above) </p>
<p>For example, if you wanted to display the Budget column as $1000, the value format line would look like:</p>
<pre>valueformat=currencyStringCurrencyRounded<br>valuefield=budget</pre>
<p>You can format numbers using the following values for the <code>valueformat</code> line of your column:</p>
<table border="2" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Example</strong> </th>
<th scope="col"><em><code>valueformat=</code></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>1234</td>
<td><pre>doubleAsString</pre> or <pre>int</pre></td>
</tr>
<tr>
<td>1,234</td>
<td><pre>doubleAsInt</pre> </td>
</tr>
<tr>
<td>$1,234</td>
<td><pre>currencyStringCurrencyRounded</pre> </td>
</tr>
<tr>
<td>1234.56</td>
<td><pre>doubleAsDouble</pre> </td>
</tr>
<tr>
<td>$1,234.56</td>
<td><pre>currencyStringCurrency</pre> </td>
</tr>
<tr>
<td>12%</td>
<td><pre>doubleAsPercentRounded</pre> </td>
</tr>
<tr>
<td>12.34%</td>
<td><pre>doubleAsPercent</pre> </td>
</tr>
<tr>
<td>(1,234.56)</td>
<td><pre>doubleAsFinancial</pre> </td>
</tr>
<tr>
<td>(1,234)</td>
<td><pre>doubleAsFiancialRounded</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

### 列规则 {#column-rules}

列规则允许在视图中添加图像、颜色、格式和文本覆盖。 列规则可以单独建立，也可以包含列的多个条件。

* [条件格式化](#conditional-formatting)
* [多种条件格式](#multiple-conditional-formats)
* [应用文本](#apply-text)
* [应用行格式](#apply-row-formats)
* [应用图像](#apply-images)

#### 条件格式化 {#conditional-formatting}

合并颜色或格式文本时必须应用特定的文本模式语句。

>[!NOTE]
>
>合并的列中可能不支持条件格式。\
>有关将列与文本模式合并的详细信息，请参阅 [查看：一个共享列中多个列的合并信息](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

在要添加条件格式的任何列中插入以下代码：

```
styledef.case.0.comparison.leftmethod= [field name]
styledef.case.0.comparison.lefttext= [field name]
styledef.case.0.comparison.righttext= [field value]
styledef.case.0.comparison.operator= [qualifier]
styledef.case.0.comparison.operatortype= [data type]
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

>[!NOTE]
>
>的 *styledef.case.0.comparison.icon* 除非使用图标，否则行始终为false。
>
>的 *styledef.case.0.comparison.truetext* 直到处理覆盖文本，行始终留空。
>
>的 *styledef.case.0.comparison.righttext* 限定符不为空时，行为空。

例如，如果我们想在项目报表中以绿色文本显示公司名称，则可以使用以下代码：

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name ;
styledef.case.0.comparison.righttext= 
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
```

>[!NOTE]
>
>* 虽然此语句可以应用于公司名称列，但也可以应用于报表上的任何其他列。 仅当项目有关联的公司时，才会显示绿色文本。 记住 `[field name]`, `[value]`和 `[qualifier]` 是否在柱子上显示条件。
>* 使用限定符时，我们建议使用 `cicontains` 而不是 `equal`. 默认情况下， `equal` 查找ID号。 使用 `cicontains` 限定符，您可以按项目名称访问项目。


![](assets/screen-shot-2013-08-15-at-2.53.51-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-2.54.08-pm-350x185.png)

无论“文本颜色”、“对齐”、“字体样式”或“背景颜色”应用于文本模式，都会使用相同的语句（如上所示）。

必须修改以下行以反映列所需的相应格式：

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

使用下表来标识需要修改的行以及应指定哪些值以定义列的格式样式：

| **文本颜色** | **行：textcolor=** |
|---|---|
| 黑色 | `000000` |
| 深蓝色 | `0c6aca` |
| 蒂尔 | `1b878c` |
| 绿色 | `03a219` |
| 紫色 | `6408c4` |
| 灰色 | `767676` |
| 红色 | `d30519` |
| 黄色 | `e19503` |

{style=&quot;table-layout:auto&quot;}

| **对齐方式** | **行：align=** |
|---|---|
| 左对齐 | `left` |
| 右对齐 | `right` |
| 居中对齐 | `center` |

{style=&quot;table-layout:auto&quot;}

| 字体 | 行： ***fontstyle=*** |
|---|---|
| 粗体 | `bold` |
| 斜体 | `italic` |

{style=&quot;table-layout:auto&quot;}

| **背景颜色** | **行：bgcolor=** |
|---|---|
| 蒂尔 | `dcf6f7` |
| 绿色 | `def6e2` |
| 灰色 | `e8e8e8` |
| 蓝色 | `e8f1ff` |
| 紫色 | `e9def4` |
| 红色 | `eac6c9` |
| 黄色 | `feecc8` |
| 白色 | `ffffff` |

{style=&quot;table-layout:auto&quot;}

#### 多种条件格式 {#multiple-conditional-formats}

可以对语句应用多个格式样式。 核心声明将保持不变，并在声明中添加任何其他格式表达式。

例如，使用前面的语句以绿色粗体文本包含公司名称。 该语句将使用以下代码编写：

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name
styledef.case.0.comparison.righttext=
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
styledef.case.0.comparison.trueproperty.1.name=fontstyle
styledef.case.0.comparison.trueproperty.1.value=bold
```

>[!NOTE]
>
>当包含多个条件格式表达式时，必须用数字标识语句中的每个表达式。 请注意，表达式0和表达式1已被识别。

![](assets/screen-shot-2013-08-15-at-3.18.45-pm-350x198.png)

#### 应用文本 {#apply-text}

如果要用所选的值替换列中填充的默认值，则在对列应用文本时可以执行此操作。

例如，在项目报表中，将“计划起始日期”列值设置为不显示项目的计划起始日期，而是显示文本“不是今天”。 对“计划起始日期”列使用以下代码：

```
case.0.comparison.leftmethod=plannedStartDate
case.0.comparison.lefttext=plannedStartDate
case.0.comparison.righttext=2013-04-10T10:45:00:000
case.0.comparison.operator=ne
case.0.comparison.operatortype=date
case.0.comparison.icon=false
case.0.comparison.truetext=not today
styledef.case.0.comparison.leftmethod=plannedStartDate
styledef.case.0.comparison.lefttext=plannedStartDate
styledef.case.0.comparison.righttext=2013-04-10T10:45:00:000 
styledef.case.0.comparison.operator=ne
styledef.case.0.comparison.operatortype=date&
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=not today
```

>[!NOTE]
>
>以开头的行 `case.0.` 用例比较以标识文本的使用。 以开头的行 **styledef.case.0。** 是早期的条件格式语句，其中我们通过 `truetext` 表达式。 确保设置 `truetext` 值，而不是将其留空。

![](assets/screen-shot-2013-08-15-at-3.22.02-pm-350x196.png)

![](assets/screen-shot-2013-08-15-at-3.22.16-pm-350x151.png)

#### 应用行格式 {#apply-row-formats}

如果要对整行应用条件，请将以下代码与列代码一起使用：

```
styledef.case.0.comparison.icon=false
```

```
styledef.case.0.comparison.isrowcase=true
```

```
styledef.case.0.comparison.leftmethod= [field name]
```

```
styledef.case.0.comparison.lefttext= [field name]
```

```
styledef.case.0.comparison.operator= [qualifier]
```

```
styledef.case.0.comparison.operatortype= [data type]
```

```
styledef.case.0.comparison.righttext= [field value]
```

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
```

```
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

```
styledef.case.0.comparison.truetext=
```

```
row.0.styledef.applyallcases=true
```

```
row.0.styledef.case.0.comparison.icon=false
```

```
row.0.styledef.case.0.comparison.isrowcase=true
```

```
row.0.styledef.case.0.comparison.leftmethod= [field name]
```

```
row.0.styledef.case.0.comparison.lefttext= [field name]
```

```
row.0.styledef.case.0.comparison.operator= [qualifier]
```

```
row.0.styledef.case.0.comparison.operatortype= [data type]
```

```
row.0.styledef.case.0.comparison.righttext= [field value]
```

```
row.0.styledef.case.0.comparison.trueproperty.0.name= [format option]
```

```
row.0.styledef.case.0.comparison.trueproperty.0.value= [format style]
```

```
row.0.styledef.case.0.comparison.truetext=
```


#### 应用图像 {#apply-images}

与文本格式类似，图像也可用于在报表中显示信息。 Workfront具有许多用于在报表设置中传递可视信息的内置图像。 要在条件格式设置中使用图像，需要以下语句：

```
image.case.0.comparison.leftmethod= [field name]
image.case.0.comparison.lefttext= [field name]
image.case.0.comparison.righttext= [field value]
image.case.0.comparison.operator= [qualifier]
image.case.0.comparison.operatortype= [data type]
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=
```

例如，在项目报表中，您要构建一列，其中显示一个与今天日期不相等的每个计划完成日期的皱眉。 使用以下文本模式代码将图标添加到列中：

```
image.case.0.comparison.leftmethod=plannedCompletionDate
image.case.0.comparison.lefttext=plannedCompletionDate
image.case.0.comparison.righttext=2013-04-10T13:00:00:000 
image.case.0.comparison.operator=ne 
image.case.0.comparison.operatortype=date
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif
```

>[!NOTE]
>
>请注意，该语句使用 `icon=true` 表达式。 此语句与其他条件格式语句也不同，因为它不使用 `style.def` 格式，而是唯一的图像格式。

![](assets/screen-shot-2013-08-15-at-3.35.08-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-3.35.22-pm-1-350x167.png)

要使用可用的图像，请应用以下代码和值：

| **图标** | **行：image.case.0.comparison.truetext=** |
|---|---|
| 皱眉脸 ![](assets/face-sad.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif` |
| 快乐的脸 ![](assets/face-happy.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_smile.gif` |
| 蓝旗  ![](assets/flag-blue-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_blue.gif` |
| 绿旗  ![](assets/flag-green-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_green.gif` |
| 红旗  ![](assets/flag-red-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_red.gif` |
| 黄旗  ![](assets/flag-yellow-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_yellow.gif` |
| 黑圈  ![](assets/dot-black.png) | =`/interface/images/v4_redux/icons/casebuilder/light_black.gif` |
| 蓝色圆圈 ![](assets/dot-blue.png) | =`/interface/images/v4_redux/icons/casebuilder/light_blue.gif` |
| 灰圆 ![](assets/dot-gray.png) | =`/interface/images/v4_redux/icons/casebuilder/light_grey.gif` |
| 绿色圆圈 ![](assets/dot-green.png) | =`/interface/images/v4_redux/icons/casebuilder/light_green.gif` |
| 橙色圆圈 ![](assets/dot-orange.png) | =`/interface/images/v4_redux/icons/casebuilder/light_orange.gif` |
| 粉红色圆圈 ![](assets/dot-pink.png) | =`/interface/images/v4_redux/icons/casebuilder/light_pink.gif` |
| 紫色圆 ![](assets/dot-purple.png) | =`/interface/images/v4_redux/icons/casebuilder/light_purple.gif` |
| 红圈 ![](assets/dot-red.png) | =`/interface/images/v4_redux/icons/casebuilder/light_red.gif` |
| 白圈 ![](assets/dot-white.png) | =`/interface/images/v4_redux/icons/casebuilder/light_white.gif` |
| 黄圈 ![](assets/dot-yellow.png) | =`/interface/images/v4_redux/icons/casebuilder/light_yellow.gif` |

{style=&quot;table-layout:auto&quot;}

### 有条件地设置 `valueexpression` {#conditionally-format-a-valueexpression}

要在列中显示计算值，可以将 `valuefield` 列中的代码行，其中包含 `valueexpression`. 计算值允许您根据同一对象上两个现有字段之间的计算来为对象显示新值。

有关如何设置 `valueexpression line`，请参阅 [文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

不能有条件地设置包含 `valueexpression` 代码行。 您可以将计算的自定义字段添加到自定义表单，并将其与您在报表中显示的对象相关联。 然后，您可以根据条件设置显示此字段的列的格式。

有关计算自定义字段的更多信息，请参阅 [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 在“文本模式”列中添加聚合器值

我们建议您先在生成器界面中构建列，在该界面中添加聚合器值，然后在文本模式中编辑列。

在文本模式下向列添加聚合时，请考虑以下事项：

* 列中的值必须具有可汇总的格式。 例如，它们必须具有以下格式之一：

   * 数字
   * 日期
   * 货币

* 您可以将聚合器添加到显示计算的列。 聚合值显示在视图或报表的分组中。 有关更多信息，请参阅 [分组：显示在分组中聚合多个计算值的结果](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
* 用于列定义的代码行必须与引入聚合器的代码行相同，并且前面有“聚合器”。 例如，如果您有一列，其中在项目中显示计划小时数，则该列主行的文本模式为：

   ```
   valuefield=workRequired
   valueformat=compound
   ```

   当您想要聚合视图分组中所有行的值时，我们可以添加以下代码以添加聚合器值： `aggregator.valuefield=workRequired` ( `aggregator.valuefield` 行必须与 `valuefield` 描述列) `aggregator.valueformat=compound` ( `aggregator.valueformat` 行必须具有与 `valueformat` 描述列) `aggregator.function=SUM` （这是一个必填行，用于指示您希望如何聚合列，在这种情况下，您需要将所有计划小时数添加到分组行中的一个数字中） `aggregator.displayformat=minutesAsHoursString` (因为小时数以分钟为单位存储在Workfront中，因此我们希望 `displayformat` （以分钟为单位存储）
