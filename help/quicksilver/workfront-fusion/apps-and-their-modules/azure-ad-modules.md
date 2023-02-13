---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Azure Active Directory模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Azure] Active Directory，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: ac966231-251e-44de-be61-00afa5ece3fd
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '991'
ht-degree: 1%

---

# [!DNL Azure Active Directory] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Azure Active Directory]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL Azure Active Directory] 模块，您必须具有 [!DNL Azure Active Directory] 帐户。

## [!DNL Azure Active Directory] 模块及其字段

配置 [!DNL Azure Active Directory] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Azure Active Directory] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

#### [!UICONTROL 监视记录] （已计划）

此轮询（已计划）触发器模块在自上次计划运行以来已创建选定对象中的记录时执行方案 [!DNL Azure Active Directory]. 它还返回与记录或记录关联的所有标准字段，以及连接所访问的任何自定义字段和值。您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure Active Directory] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>选择您要观看用户记录还是群组记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL最大记录数]</td> 
   <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 读取记录]](#read-record)
* [[!UICONTROL 创建记录]](#create-record)
* [[!UICONTROL 自定义API调用]](#custom-api-call)

#### [!UICONTROL 读取记录]

此操作模块从 [!DNL Azure Active Directory].

您指定记录的ID。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

您必须拥有足够的权限才能访问 [!DNL Azure Active Directory] 以检索此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure Active Directory] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择您是要读取[!UICONTROL User]记录还是[!UICONTROL Group]记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出]</td> 
   <td>选择要包含在此模块的输出包中的信息。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>输入或映射唯一 [!DNL Azure Active Directory] 您希望模块读取的记录的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建记录]

此操作模块会创建新的用户或组记录。

您指定所需记录的类型。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure Active Directory] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择您是要读取[!UICONTROL User]记录还是[!UICONTROL Group]记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL其他字段]</td> 
   <td>填写这些字段以设置新记录的值。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL Azure Active Directory] API。 这样，您就可以创建数据流自动化，而另一个数据流无法实现 [!DNL Azure Active Directory] 模块。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure Active Directory] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>输入或映射相对于 <code>https://graph.microsoft.com/{version}/{resource}?{query-parameters}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> </td> 
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

### 搜索

* [搜索用户](#search-users)
* [搜索用户/组增量](#search-usersgroups-delta)

#### [!UICONTROL 搜索用户]

此搜索模块在 [!DNL Azure Active Directory] 与您指定的搜索查询匹配。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure Active Directory] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL搜索条件]</td> 
   <td> <p>输入要在搜索中使用的标准。</p> <p>有关要使用的参数（如“[!UICONTROL $filter]”）的信息，请参阅 <a href="https://docs.microsoft.com/en-us/graph/query-parameters">使用查询参数自定义响应</a> 在 [!DNL Microsoft] API文档。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL输出]</td> 
   <td>选择要包含在此模块的输出包中的信息。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL记录的最大计数]</td> 
   <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索用户/组增量]

此搜索模块在 [!DNL Azure AD] 创建、更新或删除的内容。 您可以在方案的后续模块中映射此信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure Active Directory] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>
