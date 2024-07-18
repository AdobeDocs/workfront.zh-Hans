---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Split.io模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动使用 [!DNL Split.io]的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1801'
ht-degree: 0%

---

# [!DNL Split.io]模块

在[!DNL Adobe Workfront Fusion]方案中，您可以自动使用[!DNL Split.io]的工作流，并将其连接到多个第三方应用程序和服务。

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

要使用[!DNL Split.io]模块，您必须具有[!DNL Split.io]帐户。

## 将[!DNL Split.io]连接到[!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

您可以在[!DNL Split.io]模块内直接创建与[!DNL Split.io]帐户的连接。

1. 在任意[!DNL Split.io]模块中，单击[!UICONTROL 连接]字段旁边的&#x200B;**[!UICONTROL 添加]**。
1. 输入连接的名称。
1. 输入您的[!DNL Split.io] API密钥。

   有关[!DNL Split.io] API密钥的更多信息，请参阅[!DNL Split.io]文档中的[API密钥](https://help.split.io/hc/en-us/articles/360019916211-API-keys)。

1. 单击&#x200B;**[!UICONTROL 继续]**&#x200B;以创建连接并返回模块。

## [!DNL Split.io]模块及其字段

配置[!DNL split.io]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL split.io]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

* [操作](#actions)
* [搜索](#searches)

### 操作

* [[!UICONTROL 自定义API调用]](#custom-api-call)
* [[!UICONTROL 获取拆分]](#get-split)
* [[!UICONTROL 获取环境中的拆分定义]](#get-split-definition-in-environment)
* [[!UICONTROL 创建拆分]](#create-split)
* [[!UICONTROL 删除拆分]](#delete-split)
* [[!UICONTROL 在环境中创建拆分定义]](#create-split-definition-in-environment)
* [[!UICONTROL 从环境中移除拆分定义]](#remove-split-definition-from-environment)
* [[!UICONTROL 环境中的部分更新拆分定义]](#partial-update-split-definition-in-environment)
* [[!UICONTROL 关联标记]](#associate-tags)

#### [!UICONTROL 自定义API调用]

此操作模块允许您对[!DNL split.io] API进行经过身份验证的自定义调用。 这样，您可以创建其他[!DNL split.io]模块无法实现的数据流自动化。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>输入相对于<code>https://api.split.io/internal/api/v2/</code>的路径。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP请求方法。</p> </td> 
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
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>在JSON中使用条件语句（如<code>if</code>）时，请将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>输入或映射每个方案执行周期中您希望模块使用的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取拆分]

此操作模块将检索拆分。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>选择或映射包含要检索的分割的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要检索的分割的名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取环境中的拆分定义]

此操作模块从指定的环境中检索特定的拆分定义。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>选择或映射包含要检索的拆分定义的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL环境名称或ID]</td> 
   <td>选择或映射包含要检索的拆分定义的环境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要检索其拆分定义的分割的名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建拆分]

在给定流量类型的情况下，此操作模块会在您的组织中创建新拆分。

>[!NOTE]
>
>该API不会在任何环境中配置拆分。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>选择或映射要在其中创建拆分的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL流量类型ID或名称]</td> 
   <td>选择或映射要创建拆分的流量类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要创建的拆分的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL拆分说明]</td> 
   <td>为要创建的拆分输入或映射[！UICONTROL split]说明。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除拆分]

此操作模块会从您的组织中删除拆分。 这会自动从所有环境中取消配置剥离定义。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>选择或映射要删除拆分的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要删除的分割的名称。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>选择或映射要在其中创建拆分定义的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL环境名称或ID]</td> 
   <td>选择或映射要创建拆分定义的环境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要为其创建定义的分割的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Comments]</td> 
   <td>输入或映射要添加到拆分定义的任何注释。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL规则]</td> 
   <td> <p>对于要添加到定义的每个定位规则，单击<b>[！UICONTROL添加项]</b>，然后输入或映射该规则。</p> <p>有关定位规则的更多信息，请参阅[!DNL Split.io]文档中的<a href="https://docs.split.io/reference#create-split-definition-in-environment">在环境中创建拆分定义</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL默认规则]</td> 
   <td> <p>输入或映射希望拆分用于不符合其他规则规范的流量的规则。</p> <p>有关定位规则的更多信息，请参阅[!DNL Split.io]文档中的<a href="https://docs.split.io/reference#create-split-definition-in-environment">在环境中创建拆分定义</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL默认待遇]</td> 
   <td> <p>输入或映射在拆分被终止或客户不包含在流量分配中的情况下希望拆分使用的处理方式。</p> <p>有关处理的详细信息，请参阅[!DNL Split.io]文档中的<a href="https://docs.split.io/reference#create-split-definition-in-environment">在环境中创建拆分定义</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL处理]</td> 
   <td> <p>对于要添加到定义的每个处理，单击<b>[！UICONTROL添加项]</b>，然后输入或映射处理。</p> <p>有关处理的详细信息，请参阅[!DNL Split.io]文档中的<a href="https://docs.split.io/reference#create-split-definition-in-environment">在环境中创建拆分定义</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从环境中移除拆分定义]

此操作模块为特定环境取消配置拆分定义。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>选择或映射要删除拆分定义的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL环境名称或ID]</td> 
   <td>选择或映射要删除拆分定义的环境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要删除其定义的分割的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Comments]</td> 
   <td>输入或映射要添加到拆分定义的任何注释。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 环境中的部分更新拆分定义]

此操作模块更新特定环境的拆分定义。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>选择或映射要更新拆分定义的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL环境名称或ID]</td> 
   <td>选择或映射要更新拆分定义的环境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL拆分名称]</td> 
   <td> <p>输入或映射要更新其定义的分割的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL更新内容]</td> 
   <td> <p>对于要更新的拆分的每个属性，单击<b>[！UICONTROL添加项]</b>并输入或映射所需的更改。</p> <p>有关详细信息，请参阅[!DNL Split.io]文档中的<a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">环境</a>中的部分更新拆分定义。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Comments]</td> 
   <td>输入或映射要添加到拆分定义的任何注释。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 关联标记]

此操作模块将标记添加到指定的对象。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>选择或映射要添加标记的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL对象名称]</td> 
   <td>输入或映射要添加标记的对象的名称，</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL对象类型]</td> 
   <td> <p>输入或映射要添加标记的对象的类型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标记]</td> 
   <td> <p>对于要添加的每个标记，单击<b>[！UICONTROL添加项]</b>并输入或映射该标记。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

* [[!UICONTROL 获取工作区]](#get-workspaces)
* [[!UICONTROL 获取环境]](#get-environments)
* [[!UICONTROL 获取拆分]](#get-splits)
* [[!UICONTROL 列出环境中的拆分定义]](#list-split-definitions-in-an-environment)
* [[!UICONTROL 获取流量类型]](#get-traffic-types)

#### [!UICONTROL 获取工作区]

此搜索模块检索组织的工作区。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>输入或映射每个方案执行周期中您希望模块检索的最大工作区数。</td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>选择或映射包含要列出的拆分的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>输入或映射您希望模块在每个方案执行周期中检索的最大拆分数。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出环境中的拆分定义]

此搜索模块检索给定环境中的拆分定义列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>选择或映射包含要列出的拆分定义的工作区。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL环境名称或ID]</td> 
   <td>选择或映射包含要列出的拆分定义的环境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>输入或映射每个方案执行周期中您希望模块检索的最大拆分定义数。</td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Split.io]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">将[!DNL Split.io]连接到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>选择或映射包含要列出的流量类型的工作区。</td> 
  </tr> 
 </tbody> 
</table>
