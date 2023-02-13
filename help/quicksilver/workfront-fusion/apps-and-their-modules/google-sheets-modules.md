---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Google工作表模块
description: 为了使用 [!DNL Google Sheets] with [!DNL Adobe Workfront Fusion],you need the [!UICONTROL Workfront Fusion Google Sheets] 扩展（可选，但对于即时触发器是必需的）。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 11d62222-df34-472d-93d7-f0d53eb95c9b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3894'
ht-degree: 0%

---

# [!DNL Google Sheets] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Google Sheets]，并将其连接到多个第三方应用程序和服务。

有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 [创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

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
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!UICONTROL Google工作表] 模块，您必须 [!UICONTROL Google] 帐户。

## 触发器

### [!UICONTROL 监视行]

从电子表格中每个新添加的行中检索值。

模块仅检索之前未填写的新行。 触发器不会处理被覆盖的行。

>[!IMPORTANT]
>
>如果工作表包含空行，则不会处理空白行之后的任何行。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL电子表格] </td> 
   <td> <p>选择包含要查看的工作表的电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作表] </td> 
   <td> <p>选择要监视新行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表包含标题]</td> 
   <td> <p> 选择电子表格是否包含标题行。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Yes]</strong> </p> <p>模块不会作为输出数据检索标题行。 </p> <p>输出中的变量名称由标头调用。</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>模块还检索第一个表行</p> <p>输出中的变量名称称为A、B、C、D等。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL带标题的行] </td> 
   <td> <p>输入标题行的范围。 例如， <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL第一个表行]</td> 
   <td> <p>输入表第一行的范围。 例如， <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL值呈现选项]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL格式化的值]</p> <p>这些值将根据单元格的格式在回复中计算和格式化。 格式设置基于电子表格的区域设置，而不是请求用户的区域设置。 例如，如果 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式为货币，则 <code>A2</code> 将返回 <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL未格式化的值]</p> <p>将计算这些值，但不会在回复中设置格式。 例如，如果 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式为货币，则 <code>A2</code> 会返回 <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL公式]</p> <p>将不会计算这些值。 答复中将包含公式。 例如，如果 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式为货币，则 <code>A2</code> 将返回 <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL日期和时间渲染选项]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL序列号]</p> <p>指示日期、时间、日期时间和持续时间字段以“序列号”格式双倍输出，如Lotus 1-2-3所推广的。 值的整数部分（小数的左侧）计算自1899年12月30日以来的天数。 小数部分（小数的右侧）将时间计为一天的小数。 例如，1900年1月1日中午为2.5,2是因为在1899年12月30日之后为2天，而。5是因为中午为半天。 1900年2月1日下午3点将为33.625。这正确地将1900年视为不是闰年。</p> <p style="font-weight: bold;">[!UICONTROL带格式的字符串]</p> <p>指示日期、时间、日期时间和持续时间字段以其给定数字格式（取决于电子表格的区域设置）作为字符串输出。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>设置 [!DNL Workfront Fusion] 将在一个执行周期内使用。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 操作

* [[!UICONTROL 添加行]](#add-a-row)
* [[!UICONTROL 更新行]](#update-a-row)
* [[!UICONTROL 清除行]](#clear-a-row)
* [[!UICONTROL 删除行]](#delete-a-row)
* [[!UICONTROL 获取单元]](#get-a-cell)
* [[!UICONTROL 更新单元格]](#update-a-cell)
* [[!UICONTROL 清除单元格]](#clear-a-cell)
* [[!UICONTROL 添加工作表]](#add-a-sheet)
* [[!UICONTROL 创建电子表格]](#create-a-spreadsheet)
* [[!UICONTROL 删除工作表]](#delete-a-sheet)
* [[!UICONTROL 进行API调用]](#make-an-api-call)

### [!UICONTROL 添加行]

此模块会向工作表中附加一行。

配置 [!DNL Google Sheets] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Google Sheets] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>选择是手动选择电子表格和工作表，还是通过映射来选择。</p> <p>注意：例如，在 [!DNL Workfront Fusion] 方案中，并且您希望在方案中直接在新创建的电子表格中添加数据。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子表格] </td> 
   <td> <p>选择 [!DNL Google] 电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>选择要向其添加行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL列范围]</td> 
   <td>选择要处理的列范围。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL表包含标题]</td> 
   <td> <p> 选择电子表格是否包含标题行。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Yes]</strong> </p> <p>模块不会作为输出数据检索标题行。 </p> <p>输出中的变量名称由标头调用。</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>模块还检索第一个表行</p> <p>输出中的变量名称称为A、B、C、D等。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值] </td> 
   <td> <p>输入或映射要添加行的所需单元格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值输入选项]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL用户输入]</strong></p> <p>这些值会像用户在UI中键入它们一样进行解析。 数字仍然是数字，但字符串可以转换为数字、日期或其他格式，这些格式遵循在通过 [!DNL Google Sheets] UI。</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> 用户输入的值将不进行解析，并按原样存储。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL插入数据选项]</td> 
   <td> <p>指定在输入新数据时如何更改现有数据。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL插入行]</strong></p> <p>将为新数据插入行。</p> </li> 
     <li> <p><strong>[!UICONTROL覆盖]</strong> </p> <p>新数据会覆盖写入区域中的现有数据。 向工作表末尾添加数据会插入新的行或列，以便能够写入数据。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新行]

此模块允许您更改选定行中的单元格内容。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>选择是手动选择电子表格和工作表，还是通过映射来选择。</p> <p>注意：手动映射非常有用，例如，当在[!UICONTROL Workfront Fusion]方案中创建新电子表格，并且您希望直接在该方案中将数据添加到新创建的电子表格时。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子表格] </td> 
   <td> <p>选择 [!DNL Google] 电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>选择要更新中行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL行号]</td> 
   <td> <p> 输入要更新的行数。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL表包含标题]</td> 
   <td> <p> 选择电子表格是否包含标题行。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Yes]</strong> </p> <p>模块不会作为输出数据检索标题行。 </p> <p>输出中的变量名称由标头调用。</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>模块还检索第一个表行</p> <p>输出中的变量名称称为A、B、C、D等。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值] </td> 
   <td> <p>输入值或将其映射到要更改（更新）的行的所需单元格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值输入选项]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL用户输入]</strong></p> <p>这些值会像用户在UI中键入它们一样进行解析。 数字仍然是数字，但字符串可以转换为数字、日期或其他格式，这些格式遵循在通过 [!DNL Google Sheets] UI。</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> 用户输入的值将不进行解析，并按原样存储。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 清除行]

从指定的行中删除值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子表格] </td> 
   <td> <p>选择 [!DNL Google] 包含要从中清除行的工作表的电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p> 选择要从中清除数据的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL行号]</td> 
   <td> <p>输入要从中清除数据的行数。 例如， <code> 23</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 删除行]

删除指定的行。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子表格] </td> 
   <td> <p>选择包含要从中删除行的工作表的Google电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td>电子表格 </td> 
   <td> <p>选择要从中删除行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>行号</td> 
   <td> <p>输入要删除的行数。 示例: <code>23</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 获取单元]

从选定的单元格中检索值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子表格] </td> 
   <td> <p>选择 [!DNL Google] 电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>选择包含要从中检索数据的单元格的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL单元格] </td> 
   <td> <p>输入要从中检索数据的单元格的ID。 示例: <code>A6</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值呈现选项]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL格式化的值]</p> <p>这些值将根据单元格的格式在回复中计算和格式化。 格式设置基于电子表格的区域设置，而不是请求用户的区域设置。 例如，如果 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式为货币，则 <code>A2</code> 将返回 <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Unformatted value]</p> <p>将计算这些值，但不会在回复中设置格式。 例如，如果 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式为货币，则 <code>A2</code> 会返回 <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Formula]</p> <p>将不会计算这些值。 答复中将包含公式。 例如，如果 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式为货币，则 <code>A2</code> 将返回 <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!DNL Serial number]</p> <p>指示日期、时间、日期时间和持续时间字段以“序列号”格式双倍输出，如Lotus 1-2-3所推广的。 值的整数部分（小数的左侧）计算自1899年12月30日以来的天数。 小数部分（小数的右侧）将时间计为一天的小数。 例如，1900年1月1日中午为2.5,2是因为在1899年12月30日之后为2天，而。5是因为中午为半天。 1900年2月1日下午3点将为33.625。这正确地将1900年视为不是闰年。</p> <p style="font-weight: bold;">[!DNL Formatted string]</p> <p>指示日期、时间、日期时间和持续时间字段以其给定数字格式（取决于电子表格的区域设置）作为字符串输出。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新单元格]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子表格] </td> 
   <td> <p>选择 [!DNL Google] 电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL单元格] </td> 
   <td> <p>输入要更新的单元格的ID。 示例: <code>A5</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值]</td> 
   <td> <p>输入单元格的新值。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值输入选项]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL用户输入]</strong></p> <p>这些值会像用户在UI中键入它们一样进行解析。 数字仍然是数字，但字符串可以转换为数字、日期或其他格式，这些格式遵循在通过 [!DNL Google Sheets] UI。</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> 用户输入的值将不进行解析，并按原样存储。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 清除单元格]

从指定的单元格中删除值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子表格] </td> 
   <td> <p>选择包含要从中清除单元格的工作表的Google电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>选择要从中清除单元格的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL单元格] </td> 
   <td> <p>输入要清除的单元格的ID。 示例: <code>A5</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 添加工作表]

在所选电子表格中创建新工作表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子表格] </td> 
   <td> <p>选择要添加工作表的Google电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL属性]</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">[!UICONTROL标题]</p> <p>输入新工作表的名称。</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL索引]</p> <p>输入工作表位置。 缺省值为0（首先放置页面）</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 创建电子表格]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL标题] </td> 
   <td> <p>输入新电子表格的名称。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL区域设置]</td> 
   <td> <p>使用以下格式之一输入电子表格的区域设置：</p> 
    <ul> 
     <li>ISO 639-1语言代码，例如 <code>en</code></li> 
     <li>ISO 639-2语言代码，例如 <code>haw</code>，如果不存在639-1代码</li> 
     <li>ISO语言代码和国家/地区代码的组合，例如 <code>en_US</code></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL重新计算间隔]</td> 
   <td> <p>重新计算易失函数之前等待的时间：</p> <p style="font-weight: bold;">[!UICONTROL On Change]</p> <p>易失函数在每次更改时都会更新。</p> <p style="font-weight: bold;">[!UICONTROL更改时和每分钟]</p> <p>易失函数会在每次更改和每分钟更新一次。</p> <p style="font-weight: bold;">[!UICONTROL（更改时）和每小时]</p> <p>易失函数在每次更改时和每小时更新一次。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL时区]</td> 
   <td> <p> 选择电子表格的时区。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Number格式]</td> 
   <td> <p>选择电子表格中所有单元格的默认格式。</p> <p><strong>[!UICONTROL Text]</strong>:文本格式。 示例: <code>1000. 12</code></p> <p><strong>[!UICONTROL Number]</strong>:数字格式。 示例: <code>1,000.12</code></p> <p><strong>[!UICONTROL百分比]</strong>:格式百分比。 示例: <code>10. 12%</code></p> <p><strong>[!UICONTROL货币]</strong>:货币格式。 示例: <code>$1,000.12</code></p> <p><strong>[!UICONTROL日期]</strong>:日期格式。 示例: <code>9/26/2008</code></p> <p><strong>[!UICONTROL时间]</strong>:时间格式。 示例: <code>3:59:00 PM</code></p> <p><strong>[!UICONTROL日期时间]</strong>:日期和时间格式。 示例: <code>9/26/08 15:59:00</code> </p> <p><strong>[!UICONTROL Scientific]</strong>科学的数字格式。 示例: <code>1. 01E+03</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>单击 <strong>[!UICONTROL Add]</strong> 向电子表格中添加工作表。 对于每个工作表，输入或映射工作表的标题和工作表的索引。 索引为0表示第一个工作表。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 删除工作表]

删除特定工作表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子表格] </td> 
   <td> <p>选择 [!DNL Google] 电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>选择要删除的工作表。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 进行API调用]

此操作模块允许您执行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关将[Fusion App]帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>输入相对于 <code>https://sheets.googleapis.com/v4/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。例如， <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p> 以标准JSON对象的形式添加API调用的查询。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:   <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 搜索

* [[!UICONTROL 搜索行]](#search-rows)
* [[!UICONTROL 搜索行（高级）]](#search-rows-advanced)
* [[!UICONTROL 获取范围值]](#get-range-values)
* [[!UICONTROL 列表表]](#list-sheets)

### [!UICONTROL 搜索行]

使用过滤器选项搜索行。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关将[Fusion App]帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子表格] </td> 
   <td> <p>选择 [!DNL Google] 电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>选择要在中搜索行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL表包含标题]</td> 
   <td> <p> 选择电子表格是否包含标题行。 如果选择[!UICONTROL Yes]选项，则模块不会检索标题行，因为输出数据和输出中的变量名称随后由标题调用。 如果选择[!UICONTROL No]选项，则模块还会检索输出中的第一个表行和变量名称，这些名称随后将仅调用A、B、C、D等。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL列范围]</td> 
   <td>选择要处理的列范围。 示例: <code>A-F</code></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL过滤器]</td> 
   <td> <p>为要搜索的行设置过滤器。</p> <p>有关过滤器的更多信息，请参阅 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">向[!UICONTROL Adobe Workfront Fusion]中的方案添加过滤器</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL排序顺序]</td> 
   <td>选择是升序排序还是降序排序。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td>选择要排序的列。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值呈现选项]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL格式化的值]</p> <p>这些值将根据单元格的格式在回复中计算和格式化。 格式设置基于电子表格的区域设置，而不是请求用户的区域设置。 例如，如果 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式为货币，则 <code>A2</code> 将返回 <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL未格式化的值]</p> <p>将计算这些值，但不会在回复中设置格式。 例如，如果 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式为货币，则 <code>A2</code> 会返回 <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL公式]</p> <p>将不会计算这些值。 答复中将包含公式。 例如，如果 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式为货币，则 <code>A2</code> 将返回 <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日期和时间渲染选项]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL序列号]</p> <p>指示将日期、时间、日期时间和持续时间字段输出为“序列号”格式的双倍，如Lotus 1-2-3所推广的。 值的整数部分（小数的左侧）计算自1899年12月30日以来的天数。 小数部分（小数的右侧）将时间计为一天的小数。 例如，1900年1月1日中午为2.5,2是因为在1899年12月30日之后为2天，而。5是因为中午为半天。 1900年2月1日下午3点将为33.625。这正确地将1900年视为不是闰年。</p> <p style="font-weight: bold;">[!UICONTROL带格式的字符串]</p> <p>指示日期、时间、日期时间和持续时间字段以其给定数字格式（取决于电子表格的区域设置）作为字符串输出。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回行数的最大值]</td> 
   <td>设置 [!DNL Workfront Fusion] 将在一个执行周期中返回。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜索行（高级）]

返回与给定条件匹配的结果。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子表格] </td> 
   <td> <p>选择包含要搜索的工作表的Google电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>选择包含要搜索的行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL查询]</td> 
   <td> <p>使用 [!DNL Google Charts Query Language]. 示例: <code>select * where B = "John"</code></p> <p>有关 [!DNL Google Charts Query Language]，请参阅 <a href="https://developers.google.com/chart/interactive/docs/querylanguage">查询语言参考</a> 在 [!DNL Google] 文档。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 获取范围值]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子表格] </td> 
   <td> <p>选择 [!DNL Google] 电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>选择要从中获取范围内容的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL范围] </td> 
   <td> <p>输入要获取的范围。 示例: <code>A1:D25</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL表包含标题]</td> 
   <td> <p>如果工作表具有标题行，则选中此框</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL带标题的行]</td> 
   <td>输入表标题的范围。 示例 <code>A1:F1</code>. 如果将字段留空， [!DNL Workfront Fusion] 将假定标题位于指定范围的第一行中。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值呈现选项]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL格式化的值]</p> <p>这些值将根据单元格的格式在回复中计算和格式化。 格式设置基于电子表格的区域设置，而不是请求用户的区域设置。 例如，如果 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式为货币，则 <code>A2</code> 将返回 <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL未格式化的值]</p> <p>将计算这些值，但不会在回复中设置格式。 例如，如果 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式为货币，则 <code>A2</code> 会返回 <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL公式]</p> <p>将不会计算这些值。 答复中将包含公式。 例如，如果 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式为货币，则 <code>A2</code> 将返回 <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日期和时间渲染选项]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL序列号]</p> <p>指示将日期、时间、日期时间和持续时间字段输出为“序列号”格式的双倍，如Lotus 1-2-3所推广的。 值的整数部分（小数的左侧）计算自1899年12月30日以来的天数。 小数部分（小数的右侧）将时间计为一天的小数。 例如，1900年1月1日中午为2.5,2是因为在1899年12月30日之后为2天，而。5是因为中午为半天。 1900年2月1日下午3点将为33.625。这正确地将1900年视为不是闰年。</p> <p style="font-weight: bold;">[!UICONTROL带格式的字符串]</p> <p>指示日期、时间、日期时间和持续时间字段以其给定数字格式（取决于电子表格的区域设置）作为字符串输出。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 列表表]

此模块返回电子表格中所有工作表的列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Sheets] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子表格] </td> 
   <td> <p>选择 [!DNL Google] 包含要列出的工作表的电子表格。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用限制

如果出错 `429: RESOURCE_EXHAUSTED` 发生时，您已超出API速率限制。

的 [!DNL Google Sheets] API的限制是每个项目每100秒有500个请求，每个用户每100秒有100个请求。 对读取和写入的限制将单独进行跟踪。 没有每日使用限制。

有关更多详细信息，请参阅 [developers.google.com/sheets/api/limits](https://developers.google.com/sheets/api/limits).

## 提示和技巧

* [如何从 [!DNL Google] 工作表](#how-to-get-empty-cells-from-a-google-sheet)
* [在工作表中添加按钮以运行方案](#add-a-button-in-a-sheet-to-run-a-scenario)

### 如何从 [!DNL Google Sheet]

使用 [!UICONTROL 搜索行（高级）] 模块并使用此公式获取空列。
<pre>选择* [!UICONTROL，其中E为空​]</pre>其中，“E”是列，“is null”是条件。 您可以使用[Google查询语言]创建更高级的查询。](https://developers.google.com/chart/interactive/docs/querylanguage)

### 在工作表中添加按钮以运行方案

1. 在 [!DNL Workfront Fusion]，插入 **[!UICONTROL 网钩]** > **[!UICONTROL 自定义Web挂接]** 模块/触发器(请参阅 [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md))。

1. 复制Webhook的URL。
1. 执行方案。
1. 在Google工作表中，选择 **[!UICONTROL 插入]** > **[!UICONTROL 绘图]**.....

1. 在 [!UICONTROL 绘图] ，单击 **[!UICONTROL 文本框]** 图标 ![](assets/text-box.png) 靠窗顶。
1. 设计按钮并单击 **[!UICONTROL 保存并关闭]** 按钮：
1. 按钮将放置在您的工作表中。 单击按钮右上角的三个垂直圆点：
1. 选择 **[!UICONTROL 分配脚本……].** 中。
1. 输入脚本的名称（函数），例如 `runScenario` 单击 **[!UICONTROL 确定]**:
1. 选择 **[!UICONTROL 工具]** > **[!UICONTROL 脚本编辑器]** 菜单栏。

1. 插入以下代码：

   * 函数的名称必须与您在步骤9中指定的名称相对应。
   * 将URL替换为您在步骤2中复制的Webhook URL。

      <pre>函数runScenario(){</pre><pre>UrlFetchApp.fetch("<webhook you copied>“);</pre><pre>}</pre>

1. 按 **[!UICONTROL Ctrl+S]** 要保存脚本文件，请输入项目名称并单击 **[!UICONTROL 确定]**.

1. 切换回 [!DNL Google Sheets] 并单击新按钮。
1. 向脚本授予所需的授权：
1. 在 [!DNL Workfront Fusion]，确认方案已成功执行。

## 在电子表格中存储日期

如果将日期值存储在电子表格中，且没有任何格式，则它将以ISO 8601格式的文本形式显示在电子表格中。 但是， [!DNL Google Sheets] 使用日期但不理解此文本的公式或函数(示例：公式 `=A1+10`)将显示以下错误：

![](assets/mceclip6-350x87.png)

帮助允许 [!DNL Google Sheets] 要了解日期，请将其格式设置为 [[!UICONTROL formatDate] （日期）格式；[时区])](../../workfront-fusion/functions/date-and-time-functions.md#formatda) 函数。 作为第二个参数传递给函数的正确格式取决于电子表格的区域设置设置。

要确定正确的格式，请执行以下操作：

1. 选择 **[!UICONTROL 文件]** > **[!UICONTROL 电子表格]** 设置来验证/设置区域设置。

1. 验证/设置正确的区域设置后，通过选择 **[!UICONTROL 格式]** > **[!UICONTROL 数值]** 中。 格式显示在“日期时间”菜单项旁边：

1. 要撰写应传递到 [!UICONTROL formatDate()] 函数，请参阅 [中用于日期和时间格式的令牌 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md).

**示例：** 的使用 `MM/DD/YYYY HH:mm:ss` 美国区域设置的格式：

![](assets/locale-time-350x83.png)

## 开发 [!DNL Google Sheets] 函数

如果您错过了内置功能，但其特点是 [!DNL Google Sheets]，您可以利用它。 有关更多信息，请参阅 [使用 [!DNL Google Sheets] 函数](../../workfront-fusion/functions/map-using-functions.md#exploiti) in [使用 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md) .

## 保留 [!DNL Google Sheets] 从将数字更改为日期

您可能会发现，在 [!DNL Google] 工作表。 例如，您键入1-2019，并将其打算为文本，但Google将其解释为日期。 您可以将数字预格式化为纯文本，以防止出现这种情况。

1. 在 [!DNL Google Sheets]，突出显示包含数字或数字的列或单元格。
1. 单击 **[!UICONTROL 格式]** > **[!UICONTROL 数值]** > **[!UICONTROL 纯文本]**.

中的另一个解决方法 [!DNL Workfront Fusion] 是在数字前键入撇号(&#39;)，例如&#39;1-2019或&#39;1/47&#39;。 从发送数据后，单元格中不显示撇号 [!DNL Workfront Fusion].
