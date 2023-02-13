---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: 亚洛迪亚模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用Allocadia的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 0%

---

# [!DNL Allocadia] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Allocadia]，并将其连接到多个第三方应用程序和服务。

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

使用 [!DNL Allocadia] 模块，您必须具有 [!DNL Allocadia] 帐户。

## 连接 [!DNL Allocadia] to [!DNL Workfront Fusion]

您可以创建与 [!DNL Allocadia] 直接从内部帐户 [!DNL Allocadia] 模块。

1. 在任意 [!DNL Allocadia] 模块，单击 **[!UICONTROL 添加]** 旁边 [!UICONTROL 连接] 字段。
1. 选择您要使用北美服务器还是欧洲服务器。
1. 输入您的用户名和密码。
1. 单击 **[!UICONTROL 继续]** 创建连接，然后返回到模块。

## [!DNL Allocadia] 模块及其字段

配置 [!DNL Allocadia] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Allocadia] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

#### [!UICONTROL 观看记录]

当添加、更新或同时添加特定类型的对象时，此触发器模块会执行一个方案。 模块会返回与记录或记录关联的所有标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关将Allocida帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia]到Workfront Fusion</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">筛选</td> 
   <td> <p>选择是希望方案仅观看新记录、[!UICONTROL仅更新记录]，还是新记录和更新记录。</p> </td> 
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
   <td> <p>输入或映射您希望模块在每个方案执行周期中监视的最大记录数。</p> </td> 
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

通过此操作模块，您可以对 [!DNL Allocadia] API。 这样，您就可以创建数据流自动化，而另一个数据流无法实现 [!DNL Allocadia] 模块。

该操作基于您指定的实体类型（Allocida对象类型）。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Allocadia] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">连接 [!DNL Allocadia] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>输入相对于 <code>https://api-na.allocadia.com/{version}</code> 或 <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:  <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

此操作模块从 [!DNL Allocadia].

您指定记录的ID。

模块会返回与记录关联的任何标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Allocadia] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">连接 [!DNL Allocadia] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL实体类型]</td> 
   <td>选择 [!DNL Allocadia] 记录您希望模块读取的内容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出]</td> 
   <td> <p>选择要包含在模块输出中的字段。 可用字段取决于您选择的[!UICONTROL实体类型]。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>输入或映射唯一 [!DNL Allocadia] 您希望模块读取的记录的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建记录]

此操作模块会创建记录。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Allocadia] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">连接 [!DNL Allocadia] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL实体类型]</td> 
   <td>根据行项目还是列选择选择选择是要创建新记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL预算]</td> 
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

此操作模块会删除特定记录。

您指定记录的ID。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Allocadia] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">连接 [!DNL Allocadia] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL实体类型]</td> 
   <td> <p>选择要删除的实体类型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL行项目]</strong> </p> <p>输入行项目ID</p> </li> 
     <li> <p><strong>[!UICONTROL列选择]</strong> </p> <p>选择要从中删除记录的预算，然后输入列ID和选择ID。</p> </li> 
     <li> <p><strong>[!UICONTROL预测标记]</strong> </p> <p>选择要从中删除记录的预算，然后输入标记ID。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新记录]

此操作模块会更新记录，如行项目、用户或列选择。

您指定记录的ID。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关将[!UICONTROL Allocadia]帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">连接 [!DNL Allocadia] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL实体类型]</td> 
   <td>选择 [!DNL Allocadia] 记录您希望模块更新。 其他字段会根据您选择的实体类型显示。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL预算]</td> 
   <td> <p>选择要更新记录的预算。 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

#### [!UICONTROL 搜索记录]

此搜索模块在 [!DNL Allocadia] 与您指定的搜索查询匹配。

您可以在方案的后续模块中映射此信息。

您可以指定所需记录的类型。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Allocadia] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">连接 [!DNL Allocadia] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL实体类型]</td> 
   <td>选择 [!DNL Allocadia] 记录您希望模块搜索的内容。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL预算]</td> 
   <td> <p>选择要搜索的预算。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL结果集]</td> 
   <td>选择是希望模块返回“所有匹配记录”，还是仅返回“第一个匹配记录”。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录的最大计数]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索标准]</td> 
   <td>选择要搜索的字段，选择操作，然后输入或映射要搜索的值。 您可以添加 [!DNL AND] 或 [!DNL OR] 规则来进一步筛选搜索。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出]</td> 
   <td> <p>选择要包含在模块输出中的字段。 可用字段取决于您选择的实体类型。</p> </td> 
  </tr> 
 </tbody> 
</table>
