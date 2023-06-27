---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: 分配模块
description: 在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用Allocadia的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 0%

---

# [!DNL Allocadia] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Allocadia]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!DNL Allocadia] 模块，您必须拥有 [!DNL Allocadia] 帐户。

## Connect [!DNL Allocadia] 到 [!DNL Workfront Fusion]

您可以创建与 [!DNL Allocadia] 直接从 [!DNL Allocadia] 模块。

1. 在任意 [!DNL Allocadia] 模块，单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 字段。
1. 选择您要使用北美服务器还是欧洲服务器。
1. 输入用户名和密码。
1. 单击 **[!UICONTROL 继续]** 以创建连接并返回模块。

## [!DNL Allocadia] 模块及其字段

配置时 [!DNL Allocadia] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Allocadia] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

#### [!UICONTROL 观看记录]

此触发器模块执行添加、更新特定类型的对象或同时添加和更新特定类型的对象的方案。 该模块返回与一个或多个记录关联的所有标准字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关将Allocadia帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[！UICONTROL Connect Allocadia]到Workfront Fusion</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">筛选</td> 
   <td> <p>选择您希望方案仅观看“新记录”、“[！UICONTROL仅更新记录”]还是“新记录和更新记录”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">实体类型</td> 
   <td>选择您希望模块监视的Allocadia记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">输出</td> 
   <td> <p>选择要包含在模块输出中的字段。 可用字段取决于您选择的实体类型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">限制</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内监视的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [自定义API调用](#custom-api-call)
* [读取记录](#read-record)
* [创建记录](#create-record)
* [删除记录](#delete-record)
* [更新记录](#update-record)

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL Allocadia] API。 这样，您就可以创建一个其他人无法实现的数据流自动化 [!DNL Allocadia] 模块。

该操作基于您指定的图元类型（Allocadia对象类型）。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Allocadia] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>输入相对路径 <code>https://api-na.allocadia.com/{version}</code> 或 <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注释:  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

该操作模块从中的单个记录读取数据 [!DNL Allocadia].

您指定记录的ID。

该模块返回与记录关联的任何标准字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Allocadia] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL实体类型]</td> 
   <td>选择类型 [!DNL Allocadia] 您希望模块读取的记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td> <p>选择要包含在模块输出中的字段。 可用字段取决于您选择的[！UICONTROL实体类型]。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>输入或映射唯一值 [!DNL Allocadia] 您希望模块读取的记录的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建记录]

该操作模块创建一个记录。

该模块返回记录的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Allocadia] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL实体类型]</td> 
   <td>选择是要基于联机项目还是列选择创建新的记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL预算]</td> 
   <td> <p>选择要创建记录的预算。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>选择要用于创建新记录的列。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Label]</td> 
   <td>输入或映射新记录的标签</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除记录]

此操作模块删除特定记录。

您指定记录的ID。

该模块返回记录的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Allocadia] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL实体类型]</td> 
   <td> <p>选择要删除的图元类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL行项目]</strong> </p> <p>输入行项目标识</p> </li> 
     <li> <p><strong>[！UICONTROL列选择]</strong> </p> <p>选择要从中删除记录的预算，然后输入列ID和选项ID。</p> </li> 
     <li> <p><strong>[！UICONTROL预测标记]</strong> </p> <p>选择要从中删除记录的预算，然后输入标签ID。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新记录]

此操作模块更新记录，例如行项目、用户或列选择。

您指定记录的ID。

该模块返回记录的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关将您的[！UICONTROL Allocadia]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL实体类型]</td> 
   <td>选择类型 [!DNL Allocadia] 记录您希望模块更新的内容。 根据您选择的实体类型，将显示其他字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL预算]</td> 
   <td> <p>选择要更新记录的预算。 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

#### [!UICONTROL 搜索记录]

此搜索模块查找对象中的记录 [!DNL Allocadia] 与指定的搜索查询匹配的用户名称。

您可以将此信息映射到场景中的后续模块。

您可以指定所需记录的类型。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Allocadia] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL实体类型]</td> 
   <td>选择类型 [!DNL Allocadia] 您希望模块搜索的记录。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL预算]</td> 
   <td> <p>选择要搜索的预算。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL结果集]</td> 
   <td>选择您希望模块返回所有匹配记录，还是仅返回第一个匹配记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最大记录数]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜索条件]</td> 
   <td>选择要搜索的字段，选择操作，然后输入或映射要搜索的值。 您可以添加 [!DNL AND] 或 [!DNL OR] 规则以进一步筛选您的搜索。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td> <p>选择要包含在模块输出中的字段。 可用字段取决于您选择的实体类型。</p> </td> 
  </tr> 
 </tbody> 
</table>
