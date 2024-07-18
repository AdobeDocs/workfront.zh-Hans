---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Google Forms模块
description: 通过 [!DNL Adobe Workfront Fusion Google Forms] 模块，您可以在Google Forms上监视、选择、添加、更新或删除响应。
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 0%

---

# [!DNL Google Forms]模块

[!DNL Adobe Workfront Fusion] [!DNL Google Forms]模块允许您监视、选择、添加、更新或删除您的[!DNL Google Forms]响应。

要将[!DNL Google Docs]与[!DNL Adobe Workfront Fusion]一起使用，需要具有[!DNL Google]帐户。 如果您还没有[!DNL Google]帐户，则可以在[!DNL Google]帐户帮助页面中创建一个帐户。

如果需要有关创建方案的说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案。

有关模块的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模块。

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
   <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先决条件

要使用[!DNL Google Forms]模块，您必须具有[!DNL Google]帐户。

## 从表单创建电子表格

为了处理表单响应，必须创建响应中的电子表格。

1. 打开您的表单。
1. 转到&#x200B;**[!UICONTROL 响应]**&#x200B;选项卡。
1. 单击&#x200B;**[!UICONTROL 创建电子表格]**&#x200B;图标![](assets/spreadsheet-icon.png)。

1. 选择要创建新电子表格还是现有电子表格
1. 单击&#x200B;**[!UICONTROL 创建]**。

## [!DNL Google Forms]模块及其字段

配置[!DNL Google Forms]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Google Forms]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

#### [!UICONTROL 观看回应]

查看表单以获取新响应。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Spreadsheet]</td> 
   <td> <p>选择电子表格，其中包含您要监视新响应的表单中的响应。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作表]</td> 
   <td> <p> 选择包含表单响应的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL带有标题的行]</td> 
   <td>指定表的标题行。 默认行是<code>A1:Z1</code>。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值渲染选项]</td> 
   <td> <p>指定您希望如何在输出中呈现值。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL格式化的值]</strong> </p> <p>将根据单元格的格式在回复中计算和设置值的格式。 格式设置基于电子表格的区域设置，而不是请求用户的区域设置。 例如，如果<code>A1</code>是<code>1. 23</code>，<code>A2 </code>是<code>=A1</code>并且格式为货币，则<code>A2</code>返回<code>$1. 23</code>。</p> </li> 
     <li> <p><strong>[！UICONTROL未格式化的值]</strong> </p> <p>会计算值，但不在回复中设置格式。 例如，如果<code>A1</code>是<code>1. 23</code>，<code>A2 </code>是<code>=A1</code>并且格式为货币，则<code>A2</code>返回数字<code>1. 23</code>。</p> </li> 
     <li> <p><strong>[！UICONTROL公式]</strong> </p> <p>不计算值。 回复包括公式。 例如，如果<code>A1</code>是<code>1. 23</code>，<code>A2 </code>是<code>=A1</code>并且格式为货币，则<code>A2</code>返回<code>=A1</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL日期和时间渲染选项]</td> 
   <td>选择您希望日期、时间和持续时间在输出中的表示方式。 如果[！UICONTROL Value Render Option]设置为[！UICONTROL Formatted Value]，则会忽略此字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p> 设置[!DNL Workfront Fusion]在一个周期内处理的最大响应数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 添加响应]](#add-a-response)
* [[!UICONTROL 更新响应]](#update-a-response)
* [[!UICONTROL 删除响应]](#delete-a-response)

#### [!UICONTROL 添加响应]

此模块会将新响应附加到表单电子表格的底部。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Spreadsheet]</td> 
   <td> <p>选择包含要添加响应的工作表的电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作表]</td> 
   <td> <p> 选择包含表单响应的工作表。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[！UICONTROL Values]</p> </td> 
   <td> <p>输入工作表列的所需值。</p> <p>对于格式正确的[！UICONTROL Timestamp]列，请使用以下值：</p><pre>formatDate（现在；DD/MM/YYYY HH：mm；UTC）</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL值输入选项]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[！UICONTROL Raw]</strong> </p> <p> 用户输入的值不会进行解析，而是按原样存储。 </p> </li> 
     <li> <p><strong>[！UICONTROL用户已进入]</strong></p> <p>这些值会像用户在UI中键入值一样进行解析。 数字仍为数字，但字符串可能会转换为数字、日期或其他格式，这些规则与通过[!DNL Google Sheets] UI在单元格中输入文本时应用的规则相同。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL Insert data option]</td> 
   <td> <p>指定在输入新数据时如何更改现有数据。 </p> 
    <ul> 
     <li> <p><strong>[！UICONTROL覆盖]</strong> </p> <p>新数据将覆盖其写入区域中的现有数据。 将数据添加到工作表末尾会插入新的行或列，以便写入数据。</p> </li> 
     <li> <p><strong>[！UICONTROL插入行]</strong></p> <p>为新数据插入行。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新响应]

此模块将更新所选的响应。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Spreadsheet]</td> 
   <td> <p>选择包含要更新响应的工作表的电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作表]</td> 
   <td> <p> 选择包含表单响应的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL行号]</p> </td> 
   <td> <p>输入或映射要更新的行号。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Values]</p> </td> 
   <td> <p>在所需列中输入新值。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL值输入选项]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[！UICONTROL Raw]</strong> </p> <p> 用户输入的值不会进行解析，而是按原样存储。 </p> </li> 
     <li> <p><strong>[！UICONTROL用户已进入]</strong></p> <p>这些值会像用户在UI中键入值一样进行解析。 数字仍为数字，但字符串可能会转换为数字、日期或其他格式，这些规则与通过[!DNL Google Sheets] UI在单元格中输入文本时应用的规则相同。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除响应]

此模块删除所选的响应。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Spreadsheet]</td> 
   <td> <p>选择包含您要删除响应的工作表的电子表格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作表]</td> 
   <td> <p> 选择包含表单响应的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL行号]</p> </td> 
   <td> <p>输入或映射要删除的行数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

* [[!UICONTROL 搜索响应]](#search-responses)
* [[!UICONTROL 搜索响应（高级]）](#search-responses-advanced)

#### [!UICONTROL 搜索响应]

此模块会返回与给定条件匹配的响应。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>连接</td>
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[！UICONTROL Spreadsheet]</td>
   <td> <p>选择要搜索的表单。</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[！UICONTROL工作表] </td>
   <td> <p>选择包含表单响应的工作表。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[！UICONTROL列范围]</td>
   <td> <p> 选择要搜索的列范围。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL筛选器]</td> 
   <td> <p>定义要作为搜索响应依据的筛选器。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[！UICONTROL排序顺序] </td>
   <td> <p>选择是按升序还是降序对返回的响应进行排序。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[！UICONTROL Order By]</td>
   <td> <p> 选择要对返回的响应排序的列。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL值渲染选项]</td> 
   <td> <p>指定您希望如何在输出中呈现值。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL格式的值]</strong></p> <p>将根据单元格的格式在回复中计算和设置值的格式。 格式设置基于电子表格的区域设置，而不是请求用户的区域设置。 例如，如果<code>A1</code>是<code>1. 23</code>，<code>A2 </code>是<code>=A1</code>并且格式为货币，则<code>A2</code>返回<code>$1. 23</code>。</p> </li> 
     <li> <p><strong>[！UICONTROL未格式化的值]</strong> </p> <p>会计算值，但不在回复中设置格式。 例如，如果<code>A1</code>是<code>1. 23</code>，<code>A2 </code>是<code>=A1</code>并且格式为货币，则<code>A2</code>返回数字<code>1. 23</code>。</p> </li> 
     <li> <p><strong>[！UICONTROL公式]</strong> </p> <p>不计算值。 回复包括公式。 例如，如果<code>A1</code>是<code>1. 23</code>，<code>A2 </code>是<code>=A1</code>并且格式为货币，则<code>A2</code>返回<code>=A1</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[！UICONTROL日期和时间渲染选项]</td>
    <td>选择您希望日期、时间和持续时间在输出中的表示方式。 如果[！UICONTROL Value Render]选项设置为“格式化的值”，则忽略此字段。 </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[！UICONTROL返回的最大响应数]</td>
   <td> <p> 设置[!DNL Workfront Fusion]在一个周期内返回的最大响应数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索响应（高级）]

此模块使用[[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage)执行搜索。 此模块不返回行号。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL Spreadsheet]</td>
   <td> <p>选择包含要搜索的工作表的电子表格。</p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL工作表]</td>
   <td> <p> 选择包含表单响应的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL筛选器]</td> 
   <td> <p>使用<a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>定义搜索查询。</p> <p>示例： <code>select * where C = "John"</code>检索C列为“John”的行的所有值。</p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL返回的最大行数]</td>
   <td> <p> 设置[!DNL Workfront Fusion]在一个周期内返回的最大响应数。</p> </td> 
  </tr> 
 </tbody> 
</table>
