---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 使用Adobe Workfront Fusion DevTool调试方案
description: 利用Adobe Workfront Fusion DevTool，可了解情景并排除其故障。 DevTool向Chrome开发人员工具中添加了一个额外的面板。 使用此调试器面板，您可以检查方案的所有手动运行，查看所有已执行的操作，并查看每个已执行API调用的详细信息。 您可以查看哪个模块、操作或单个响应导致了错误，并使用该知识来优化您的方案。
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1665'
ht-degree: 0%

---

# 使用 [!DNL Adobe Workfront Fusion] DevTool

的 [!DNL Adobe Workfront Fusion] DevTool允许您了解情景并排除其故障。 DevTool会向 [!DNL Chrome Developer Tools]. 使用此调试器面板，您可以检查方案的所有手动运行，查看所有已执行的操作，并查看每个已执行API调用的详细信息。 您可以查看哪个模块、操作或单个响应导致了错误，并使用该知识来优化您的方案。

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

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
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化） </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 安装 [!DNL Chrome] DevTool扩展

使用 [!DNL Workfront Fusion] DevTool，您首先需要安装它。

1. 单击 [此链接](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/workfront-fusion-devtool.zip) 下载扩展。
1. 下载文件后，将其解压缩到您选择的文件夹。
1. 在中打开选项卡 [!DNL Chrome]
1. 在选项卡的搜索栏中，输入 `chrome://extensions`.
1. 单击 **[!UICONTROL 开发人员模式]** 在屏幕的右上角切换以启用开发人员模式。 如果切换到右侧，则会启用开发人员模式。
1. 单击 **[!UICONTROL 加载已解压的]**.
1. 选择包含DevTool的文件夹（您在步骤2中已将文件解压到该文件夹）。

   解压后，DevTool会显示在您的其他Chrome扩展中。

## 找到 [!DNL Workfront Fusion] DevTool

使用 [!DNL Workfront Fusion] DevTool中，您必须将 [!DNL Workfront Fusion] DevTool扩展 [!DNL Chrome] 浏览器，如 [安装Chrome DevTool扩展](#install-the-chrome-devtool-extension).

1. 打开 [!DNL Workfront Fusion] 情景。
1. 打开 [!DNL Chrome Developer Tools]:

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
   >我们建议将 [!DNL Chrome Developer Console] 以更好地查看您的模块。

1. 单击 **[!DNL Workfront Fusion]** 选项卡 [!DNL Chrome Dev Tools].

## 使用 [!DNL Workfront Fusion] DevTool

Workfront Fusion DevTool分为3个主要部分。 您可以在DevTool窗口的左侧面板中找到这些组件。

* [实时流](#live-stream)
* [方案调试器](#scenario-debugger)
* [工具](#tools)

### 实时流

在方案中，当您单击运行一次时，实时流会显示在后台发生的情况。

1. 单击 **[!UICONTROL 实时流]** 图标 ![](assets/live-stream-icon.png) 以打开实时流部分。
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
      <td> <p>您可以查看方案中每个模块的以下信息</p> 
       <ul> 
        <li> <p>请求头（API端点URL、http方法、调用请求的时间和日期、请求头和查询字符串）</p> </li> 
        <li> <p>请求正文</p> </li> 
        <li> <p>响应标头</p> </li> 
        <li> <p>响应正文</p> </li> 
       </ul> <p>要查看此信息，请单击 [!DNL Workfront Fusion] 开发工具。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>搜索请求和响应</p> </td> 
      <td> <p>在 [!DNL Workfront Fusion] DevTool来仅显示包含搜索词的请求。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>删除请求列表 </p> </td> 
      <td> <p>单击DevTool左侧面板右上角的垃圾桶图标，以清除 [!DNL Workfront Fusion] 开发工具。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>启用控制台日志记录</p> </td> 
      <td> <p>单击计算机图标 <img src="assets/console-computer-icon.png"> 工具的右上角。</p> <p>当计算机图标为绿色时，控制台中会启用日志记录功能。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>使用原始JSON格式或cURL检索请求</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>原始JSON</strong> </p> <p>单击 <strong>[!UICONTROL Copy RAW]</strong> 工具右窗格的右上角。</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>单击 <strong>[!UICONTROL Copy cURL]</strong> 工具右窗格的右上角。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### 方案调试器

情景调试器对于更复杂的情景非常有用。 它显示方案运行的历史记录，并允许您按模块的名称或ID搜索模块。

1. 单击 **[!UICONTROL 方案调试器]** 图标 ![](assets/scenario-debugger-icon.png) 以打开方案调试器。
1. （可选）在的左窗格的搜索字段中输入搜索词（名称或模块ID） [!DNL Workfront Fusion] 中的DevTool [!UICONTROL 方案调试器] 中。
1. 双击模块的名称，以在方案编辑器中打开其设置。
1. 通过单击所需的操作，查看请求详细信息。

### 工具

的 [!DNL Workfront Fusion] DevTool具有一些工具，可让您更轻松地设置方案。

1. 单击 **[!UICONTROL 工具]** 图标 ![](assets/console-tools-icon.png) 打开工具。
1. 选择要使用的工具
1. 按如下所述配置字段。
1. 单击 **[!UICONTROL 运行]**.

工具及其字段：

* [集中模块](#focus-a-module)
* [通过映射查找模块](#find-modules-by-mapping)
* [获取应用程序元数据](#get-app-metadata)
* [复制映射](#copy-mapping)
* [复制筛选器](#copy-filter)
* [交换连接](#swap-connection)
* [交换变量](#swap-variable)
* [交换应用程序](#swap-app)
* [基64](#base-64)
* [复制模块名称](#copy-module-name)
* [重新映射源](#remap-source)
* [突出显示应用程序](#highlight-app)
* [迁移GS](#migrate-gs)

#### [!UICONTROL 集中模块]

按ID打开指定模块的设置。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL模块ID]</td>
        <td>输入要为其打开设置的模块的ID。</td>
    </tr>
</table>

#### [!UICONTROL 通过映射查找模块]

用于搜索指定术语的模块值。 输出包含包含您搜索的术语的模块ID。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL关键字]</td> 
   <td> <p> 输入要搜索的术语。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL仅使用值]</p> </td> 
   <td> <p>启用此选项可仅在模块字段的值中搜索。</p> <p>禁用此选项，也可在模块字段名称中搜索。</p> <p>通过名称和标签参数执行搜索。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取应用程序元数据]

按应用程序的模块名称或ID检索应用程序的元数据。 例如，当您需要了解情景中使用的应用程序版本时，这项功能非常有用。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL源模块]</td>
        <td>选择要检索其元数据的模块。</td>
    </tr>
</table>

#### [!UICONTROL 复制映射]

将值从源模块复制到目标模块。

>[!CAUTION]
>
>确保设置正确的源模块和目标模块。 如果选择其他类型的模块，则将删除目标模块中的值。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模块]</td> 
   <td> <p> 选择模块或输入要从中复制字段值的模块的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target模块]</p> </td> 
   <td> <p>选择模块或输入要插入源模块值的模块的ID。</p> <p>重要信息：目标模块中的值将被覆盖。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 复制筛选器]

将筛选器设置从源模块复制到目标模块。

>[!NOTE]
>
>复制操作将对置于选定模块左侧的过滤器执行。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模块]</td> 
   <td> <p> 选择模块或输入要从中复制筛选器值的模块的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target模块]</p> </td> 
   <td> <p>选择模块或输入要从源模块插入筛选值的模块的ID。</p> <p>重要信息：目标模块中的值将被覆盖。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL保留回退路由设置]</p> </td> 
   <td> <p>源筛选器将设置为回退路由。 启用此选项还可将目标筛选器设置为回退路由。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 交换连接]

将源模块中的连接复制到同一应用程序方案中的每个模块。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL源模块]</td>
        <td>选择模块或输入要从中复制连接的模块的ID。</td>
    </tr>
</table>

#### [!UICONTROL 交换变量]

在方案中搜索指定的变量，并将其替换为新变量。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！要查找的UICONTROL变量]</td> 
   <td> <p> 在方案中的模块中找到要替换的变量药丸，并将其复制到此（[!UICONTROL要查找的变量]）字段。 在字段中，显示双花括号。 示例: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL替换为]</p> </td> 
   <td> <p>在方案中的模块中找到要将变量替换为的变量药丸，并将其复制到此（[!UICONTROL要查找的变量]）字段。 在字段中，显示双花括号。 示例: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL模块]</p> </td> 
   <td> <p>选择要替换变量的模块。 如果未选择任何模块，则变量将在整个方案中替换。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 交换应用程序]

将方案中的选定应用程序版本替换为其他应用程序版本。

例如，可以使用此功能将Gmail和电子邮件应用程序的模块升级到最新版本。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！要替换的UICONTROL应用程序]</td> 
   <td> <p> 选择要替换的应用程序。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL替换为]</p> </td> 
   <td> <p>选择要将其替换为的应用程序。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 基64]

用于将输入的数据编码为Base64或对Base64进行解码。 某些请求将编码为Base64。 当您想要在编码请求中搜索特定数据时，此工具会非常有用。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL操作] </td> 
   <td> <p>选择是要将[!UICONTROL Raw Data]字段中的数据编码为Base64，还是将Base64解码为Raw Data。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL原始数据]</p> </td> 
   <td> <p> 根据上面[!UICONTROL Operation]字段中选择的选项，输入要编码为Base64或Base64（如果要解码为原始数据）的数据。</p> </td> 
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
   <td role="rowheader">[!UICONTROL模块] </td> 
   <td> <p>选择要复制的模块名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重新映射源]

用于将映射源从一个模块更改为另一个模块。

您必须首先将要用作源模块的模块添加到方案中的路由。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模块] </td> 
   <td> <p> 选择要替换的模块作为方案中其他模块的映射源。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target模块]</p> </td> 
   <td> <p>选择要用作新映射源的模块。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！要编辑的UICONTROL模块]</p> </td> 
   <td> <p>如果不想在整个方案中更改映射，请选择要更改映射的模块。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 突出显示应用程序]

在您的方案中突出显示指定应用程序的模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！要高亮显示的UICONTROL应用程序] </td> 
   <td> <p> 选择要在方案中突出显示的应用程序。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL版本] </p> </td> 
   <td> <p>选择要突出显示的应用程序版本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL高亮显示颜色]</p> </td> 
   <td> <p> 输入要用于突出显示模块的十六进制颜色。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 迁移GS]

此工具专门用于升级 [!DNL Google Sheets] （旧版）模块到最新版本 [!DNL Google Sheets] 版本。 它会在方案路由中模块的旧版本之后添加模块的新版本。

此模块不要求您设置任何参数。
