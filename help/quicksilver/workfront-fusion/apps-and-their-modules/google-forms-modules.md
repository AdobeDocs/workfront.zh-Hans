---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Google Forms模块
description: 的 [!DNL Adobe Workfront Fusion Google Forms] 利用模块，可监视、选择、添加、更新或删除Google Forms上的响应。
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1382'
ht-degree: 0%

---

# [!DNL Google Forms] 模块

的 [!DNL Adobe Workfront Fusion] [!DNL Google Forms] 利用模块，可监视、选择、添加、更新或删除您的 [!DNL Google Forms].

为了使用 [!DNL Google Docs] with [!DNL Adobe Workfront Fusion]，则需要具有 [!DNL Google] 帐户。 如果你没有 [!DNL Google] 帐户，您可以在 [!DNL Google] 帐户帮助页面。

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
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!DNL Google Forms] 模块，您必须 [!DNL Google] 帐户。

## 从表单创建电子表格

要处理表单响应，必须从响应中创建电子表格。

1. 打开您的表单。
1. 转到 **[!UICONTROL 响应]** 选项卡。
1. 单击 **[!UICONTROL 创建电子表格]** 图标 ![](assets/spreadsheet-icon.png).

1. 选择是要创建新电子表格还是要创建现有电子表格
1. 单击&#x200B;**[!UICONTROL 创建]**。

## [!DNL Google Forms] 模块及其字段

配置 [!DNL Google Forms] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Google Forms] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

#### [!UICONTROL 监视响应]

监视表单以获取新响应。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL电子表格]</td> 
   <td> <p>选择包含表单中要查看新响应的响应的电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作表]</td> 
   <td> <p> 选择包含表单响应的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL带标题的行]</td> 
   <td>指定表的标题行。 默认行为 <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL值呈现选项]</td> 
   <td> <p>指定希望如何在输出中呈现值。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL格式化的值]</strong> </p> <p>根据单元格的格式，在回复中计算值并设置其格式。 格式设置基于电子表格的区域设置，而不是请求用户的区域设置。 例如，如果 <code>A1</code> is <code>1. 23</code> 和 <code>A2 </code>is <code>=A1</code> 格式为货币，则 <code>A2</code> 返回 <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL未格式化的值]</strong> </p> <p>值会进行计算，但不会在回复中设置格式。 例如，如果 <code>A1</code> is <code>1. 23</code> 和 <code>A2 </code>is <code>=A1</code> 格式为货币，则 <code>A2</code> 返回数字 <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL公式]</strong> </p> <p>不计算值。 答复中包含公式。 例如，如果 <code>A1</code> is <code>1. 23</code> 和 <code>A2 </code>is <code>=A1</code> 格式为货币，则 <code>A2</code> 返回 <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日期和时间渲染选项]</td> 
   <td>选择您希望在输出中显示日期、时间和持续时间的方式。 如果将[!UICONTROL Value Render Options]设置为[!UICONTROL Formated Value]，则忽略此字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p> 设置最大响应数 [!DNL Workfront Fusion] 可在一个周期中使用。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 添加响应]](#add-a-response)
* [[!UICONTROL 更新响应]](#update-a-response)
* [[!UICONTROL 删除响应]](#delete-a-response)

#### [!UICONTROL 添加响应]

此模块会在表单电子表格的底部附加一个新响应。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL电子表格]</td> 
   <td> <p>选择包含要添加响应的工作表的电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作表]</td> 
   <td> <p> 选择包含表单响应的工作表。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL值]</p> </td> 
   <td> <p>在工作表列中输入所需的值。</p> <p>对于格式正确的[!UICONTROL Timestamp]列，请使用以下值：</p><pre>formatDate(now;DD/MM/YYYY HH:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL值输入选项]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> 用户输入的值将不进行解析，并按原样存储。 </p> </li> 
     <li> <p><strong>[!UICONTROL用户输入]</strong></p> <p>这些值会像用户在UI中键入它们一样进行解析。 数字仍然是数字，但字符串可以转换为数字、日期或其他格式，这些格式遵循在通过 [!DNL Google Sheets] UI。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL插入数据选项]</td> 
   <td> <p>指定在输入新数据时如何更改现有数据。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL覆盖]</strong> </p> <p>新数据会覆盖写入区域中的现有数据。 向工作表末尾添加数据会插入新的行或列，以便能够写入数据。</p> </li> 
     <li> <p><strong>[!UICONTROL插入行]</strong></p> <p>将为新数据插入行。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新响应]

此模块更新所选响应。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL电子表格]</td> 
   <td> <p>选择包含要更新响应的工作表的电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作表]</td> 
   <td> <p> 选择包含表单响应的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL行号]</p> </td> 
   <td> <p>输入或映射要更新的行数。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL值]</p> </td> 
   <td> <p>为所需列输入新值。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL值输入选项]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> 用户输入的值将不进行解析，并按原样存储。 </p> </li> 
     <li> <p><strong>[!UICONTROL用户输入]</strong></p> <p>这些值会像用户在UI中键入它们一样进行解析。 数字仍然是数字，但字符串可以转换为数字、日期或其他格式，这些格式遵循在通过 [!DNL Google Sheets] UI。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除响应]

此模块会删除选定的响应。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL电子表格]</td> 
   <td> <p>选择包含要删除响应的工作表的电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作表]</td> 
   <td> <p> 选择包含表单响应的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL行号]</p> </td> 
   <td> <p>输入或映射要删除的行数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

* [[!UICONTROL 搜索响应]](#search-responses)
* [[!UICONTROL 搜索响应（高级）])](#search-responses-advanced)

#### [!UICONTROL 搜索响应]

此模块会返回与给定条件匹配的响应。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>连接</td>
   <td> <p>有关连接 [!DNL Google] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL电子表格]</td>
   <td> <p>选择要搜索的表单。</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL工作表] </td>
   <td> <p>选择包含表单响应的工作表。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL列范围]</td>
   <td> <p> 选择要搜索的列范围。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL过滤器]</td> 
   <td> <p>定义要按搜索响应的过滤器。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL排序顺序] </td>
   <td> <p>选择是按升序还是按降序对返回的响应进行排序。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Order By]</td>
   <td> <p> 选择要对返回的响应进行排序的列。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL值呈现选项]</td> 
   <td> <p>指定希望如何在输出中呈现值。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL格式化的值]</strong></p> <p>根据单元格的格式，在回复中计算值并设置其格式。 格式设置基于电子表格的区域设置，而不是请求用户的区域设置。 例如，如果 <code>A1</code> is <code>1. 23</code> 和 <code>A2 </code>is <code>=A1</code> 格式为货币，则 <code>A2</code> 返回 <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL未格式化的值]</strong> </p> <p>值会进行计算，但不会在回复中设置格式。 例如，如果 <code>A1</code> is <code>1. 23</code> 和 <code>A2 </code>is <code>=A1</code> 格式为货币，则 <code>A2</code> 返回数字 <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL公式]</strong> </p> <p>不计算值。 答复中包含公式。 例如，如果 <code>A1</code> is <code>1. 23</code> 和 <code>A2 </code>is <code>=A1</code> 格式为货币，则 <code>A2</code> 返回 <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL日期和时间渲染选项]</td>
    <td>选择您希望在输出中显示日期、时间和持续时间的方式。 如果[!UICONTROL Value Render]选项设置为“格式化值”，则忽略此字段。 </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL返回的最大响应数]</td>
   <td> <p> 设置最大响应数 [!DNL Workfront Fusion] 在一个周期中返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索响应（高级）]

此模块使用 [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage). 此模块不返回行号。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL连接]</td>
   <td> <p>有关连接 [!DNL Google] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL电子表格]</td>
   <td> <p>选择包含要搜索的工作表的电子表格。</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL工作表]</td>
   <td> <p> 选择包含表单响应的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL过滤器]</td> 
   <td> <p>使用定义搜索查询 <a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>.</p> <p>示例： <code>select * where C = "John"</code> 检索C列为“John”的行的所有值。</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL返回行数的最大值]</td>
   <td> <p> 设置最大响应数 [!DNL Workfront Fusion] 在一个周期中返回。</p> </td> 
  </tr> 
 </tbody> 
</table>
