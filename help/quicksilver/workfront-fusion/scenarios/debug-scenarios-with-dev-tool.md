---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 使用Adobe Workfront Fusion Devtool调试场景
description: Adobe Workfront Fusion Devtool允许您了解场景并排除其故障。 Devtool向Chrome开发人员工具添加了一个额外的面板。 使用此调试器面板，您可以检查场景的所有手动运行，查看所有执行的操作，并查看每个执行的API调用的详细信息。 您可以查看导致错误的模块、操作或单个响应，并使用该知识来优化场景。
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 6edcb5b826bdcf37b62396a926c923875a3a1436
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 1%

---

# 使用调试方案 [!DNL Adobe Workfront Fusion] Devtool

此 [!DNL Adobe Workfront Fusion] 通过Devtool，您可以了解各种方案并排除其故障。 Devtool会添加一个额外的面板到 [!DNL Chrome Developer Tools]. 使用此调试器面板，您可以检查场景的所有手动运行，查看所有执行的操作，并查看每个执行的API调用的详细信息。 您可以查看导致错误的模块、操作或单个响应，并使用该知识来优化场景。

>[!NOTE]
>
>对于机密场景、自动执行和成功操作，调试器面板中的记录将受限或不可用。

有关Fusion Devtool的视频介绍和演练，请参见

* [Fusion开发工具](https://video.tv.adobe.com/v/3427031/){target=_blank}.
* [Devtool演练](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/troubleshooting-and-error-handling/dev-tool-walkthrough.html?lang=en)

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
  <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 对于工作自动化和集成]，[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 访问Workfront Fusion Devtool

根据您是否在中使用Fusion，访问Devtool会有所不同 [!DNL Adobe Unified Experience].

* [在中访问开发工具 [!DNL Adobe Unified Experience]](#access-the-devtool-in-the-adobe-unified-experience)
* [访问Classic中的Devtool [!DNL Fusion] 体验](#access-the-devtool-in-the-classic-fusion-experience)

### 在中访问开发工具 [!DNL Adobe Unified Experience] 或新的Fusion体验

如果您在AdobeUnified Shell中使用Fusion，或者已更新到新的Fusion Experience，则可以从场景编辑器访问开发工具。

1. 单击 **辅助工具** ![辅助工具](assets/debugger-icon.png) 图标（靠近屏幕底部）。

或：

1. 转到要调试的方案的方案编辑器。

   要查找方案编辑器，请参阅 [方案编辑器](/help/quicksilver/workfront-fusion/scenarios/scenario-editor.md).

1. 右键单击页面的空白区域（不是模块）。
1. 选择 **打开Devtool**.

### 访问Classic中的Devtool [!DNL Fusion] 体验

在Classic中使用开发工具 [!DNL Fusion] experience，您必须安装 [!DNL Chrome] 扩展。 然后，您可以从 [!DNL Chrome] 开发人员工具。

* [安装安装 [!DNL Chrome] Devtool扩展](#install-the-chrome-devtool-extension)
* [找到 [!DNL Workfront Fusion] Devtool](#locate-the-workfront-fusion-devtool)

#### 安装 [!DNL Chrome] Devtool扩展

您可以添加 [!DNL Workfront Fusion] 开发工具到 [!DNL Chrome] 通过 [!UICONTROL [!DNL Chrome] 网络商店].

1. 单击 [此链接](https://chromewebstore.google.com/u/1/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn) 以转到 [!DNL Workfront Fusion] 开发工具 [!UICONTROL [!DNL Chrome] 网络商店].
1. 单击 **[!UICONTROL 添加至[!DNL Chrome]]**.
1. 在打开的窗口中，检查权限。 如果您同意这些权限，请单击 **[!UICONTROL 添加扩展]**.

此 [!DNL Workfront Fusion] Devtool扩展将添加到 [!DNL Chrome] 扩展。


#### 找到 [!DNL Workfront Fusion] Devtool

要使用 [!DNL Workfront Fusion] Devtool，您必须添加 [!DNL Workfront Fusion] Devtool扩展到 [!DNL Chrome] 浏览器，如中所述 [安装Chrome Devtool扩展](#install-the-chrome-Devtool-extension).

1. 打开您的 [!DNL Workfront Fusion] 方案。
1. 打开 [!DNL Chrome Developer Tools]：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Command + Option + I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Control + Shift + I</p> <p> 或 </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >我们建议停靠 [!DNL Chrome Developer Console] 以更好地查看您的模块。

1. 单击 **[!DNL Workfront Fusion]** tab in [!DNL Chrome Dev Tools].

## 使用 [!DNL Workfront Fusion] Devtool

Workfront Fusion Devtool分为3个主要部分。 您可以在Devtool窗口的左侧面板中找到这些内容。

* [实时流](#live-stream)
* [场景调试器](#scenario-debugger)
* [工具](#tools)

### 实时流

在您的场景中单击运行一次后，实时流会显示后台发生的情况。

1. 单击 **[!UICONTROL 实时流]** 图标 ![](assets/live-stream-icon.png) 以打开Live Stream部分。
1. 执行以下任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>操作</th> 
      <th>说明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">查看请求信息</td> 
      <td> <p>您可以查看场景中每个模块的以下信息</p> 
       <ul> 
        <li> <p>请求标头（API端点URL、http方法、调用请求的时间和日期、请求标头以及查询字符串）</p> </li> 
        <li> <p>请求正文</p> </li> 
        <li> <p>响应标头</p> </li> 
        <li> <p>响应正文</p> </li> 
       </ul> <p>要查看此信息，请单击右侧面板中相应的选项卡， [!DNL Workfront Fusion] 开发工具。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>搜索请求和响应</p> </td> 
      <td> <p>在左侧面板的搜索字段中输入搜索词 [!DNL Workfront Fusion] Devtool ，用于仅显示包含搜索词的请求。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>删除请求列表 </p> </td> 
      <td> <p>单击Devtool左面板右上角的垃圾桶图标，以清除记录在 [!DNL Workfront Fusion] 开发工具。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>启用控制台日志记录</p> </td> 
      <td> <p>单击计算机图标 <img src="assets/console-computer-icon.png"> 位于Devtool左面板的右上角。</p> <p>当计算机图标为绿色时，将启用控制台中的日志记录。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>以原始JSON格式或cURL检索请求</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>原始JSON</strong> </p> <p>单击 <strong>[！UICONTROL原始副本]</strong> 在开发工具右窗格的右上角。</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>单击 <strong>[！UICONTROL复制cURL]</strong> 在开发工具右窗格的右上角。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### 场景调试器

场景调试器适用于更复杂的场景。 它显示方案运行的历史记录，使您能够按名称或ID搜索模块。

1. 单击 **[!UICONTROL 场景调试器]** 图标 ![](assets/scenario-debugger-icon.png) 以打开方案调试器。
1. （可选）在的左窗格中的搜索字段中输入搜索词（名称或模块ID） [!DNL Workfront Fusion] 中的开发工具 [!UICONTROL 场景调试器] 部分。
1. 双击模块名称以在方案编辑器中打开其设置。
1. 通过单击所需操作查看请求详细信息。

### 工具

此 [!DNL Workfront Fusion] Devtool提供了一些工具，可让您更轻松地设置场景。

1. 单击 **[!UICONTROL 工具]** 图标 ![](assets/console-tools-icon.png) 以打开“工具”。
1. 选择要使用的工具
1. 配置字段，如下所述。
1. 单击 **[!UICONTROL 运行]**.

工具及其字段：

* [焦点模块](#focus-a-module)
* [通过映射查找模块](#find-modules-by-mapping)
* [获取应用程序元数据](#get-app-metadata)
* [复制映射](#copy-mapping)
* [复制筛选器](#copy-filter)
* [交换连接](#swap-connection)
* [交换变量](#swap-variable)
* [交换应用程序](#swap-app)
* [以64为底](#base-64)
* [复制模块名称](#copy-module-name)
* [重新映射源](#remap-source)
* [突出显示应用程序](#highlight-app)
* [迁移GS](#migrate-gs)

#### [!UICONTROL 焦点模块]

按ID打开指定模块的设置。

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL模块ID]</td>
        <td>输入要打开其设置的模块的ID。</td>
    </tr>
</table>

#### [!UICONTROL 通过映射查找模块]

允许您搜索指定术语的模块值。 输出包含包含已搜索术语的模块ID。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Keyword]</td> 
   <td> <p> 输入要搜索的搜索词。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL仅使用值]</p> </td> 
   <td> <p>启用此选项可仅搜索模块字段的值。</p> <p>禁用此选项还可搜索模块字段的名称。</p> <p>通过名称和标签参数执行搜索。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取应用程序元数据]

按应用程序的模块名称或ID检索应用程序的元数据。 例如，在需要了解场景中使用的应用程序版本时，这非常有用。

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL源模块]</td>
        <td>选择要检索元数据的模块。</td>
    </tr>
</table>

#### [!UICONTROL 复制映射]

将值从源模块复制到目标模块。

>[!CAUTION]
>
>确保设置了正确的源模块和目标模块。 如果选择其他类型的模块，则将删除目标模块中的值。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL源模块]</td> 
   <td> <p> 选择模块或输入要从中复制字段值的模块的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL目标模块]</p> </td> 
   <td> <p>选择模块或输入要插入源模块值的模块的ID。</p> <p>重要信息：将覆盖目标模块中的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 复制筛选器]

将过滤器设置从源模块复制到目标模块。

>[!NOTE]
>
>复制操作在位于所选模块左侧的过滤器上执行。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL源模块]</td> 
   <td> <p> 选择模块或输入要从中复制筛选器值的模块的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL目标模块]</p> </td> 
   <td> <p>选择模块或输入要插入源模块中的过滤器值的模块的ID。</p> <p>重要信息：将覆盖目标模块中的值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL保留回退路由设置]</p> </td> 
   <td> <p>源筛选器设置为回退路由。 启用此选项还可以将目标过滤器设置为回退路由。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 交换连接]

在同一应用程序的场景中，复制从源模块到每个模块的连接。

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL源模块]</td>
        <td>选择模块或输入要从中复制连接的模块的ID。</td>
    </tr>
</table>

#### [!UICONTROL 交换变量]

在场景中搜索指定的变量并使用新变量替换它们。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL变量查找]</td> 
   <td> <p> 在场景中从模块找到要替换的可变丸子，并将其复制到此（[！UICONTROL变量到查找]）字段中。 在字段中，它带有双大括号。 示例： <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL替换为]</p> </td> 
   <td> <p>在场景的模块中，找到要用来替换变量的变量，并将其复制到此（[！UICONTROL要查找的变量]）字段中。 在字段中，它带有双大括号。 示例： <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL模块]</p> </td> 
   <td> <p>选择要替换变量的模块。 如果未选择任何模块，则变量将在整个场景中被替换。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 交换应用程序]

将场景中选定的应用程序版本替换为其他应用程序版本。

例如，这可用于将Gmail和电子邮件应用程序的模块升级到最新版本。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">要替换的[！UICONTROL应用程序]</td> 
   <td> <p> 选择要替换的应用程序。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL替换为]</p> </td> 
   <td> <p>选择要替换它的应用程序。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 以64为底]

允许您将输入的数据编码为Base64或解码Base64。 有些请求被编码为Base64。 当您想要搜索编码请求中的特定数据时，此工具可能很有用。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL操作] </td> 
   <td> <p>选择是要将数据从[！UICONTROL Raw Data]字段编码为Base64，还是要将Base64解码为Raw Data。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL原始数据]</p> </td> 
   <td> <p> 根据上面[！UICONTROL Operation]字段中选择的选项，输入要编码为Base64的数据，如果要解码为原始数据，则输入Base64。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 复制模块名称]

将所选模块的名称复制到剪贴板。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL模块] </td> 
   <td> <p>选择要复制其名称的模块。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重新映射源]

允许您将映射源从一个模块更改为另一个模块。

您必须首先将要用作源模块的模块添加到方案中的路由。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL源模块] </td> 
   <td> <p> 选择要替换的模块作为场景中其他模块的映射源。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL目标模块]</p> </td> 
   <td> <p>选择要用作新映射源的模块。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL要编辑的模块]</p> </td> 
   <td> <p>如果不想更改整个方案中的映射，请选择要更改映射的模块。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 突出显示应用程序]

突出显示场景中指定应用程序的模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL应用程序将突出显示] </td> 
   <td> <p> 选择要在场景中突出显示的应用程序。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL版本] </p> </td> 
   <td> <p>选择要高亮显示的应用程序版本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL高亮颜色]</p> </td> 
   <td> <p> 输入要用于突出显示模块的颜色十六进制。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 迁移GS]

此工具专为升级而设计 [!DNL Google Sheets] （旧版）模块到最新 [!DNL Google Sheets] 版本。 它在场景路由中的模块的以前版本之后添加了该模块的新版本。

此模块不需要您设置任何参数。
