---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: 数据模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用Datadog的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# [!DNL Datadog] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Datadog]，并将其连接到多个第三方应用程序和服务。

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

使用 [!DNL Datadog] 模块，您必须 [!DNL Datadog] 帐户。

## 连接 [!DNL Datadog] to [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### 检索API密钥和应用程序密钥 {#retrieve-your-api-key-and-application-key}

连接 [!DNL Datadog] 帐户 [!DNL Workfront Fusion] 您需要从 [!DNL Datadog] 帐户。

1. 登录到 [!DNL Datadog] 帐户。
1. 在左侧导航面板中，单击 **[!UICONTROL 集成]**，然后单击 **[!UICONTROL API]**.
1. 在主屏幕上，单击 **[!UICONTROL API密钥]**.
1. 将鼠标悬停在紫色栏上以显示API密钥。
1. 将API密钥复制到安全位置。
1. 在主屏幕上，单击 **[!UICONTROL 应用程序键]**.
1. 将鼠标悬停在紫色栏上以显示应用程序键。
1. 将应用程序密钥复制到安全位置。

### 创建连接 [!DNL Datadog] in [!DNL Workfront Fusion]

您可以创建与 [!DNL Datadog] 直接从内部帐户 [!UICONTROL Datadog] 模块。

1. 在任意 [!UICONTROL Datadog] 模块，单击 **[!UICONTROL 添加]** 旁边 [!UICONTROL 连接] 字段。
1. 按如下方式填写模块的字段：

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL连接类型]</td> 
      <td> <p> 选择[!UICONTROL [!DNL Datadog] 应用程序]选项，以获取 [!DNL Datadog] API。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL连接名称]</td> 
      <td> <p> 输入连接的名称。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL域] </td> 
      <td> <p>选择要连接到的域（美国或欧盟）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API密钥]</td> 
      <td> <p> 输入 [!DNL Datadog] API密钥。 </p> <p>有关检索API密钥的说明，请参阅 <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">检索API密钥和应用程序密钥</a> 在本文中。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL应用程序密钥]</td> 
      <td> <p> 输入 [!DNL Datadog] 应用程序密钥。 </p> <p>有关检索应用程序密钥的说明，请参阅 <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">检索API密钥和应用程序密钥</a> 在本文中。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 继续]** 创建连接，然后返回到模块。

## [!DNL Datadog] 模块及其字段

配置 [!DNL Datadog] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Datadog] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 操作

* [[!UICONTROL 帖子时间点]](#post-timeseries-points)
* [[!UICONTROL 进行API调用]](#make-an-api-call)

#### [!UICONTROL 帖子时间点]

利用模块，可发布可在上绘制图表的时间系列数据 [!DNL Datadog]功能板。

压缩负载的限制为3.2 MB(3200000)，解压缩负载的限制为62 MB(62914560)。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Datadog] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">连接 [!DNL Datadog] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL系列]</td> 
   <td> <p>添加要提交到的时间系列 [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL量度]</strong> </p> <p>输入时间系列的名称。</p> </li> 
     <li> <p><strong>[!UICONTROL Type]</strong> </p> <p>选择量度的类型。</p> </li> 
     <li> <p><strong>[!UICONTROL Interval]</strong> </p> <p> 如果量度的类型是比率或计数，请定义相应的间隔。</p> </li> 
     <li> <p><strong>[!UICONTROL点]</strong> </p> <p>添加与量度相关的点。</p> <p>这是一个JSON点数组。 每个点都具有以下格式： <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>注释:  <p>时间戳必须以秒为单位。</p> <p>时间戳必须是当前时间戳。 “当前”是指将来不超过10分钟或过去超过1小时。</p> <p> 数值格式应为浮点值。</p> </p> <p>此字段必须至少包含1个项目。</p> </li> 
     <li> <p><strong>[!UICONTROL主机]</strong> </p> <p>输入生成量度的主机的名称。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 进行API调用]

此操作模块允许您执行自定义API调用。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Datadog] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">连接 [!DNL Datadog] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>输入相对于 <code>https://api.datadoghq.com/api/</code>. 示例:<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion会为您添加授权标头。</p> </td> 
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

**示例：** 以下API调用会返回 [!DNL Datadog] 帐户：

URL: `/v1/dashboard`

方法: `GET`

![](assets/datadog-api-example.png)

结果可在模块的“输出”中的“包”>“正文”>“功能板”下找到。

在本例中，返回了3个功能板：

![](assets/datadog-api-response-example.png)
