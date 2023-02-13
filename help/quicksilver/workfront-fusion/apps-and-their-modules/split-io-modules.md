---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Split.io模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Split.io]，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1773'
ht-degree: 0%

---

# [!DNL Split.io] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Split.io]，并将其连接到多个第三方应用程序和服务。

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

使用 [!DNL Split.io] 模块，您必须 [!DNL Split.io] 帐户。

## 连接 [!DNL Split.io] to [!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

您可以创建与 [!DNL Split.io] 直接从内部帐户 [!DNL Split.io] 模块。

1. 在任意 [!DNL Split.io] 模块，单击 **[!UICONTROL 添加]** 旁边 [!UICONTROL 连接] 字段。
1. 输入连接的名称。
1. 输入 [!DNL Split.io] API密钥。

   有关 [!DNL Split.io] API密钥，请参阅 [API密钥](https://help.split.io/hc/en-us/articles/360019916211-API-keys) 在 [!DNL Split.io] 文档。

1. 单击 **[!UICONTROL 继续]** 创建连接，然后返回到模块。

## [!DNL Split.io] 模块及其字段

配置 [!DNL split.io] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL split.io] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [操作](#actions)
* [搜索](#searches)

### 操作

* [[!UICONTROL 自定义API调用]](#custom-api-call)
* [[!UICONTROL 拆分]](#get-split)
* [[!UICONTROL 在环境中获取拆分定义]](#get-split-definition-in-environment)
* [[!UICONTROL 创建拆分]](#create-split)
* [[!UICONTROL 删除拆分]](#delete-split)
* [[!UICONTROL 在环境中创建拆分定义]](#create-split-definition-in-environment)
* [[!UICONTROL 从环境中删除拆分定义]](#remove-split-definition-from-environment)
* [[!UICONTROL 环境中的部分更新拆分定义]](#partial-update-split-definition-in-environment)
* [[!UICONTROL 关联标记]](#associate-tags)

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL split.io] API。 这样，您就可以创建数据流自动化，而另一个数据流无法实现 [!DNL split.io] 模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>输入相对于 <code>https://api.split.io/internal/api/v2/</code>.</td> 
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
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>输入或映射您希望模块在每个方案执行周期期间处理的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 拆分]

此操作模块将检索拆分。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>选择或映射包含要检索的拆分的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要检索的拆分的名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 在环境中获取拆分定义]

此操作模块从指定的环境中检索特定拆分定义。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>选择或映射包含要检索的拆分定义的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL环境名称或ID]</td> 
   <td>选择或映射包含要检索的拆分定义的环境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要检索其拆分定义的拆分名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建拆分]

此操作模块会在您的组织中创建一个新的拆分（假定流量类型）。

>[!NOTE]
>
>API不会在任何环境中配置拆分。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>选择或映射要创建拆分的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL流量类型ID或名称]</td> 
   <td>选择或映射要创建拆分的流量类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要创建的拆分的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分描述]</td> 
   <td>输入或映射要创建拆分的[!UICONTROL split]描述。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除拆分]

此操作模块会从您的组织中删除拆分。 这会自动从所有环境中取消配置拆分定义。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>选择或映射要删除拆分的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要删除的拆分的名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 在环境中创建拆分定义]

此操作模块为特定环境配置拆分定义。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>选择或映射要创建拆分定义的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL环境名称或ID]</td> 
   <td>选择或映射要创建拆分定义的环境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要为其创建定义的拆分的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL注释]</td> 
   <td>输入或映射要添加到拆分定义的任何注释。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL规则]</td> 
   <td> <p>对于要添加到定义的每个定位规则，单击 <b>[!UICONTROL添加项目]</b>，然后输入或映射规则。</p> <p>有关定位规则的更多信息，请参阅 <a href="https://docs.split.io/reference#create-split-definition-in-environment">在环境中创建拆分定义</a> 在 [!DNL Split.io] 文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL默认规则]</td> 
   <td> <p>输入或映射您希望拆分用于不符合其他规则规范的流量的规则。</p> <p>有关定位规则的更多信息，请参阅 <a href="https://docs.split.io/reference#create-split-definition-in-environment">在环境中创建拆分定义</a> 在 [!DNL Split.io] 文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL默认处理]</td> 
   <td> <p>输入或映射在拆分终止或客户未包含在流量分配中时希望拆分使用的处理。</p> <p>有关治疗的更多信息，请参阅 <a href="https://docs.split.io/reference#create-split-definition-in-environment">在环境中创建拆分定义</a> 在 [!DNL Split.io] 文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL处理方法]</td> 
   <td> <p>对于要添加到定义中的每个治疗，单击 <b>[!UICONTROL添加项目]</b>，然后输入或映射处理。</p> <p>有关治疗的更多信息，请参阅 <a href="https://docs.split.io/reference#create-split-definition-in-environment">在环境中创建拆分定义</a> 在 [!DNL Split.io] 文档。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从环境中删除拆分定义]

此操作模块将为特定环境取消配置拆分定义。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>选择或映射要删除拆分定义的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL环境名称或ID]</td> 
   <td>选择或映射要删除拆分定义的环境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要删除其定义的拆分的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL注释]</td> 
   <td>输入或映射要添加到拆分定义的任何注释。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 环境中的部分更新拆分定义]

此操作模块可更新特定环境的拆分定义。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>选择或映射要更新拆分定义的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL环境名称或ID]</td> 
   <td>选择或映射要更新拆分定义的环境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要更新其定义的拆分的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL更新内容]</td> 
   <td> <p>对于要更新的拆分的每个属性，单击 <b>[!UICONTROL添加项目]</b> ，然后输入或映射所需的更改。</p> <p>有关更多信息，请参阅 <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">环境中的部分更新拆分定义</a> 在 [!DNL Split.io] 文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL注释]</td> 
   <td>输入或映射要添加到拆分定义的任何注释。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 关联标记]

此操作模块会将标记添加到指定的对象。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>选择或映射要添加标记的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL对象名称]</td> 
   <td>输入或映射要添加标记的对象的名称，</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL对象类型]</td> 
   <td> <p>输入或映射要添加标记的对象类型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标记]</td> 
   <td> <p>对于要添加的每个标记，单击 <b>[!UICONTROL添加项目]</b> 并输入或映射标记。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

* [[!UICONTROL 获取工作区]](#get-workspaces)
* [[!UICONTROL 获取环境]](#get-environments)
* [[!UICONTROL 获取拆分]](#get-splits)
* [[!UICONTROL 在环境中列出拆分定义]](#list-split-definitions-in-an-environment)
* [[!UICONTROL 获取流量类型]](#get-traffic-types)

#### [!UICONTROL 获取工作区]

此搜索模块可检索组织的工作区。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>输入或映射您希望模块在每个方案执行周期期间检索的最大工作区数。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取环境]

此搜索模块可检索环境列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>选择或映射包含要列出的环境的工作区。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取拆分]

此搜索模块检索拆分列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>选择或映射包含要列出的拆分的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>输入或映射您希望模块在每个方案执行周期期间检索的最大拆分数。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 在环境中列出拆分定义]

此搜索模块可检索给定环境中的拆分定义列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>选择或映射包含要列出的拆分定义的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL环境名称或ID]</td> 
   <td>选择或映射包含要列出的拆分定义的环境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>输入或映射您希望模块在每个方案执行周期期间检索的最大拆分定义数。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取流量类型]

此搜索模块可检索流量类型的列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Split.io] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">连接 [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>选择或映射包含要列出的流量类型的工作区。</td> 
  </tr> 
 </tbody> 
</table>
