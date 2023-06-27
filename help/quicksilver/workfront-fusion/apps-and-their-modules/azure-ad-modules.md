---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Azure Active Directory模块
description: 在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Azure] Active Directory ，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: ac966231-251e-44de-be61-00afa5ece3fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 1%

---

# [!DNL Azure Active Directory] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Azure Active Directory]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL Azure Active Directory] 模块，您必须拥有 [!DNL Azure Active Directory] 帐户。

## [!DNL Azure Active Directory] 模块及其字段

配置时 [!DNL Azure Active Directory] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Azure Active Directory] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

#### [!UICONTROL 观看记录] （已计划）

此轮询（计划）触发器模块执行的情况是，自中上次计划运行以来在选定对象中创建了记录 [!DNL Azure Active Directory]. 它还返回与一个或多个记录关联的所有标准字段，以及连接访问的任何自定义字段和值。您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure Active Directory] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL类型]</td> 
   <td>选择是要监视用户记录还是组记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最大记录数]</td> 
   <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 读取记录]](#read-record)
* [[!UICONTROL 创建记录]](#create-record)
* [[!UICONTROL 自定义API调用]](#custom-api-call)

#### [!UICONTROL 读取记录]

该操作模块从中的单个记录读取数据 [!DNL Azure Active Directory].

您指定记录的ID。

该模块返回记录的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

您必须具有足够的权限才能访问中的记录 [!DNL Azure Active Directory] 以检索此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure Active Directory] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td>选择您要读取[！UICONTROL User]记录还是[！UICONTROL Group]记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td>选择要包含在此模块的输出包中的信息。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>输入或映射唯一值 [!DNL Azure Active Directory] 您希望模块读取的记录的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建记录]

此操作模块创建新用户或组记录。

指定所需记录的类型。

该模块返回记录的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure Active Directory] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td>选择您要读取[！UICONTROL User]记录还是[！UICONTROL Group]记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL其他字段]</td> 
   <td>填写这些字段以设置新记录的值。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL Azure Active Directory] API。 这样，您就可以创建一个其他人无法实现的数据流自动化 [!DNL Azure Active Directory] 模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure Active Directory] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>输入或映射相对路径 <code>https://graph.microsoft.com/{version}/{resource}?{query-parameters}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> </td> 
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

### 搜索

* [搜索用户](#search-users)
* [搜索用户/组增量](#search-usersgroups-delta)

#### [!UICONTROL 搜索用户]

此搜索模块查找对象中的记录 [!DNL Azure Active Directory] 与指定的搜索查询匹配的用户名称。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure Active Directory] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL搜索条件]</td> 
   <td> <p>输入要在搜索中使用的标准。</p> <p>有关要使用的参数（如“[！UICONTROL $filter]”）的信息，请参阅 <a href="https://docs.microsoft.com/en-us/graph/query-parameters">使用查询参数自定义响应</a> 在 [!DNL Microsoft] api文档。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td>选择要包含在此模块的输出包中的信息。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL最大记录数]</td> 
   <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索用户/组增量]

此搜索模块在以下位置查找记录： [!DNL Azure AD] 已创建、更新或删除的页面。 您可以将此信息映射到场景中的后续模块。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure Active Directory] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>
