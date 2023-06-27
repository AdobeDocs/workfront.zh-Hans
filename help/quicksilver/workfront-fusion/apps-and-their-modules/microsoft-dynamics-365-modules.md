---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365模块
description: 在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用Microsoft Dynamics 365的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1589'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Microsoft Dynamics 365]，并将其连接到多个第三方应用程序和服务。

>[!NOTE]
>
>此 [!DNL Microsoft Dynamics 365] 连接器不支持 [!DNL Dynamics Finance and Operations].

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

使用 [!DNL Microsoft Dynamics] 365，您必须拥有 [!DNL Microsoft Dynamics 365] 帐户。

## 将Microsoft Dynamics 365连接到Workfront Fusion

您可以创建与 [!DNL Microsoft Dynamics 365] 直接从 [!DNL Microsoft Dynamics 365] 模块。

1. 在任意 [!DNL Microsoft Dynamics 365] 模块，单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 字段。
1. 输入连接的名称。
1. 在 **[!UICONTROL 资源]** 字段中，输入您的电子邮件地址 [!DNL Dynamics 365] 帐户，不含 `https://`.
1. 单击 **[!UICONTROL 继续]** 以创建连接并返回模块。

>[!NOTE]
>
>注册时 [!DNL Workfront Fusion] 在您的 [!DNL Microsoft Azure] 入口，请使用以下重定向URI：
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## [!DNL Microsoft Dynamics 365] 模块及其字段

配置时 [!DNL Microsoft Dynamics 365] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Microsoft Dynamics 365] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 观看记录（已计划）]](#watch-records-scheduled)
* [[!UICONTROL 观看记录（实时）]](#watch-records-real-time)
* [[!UICONTROL 创建记录]](#create-record)
* [[!UICONTROL 进行API调用]](#make-an-api-call)
* [[!UICONTROL 删除记录]](#delete-record)
* [[!UICONTROL 读取记录]](#read-records)
* [[!UICONTROL 更新记录]](#update-record)
* [[!UICONTROL 搜索记录]](#search-records)

### [!UICONTROL 观看记录（已计划）]

此计划触发器模块执行一个方案，即在中的上次计划运行之后创建或更新指定对象中的记录时 [!DNL Dynamics 365].

模块的输出指示找到的记录是新的还是更新的（如果在该时间段内既添加又更新，则标记为新）。 您可以将此信息映射到场景中的后续模块。

此操作在您指定的定期计划间隔内发生。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Microsoft Dynamics 365] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] 到 [!DNL Workfront Fusion]</a> 本文章中。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Include]</td> 
   <td>选择是否希望模块观看 <strong>[！UICONTROL仅新记录]</strong>， <strong>[！UICONTROL仅更新记录]</strong>，或 <strong>[！UICONTROL新记录和所有更改]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL实体类型]</td> 
   <td>选择要让场景观看的[！UICONTROL Microsoft Dynamics 365]记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最大记录数]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 观看记录（实时）]

当在中创建或更新您指定的记录（对象）时，此即时触发器模块会执行场景 [!DNL Dynamics 365].

此模块中需要webhook。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook]</td> 
   <td> <p>选择要用于此模块的webhook。 </p> <p>要添加新的webhook，请执行以下操作：</p> 
    <ol> 
     <li value="1"> <p>单击 <strong>[！UICONTROL添加]</strong> Webhook字段的右侧</p> </li> 
     <li value="2"> <p>在 <strong>[！UICONTROL Webhook]</strong> 名称字段，为webhook键入描述性名称。</p> </li> 
     <li value="3"> <p>在 <strong>[！UICONTROL连接]</strong> 字段中，选择要使用的连接</p> <p>有关连接 [!DNL Microsoft Dynamics 365] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] 到 [!DNL Workfront Fusion]</a> 本文章中。 </p> </li> 
     <li value="4"> <p>单击 <strong>[！UICONTROL保存]</strong> 以保存webhook并返回到模块。</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 创建记录]

此操作模块创建一个实体，如约会或任务。

可指定有关要创建的图元的信息。

模块返回新实体的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Microsoft Dynamics 365] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] 到 [!DNL Workfront Fusion]</a> 本文章中。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL实体类型]</td> 
   <td>选择您希望模块创建的实体类型。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL属性字段]</td> 
   <td>在这些字段中，输入您希望工作项对于给定属性具有的值。 可用字段取决于实体类型。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 进行API调用]

通过此操作模块，您可以对 [!DNL Microsoft Dynamics 365] API。 这样，您就可以创建一个其他人无法实现的数据流自动化 [!DNL Microsoft Dynamics 365] 模块。

模块返回有关状态代码、标头和正文的信息。 您可以将此信息映射到场景中的后续模块。

要了解更多信息，请参阅 [!DNL Microsoft] 有关使用的文档 [!DNL Dynamics 365 Customer Engagement Web API].

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Microsoft Dynamics 365] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] 到 [!DNL Workfront Fusion]</a> 本文章中。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td> <p>输入相对路径 <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> <p>有关详情，请参阅</p> </td> 
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

### [!UICONTROL 删除记录]

此操作模块删除实体。

可指定实体的ID。

模块返回实体的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Microsoft Dynamics 365] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] 到 [!DNL Workfront Fusion]</a> 本文章中。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL实体类型]</td> 
   <td> <p>选择您希望模块删除的实体类型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td> <p>输入或映射唯一值 [!DNL Microsoft Dynamics 365] 您希望模块删除的记录的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 读取记录]

该操作模块从中的单个实体读取数据 [!DNL Microsoft Dynamics 365].

可指定实体的ID。

模块返回实体的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Microsoft Dynamics 365] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] 到 [!DNL Workfront Fusion]</a> 本文章中。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL实体类型]</td> 
   <td>选择您希望模块读取的实体类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>输入或映射唯一值 [!DNL Microsoft Dynamics 365] 您希望模块读取的记录的ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新记录]

此操作模块可更新实体。

可指定实体的ID。

该模块返回更新记录的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Microsoft Dynamics 365] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] 到 [!DNL Workfront Fusion]</a> 本文章中。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL实体类型]</td> 
   <td>选择要更新模块的实体类型。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL属性字段]</td> 
   <td>在这些字段中，输入您希望工作项对于给定属性具有的值。 可用字段取决于实体类型。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>输入或映射唯一值 [!DNL Microsoft Dynamics] 您希望模块更新的记录的365 ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜索记录]

此搜索模块查找对象中的记录 [!DNL Microsoft Dynamics 365] 与指定的搜索查询匹配的用户名称。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
  <td> <p>有关连接 [!DNL Microsoft Dynamics 365] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] 到 [!DNL Workfront Fusion]</a> 本文章中。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL实体类型]</td> 
   <td>选择要更新模块的实体类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL筛选器]</td> 
   <td> <p>选择要用于此搜索的过滤器。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL标准筛选器]</strong> </p> <p>通过选择字段和运算符，然后输入或映射要搜索的值，设置过滤器。 您可以在筛选器中使用AND或OR规则。</p> </li> 
     <li> <p><strong>[！UICONTROL查询函数]</strong> </p> <p>输入 [!DNL Dynamics 365] 要用于搜索的Web API查询函数。 </p> <p>有关查询函数的更多信息，请参阅 <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Web API查询函数参考</a> 在 [!DNL Microsoft] 文档。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序]</td> 
   <td> <p>指定返回项目的顺序。 您可以添加多个排序。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL字段]</strong> </p> <p>指定要按其对结果进行排序的字段。</p> </li> 
     <li> <p><strong>[！UICONTROL方向]</strong> </p> <p>指定排序方向（升序或降序）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最大记录数]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
 </tbody> 
</table>
