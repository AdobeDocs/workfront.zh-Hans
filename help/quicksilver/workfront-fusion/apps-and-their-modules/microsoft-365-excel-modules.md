---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Excel模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用Microsoft 365 Excel的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2768'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel]模块

在[!DNL Adobe Workfront Fusion]方案中，您可以自动使用[!DNL Microsoft 365 Excel]的工作流，并将其连接到多个第三方应用程序和服务。

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

要使用[!DNL Microsoft office 365 Excel]，您必须拥有Microsoft帐户。

## Microsoft Office 365 Excel API信息

Microsoft Office 365 Excel连接器使用以下内容：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基本URL</td> 
   <td> https://graph.microsoft.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> v1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API标记</td> 
   <td>v2.0.16</td> 
  </tr>
 </tbody> 
 </table>



## 正在将[!DNL Office 365 Excel]服务连接到[!DNL Workfront Fusion]

有关将[!DNL Office 365 Excel]帐户连接到[!UICONTROL Workfront Fusion]的说明，请参阅[创建与[!UICONTROL Adobe Workfront Fusion]的连接 — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>某些Microsoft应用程序使用相同的连接，该连接与单个用户权限相关联。 因此，在创建连接时，权限同意屏幕除了显示当前应用程序所需的任何新权限外，还会显示以前授予此用户连接的任何权限。
>
>例如，如果用户拥有通过Excel Connector授予的“读取表”权限，然后在Outlook Connector中创建连接以读取电子邮件，则权限同意屏幕将显示已授予的“读取表”权限和新要求的“写入电子邮件”权限。

## [!DNL Microsoft Office 365 Excel]模块及其字段

配置[!DNL Microsoft 365 Excel]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Microsoft 365 Excel]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

* [工作簿](#workbook)
* [工作表](#worksheet)
* [表](#table)
* [其他](#other)

### 工作簿

* [Watch工作簿](#watch-workbooks)
* [搜索工作簿](#search-workbooks)
* [下载工作簿](#download-a-workbook)

#### [!UICONTROL 观看工作簿]

此触发器模块在创建工作簿时启动方案。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹]</td> 
   <td> <p>选择要监视新工作簿的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL筛选器]</p> </td> 
   <td> <p>您可以将过滤器设置为仅监视符合所选条件的工作簿。</p> <p>对于每个筛选器，输入希望筛选器计算的字段、运算符以及希望筛选器允许的值。 您可以通过添加AND或OR规则来使用多个过滤器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射每个方案执行周期中您希望模块返回的最大工作簿数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索工作簿]

此操作模块搜索[!DNL Excel]工作簿。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹]</td> 
   <td> <p>选择要搜索工作簿的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL筛选器]</p> </td> 
   <td> <p>您可以设置过滤器，以仅搜索符合您选择标准的工作簿。</p> <p>对于每个筛选器，输入希望筛选器计算的字段、运算符以及希望筛选器允许的值。 您可以通过添加AND或OR规则来使用多个过滤器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射每个方案执行周期中您希望模块返回的最大工作表数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载工作簿]

此操作模块下载指定Excel工作簿的内容。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL下载工作簿]</td> 
   <td> <p>选择您希望如何标识要下载的模块的工作簿。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL，通过手动输入ID]</strong> </p> <p>在[！UICONTROL工作簿ID]字段中，输入或映射您希望模块下载的特定工作簿的ID。</p> </li> 
     <li> <p>通过从路径中选择<strong>[！UICONTROL]</strong> </p> <p>在[！UICONTROL工作簿]字段中，选择要让模块下载的工作簿。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 工作表

* [[!UICONTROL 监视工作表行]](#watch-worksheet-rows)
* [[!UICONTROL 列出工作表]](#list-worksheets)
* [[!UICONTROL 列出工作表行]](#list-worksheet-rows)
* [[!UICONTROL 添加工作表]](#add-a-worksheet)
* [[!UICONTROL 添加工作表行]](#add-a-worksheet-row)
* [[!UICONTROL 更新工作表行]](#update-a-worksheet-row)
* [[!UICONTROL 删除工作表行]](#delete-a-worksheet-row)

#### [!UICONTROL 监视工作表行]

此触发器模块会在工作表中添加新行时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作簿] </td>
   <td> <p>选择包含您要监视新行的工作表的工作簿。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>选择要监视新行的Excel工作表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL限制]</td>
   <td> <p>输入或映射每个方案执行周期中您希望模块返回的最大工作表行数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出工作表]

此操作模块检索指定工作簿中的工作表列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作簿] </td>
   <td> <p>选择包含您希望模块列出的工作表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL限制]</td>
   <td> <p>输入或映射每个方案执行周期中您希望模块返回的最大工作表数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出工作表行]

此操作模块检索指定工作表中的行列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[！UICONTROL工作簿] </td>
   <td> <p>选择包含工作表的工作簿，该工作表包含要列出的行。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>选择包含要列出的行的工作表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL限制]</td>
   <td> <p>输入或映射每个方案执行周期中您希望模块返回的最大工作表行数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加工作表]

此操作模块在所选工作簿中创建新工作表。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[！UICONTROL工作簿] </td>
   <td> <p>选择要添加工作表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL名称] </td>
   <td> <p>输入或映射新工作表的名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加工作表行]

此操作模块向所选工作表添加一个新行。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作簿] </td>
   <td> <p>选择包含要添加行的工作表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>选择要添加行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL要输入的值的类型]</p> </td> 
   <td> <p>选择要输入工作表的值的类型。 </p> 
    <ul> 
     <li> <p><strong>[！UICONTROL公式]</strong> </p> <p> Excel尝试计算指定的表达式。 公式中的函数名称为英文。 示例： <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[！UICONTROL公式本地]</strong> </p> <p>Excel尝试计算指定的表达式。 函数名称使用Excel应用程序的语言。 示例：<code>=SUM(A1, 1.5)</code>与 <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[！UICONTROL值]</strong> </p> <p>Excel不计算该值。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL Row]</td>
    <td>对于每个列，输入您希望该列在新行中的值。</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新工作表行]

此操作模块可更新现有的工作表行。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作簿] </td>
   <td> <p>选择包含要更新的行的工作表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>选择包含要更新的行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL要输入的值的类型]</p> </td> 
   <td> <p>选择要输入工作表的值的类型。 </p> 
    <ul> 
     <li> <p><strong>[！UICONTROL公式]</strong> </p> <p> Excel尝试计算指定的表达式。 公式中的函数名称为英文。 示例： <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[！UICONTROL公式本地]</strong> </p> <p>Excel尝试计算指定的表达式。 函数名称使用Excel应用程序的语言。 示例：<code>=SUM(A1, 1.5)</code>与 <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[！UICONTROL值]</strong> </p> <p>Excel不计算该值。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行ID]</td> 
   <td>选择要更新的行的编号。</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL Row]</td>
    <td>对于每个列，输入您希望该列在新行中的值。</td>
   —&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除工作表行]

此操作模块从工作表中删除一行。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作簿] </td>
   <td> <p>选择包含您要删除的行的工作表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表]</td>
   <td> <p> 选择包含要删除的行的工作表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL行ID]</td>
   <td>输入或映射要删除的行的ID。</td> 
  </tr> 
 </tbody> 
</table>

### 表

* [[!UICONTROL 监视表行]](#watch-table-rows)
* [[!UICONTROL 列出表]](#list-tables)
* [[!UICONTROL 列出表行]](#list-table-rows)
* [[!UICONTROL 获取表]](#get-a-table)
* [[!UICONTROL 添加表]](#add-a-table)
* [[!UICONTROL 添加表格行]](#add-a-table-row)
* [[!UICONTROL 更新表]](#update-a-table)
* [[!UICONTROL 删除表]](#delete-a-table)

#### [!UICONTROL 监视表行]

在向表中添加新行时，此触发器将启动一个方案。

>[!NOTE]
>
>此处的表引用工作簿中嵌入的表元素。 不是整个表（工作簿/工作表）。

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL工作簿]</p> </td> 
   <td> <p>选择包含要监视的表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p> 选择包含要监视的表的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL表]</p> </td> 
   <td> <p>选择要监视的表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL限制]</td>
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大行数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出表]

此搜索模块检索所有表对象的列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[！UICONTROL工作簿] </td>
   <td> <p>选择包含要列出的表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>选择包含要列出的表的工作表</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL限制]</td>
   <td> <p>输入或映射每个方案执行周期中您希望模块返回的最大表数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出表行]

此搜索模块检索工作簿中所有表行的列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作簿] </td>
   <td> <p>选择包含要列出行的表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>选择包含要列出行的表的工作表</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL表] </td>
   <td> <p>选择包含要列出的行的表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL限制]</td>
   <td> <p>输入或映射您希望模块在每个方案执行周期中返回的最大表行数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取表]

此操作模块检索指定表的元数据。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[！UICONTROL Connection]</p>
   </td> 
   <td> 
     <p>有关将Office 365帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL获取表]</td> 
   <td> <p>选择您希望如何标识要检索的表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在[！UICONTROL工作簿ID]字段中，输入或映射包含要检索的表的工作簿ID。</p> <p>在[！UICONTROL表名称]字段中，输入或映射要检索的表的名称。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择包含要检索的表的工作簿和工作表，然后选择该表。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加表]

此操作模块会在Excel工作表中创建一个表元素。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作簿] </td> 
   <td> <p>选择包含要添加表的工作表的工作簿。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作表] </td> 
   <td> <p>选择要添加表的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Has headers]</td> 
   <td> <p>启用此选项可将第一行定义为表标题。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL地址]</p> </td> 
   <td> <p>通过指示左上单元格和右下单元格来设置表的大小。 示例： <code>A1:C10</code>创建了一个包含3列和10行的表。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加表格行]

此操作模块修改现有表。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作簿] </td>
   <td> <p>选择包含要添加行的表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>选择包含要添加行的表的工作表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL表]</td>
   <td>选择要添加行的表。</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[！UICONTROL Row]</td>
    <td>对于每个列，输入您希望该列在新行中的值。</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL行ID]</p> </td> 
   <td> <p>要在表格上的特定位置添加行，请输入或映射行号。 模块在此行之后插入新行。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新表]

此操作模块更新现有的表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL更新表]</td> 
   <td> <p>选择您希望如何标识要更新的表。</p> 
    <ul> 
     <li> <p><strong>手动输入</strong> </p> <p>在[！UICONTROL工作簿ID]字段中，输入或映射包含要更新的表的工作簿ID。</p> <p>在[！UICONTROL表名]字段中，输入或映射要更新的表名。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择包含要更新的表的工作簿和工作表，然后选择该表。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL表] </td> 
   <td> <p>选择要更新的表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名称]</td> 
   <td> <p>如果要重命名表，请输入或映射表的新名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Show Headers]</td> 
   <td> <p>启用此选项以显示更新表的标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL显示总计]</td> 
   <td>启用此选项以显示表的总值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL样式]</td> 
   <td>为新表选择样式。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除表]

此操作模块从[!DNL Excel]工作表中删除指定的表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL获取表]</td> 
   <td> <p>选择您希望如何标识要删除的表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在[！UICONTROL工作簿ID]字段中，输入或映射包含要删除表的工作簿的ID。</p> <p>在[！UICONTROL表名称]字段中，输入或映射要删除的表的名称。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择包含要删除表的工作簿和工作表，然后选择该表。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 检索数据]](#retrieve-data)
* [[!UICONTROL 进行API调用]](#make-an-api-call)

#### [!UICONTROL 检索数据]

此操作从定义的工作表范围中检索数据，并为每行返回一个捆绑。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作簿] </td> 
   <td> <p>选择包含要检索的数据的工作簿。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作表] </td> 
   <td> <p>选择包含要检索的数据的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL范围] </td> 
   <td> <p>通过指定左上单元格和右下单元格，指定要从中检索数据的工作表区域。 示例： <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 进行API调用]

此操作模块允许您进行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>输入相对于<code>https://graph.microsoft.com</code>的路径。 示例：<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP请求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion会为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：   <p>在JSON中使用条件语句（如<code>if</code>）时，请将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
